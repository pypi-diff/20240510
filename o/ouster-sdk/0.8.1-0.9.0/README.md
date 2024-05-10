# Comparing `tmp/ouster-sdk-0.8.1.tar.gz` & `tmp/ouster-sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/lib/jenkins/workspace/SDK_SDK_Extensions_master@2/build/sdist/.tmp-9rdjmm9k/ouster-sdk-0.8.1.tar", last modified: Mon Apr  3 20:58:58 2023, max compression
+gzip compressed data, was "/var/lib/jenkins/workspace/SDK_Extensions_master/build/sdist/.tmp-dbkjt8uq/ouster-sdk-0.9.0.tar", last modified: Fri Jul  7 21:18:00 2023, max compression
```

## Comparing `ouster-sdk-0.8.1.tar` & `ouster-sdk-0.9.0.tar`

### file list

```diff
@@ -1,325 +1,474 @@
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/
--rw-r--r--   0 build      (114) build      (118)     2633 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/CMakeLists.txt
--rw-r--r--   0 build      (114) build      (118)      182 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/MANIFEST.in
--rw-r--r--   0 build      (114) build      (118)     3251 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/PKG-INFO
--rw-r--r--   0 build      (114) build      (118)     1685 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/README.rst
--rw-r--r--   0 build      (114) build      (118)      418 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/mypy.ini
--rw-r--r--   0 build      (114) build      (118)      230 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/pyproject.toml
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/
--rw-r--r--   0 build      (114) build      (118)      138 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/.clang-format
--rw-r--r--   0 build      (114) build      (118)       37 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/.clangd
--rw-r--r--   0 build      (114) build      (118)       40 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/.dockerignore
--rw-r--r--   0 build      (114) build      (118)       35 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/.git
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/.github/
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 build      (114) build      (118)      817 2023-03-29 18:30:49.000000 ouster-sdk-0.8.1/sdk/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 build      (114) build      (118)     1064 2023-03-29 18:30:49.000000 ouster-sdk-0.8.1/sdk/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 build      (114) build      (118)      641 2023-03-29 18:30:49.000000 ouster-sdk-0.8.1/sdk/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 build      (114) build      (118)       62 2023-03-29 18:30:49.000000 ouster-sdk-0.8.1/sdk/.github/pull_request_template.md
--rw-r--r--   0 build      (114) build      (118)      148 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/.gitignore
--rw-r--r--   0 build      (114) build      (118)    23899 2023-03-29 18:30:49.000000 ouster-sdk-0.8.1/sdk/CHANGELOG.rst
--rw-r--r--   0 build      (114) build      (118)     3313 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/CMakeLists.txt
--rw-r--r--   0 build      (114) build      (118)     1070 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/CMakeSettings.json
--rw-r--r--   0 build      (114) build      (118)     3219 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/LICENSE
--rw-r--r--   0 build      (114) build      (118)    14183 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/LICENSE-bin
--rw-r--r--   0 build      (114) build      (118)     1836 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/README.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/cmake/
--rw-r--r--   0 build      (114) build      (118)      361 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/DefaultBuildType.cmake
--rw-r--r--   0 build      (114) build      (118)     1292 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/FindCURL.cmake
--rw-r--r--   0 build      (114) build      (118)      401 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/FindEigen3.cmake
--rw-r--r--   0 build      (114) build      (118)     1887 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/FindGTest.cmake
--rw-r--r--   0 build      (114) build      (118)      217 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/FindOusterSDK.cmake
--rw-r--r--   0 build      (114) build      (118)      561 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/FindPcap.cmake
--rw-r--r--   0 build      (114) build      (118)      471 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/Findglfw3.cmake
--rw-r--r--   0 build      (114) build      (118)     1980 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/Findjsoncpp.cmake
--rw-r--r--   0 build      (114) build      (118)     2279 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/Findlibtins.cmake
--rw-r--r--   0 build      (114) build      (118)      722 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/OusterSDKConfig.cmake.in
--rw-r--r--   0 build      (114) build      (118)      852 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/VcpkgEnv.cmake
--rw-r--r--   0 build      (114) build      (118)     1897 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/VersionGen.cmake
--rw-r--r--   0 build      (114) build      (118)      383 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/cmake/build.h.in
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/conan/
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/conan/test_package/
--rw-r--r--   0 build      (114) build      (118)      142 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/conan/test_package/CMakeLists.txt
--rw-r--r--   0 build      (114) build      (118)     1077 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/conan/test_package/conanfile.py
--rw-r--r--   0 build      (114) build      (118)     4621 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/conanfile.py
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/
--rw-r--r--   0 build      (114) build      (118)   114140 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/Doxyfile
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/_static/
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/_static/css/
--rw-r--r--   0 build      (114) build      (118)     1100 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/_static/css/ouster_rtd_tweaks.css
--rw-r--r--   0 build      (114) build      (118)     6869 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/conf.py
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/cpp/
--rw-r--r--   0 build      (114) build      (118)      201 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/api.rst
--rw-r--r--   0 build      (114) build      (118)     4915 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/building.rst
--rw-r--r--   0 build      (114) build      (118)     5891 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/examples.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_client/
--rw-r--r--   0 build      (114) build      (118)      891 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_client/client.rst
--rw-r--r--   0 build      (114) build      (118)      230 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_client/image_processing.rst
--rw-r--r--   0 build      (114) build      (118)      253 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_client/index.rst
--rw-r--r--   0 build      (114) build      (118)      827 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_client/lidar_scan.rst
--rw-r--r--   0 build      (114) build      (118)     3818 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_client/types.rst
--rw-r--r--   0 build      (114) build      (118)      307 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_client/version.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_pcap/
--rw-r--r--   0 build      (114) build      (118)      119 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_pcap/index.rst
--rw-r--r--   0 build      (114) build      (118)     1340 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_pcap/os_pcap.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_viz/
--rw-r--r--   0 build      (114) build      (118)      119 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_viz/index.rst
--rw-r--r--   0 build      (114) build      (118)      556 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/cpp/ouster_viz/point_viz.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/images/
--rw-r--r--   0 build      (114) build      (118)     9472 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/Ouster_Logo_TM_Horiz_Black_RGB_600px.png
--rw-r--r--   0 build      (114) build      (118)     2455 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/Ouster_Logo_TM_Horiz_White_RGB.svg
--rw-r--r--   0 build      (114) build      (118)     2528 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/Ouster_Logo_TM_Stacked_White_RGB.svg
--rw-r--r--   0 build      (114) build      (118)    61758 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/brooklyn_bridge_ls_50_range_image.png
--rw-r--r--   0 build      (114) build      (118)   452167 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/brooklyn_bridge_ls_50_xyz_cut.png
--rw-r--r--   0 build      (114) build      (118)   143035 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/lidar_scan_destaggered.png
--rw-r--r--   0 build      (114) build      (118)   148784 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/lidar_scan_staggered.png
--rw-r--r--   0 build      (114) build      (118)   829483 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/lidar_scan_xyz_84.png
--rw-r--r--   0 build      (114) build      (118)   570786 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/lidar_scan_xyz_84_3d.png
--rw-r--r--   0 build      (114) build      (118)   290021 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/simple-viz.png
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/
--rw-r--r--   0 build      (114) build      (118)   217741 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/axes_helper_unstructured.png
--rw-r--r--   0 build      (114) build      (118)     2181 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/empty_point_viz.png
--rw-r--r--   0 build      (114) build      (118)     4656 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/image_set_pos_bot_right.png
--rw-r--r--   0 build      (114) build      (118)     5515 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/image_set_pos_center.png
--rw-r--r--   0 build      (114) build      (118)     4683 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/image_set_pos_left.png
--rw-r--r--   0 build      (114) build      (118)     4648 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/image_set_pos_right.png
--rw-r--r--   0 build      (114) build      (118)    90497 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_fields_images.png
--rw-r--r--   0 build      (114) build      (118)    90193 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_fields_images_labels.png
--rw-r--r--   0 build      (114) build      (118)   238846 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_structured.png
--rw-r--r--   0 build      (114) build      (118)   154619 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_viz.png
--rw-r--r--   0 build      (114) build      (118)   151016 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_viz_checkers.png
--rw-r--r--   0 build      (114) build      (118)   159107 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_viz_labels.png
--rw-r--r--   0 build      (114) build      (118)     1439 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/docs/index.rst
--rw-r--r--   0 build      (114) build      (118)     3595 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/installation.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/migration/
--rw-r--r--   0 build      (114) build      (118)     5050 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/migration/migration-20220927-20230114.rst
--rw-r--r--   0 build      (114) build      (118)     5919 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/docs/migration/migration-20230114-20230403.rst
--rw-r--r--   0 build      (114) build      (118)     3530 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/docs/overview.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/python/
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/python/api/
--rw-r--r--   0 build      (114) build      (118)     1596 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/api/client.rst
--rw-r--r--   0 build      (114) build      (118)      997 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/api/examples.rst
--rw-r--r--   0 build      (114) build      (118)       95 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/api/index.rst
--rw-r--r--   0 build      (114) build      (118)      167 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/api/pcap.rst
--rw-r--r--   0 build      (114) build      (118)     1318 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/api/viz.rst
--rw-r--r--   0 build      (114) build      (118)     5725 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/docs/python/devel.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/python/examples/
--rw-r--r--   0 build      (114) build      (118)     3131 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/examples/basics-sensor.rst
--rw-r--r--   0 build      (114) build      (118)     3582 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/examples/conversion.rst
--rw-r--r--   0 build      (114) build      (118)      846 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/examples/index.rst
--rw-r--r--   0 build      (114) build      (118)     5540 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/examples/lidar-scan.rst
--rw-r--r--   0 build      (114) build      (118)     2345 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/examples/record-stream.rst
--rw-r--r--   0 build      (114) build      (118)     1203 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/examples/udp-packets.rst
--rw-r--r--   0 build      (114) build      (118)     7749 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/examples/visualizations.rst
--rw-r--r--   0 build      (114) build      (118)     5442 2023-03-29 18:30:49.000000 ouster-sdk-0.8.1/sdk/docs/python/quickstart.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/python/viz/
--rw-r--r--   0 build      (114) build      (118)     1090 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/viz/index.rst
--rw-r--r--   0 build      (114) build      (118)    12817 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/viz/viz-api-tutorial.rst
--rw-r--r--   0 build      (114) build      (118)     3349 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/python/viz/viz-run.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/docs/reference/
--rw-r--r--   0 build      (114) build      (118)       66 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/reference/changelog.rst
--rw-r--r--   0 build      (114) build      (118)     8871 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/reference/lidar-scan.rst
--rw-r--r--   0 build      (114) build      (118)     1807 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/docs/sample-data.rst
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/examples/
--rw-r--r--   0 build      (114) build      (118)     1117 2023-03-29 18:30:49.000000 ouster-sdk-0.8.1/sdk/examples/CMakeLists.txt
--rw-r--r--   0 build      (114) build      (118)     7585 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/examples/client_example.cpp
--rw-r--r--   0 build      (114) build      (118)     4510 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/examples/config_example.cpp
--rw-r--r--   0 build      (114) build      (118)     1477 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/examples/helpers.cpp
--rw-r--r--   0 build      (114) build      (118)      419 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/examples/helpers.h
--rw-r--r--   0 build      (114) build      (118)     5748 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/examples/lidar_scan_example.cpp
--rw-r--r--   0 build      (114) build      (118)     2484 2023-03-29 18:30:49.000000 ouster-sdk-0.8.1/sdk/examples/mtp_client_example.cpp
--rw-r--r--   0 build      (114) build      (118)     6603 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/examples/representations_example.cpp
--rw-r--r--   0 build      (114) build      (118)     1870 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/examples/viz_example.cpp
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_client/
--rw-r--r--   0 build      (114) build      (118)     1783 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/CMakeLists.txt
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/optional-lite/
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/optional-lite/nonstd/
--rw-r--r--   0 build      (114) build      (118)    52100 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/optional-lite/nonstd/optional.hpp
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/
--rw-r--r--   0 build      (114) build      (118)     5100 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/buffered_udp_source.h
--rw-r--r--   0 build      (114) build      (118)     9413 2023-03-29 18:30:49.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/client.h
--rw-r--r--   0 build      (114) build      (118)     3422 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/image_processing.h
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/impl/
--rw-r--r--   0 build      (114) build      (118)     2495 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/impl/cartesian.h
--rw-r--r--   0 build      (114) build      (118)     9835 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/impl/lidar_scan_impl.h
--rw-r--r--   0 build      (114) build      (118)    15871 2023-03-23 23:26:52.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/lidar_scan.h
--rw-r--r--   0 build      (114) build      (118)     3680 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/sensor_http.h
--rw-r--r--   0 build      (114) build      (118)    34195 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/types.h
--rw-r--r--   0 build      (114) build      (118)     2936 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/version.h
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/
--rw-r--r--   0 build      (114) build      (118)     6773 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/buffered_udp_source.cpp
--rw-r--r--   0 build      (114) build      (118)    21679 2023-04-03 20:58:19.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/client.cpp
--rw-r--r--   0 build      (114) build      (118)     3516 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/curl_client.h
--rw-r--r--   0 build      (114) build      (118)     1212 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/http_client.h
--rw-r--r--   0 build      (114) build      (118)     8265 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/image_processing.cpp
--rw-r--r--   0 build      (114) build      (118)    24786 2023-03-29 18:30:49.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/lidar_scan.cpp
--rw-r--r--   0 build      (114) build      (118)     3197 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/logging.cpp
--rw-r--r--   0 build      (114) build      (118)      810 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/logging.h
--rw-r--r--   0 build      (114) build      (118)     2447 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/netcompat.cpp
--rw-r--r--   0 build      (114) build      (118)     2051 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/netcompat.h
--rw-r--r--   0 build      (114) build      (118)    17467 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/parsing.cpp
--rw-r--r--   0 build      (114) build      (118)     1932 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/sensor_http.cpp
--rw-r--r--   0 build      (114) build      (118)     4964 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/sensor_http_imp.cpp
--rw-r--r--   0 build      (114) build      (118)     4771 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/sensor_http_imp.h
--rw-r--r--   0 build      (114) build      (118)     6866 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/sensor_tcp_imp.cpp
--rw-r--r--   0 build      (114) build      (118)     3701 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/sensor_tcp_imp.h
--rw-r--r--   0 build      (114) build      (118)    49976 2023-04-03 20:58:19.000000 ouster-sdk-0.8.1/sdk/ouster_client/src/types.cpp
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/
--rw-r--r--   0 build      (114) build      (118)      928 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/CMakeLists.txt
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/include/
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/include/ouster/
--rw-r--r--   0 build      (114) build      (118)     3223 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/include/ouster/indexed_pcap_reader.h
--rw-r--r--   0 build      (114) build      (118)    10962 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/include/ouster/os_pcap.h
--rw-r--r--   0 build      (114) build      (118)     6563 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/include/ouster/pcap.h
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/src/
--rw-r--r--   0 build      (114) build      (118)     3598 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/src/indexed_pcap_reader.cpp
--rw-r--r--   0 build      (114) build      (118)    13742 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/src/os_pcap.cpp
--rw-r--r--   0 build      (114) build      (118)    12531 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/sdk/ouster_pcap/src/pcap.cpp
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_viz/
--rw-r--r--   0 build      (114) build      (118)     1401 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/CMakeLists.txt
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_viz/include/
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_viz/include/ouster/
--rw-r--r--   0 build      (114) build      (118)    27365 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/include/ouster/point_viz.h
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/
--rw-r--r--   0 build      (114) build      (118)     7737 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/camera.cpp
--rw-r--r--   0 build      (114) build      (118)      524 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/camera.h
--rw-r--r--   0 build      (114) build      (118)    10438 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/cloud.cpp
--rw-r--r--   0 build      (114) build      (118)     1461 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/cloud.h
--rw-r--r--   0 build      (114) build      (118)    67424 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/colormaps.h
--rw-r--r--   0 build      (114) build      (118)    10693 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/common.h
--rw-r--r--   0 build      (114) build      (118)     8270 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/glfw.cpp
--rw-r--r--   0 build      (114) build      (118)     1427 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/glfw.h
--rw-r--r--   0 build      (114) build      (118)      163 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/gltext.cpp
--rw-r--r--   0 build      (114) build      (118)    40590 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/gltext.h
--rw-r--r--   0 build      (114) build      (118)     5832 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/image.cpp
--rw-r--r--   0 build      (114) build      (118)     1502 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/image.h
--rw-r--r--   0 build      (114) build      (118)    10319 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/misc.cpp
--rw-r--r--   0 build      (114) build      (118)     2918 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/misc.h
--rw-r--r--   0 build      (114) build      (118)    24828 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/ouster_viz/src/point_viz.cpp
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/tests/
--rw-r--r--   0 build      (114) build      (118)     2172 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/CMakeLists.txt
--rw-r--r--   0 build      (114) build      (118)     4085 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/tests/bcompat_meta_json_test.cpp
--rw-r--r--   0 build      (114) build      (118)    72409 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/tests/bcompat_sensor_info_data.h
--rw-r--r--   0 build      (114) build      (118)     8367 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/cartesian_test.cpp
--rw-r--r--   0 build      (114) build      (118)    11074 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/lidar_scan_test.cpp
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/tests/metadata/
--rw-r--r--   0 build      (114) build      (118)     4616 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_12_os1-991913000010-64.json
--rw-r--r--   0 build      (114) build      (118)     1629 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_12_os1-991937000062-16A0_legacy.json
--rw-r--r--   0 build      (114) build      (118)     1626 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_12_os1-991937000062-64_legacy.json
--rw-r--r--   0 build      (114) build      (118)     4657 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_13_os1-991913000010-64.json
--rw-r--r--   0 build      (114) build      (118)     1203 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_13_os1-991937000062-16A0_legacy.json
--rw-r--r--   0 build      (114) build      (118)     1348 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_13_os1-991937000062-32A02_legacy.json
--rw-r--r--   0 build      (114) build      (118)     1631 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_13_os1-991937000062-64_legacy.json
--rw-r--r--   0 build      (114) build      (118)     3275 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_14_6cccd_os-882002000138-128_legacy.json
--rw-r--r--   0 build      (114) build      (118)     1486 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_14_6cccd_os-882002000138-32U0_legacy.json
--rw-r--r--   0 build      (114) build      (118)     2073 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_14_6cccd_os-882002000138-64U02_legacy.json
--rw-r--r--   0 build      (114) build      (118)     3625 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_14_beta_os-882004000055-128_legacy.json
--rw-r--r--   0 build      (114) build      (118)     1187 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_14_beta_os1-991937000062-16A0_legacy.json
--rw-r--r--   0 build      (114) build      (118)     1487 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_14_beta_os1-991937000062-32A02_legacy.json
--rw-r--r--   0 build      (114) build      (118)     2079 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/1_14_beta_os1-991937000062-64_legacy.json
--rw-r--r--   0 build      (114) build      (118)     6052 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_0_0_os1-991913000010-64.json
--rw-r--r--   0 build      (114) build      (118)     3683 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_0_0_os1-992008000494-128_col_win_legacy.json
--rw-r--r--   0 build      (114) build      (118)     1622 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_0_rc2_os-992011000121-32U0_legacy.json
--rw-r--r--   0 build      (114) build      (118)     6150 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_1_2_os1-991913000010-64.json
--rw-r--r--   0 build      (114) build      (118)     4333 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_1_2_os1-991913000010-64_legacy.json
--rw-r--r--   0 build      (114) build      (118)     9621 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_2_os-992119000444-128.json
--rw-r--r--   0 build      (114) build      (118)     7194 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_2_os-992119000444-128_legacy.json
--rw-r--r--   0 build      (114) build      (118)     9671 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_3_1_os-992146000760-128.json
--rw-r--r--   0 build      (114) build      (118)     7231 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_3_1_os-992146000760-128_legacy.json
--rw-r--r--   0 build      (114) build      (118)     9648 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_3_os-992146000760-128.json
--rw-r--r--   0 build      (114) build      (118)     7217 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_3_os-992146000760-128_legacy.json
--rw-r--r--   0 build      (114) build      (118)     9608 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_4_0_os-992146000760-128.json
--rw-r--r--   0 build      (114) build      (118)     7225 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_4_0_os-992146000760-128_legacy.json
--rw-r--r--   0 build      (114) build      (118)     9922 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_5_0_os-992146000760-128.json
--rw-r--r--   0 build      (114) build      (118)     7476 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/tests/metadata/2_5_0_os-992146000760-128_legacy.json
--rw-r--r--   0 build      (114) build      (118)     9916 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/tests/metadata/3_0_1_os-122246000293-128.json
--rw-r--r--   0 build      (114) build      (118)     7466 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/sdk/tests/metadata/3_0_1_os-122246000293-128_legacy.json
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/tests/metadata/malformed/
--rw-r--r--   0 build      (114) build      (118)     6427 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/malformed/complete_but_all_zeros_legacy.json
--rw-r--r--   0 build      (114) build      (118)     4895 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/malformed/garbled_legacy_and_nonlegacy.json
--rw-r--r--   0 build      (114) build      (118)     7190 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/malformed/incomplete_data_format_legacy.json
--rw-r--r--   0 build      (114) build      (118)     9574 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/malformed/incomplete_data_format_nonlegacy.json
--rw-r--r--   0 build      (114) build      (118)     9464 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/malformed/incomplete_no_calref_nonlegacy.json
--rw-r--r--   0 build      (114) build      (118)     9256 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/malformed/incomplete_no_sensor_info_nonlegacy.json
--rw-r--r--   0 build      (114) build      (118)     1194 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/malformed/incorrect_nbeam_angles_legacy_113.json
--rw-r--r--   0 build      (114) build      (118)     7390 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/malformed/legacy_with_calibration_status.json
--rw-r--r--   0 build      (114) build      (118)     2600 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata/ouster-studio-reduced-config-v1.json
--rw-r--r--   0 build      (114) build      (118)     1960 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/metadata_errors_test.cpp
--rw-r--r--   0 build      (114) build      (118)     6036 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/sdk/tests/pcap_test.cpp
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/
--rw-r--r--   0 build      (114) build      (118)     7273 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10.json
--rw-r--r--   0 build      (114) build      (118)   545468 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10.pcap
--rw-r--r--   0 build      (114) build      (118)     1103 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10_digest.json
--rw-r--r--   0 build      (114) build      (118)     8530 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10-single-packet.pcap
--rw-r--r--   0 build      (114) build      (118)     1773 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10.json
--rw-r--r--   0 build      (114) build      (118)   545468 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10.pcap
--rw-r--r--   0 build      (114) build      (118)     1798 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10_digest.json
--rw-r--r--   0 build      (114) build      (118)     1441 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10.json
--rw-r--r--   0 build      (114) build      (118)   417432 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10.pcap
--rw-r--r--   0 build      (114) build      (118)     1155 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10_digest.json
--rw-r--r--   0 build      (114) build      (118)     7133 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10.json
--rw-r--r--   0 build      (114) build      (118)  1594044 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10.pcap
--rw-r--r--   0 build      (114) build      (118)     1333 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10_digest.json
--rw-r--r--   0 build      (114) build      (118)     1478 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10.json
--rw-r--r--   0 build      (114) build      (118)   417432 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10.pcap
--rw-r--r--   0 build      (114) build      (118)     1156 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10_digest.json
--rw-r--r--   0 build      (114) build      (118)     1098 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/setup.cfg
--rw-r--r--   0 build      (114) build      (118)     5556 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/setup.py
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/cpp/
--rw-r--r--   0 build      (114) build      (118)    50818 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/src/cpp/_client.cpp
--rw-r--r--   0 build      (114) build      (118)    10500 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/src/cpp/_pcap.cpp
--rw-r--r--   0 build      (114) build      (118)    34188 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/cpp/_viz.cpp
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster/
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster/client/
--rw-r--r--   0 build      (114) build      (118)     1232 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/src/ouster/client/__init__.py
--rw-r--r--   0 build      (114) build      (118)    16927 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/src/ouster/client/_client.pyi
--rw-r--r--   0 build      (114) build      (118)     5030 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/client/_digest.py
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster/client/_utils/
--rw-r--r--   0 build      (114) build      (118)      202 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/client/_utils/__init__.py
--rw-r--r--   0 build      (114) build      (118)    18508 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/src/ouster/client/core.py
--rw-r--r--   0 build      (114) build      (118)    13802 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/client/data.py
--rw-r--r--   0 build      (114) build      (118)        0 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/client/py.typed
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster/pcap/
--rw-r--r--   0 build      (114) build      (118)      296 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/pcap/__init__.py
--rw-r--r--   0 build      (114) build      (118)     2418 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/pcap/_pcap.pyi
--rw-r--r--   0 build      (114) build      (118)    10534 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/pcap/pcap.py
--rw-r--r--   0 build      (114) build      (118)        0 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/pcap/py.typed
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster/sdk/
--rw-r--r--   0 build      (114) build      (118)        0 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/__init__.py
--rw-r--r--   0 build      (114) build      (118)     6421 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/_viz.pyi
--rw-r--r--   0 build      (114) build      (118)      751 2023-03-29 00:36:03.000000 ouster-sdk-0.8.1/src/ouster/sdk/convert_to_legacy.py
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster/sdk/examples/
--rw-r--r--   0 build      (114) build      (118)      226 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/examples/__init__.py
--rw-r--r--   0 build      (114) build      (118)    10649 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/examples/client.py
--rw-r--r--   0 build      (114) build      (118)    19034 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/examples/colormaps.py
--rw-r--r--   0 build      (114) build      (118)    10629 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/examples/open3d.py
--rw-r--r--   0 build      (114) build      (118)    15416 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/examples/pcap.py
--rw-r--r--   0 build      (114) build      (118)     5943 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/examples/reference.py
--rw-r--r--   0 build      (114) build      (118)    12231 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/examples/viz.py
--rw-r--r--   0 build      (114) build      (118)        0 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/py.typed
--rw-r--r--   0 build      (114) build      (118)     3009 2023-04-03 20:58:19.000000 ouster-sdk-0.8.1/src/ouster/sdk/simple_viz.py
--rw-r--r--   0 build      (114) build      (118)     2964 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/util.py
--rw-r--r--   0 build      (114) build      (118)    36288 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/src/ouster/sdk/viz.py
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster_sdk.egg-info/
--rw-r--r--   0 build      (114) build      (118)     3251 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster_sdk.egg-info/PKG-INFO
--rw-r--r--   0 build      (114) build      (118)    10217 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 build      (114) build      (118)        1 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 build      (114) build      (118)      117 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster_sdk.egg-info/entry_points.txt
--rw-r--r--   0 build      (114) build      (118)        1 2023-04-03 20:58:57.000000 ouster-sdk-0.8.1/src/ouster_sdk.egg-info/not-zip-safe
--rw-r--r--   0 build      (114) build      (118)      400 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster_sdk.egg-info/requires.txt
--rw-r--r--   0 build      (114) build      (118)       11 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/src/ouster_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 build      (114) build      (118)        0 2023-04-03 20:58:58.000000 ouster-sdk-0.8.1/tests/
--rw-r--r--   0 build      (114) build      (118)        0 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/tests/__init__.py
--rw-r--r--   0 build      (114) build      (118)     3646 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/tests/conftest.py
--rw-r--r--   0 build      (114) build      (118)     7510 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/tests/test_batching.py
--rw-r--r--   0 build      (114) build      (118)    15564 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/tests/test_config.py
--rw-r--r--   0 build      (114) build      (118)    10103 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/tests/test_core.py
--rw-r--r--   0 build      (114) build      (118)    14423 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/tests/test_data.py
--rw-r--r--   0 build      (114) build      (118)     3989 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/tests/test_destagger.py
--rw-r--r--   0 build      (114) build      (118)     8371 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/tests/test_metadata.py
--rw-r--r--   0 build      (114) build      (118)    22905 2023-03-24 21:03:00.000000 ouster-sdk-0.8.1/tests/test_pcap.py
--rw-r--r--   0 build      (114) build      (118)    19966 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/tests/test_viz.py
--rw-r--r--   0 build      (114) build      (118)     5023 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/tests/test_xyzlut.py
--rw-r--r--   0 build      (114) build      (118)     2378 2023-03-23 21:17:09.000000 ouster-sdk-0.8.1/tox.ini
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/
+-rw-r--r--   0 build      (114) build      (118)     2894 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/CMakeLists.txt
+-rw-r--r--   0 build      (114) build      (118)      182 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/MANIFEST.in
+-rw-r--r--   0 build      (114) build      (118)     3319 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/PKG-INFO
+-rw-r--r--   0 build      (114) build      (118)     1678 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/README.rst
+-rw-r--r--   0 build      (114) build      (118)      514 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/mypy.ini
+-rw-r--r--   0 build      (114) build      (118)      250 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/pyproject.toml
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/
+-rw-r--r--   0 build      (114) build      (118)      138 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.clang-format
+-rw-r--r--   0 build      (114) build      (118)       37 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.clangd
+-rw-r--r--   0 build      (114) build      (118)       40 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.dockerignore
+-rw-r--r--   0 build      (114) build      (118)       35 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.git
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/.github/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 build      (114) build      (118)      817 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 build      (114) build      (118)     1064 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 build      (114) build      (118)      641 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 build      (114) build      (118)     1203 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.github/check_title_and_description.py
+-rw-r--r--   0 build      (114) build      (118)       62 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.github/pull_request_template.md
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/.github/workflows/
+-rw-r--r--   0 build      (114) build      (118)      685 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.github/workflows/check-commit-message.yml
+-rw-r--r--   0 build      (114) build      (118)      277 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/.gitignore
+-rw-r--r--   0 build      (114) build      (118)    25744 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/CHANGELOG.rst
+-rw-r--r--   0 build      (114) build      (118)     3449 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/CMakeLists.txt
+-rw-r--r--   0 build      (114) build      (118)     1070 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/CMakeSettings.json
+-rw-r--r--   0 build      (114) build      (118)     3219 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/LICENSE
+-rw-r--r--   0 build      (114) build      (118)    14183 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/LICENSE-bin
+-rw-r--r--   0 build      (114) build      (118)     1920 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/README.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/cmake/
+-rw-r--r--   0 build      (114) build      (118)      361 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/DefaultBuildType.cmake
+-rw-r--r--   0 build      (114) build      (118)     1292 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/FindCURL.cmake
+-rw-r--r--   0 build      (114) build      (118)      401 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/FindEigen3.cmake
+-rw-r--r--   0 build      (114) build      (118)     1887 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/FindGTest.cmake
+-rw-r--r--   0 build      (114) build      (118)      217 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/FindOusterSDK.cmake
+-rw-r--r--   0 build      (114) build      (118)      842 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/FindPcap.cmake
+-rw-r--r--   0 build      (114) build      (118)     2067 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/FindPybind11Internal.cmake
+-rw-r--r--   0 build      (114) build      (118)      471 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/Findglfw3.cmake
+-rw-r--r--   0 build      (114) build      (118)     1980 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/Findjsoncpp.cmake
+-rw-r--r--   0 build      (114) build      (118)     2325 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/Findlibtins.cmake
+-rw-r--r--   0 build      (114) build      (118)      890 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/OusterSDKConfig.cmake.in
+-rw-r--r--   0 build      (114) build      (118)      852 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/VcpkgEnv.cmake
+-rw-r--r--   0 build      (114) build      (118)     1897 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/VersionGen.cmake
+-rw-r--r--   0 build      (114) build      (118)      383 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/cmake/build.h.in
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/conan/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/conan/test_package/
+-rw-r--r--   0 build      (114) build      (118)      142 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/conan/test_package/CMakeLists.txt
+-rw-r--r--   0 build      (114) build      (118)     1215 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/conan/test_package/conanfile.py
+-rw-r--r--   0 build      (114) build      (118)     4679 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/conanfile.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/
+-rw-r--r--   0 build      (114) build      (118)   114140 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/Doxyfile
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/_static/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/_static/css/
+-rw-r--r--   0 build      (114) build      (118)     1100 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/_static/css/ouster_rtd_tweaks.css
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/cli/
+-rw-r--r--   0 build      (114) build      (118)       64 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cli/changelog.rst
+-rw-r--r--   0 build      (114) build      (118)     4086 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cli/common-use-cases.rst
+-rw-r--r--   0 build      (114) build      (118)     3394 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cli/getting-started.rst
+-rw-r--r--   0 build      (114) build      (118)      467 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cli/overview.rst
+-rw-r--r--   0 build      (114) build      (118)     3275 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cli/sample-sessions.rst
+-rw-r--r--   0 build      (114) build      (118)     6937 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/conf.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/cpp/
+-rw-r--r--   0 build      (114) build      (118)      201 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/api.rst
+-rw-r--r--   0 build      (114) build      (118)     5393 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/building.rst
+-rw-r--r--   0 build      (114) build      (118)     5891 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/examples.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_client/
+-rw-r--r--   0 build      (114) build      (118)      891 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_client/client.rst
+-rw-r--r--   0 build      (114) build      (118)      230 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_client/image_processing.rst
+-rw-r--r--   0 build      (114) build      (118)      253 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_client/index.rst
+-rw-r--r--   0 build      (114) build      (118)      827 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_client/lidar_scan.rst
+-rw-r--r--   0 build      (114) build      (118)     3818 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_client/types.rst
+-rw-r--r--   0 build      (114) build      (118)      307 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_client/version.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_pcap/
+-rw-r--r--   0 build      (114) build      (118)      119 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_pcap/index.rst
+-rw-r--r--   0 build      (114) build      (118)     1340 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_pcap/os_pcap.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_viz/
+-rw-r--r--   0 build      (114) build      (118)      119 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_viz/index.rst
+-rw-r--r--   0 build      (114) build      (118)      556 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/cpp/ouster_viz/point_viz.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/images/
+-rw-r--r--   0 build      (114) build      (118)     9472 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/Ouster_Logo_TM_Horiz_Black_RGB_600px.png
+-rw-r--r--   0 build      (114) build      (118)     2455 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/Ouster_Logo_TM_Horiz_White_RGB.svg
+-rw-r--r--   0 build      (114) build      (118)     2528 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/Ouster_Logo_TM_Stacked_White_RGB.svg
+-rw-r--r--   0 build      (114) build      (118)    61758 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/brooklyn_bridge_ls_50_range_image.png
+-rw-r--r--   0 build      (114) build      (118)   452167 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/brooklyn_bridge_ls_50_xyz_cut.png
+-rw-r--r--   0 build      (114) build      (118)   143035 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/lidar_scan_destaggered.png
+-rw-r--r--   0 build      (114) build      (118)   148784 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/lidar_scan_staggered.png
+-rw-r--r--   0 build      (114) build      (118)   829483 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/lidar_scan_xyz_84.png
+-rw-r--r--   0 build      (114) build      (118)   570786 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/lidar_scan_xyz_84_3d.png
+-rw-r--r--   0 build      (114) build      (118)   290021 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/simple-viz.png
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/
+-rw-r--r--   0 build      (114) build      (118)   217741 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/axes_helper_unstructured.png
+-rw-r--r--   0 build      (114) build      (118)     2181 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/empty_point_viz.png
+-rw-r--r--   0 build      (114) build      (118)     4656 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/image_set_pos_bot_right.png
+-rw-r--r--   0 build      (114) build      (118)     5515 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/image_set_pos_center.png
+-rw-r--r--   0 build      (114) build      (118)     4683 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/image_set_pos_left.png
+-rw-r--r--   0 build      (114) build      (118)     4648 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/image_set_pos_right.png
+-rw-r--r--   0 build      (114) build      (118)    90497 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_fields_images.png
+-rw-r--r--   0 build      (114) build      (118)    90193 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_fields_images_labels.png
+-rw-r--r--   0 build      (114) build      (118)   238846 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_structured.png
+-rw-r--r--   0 build      (114) build      (118)   154619 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_viz.png
+-rw-r--r--   0 build      (114) build      (118)   151016 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_viz_checkers.png
+-rw-r--r--   0 build      (114) build      (118)   159107 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_viz_labels.png
+-rw-r--r--   0 build      (114) build      (118)     1687 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/index.rst
+-rw-r--r--   0 build      (114) build      (118)     4121 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/installation.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/migration/
+-rw-r--r--   0 build      (114) build      (118)     5050 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/migration/migration-20220927-20230114.rst
+-rw-r--r--   0 build      (114) build      (118)     5919 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/migration/migration-20230114-20230403.rst
+-rw-r--r--   0 build      (114) build      (118)     3558 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/overview.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/python/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/python/api/
+-rw-r--r--   0 build      (114) build      (118)     1596 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/api/client.rst
+-rw-r--r--   0 build      (114) build      (118)      997 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/api/examples.rst
+-rw-r--r--   0 build      (114) build      (118)       95 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/api/index.rst
+-rw-r--r--   0 build      (114) build      (118)      167 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/api/pcap.rst
+-rw-r--r--   0 build      (114) build      (118)     1318 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/api/viz.rst
+-rw-r--r--   0 build      (114) build      (118)     6042 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/devel.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/python/examples/
+-rw-r--r--   0 build      (114) build      (118)     3131 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/examples/basics-sensor.rst
+-rw-r--r--   0 build      (114) build      (118)     3551 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/examples/conversion.rst
+-rw-r--r--   0 build      (114) build      (118)      846 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/examples/index.rst
+-rw-r--r--   0 build      (114) build      (118)     5540 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/examples/lidar-scan.rst
+-rw-r--r--   0 build      (114) build      (118)     2345 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/examples/record-stream.rst
+-rw-r--r--   0 build      (114) build      (118)     1203 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/examples/udp-packets.rst
+-rw-r--r--   0 build      (114) build      (118)     7749 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/examples/visualizations.rst
+-rw-r--r--   0 build      (114) build      (118)     5442 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/quickstart.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/python/viz/
+-rw-r--r--   0 build      (114) build      (118)     1088 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/viz/index.rst
+-rw-r--r--   0 build      (114) build      (118)    12817 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/viz/viz-api-tutorial.rst
+-rw-r--r--   0 build      (114) build      (118)     3475 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/python/viz/viz-run.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/docs/reference/
+-rw-r--r--   0 build      (114) build      (118)       66 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/reference/changelog.rst
+-rw-r--r--   0 build      (114) build      (118)     8871 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/reference/lidar-scan.rst
+-rw-r--r--   0 build      (114) build      (118)     1807 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/docs/sample-data.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/examples/
+-rw-r--r--   0 build      (114) build      (118)     1371 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/examples/CMakeLists.txt
+-rw-r--r--   0 build      (114) build      (118)     7495 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/examples/client_example.cpp
+-rw-r--r--   0 build      (114) build      (118)     4510 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/examples/config_example.cpp
+-rw-r--r--   0 build      (114) build      (118)     1477 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/examples/helpers.cpp
+-rw-r--r--   0 build      (114) build      (118)      419 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/examples/helpers.h
+-rw-r--r--   0 build      (114) build      (118)     5748 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/examples/lidar_scan_example.cpp
+-rw-r--r--   0 build      (114) build      (118)     2484 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/examples/mtp_client_example.cpp
+-rw-r--r--   0 build      (114) build      (118)     1490 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/examples/osf_reader_example.cpp
+-rw-r--r--   0 build      (114) build      (118)     6603 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/examples/representations_example.cpp
+-rw-r--r--   0 build      (114) build      (118)     1870 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/examples/viz_example.cpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_client/
+-rw-r--r--   0 build      (114) build      (118)     1811 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/CMakeLists.txt
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/optional-lite/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/optional-lite/nonstd/
+-rw-r--r--   0 build      (114) build      (118)    52100 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/optional-lite/nonstd/optional.hpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/
+-rw-r--r--   0 build      (114) build      (118)     5100 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/buffered_udp_source.h
+-rw-r--r--   0 build      (114) build      (118)     9759 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/client.h
+-rw-r--r--   0 build      (114) build      (118)       71 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/defaults.h
+-rw-r--r--   0 build      (114) build      (118)     3422 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/image_processing.h
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/impl/
+-rw-r--r--   0 build      (114) build      (118)     2495 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/impl/cartesian.h
+-rw-r--r--   0 build      (114) build      (118)     9835 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/impl/lidar_scan_impl.h
+-rw-r--r--   0 build      (114) build      (118)      555 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/impl/profile_extension.h
+-rw-r--r--   0 build      (114) build      (118)    15235 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/lidar_scan.h
+-rw-r--r--   0 build      (114) build      (118)     3878 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/sensor_http.h
+-rw-r--r--   0 build      (114) build      (118)    34721 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/types.h
+-rw-r--r--   0 build      (114) build      (118)     2936 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/version.h
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/
+-rw-r--r--   0 build      (114) build      (118)     6773 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/buffered_udp_source.cpp
+-rw-r--r--   0 build      (114) build      (118)    22142 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/client.cpp
+-rw-r--r--   0 build      (114) build      (118)     3610 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/curl_client.h
+-rw-r--r--   0 build      (114) build      (118)     1212 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/http_client.h
+-rw-r--r--   0 build      (114) build      (118)     8265 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/image_processing.cpp
+-rw-r--r--   0 build      (114) build      (118)    23835 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/lidar_scan.cpp
+-rw-r--r--   0 build      (114) build      (118)     3197 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/logging.cpp
+-rw-r--r--   0 build      (114) build      (118)      810 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/logging.h
+-rw-r--r--   0 build      (114) build      (118)     2447 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/netcompat.cpp
+-rw-r--r--   0 build      (114) build      (118)     2051 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/netcompat.h
+-rw-r--r--   0 build      (114) build      (118)    17481 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/parsing.cpp
+-rw-r--r--   0 build      (114) build      (118)     4957 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/profile_extension.cpp
+-rw-r--r--   0 build      (114) build      (118)     2061 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/sensor_http.cpp
+-rw-r--r--   0 build      (114) build      (118)     5054 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/sensor_http_imp.cpp
+-rw-r--r--   0 build      (114) build      (118)     4822 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/sensor_http_imp.h
+-rw-r--r--   0 build      (114) build      (118)     6866 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/sensor_tcp_imp.cpp
+-rw-r--r--   0 build      (114) build      (118)     3701 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/sensor_tcp_imp.h
+-rw-r--r--   0 build      (114) build      (118)    50366 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_client/src/types.cpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_osf/
+-rw-r--r--   0 build      (114) build      (118)       97 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/CHANGELOG.rst
+-rw-r--r--   0 build      (114) build      (118)     5782 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/CMakeLists.txt
+-rw-r--r--   0 build      (114) build      (118)      701 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/README.rst
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_osf/cmake/
+-rw-r--r--   0 build      (114) build      (118)    13574 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/cmake/osf_fb_utils.cmake
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_osf/fb/
+-rw-r--r--   0 build      (114) build      (118)      722 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/fb/chunk.fbs
+-rw-r--r--   0 build      (114) build      (118)     1042 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/fb/header.fbs
+-rw-r--r--   0 build      (114) build      (118)     1083 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/fb/metadata.fbs
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_osf/fb/os_sensor/
+-rw-r--r--   0 build      (114) build      (118)      477 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/fb/os_sensor/extrinsics.fbs
+-rw-r--r--   0 build      (114) build      (118)     2218 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/fb/os_sensor/lidar_scan_stream.fbs
+-rw-r--r--   0 build      (114) build      (118)      242 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/fb/os_sensor/lidar_sensor.fbs
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_osf/fb/streaming/
+-rw-r--r--   0 build      (114) build      (118)     1445 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/fb/streaming/streaming_info.fbs
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/
+-rw-r--r--   0 build      (114) build      (118)     5296 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/basics.h
+-rw-r--r--   0 build      (114) build      (118)      919 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/crc32.h
+-rw-r--r--   0 build      (114) build      (118)     4492 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/file.h
+-rw-r--r--   0 build      (114) build      (118)     1140 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/layout_standard.h
+-rw-r--r--   0 build      (114) build      (118)     1861 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/layout_streaming.h
+-rw-r--r--   0 build      (114) build      (118)     1918 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/meta_extrinsics.h
+-rw-r--r--   0 build      (114) build      (118)     2718 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/meta_lidar_sensor.h
+-rw-r--r--   0 build      (114) build      (118)     2703 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/meta_streaming_info.h
+-rw-r--r--   0 build      (114) build      (118)    14319 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/metadata.h
+-rw-r--r--   0 build      (114) build      (118)     1177 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/operations.h
+-rw-r--r--   0 build      (114) build      (118)     2904 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/pcap_source.h
+-rw-r--r--   0 build      (114) build      (118)    16169 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/reader.h
+-rw-r--r--   0 build      (114) build      (118)     4145 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/stream_lidar_scan.h
+-rw-r--r--   0 build      (114) build      (118)     4905 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/include/ouster/osf/writer.h
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/
+-rw-r--r--   0 build      (114) build      (118)     4425 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/basics.cpp
+-rw-r--r--   0 build      (114) build      (118)     8022 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/compat_ops.cpp
+-rw-r--r--   0 build      (114) build      (118)     1270 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/compat_ops.h
+-rw-r--r--   0 build      (114) build      (118)      625 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/crc32.cpp
+-rw-r--r--   0 build      (114) build      (118)     6209 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/fb_utils.cpp
+-rw-r--r--   0 build      (114) build      (118)     4466 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/fb_utils.h
+-rw-r--r--   0 build      (114) build      (118)    11433 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/file.cpp
+-rw-r--r--   0 build      (114) build      (118)      743 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/json_utils.cpp
+-rw-r--r--   0 build      (114) build      (118)      302 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/json_utils.h
+-rw-r--r--   0 build      (114) build      (118)     1079 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/layout_standard.cpp
+-rw-r--r--   0 build      (114) build      (118)     2795 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/layout_streaming.cpp
+-rw-r--r--   0 build      (114) build      (118)     2141 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/meta_extrinsics.cpp
+-rw-r--r--   0 build      (114) build      (118)     1995 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/meta_lidar_sensor.cpp
+-rw-r--r--   0 build      (114) build      (118)     5300 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/meta_streaming_info.cpp
+-rw-r--r--   0 build      (114) build      (118)     2886 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/metadata.cpp
+-rw-r--r--   0 build      (114) build      (118)     7805 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/operations.cpp
+-rw-r--r--   0 build      (114) build      (118)     2367 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/pcap_source.cpp
+-rw-r--r--   0 build      (114) build      (118)    52619 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/png_tools.cpp
+-rw-r--r--   0 build      (114) build      (118)    14067 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/png_tools.h
+-rw-r--r--   0 build      (114) build      (118)    37990 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/reader.cpp
+-rw-r--r--   0 build      (114) build      (118)    14183 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/stream_lidar_scan.cpp
+-rw-r--r--   0 build      (114) build      (118)     7008 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/src/writer.cpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/
+-rw-r--r--   0 build      (114) build      (118)     1383 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/CMakeLists.txt
+-rw-r--r--   0 build      (114) build      (118)     5298 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/common.h
+-rw-r--r--   0 build      (114) build      (118)      751 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/crc_test.cpp
+-rw-r--r--   0 build      (114) build      (118)     4327 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/file_ops_test.cpp
+-rw-r--r--   0 build      (114) build      (118)     4607 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/file_test.cpp
+-rw-r--r--   0 build      (114) build      (118)     2534 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/operations_test.cpp
+-rw-r--r--   0 build      (114) build      (118)     1459 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/osf_test.h
+-rw-r--r--   0 build      (114) build      (118)     1042 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/pcap_source_test.cpp
+-rw-r--r--   0 build      (114) build      (118)    12486 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/png_tools_test.cpp
+-rw-r--r--   0 build      (114) build      (118)     5252 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/reader_test.cpp
+-rw-r--r--   0 build      (114) build      (118)     4475 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/writer_custom_test.cpp
+-rw-r--r--   0 build      (114) build      (118)    19459 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_osf/tests/writer_test.cpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/
+-rw-r--r--   0 build      (114) build      (118)      938 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/CMakeLists.txt
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/include/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/include/ouster/
+-rw-r--r--   0 build      (114) build      (118)     2926 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/include/ouster/indexed_pcap_reader.h
+-rw-r--r--   0 build      (114) build      (118)    11139 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/include/ouster/os_pcap.h
+-rw-r--r--   0 build      (114) build      (118)     6597 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/include/ouster/pcap.h
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/src/
+-rw-r--r--   0 build      (114) build      (118)     2769 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/src/indexed_pcap_reader.cpp
+-rw-r--r--   0 build      (114) build      (118)    12979 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/src/os_pcap.cpp
+-rw-r--r--   0 build      (114) build      (118)    12895 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_pcap/src/pcap.cpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_viz/
+-rw-r--r--   0 build      (114) build      (118)     1401 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/CMakeLists.txt
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_viz/include/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_viz/include/ouster/
+-rw-r--r--   0 build      (114) build      (118)    27897 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/include/ouster/point_viz.h
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/
+-rw-r--r--   0 build      (114) build      (118)     7737 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/camera.cpp
+-rw-r--r--   0 build      (114) build      (118)      524 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/camera.h
+-rw-r--r--   0 build      (114) build      (118)    10438 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/cloud.cpp
+-rw-r--r--   0 build      (114) build      (118)     1461 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/cloud.h
+-rw-r--r--   0 build      (114) build      (118)    67424 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/colormaps.h
+-rw-r--r--   0 build      (114) build      (118)    10693 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/common.h
+-rw-r--r--   0 build      (114) build      (118)     8270 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/glfw.cpp
+-rw-r--r--   0 build      (114) build      (118)     1427 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/glfw.h
+-rw-r--r--   0 build      (114) build      (118)      163 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/gltext.cpp
+-rw-r--r--   0 build      (114) build      (118)    40590 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/gltext.h
+-rw-r--r--   0 build      (114) build      (118)     5832 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/image.cpp
+-rw-r--r--   0 build      (114) build      (118)     1502 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/image.h
+-rw-r--r--   0 build      (114) build      (118)    10319 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/misc.cpp
+-rw-r--r--   0 build      (114) build      (118)     2918 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/misc.h
+-rw-r--r--   0 build      (114) build      (118)    25546 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/ouster_viz/src/point_viz.cpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/tests/
+-rw-r--r--   0 build      (114) build      (118)     2454 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/CMakeLists.txt
+-rw-r--r--   0 build      (114) build      (118)     4085 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/bcompat_meta_json_test.cpp
+-rw-r--r--   0 build      (114) build      (118)    72409 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/bcompat_sensor_info_data.h
+-rw-r--r--   0 build      (114) build      (118)     8367 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/cartesian_test.cpp
+-rw-r--r--   0 build      (114) build      (118)    11074 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/lidar_scan_test.cpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/tests/metadata/
+-rw-r--r--   0 build      (114) build      (118)     4616 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_12_os1-991913000010-64.json
+-rw-r--r--   0 build      (114) build      (118)     1629 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_12_os1-991937000062-16A0_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     1626 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_12_os1-991937000062-64_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     4657 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_13_os1-991913000010-64.json
+-rw-r--r--   0 build      (114) build      (118)     1203 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_13_os1-991937000062-16A0_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     1348 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_13_os1-991937000062-32A02_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     1631 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_13_os1-991937000062-64_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     3275 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_14_6cccd_os-882002000138-128_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     1486 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_14_6cccd_os-882002000138-32U0_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     2073 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_14_6cccd_os-882002000138-64U02_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     3625 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_14_beta_os-882004000055-128_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     1187 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_14_beta_os1-991937000062-16A0_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     1487 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_14_beta_os1-991937000062-32A02_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     2079 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/1_14_beta_os1-991937000062-64_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     6052 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_0_0_os1-991913000010-64.json
+-rw-r--r--   0 build      (114) build      (118)     3683 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_0_0_os1-992008000494-128_col_win_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     1622 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_0_rc2_os-992011000121-32U0_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     6150 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_1_2_os1-991913000010-64.json
+-rw-r--r--   0 build      (114) build      (118)     4333 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_1_2_os1-991913000010-64_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     9621 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_2_os-992119000444-128.json
+-rw-r--r--   0 build      (114) build      (118)     7194 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_2_os-992119000444-128_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     9671 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_3_1_os-992146000760-128.json
+-rw-r--r--   0 build      (114) build      (118)     7231 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_3_1_os-992146000760-128_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     9648 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_3_os-992146000760-128.json
+-rw-r--r--   0 build      (114) build      (118)     7217 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_3_os-992146000760-128_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     9608 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_4_0_os-992146000760-128.json
+-rw-r--r--   0 build      (114) build      (118)     7225 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_4_0_os-992146000760-128_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     9922 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_5_0_os-992146000760-128.json
+-rw-r--r--   0 build      (114) build      (118)     7476 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/2_5_0_os-992146000760-128_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     9916 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/3_0_1_os-122246000293-128.json
+-rw-r--r--   0 build      (114) build      (118)     7466 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/3_0_1_os-122246000293-128_legacy.json
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/tests/metadata/malformed/
+-rw-r--r--   0 build      (114) build      (118)     6427 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/malformed/complete_but_all_zeros_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     4895 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/malformed/garbled_legacy_and_nonlegacy.json
+-rw-r--r--   0 build      (114) build      (118)     7190 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/malformed/incomplete_data_format_legacy.json
+-rw-r--r--   0 build      (114) build      (118)     9574 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/malformed/incomplete_data_format_nonlegacy.json
+-rw-r--r--   0 build      (114) build      (118)     9464 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/malformed/incomplete_no_calref_nonlegacy.json
+-rw-r--r--   0 build      (114) build      (118)     9256 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/malformed/incomplete_no_sensor_info_nonlegacy.json
+-rw-r--r--   0 build      (114) build      (118)     1194 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/malformed/incorrect_nbeam_angles_legacy_113.json
+-rw-r--r--   0 build      (114) build      (118)     7390 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/malformed/legacy_with_calibration_status.json
+-rw-r--r--   0 build      (114) build      (118)     2600 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata/ouster-studio-reduced-config-v1.json
+-rw-r--r--   0 build      (114) build      (118)     1960 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/metadata_errors_test.cpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/tests/osfs/
+-rw-r--r--   0 build      (114) build      (118)  1021684 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/osfs/OS-1-128_v2.3.0_1024x10_lb_n3.osf
+-rw-r--r--   0 build      (114) build      (118)     6543 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcap_test.cpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/
+-rw-r--r--   0 build      (114) build      (118)     7273 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10.json
+-rw-r--r--   0 build      (114) build      (118)   545468 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10.pcap
+-rw-r--r--   0 build      (114) build      (118)     1103 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10_digest.json
+-rw-r--r--   0 build      (114) build      (118)     8530 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10-single-packet.pcap
+-rw-r--r--   0 build      (114) build      (118)     1773 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10.json
+-rw-r--r--   0 build      (114) build      (118)   545468 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10.pcap
+-rw-r--r--   0 build      (114) build      (118)     1798 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10_digest.json
+-rw-r--r--   0 build      (114) build      (118)     7187 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-1-128_v2.3.0_1024x10.json
+-rw-r--r--   0 build      (114) build      (118)  1636356 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-1-128_v2.3.0_1024x10_lb_n3.pcap
+-rw-r--r--   0 build      (114) build      (118)      908 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-1-128_v2.3.0_1024x10_lb_n3_poses_kitti.txt
+-rw-r--r--   0 build      (114) build      (118)   340956 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-1-128_v3.0.1_1024x10_20230216_142857_poses_kitti.txt
+-rw-r--r--   0 build      (114) build      (118)     1441 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10.json
+-rw-r--r--   0 build      (114) build      (118)   417432 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10.pcap
+-rw-r--r--   0 build      (114) build      (118)     1155 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10_digest.json
+-rw-r--r--   0 build      (114) build      (118)     7133 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10.json
+-rw-r--r--   0 build      (114) build      (118)  1594044 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10.pcap
+-rw-r--r--   0 build      (114) build      (118)     1333 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10_digest.json
+-rw-r--r--   0 build      (114) build      (118)     1478 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10.json
+-rw-r--r--   0 build      (114) build      (118)   417432 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10.pcap
+-rw-r--r--   0 build      (114) build      (118)     1156 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10_digest.json
+-rw-r--r--   0 build      (114) build      (118)     1294 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/pcaps/VLI-16-one-packet.pcap
+-rw-r--r--   0 build      (114) build      (118)     2203 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/sdk/tests/profile_extension_test.cpp
+-rw-r--r--   0 build      (114) build      (118)     1138 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/setup.cfg
+-rw-r--r--   0 build      (114) build      (118)     6936 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/setup.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/cpp/
+-rw-r--r--   0 build      (114) build      (118)    52053 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/cpp/_client.cpp
+-rw-r--r--   0 build      (114) build      (118)    34575 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/cpp/_osf.cpp
+-rw-r--r--   0 build      (114) build      (118)    10693 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/cpp/_pcap.cpp
+-rw-r--r--   0 build      (114) build      (118)    33491 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/cpp/_viz.cpp
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/cli/
+-rw-r--r--   0 build      (114) build      (118)      123 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/__init__.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/cli/core/
+-rw-r--r--   0 build      (114) build      (118)     8229 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/core/__init__.py
+-rw-r--r--   0 build      (114) build      (118)      240 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/core/borg.py
+-rw-r--r--   0 build      (114) build      (118)      759 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/core/cli_args.py
+-rw-r--r--   0 build      (114) build      (118)     5867 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/core/osf.py
+-rw-r--r--   0 build      (114) build      (118)    36215 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/core/pcap.py
+-rw-r--r--   0 build      (114) build      (118)    13340 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/core/sensor.py
+-rw-r--r--   0 build      (114) build      (118)    11178 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/core/util.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/cli/plugins/
+-rw-r--r--   0 build      (114) build      (118)     4827 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/plugins/discover.py
+-rw-r--r--   0 build      (114) build      (118)     3319 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/plugins/io_type.py
+-rw-r--r--   0 build      (114) build      (118)    19556 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/plugins/source.py
+-rw-r--r--   0 build      (114) build      (118)     3252 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/plugins/source_mapping.py
+-rw-r--r--   0 build      (114) build      (118)     5641 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/plugins/source_osf.py
+-rw-r--r--   0 build      (114) build      (118)     3368 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/plugins/testing.py
+-rw-r--r--   0 build      (114) build      (118)        0 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/cli/py.typed
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/client/
+-rw-r--r--   0 build      (114) build      (118)     1583 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/client/__init__.py
+-rw-r--r--   0 build      (114) build      (118)    17484 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/client/_client.pyi
+-rw-r--r--   0 build      (114) build      (118)     5030 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/client/_digest.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/client/_utils/
+-rw-r--r--   0 build      (114) build      (118)      202 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/client/_utils/__init__.py
+-rw-r--r--   0 build      (114) build      (118)    20217 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/client/core.py
+-rw-r--r--   0 build      (114) build      (118)    15904 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/client/data.py
+-rw-r--r--   0 build      (114) build      (118)        0 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/client/py.typed
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/osf/
+-rw-r--r--   0 build      (114) build      (118)      616 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/osf/__init__.py
+-rw-r--r--   0 build      (114) build      (118)     5418 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/osf/_osf.pyi
+-rw-r--r--   0 build      (114) build      (118)     7556 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/osf/data.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/pcap/
+-rw-r--r--   0 build      (114) build      (118)      296 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/pcap/__init__.py
+-rw-r--r--   0 build      (114) build      (118)     2418 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/pcap/_pcap.pyi
+-rw-r--r--   0 build      (114) build      (118)    11367 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/pcap/pcap.py
+-rw-r--r--   0 build      (114) build      (118)        0 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/pcap/py.typed
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/sdk/
+-rw-r--r--   0 build      (114) build      (118)        0 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/__init__.py
+-rw-r--r--   0 build      (114) build      (118)     6421 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/_viz.pyi
+-rw-r--r--   0 build      (114) build      (118)      751 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/convert_to_legacy.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/sdk/examples/
+-rw-r--r--   0 build      (114) build      (118)      226 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/examples/__init__.py
+-rw-r--r--   0 build      (114) build      (118)    10649 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/examples/client.py
+-rw-r--r--   0 build      (114) build      (118)    19034 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/examples/colormaps.py
+-rw-r--r--   0 build      (114) build      (118)    10629 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/examples/open3d.py
+-rw-r--r--   0 build      (114) build      (118)    11217 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/examples/pcap.py
+-rw-r--r--   0 build      (114) build      (118)     5943 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/examples/reference.py
+-rw-r--r--   0 build      (114) build      (118)    12231 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/examples/viz.py
+-rw-r--r--   0 build      (114) build      (118)    25522 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/pose_util.py
+-rw-r--r--   0 build      (114) build      (118)        0 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/py.typed
+-rw-r--r--   0 build      (114) build      (118)      252 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/simple_viz.py
+-rw-r--r--   0 build      (114) build      (118)     3645 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/util.py
+-rw-r--r--   0 build      (114) build      (118)    46040 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/viz.py
+-rw-r--r--   0 build      (114) build      (118)     3310 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdk/viz_util.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/sdkx/
+-rw-r--r--   0 build      (114) build      (118)      190 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/__init__.py
+-rw-r--r--   0 build      (114) build      (118)     3506 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/bag.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster/sdkx/mapping/
+-rw-r--r--   0 build      (114) build      (118)      235 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/mapping/README.rst
+-rw-r--r--   0 build      (114) build      (118)       21 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/mapping/__init__.py
+-rw-r--r--   0 build      (114) build      (118)     2620 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/mapping/kiss_backend.py
+-rw-r--r--   0 build      (114) build      (118)    14621 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/mapping/mapping.py
+-rw-r--r--   0 build      (114) build      (118)      120 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/mapping/slam.py
+-rw-r--r--   0 build      (114) build      (118)      624 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/mapping/slam_backend.py
+-rw-r--r--   0 build      (114) build      (118)     3846 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/mapping/util.py
+-rw-r--r--   0 build      (114) build      (118)     6484 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/packet_iter.py
+-rw-r--r--   0 build      (114) build      (118)    30535 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/parsing.py
+-rw-r--r--   0 build      (114) build      (118)        0 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/py.typed
+-rw-r--r--   0 build      (114) build      (118)     7153 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/src/ouster/sdkx/util.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster_sdk.egg-info/
+-rw-r--r--   0 build      (114) build      (118)     3319 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 build      (114) build      (118)    14685 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 build      (114) build      (118)        1 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 build      (114) build      (118)      150 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 build      (114) build      (118)        1 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 build      (114) build      (118)      723 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster_sdk.egg-info/requires.txt
+-rw-r--r--   0 build      (114) build      (118)       11 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/src/ouster_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/tests/
+-rw-r--r--   0 build      (114) build      (118)        0 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/__init__.py
+-rw-r--r--   0 build      (114) build      (118)     4011 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/conftest.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/tests/osf/
+-rw-r--r--   0 build      (114) build      (118)     3343 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/osf/test_osf_basics.py
+-rw-r--r--   0 build      (114) build      (118)     1289 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/osf/test_osf_extrinsics.py
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/tests/ouster/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/tests/ouster/cli/
+drwxr-xr-x   0 build      (114) build      (118)        0 2023-07-07 21:18:00.000000 ouster-sdk-0.9.0/tests/ouster/cli/plugins/
+-rw-r--r--   0 build      (114) build      (118)       32 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/ouster/cli/plugins/bad_plugin.py
+-rw-r--r--   0 build      (114) build      (118)     7510 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_batching.py
+-rw-r--r--   0 build      (114) build      (118)    18598 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_cli.py
+-rw-r--r--   0 build      (114) build      (118)     1433 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_cli_util.py
+-rw-r--r--   0 build      (114) build      (118)    15564 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_config.py
+-rw-r--r--   0 build      (114) build      (118)    10269 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_core.py
+-rw-r--r--   0 build      (114) build      (118)    19830 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_data.py
+-rw-r--r--   0 build      (114) build      (118)     3989 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_destagger.py
+-rw-r--r--   0 build      (114) build      (118)     2715 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_discover.py
+-rw-r--r--   0 build      (114) build      (118)     2053 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_extended_profiles.py
+-rw-r--r--   0 build      (114) build      (118)     1417 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_http_client.py
+-rw-r--r--   0 build      (114) build      (118)     1594 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_mapping.py
+-rw-r--r--   0 build      (114) build      (118)     9084 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_metadata.py
+-rw-r--r--   0 build      (114) build      (118)     4765 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_packet_iter.py
+-rw-r--r--   0 build      (114) build      (118)    23984 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_pcap.py
+-rw-r--r--   0 build      (114) build      (118)     1367 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_plugins.py
+-rw-r--r--   0 build      (114) build      (118)     2133 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_pose.py
+-rw-r--r--   0 build      (114) build      (118)     8022 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_pose_util.py
+-rw-r--r--   0 build      (114) build      (118)    19966 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_viz.py
+-rw-r--r--   0 build      (114) build      (118)    13130 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_viz_utils.py
+-rw-r--r--   0 build      (114) build      (118)     5023 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tests/test_xyzlut.py
+-rw-r--r--   0 build      (114) build      (118)     2385 2023-07-07 21:15:26.000000 ouster-sdk-0.9.0/tox.ini
```

### Comparing `ouster-sdk-0.8.1/CMakeLists.txt` & `ouster-sdk-0.9.0/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,19 @@
   add_compile_options(/W2 /wd4996)
   add_compile_definitions(NOMINMAX _USE_MATH_DEFINES WIN32_LEAN_AND_MEAN)
 else()
   add_compile_options(-Wall -Wextra -Wno-error=deprecated-declarations)
 endif()
 
 option(BUILD_VIZ "Enabled for Python build" ON)
+option(BUILD_OSF "Build OSF library." ON)
 option(BUILD_PCAP "Enabled for Python build" ON)
 
 # ==== Requirements ====
-find_package(pybind11 2.0 REQUIRED)
+find_package(Pybind11Internal)
 find_package(Eigen3 REQUIRED)
 find_package(OusterSDK REQUIRED)
 find_package(spdlog REQUIRED)
 
 # when building as a top-level project
 if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME)
   message(STATUS "Ouster SDK client: Using EIGEN_MAX_ALIGN_BYTES = 32")
@@ -66,7 +67,13 @@
 
 pybind11_add_module(_viz src/cpp/_viz.cpp)
 target_link_libraries(_viz PRIVATE ouster_client ouster_viz ouster_build)
 target_include_directories(_viz SYSTEM PRIVATE ${EIGEN3_INCLUDE_DIR})
 set_target_properties(_viz PROPERTIES
   POSITION_INDEPENDENT_CODE TRUE
   LIBRARY_OUTPUT_DIRECTORY ${EXT_DIR}/sdk/$<0:>)
+
+pybind11_add_module(_osf src/cpp/_osf.cpp)
+target_link_libraries(_osf PRIVATE ouster_osf ouster_build)
+set_target_properties(_osf PROPERTIES
+  POSITION_INDEPENDENT_CODE TRUE
+  LIBRARY_OUTPUT_DIRECTORY ${EXT_DIR}/osf/$<0:>)
```

### Comparing `ouster-sdk-0.8.1/PKG-INFO` & `ouster-sdk-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ouster-sdk
-Version: 0.8.1
-Summary: Ouster sensor SDK
+Version: 0.9.0
+Summary: Ouster Sensor SDK
 Home-page: https://github.com/ouster-lidar/ouster_example
 Author: Ouster Sensor SDK Developers
 Author-email: oss@ouster.io
 License: BSD 3-Clause License
 Project-URL: Ouster SDK Documentation, https://static.ouster.dev/sdk-docs/index.html
 Project-URL: Bug Tracker, https://github.com/ouster-lidar/ouster_example/issues
 Project-URL: Ouster Customer Support, https://ouster.atlassian.net/servicedesk/customer/portal/8
@@ -20,24 +20,26 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: examples
+Provides-Extra: mapping
 
 =================
 Ouster Python SDK
 =================
 
 ..
     [sdk-overview-start]
@@ -74,15 +76,15 @@
   ``manylinux2014_aarch64``)
 - macOS >= 10.13 on x86_64 platforms (``macosx_10_13_x86_64``)
 - macOS >= 11.0 on Apple M1 for Python >= 3.8 (``macosx_11_0_arm64``)
 - Windows 10 on x86_64 platforms (``win_amd64``)
 
 Building from source is supported on:
 
-- Ubuntu 18.04, 20.04, 22.04, and Debian 10 (x86-64, aarch64)
+- Ubuntu 20.04, 22.04, and Debian 11 (x86-64, aarch64)
 - macOS >= 10.13 (x86-64), >= 11.0 (arm64)
 - Windows 10 (x86-64)
 
 .. _PyPI: https://pypi.org/project/ouster-sdk/
 
 ..
     [python-supported-platforms-end]
```

### Comparing `ouster-sdk-0.8.1/README.rst` & `ouster-sdk-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
   ``manylinux2014_aarch64``)
 - macOS >= 10.13 on x86_64 platforms (``macosx_10_13_x86_64``)
 - macOS >= 11.0 on Apple M1 for Python >= 3.8 (``macosx_11_0_arm64``)
 - Windows 10 on x86_64 platforms (``win_amd64``)
 
 Building from source is supported on:
 
-- Ubuntu 18.04, 20.04, 22.04, and Debian 10 (x86-64, aarch64)
+- Ubuntu 20.04, 22.04, and Debian 11 (x86-64, aarch64)
 - macOS >= 10.13 (x86-64), >= 11.0 (arm64)
 - Windows 10 (x86-64)
 
 .. _PyPI: https://pypi.org/project/ouster-sdk/
 
 ..
     [python-supported-platforms-end]
```

### Comparing `ouster-sdk-0.8.1/sdk/.github/ISSUE_TEMPLATE/bug_report.md` & `ouster-sdk-0.9.0/sdk/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/.github/ISSUE_TEMPLATE/feature_request.md` & `ouster-sdk-0.9.0/sdk/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/.github/ISSUE_TEMPLATE/question.md` & `ouster-sdk-0.9.0/sdk/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/CHANGELOG.rst` & `ouster-sdk-0.9.0/sdk/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,69 @@
 =========
 Changelog
 =========
 
+20230710
+========
+
+* Update vcpkg ref of build to 2023-02-24
+* 
+
+ouster_osf
+----------
+
+* Add Ouster OSF C++/Python library to save stream of LidarScans with metadata
+
+ouster_client
+-------------
+
+* Add ``LidarScan.pose`` with poses per column
+* Add ``_client.IndexedPcapReader`` and ``_client.PcapIndex`` to enable random
+  pcap file access by frame number
+* [BREAKING] remove ``ouster::Imu`` object
+* Add get_field_types function for LidarScan, from sensor_info
+* bugfix: return metadata regardless of sensor_info status field
+* Make timeout on curl more configurable
+
+ouster_viz
+----------
+
+* [BREAKING] Changed Python binding for ``Cloud.set_column_poses()`` to accept ``[Wx4x4]`` array
+  of poses, column-storage order
+* bugfix: fix label re-use
+* Add ``LidarScan.pose`` handling to ``viz.LidarScanViz``, and new ``T`` keyboard
+  binding to toggle column poses usage
+
+ouster_pcap
+-----------
+* bugfix: Use unordered map to store stream_keys to avoid comparison operators on map
+
+Python SDK
+----------
+* Add Python 3.11 wheels
+* Retire simple-viz for ouster-cli utility
+* Add default ? key binding to LidarScanViz and consolidate bindings into stored definition
+* Remove pcap-to-csv for ouster-cli utility
+* Add validator class for LidarPacket
+
+ouster-cli
+----------
+This release also marks the introduction of the ouster-cli utility which includes, among many features:
+* Visualization from a connected sensor with automatic configuration
+* Recording from a connected sensor
+* Simultaneous record and viz from a connected sensor
+* Obtaining metadata from a connected sensor
+* Visualization from a specified PCAP
+* Slice, info, and conversion for a specificed PCAP
+* Utilities for benchmarking system, printing system-info
+* Discovery which indicates all connected sensors on network
+* Automatic logging to .ouster-cli
+* Mapping utilities
+
+
 [20230403]
 ==========
 
 * Default metadata output across all functionality has been switched to the non-legacy format
 
 ouster_client
 -------------
```

### Comparing `ouster-sdk-0.8.1/sdk/CMakeLists.txt` & `ouster-sdk-0.9.0/sdk/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 list(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake)
 include(DefaultBuildType)
 
 # configure vcpkg from environment variables, if present
 include(VcpkgEnv)
 
 # ==== Project Name ====
-project(ouster_example VERSION 20230403)
+project(ouster_example VERSION 20230710)
 
 # generate version header
-set(OusterSDK_VERSION_STRING 0.8.1)
+set(OusterSDK_VERSION_STRING 0.9.0)
 include(VersionGen)
 
 # ==== Options ====
 option(CMAKE_POSITION_INDEPENDENT_CODE "Build position independent code." ON)
 option(BUILD_SHARED_LIBS "Build shared libraries." OFF)
 option(BUILD_PCAP "Build pcap utils." ON)
+option(BUILD_OSF "Build Ouster OSF library." OFF)
 option(BUILD_VIZ "Build Ouster visualizer." ON)
 option(BUILD_TESTING "Build tests" OFF)
 option(BUILD_EXAMPLES "Build C++ examples" OFF)
 option(OUSTER_USE_EIGEN_MAX_ALIGN_BYTES_32 "Eigen max aligned bytes." ON)
 
 # when building as a top-level project
 if(CMAKE_PROJECT_NAME STREQUAL PROJECT_NAME)
@@ -52,14 +53,18 @@
   target_compile_definitions(ouster_client PUBLIC EIGEN_MAX_ALIGN_BYTES=32)
 endif()
 
 if(BUILD_PCAP)
   add_subdirectory(ouster_pcap)
 endif()
 
+if(BUILD_OSF)
+  add_subdirectory(ouster_osf)
+endif()
+
 if(BUILD_VIZ)
   add_subdirectory(ouster_viz)
 endif()
 
 if(BUILD_EXAMPLES)
   add_subdirectory(examples)
 endif()
@@ -84,15 +89,15 @@
 set(CPACK_SOURCE_GENERATOR "TGZ;ZIP")
 set(CPACK_SOURCE_IGNORE_FILES /.git /dist)
 
 # deb options
 set(CPACK_DEBIAN_PACKAGE_NAME ouster-sdk)
 set(CPACK_DEBIAN_FILE_NAME DEB-DEFAULT)
 set(CPACK_DEBIAN_PACKAGE_DEPENDS
-  "libjsoncpp-dev, libeigen3-dev, libtins-dev, libglfw3-dev, libglew-dev, libspdlog-dev")
+  "libjsoncpp-dev, libeigen3-dev, libtins-dev, libglfw3-dev, libglew-dev, libspdlog-dev, libpng-dev, libflatbuffers-dev")
 include(CPack)
 
 # ==== Install ====
 include(CMakePackageConfigHelpers)
 write_basic_package_version_file(
   OusterSDKConfigVersion.cmake
   VERSION ${PACKAGE_VERSION}
```

### Comparing `ouster-sdk-0.8.1/sdk/CMakeSettings.json` & `ouster-sdk-0.9.0/sdk/CMakeSettings.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/LICENSE` & `ouster-sdk-0.9.0/sdk/LICENSE`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/LICENSE-bin` & `ouster-sdk-0.9.0/sdk/LICENSE-bin`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/README.rst` & `ouster-sdk-0.9.0/sdk/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 - `Ouster Sensor Documentaion <https://static.ouster.dev/sensor-docs>`_ 
 
 This repository contains Ouster SDK source code for connecting to and configuring ouster sensors,
 reading and visualizing data.
 
 * `ouster_client <ouster_client/>`_ contains an example C++ client for ouster sensors
 * `ouster_pcap <ouster_pcap/>`_ contains C++ pcap functions for ouster sensors
+* `ouster_osf <ouster_osf/>`_ contains C++ OSF library to store ouster sensors data
 * `ouster_viz <ouster_viz/>`_ contains a customizable point cloud visualizer
 * `python <python/>`_ contains the code for the ouster sensor python SDK (``ouster-sdk`` Python package)
 
 .. note::
     Ouster ROS driver code has been moved out to a separate GitHub repository. To get started using the
     driver follow the instructions provided on the repository's main page: https://github.com/ouster-lidar/ouster-ros
```

### Comparing `ouster-sdk-0.8.1/sdk/cmake/FindCURL.cmake` & `ouster-sdk-0.9.0/sdk/cmake/FindCURL.cmake`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/cmake/FindGTest.cmake` & `ouster-sdk-0.9.0/sdk/cmake/FindGTest.cmake`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/cmake/FindPcap.cmake` & `ouster-sdk-0.9.0/sdk/cmake/FindPcap.cmake`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,22 @@
   NAMES pcap.h
   HINTS ${PC_PCAP_INCLUDE_DIRS})
 
 find_library(PCAP_LIBRARY
   NAMES pcap pcap_static wpcap
   HINTS ${PC_PCAP_LIBRARY_DIRS})
 
+if(NOT TARGET libpcap::libpcap)
+  add_library(libpcap::libpcap UNKNOWN IMPORTED)
+  set_target_properties(libpcap::libpcap PROPERTIES
+    INTERFACE_INCLUDE_DIRECTORIES "${PCAP_INCLUDE_DIR}"
+    IMPORTED_LINK_INTERFACE_LANGUAGES "C"
+    IMPORTED_LOCATION "${PCAP_LIBRARY}")
+endif()
+
 include(FindPackageHandleStandardArgs)
 find_package_handle_standard_args(Pcap
   REQUIRED_VARS PCAP_LIBRARY PCAP_INCLUDE_DIR
   VERSION_VAR PCAP_VERSION_STRING)
 
 mark_as_advanced(
   PCAP_INCLUDE_DIR
```

### Comparing `ouster-sdk-0.8.1/sdk/cmake/Findjsoncpp.cmake` & `ouster-sdk-0.9.0/sdk/cmake/Findjsoncpp.cmake`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/cmake/Findlibtins.cmake` & `ouster-sdk-0.9.0/sdk/cmake/Findlibtins.cmake`

 * *Files 3% similar despite different names*

```diff
@@ -50,9 +50,10 @@
 
 # LIBTINS_LIBRARIES is set, add target with a name compatible with the conan
 # package
 if(NOT TARGET libtins)
   add_library(libtins INTERFACE)
   set_target_properties(libtins PROPERTIES
     INTERFACE_LINK_LIBRARIES ${LIBTINS_LIBRARIES})
+  add_library(libtins::libtins ALIAS libtins)
   install(TARGETS libtins EXPORT ouster-sdk-targets)
 endif()
```

### Comparing `ouster-sdk-0.8.1/sdk/cmake/OusterSDKConfig.cmake.in` & `ouster-sdk-0.9.0/sdk/cmake/OusterSDKConfig.cmake.in`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 # ouster_client dependencies
 find_dependency(Eigen3)
 find_dependency(jsoncpp)
 find_dependency(CURL)
 find_dependency(spdlog)
 
+# ouster_osf dependencies
+if(@BUILD_OSF@)
+  find_package(ZLIB REQUIRED)
+  find_package(PNG REQUIRED)
+  find_package(Flatbuffers NAMES Flatbuffers FlatBuffers)
+endif()
+
 # viz dependencies
 if(@BUILD_VIZ@)
   set(OpenGL_GL_PREFERENCE GLVND)
   find_dependency(OpenGL)
   find_dependency(glfw3)
 
   if(@OUSTER_VIZ_USE_GLAD@)
```

### Comparing `ouster-sdk-0.8.1/sdk/cmake/VcpkgEnv.cmake` & `ouster-sdk-0.9.0/sdk/cmake/VcpkgEnv.cmake`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/cmake/VersionGen.cmake` & `ouster-sdk-0.9.0/sdk/cmake/VersionGen.cmake`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/conan/test_package/conanfile.py` & `ouster-sdk-0.9.0/sdk/conan/test_package/conanfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     settings = "os", "compiler", "build_type", "arch"
     generators = "cmake_paths", "cmake_find_package"
 
     def build(self):
         cmake = CMake(self)
         # Current dir is "test_package/build/<build_id>" and CMakeLists.txt is
         # in "test_package"
+        cmake.definitions["BUILD_OSF"] = True
         cmake.definitions[
             "CMAKE_PROJECT_PackageTest_INCLUDE"] = os.path.join(
                 self.build_folder, "conan_paths.cmake")
         cmake.configure()
         cmake.build()
 
     def imports(self):
@@ -23,8 +24,11 @@
         self.copy('*.so*', dst='bin', src='lib')
 
     def test(self):
         if not tools.cross_building(self):
             os.chdir("examples")
             # on Windows VS puts execulables under `./Release` or `./Debug` folders
             exec_path = f"{os.sep}{self.settings.build_type}" if self.settings.os == "Windows" else ""
-            self.run(".%s%sclient_example" % (exec_path, os.sep))
+            self.run(f".{exec_path}{os.sep}client_example")
+
+            # Smoke test OSF lib
+            self.run(f".{exec_path}{os.sep}osf_reader_example")
```

### Comparing `ouster-sdk-0.8.1/sdk/conanfile.py` & `ouster-sdk-0.9.0/sdk/conanfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,34 +13,37 @@
     description = "Ouster SDK - tools for working with Ouster Lidars"
     topics = ("lidar", "driver", "hardware", "point cloud", "3d", "robotics", "automotive")
     settings = "os", "compiler", "build_type", "arch"
 
     options = {
         "build_viz": [True, False],
         "build_pcap": [True, False],
+        "build_osf": [True, False],
         "shared": [True, False],
         "fPIC": [True, False],
         "ensure_cpp17": [True, False],
         "eigen_max_align_bytes": [True, False],
     }
     default_options = {
         "build_viz": False,
         "build_pcap": False,
+        "build_osf": False,
         "shared": False,
         "fPIC": True,
         "ensure_cpp17": False,
         "eigen_max_align_bytes": False,
     }
 
     generators = "cmake_paths", "cmake_find_package"
     exports_sources = [
         "cmake/*",
         "conan/*",
         "ouster_client/*",
         "ouster_pcap/*",
+        "ouster_osf/*",
         "ouster_viz/*",
         "tests/*",
         "CMakeLists.txt",
         "CMakeSettings.json",
         "LICENSE",
         "LICENSE-bin",
         "README.rst"
@@ -53,40 +56,40 @@
         self.version = version.strip()
 
     def config_options(self):
         if self.settings.os == "Windows":
             del self.options.fPIC
 
     def requirements(self):
-        # not required directly here but because libtins and libcurl pulling
-        # slightly different versions of zlib and openssl we need to set it
-        # here explicitly
-        self.requires("zlib/1.2.13")
-        self.requires("openssl/1.1.1s")
-
         self.requires("eigen/3.4.0")
         self.requires("jsoncpp/1.9.5")
-        self.requires("spdlog/1.10.0")
+        self.requires("spdlog/1.11.0")
+        self.requires("fmt/9.1.0")
         self.requires("libcurl/7.84.0")
 
         if self.options.build_pcap:
             self.requires("libtins/4.3")
 
+        if self.options.build_osf:
+            self.requires("flatbuffers/23.5.26")
+            self.requires("libpng/1.6.39")
+
         if self.options.build_viz:
             self.requires("glad/0.1.34")
             if self.settings.os != "Windows":
                 self.requires("xorg/system")
             self.requires("glfw/3.3.6")
             # maybe needed for cpp examples, but not for the lib
             # self.requires("tclap/1.2.4")
 
     def configure_cmake(self):
         cmake = CMake(self)
         cmake.definitions["BUILD_VIZ"] = self.options.build_viz
         cmake.definitions["BUILD_PCAP"] = self.options.build_pcap
+        cmake.definitions["BUILD_OSF"] = self.options.build_osf
         cmake.definitions["OUSTER_USE_EIGEN_MAX_ALIGN_BYTES_32"] = self.options.eigen_max_align_bytes
         # alt way, but we use CMAKE_TOOLCHAIN_FILE in other pipeline so avoid overwrite
         # cmake.definitions["CMAKE_TOOLCHAIN_FILE"] = os.path.join(self.build_folder, "conan_paths.cmake")
         cmake.definitions[
             "CMAKE_PROJECT_ouster_example_INCLUDE"] = os.path.join(
                 self.build_folder, "conan_paths.cmake")
         cmake.definitions["BUILD_SHARED_LIBS"] = True if self.options.shared else False
```

### Comparing `ouster-sdk-0.8.1/sdk/docs/Doxyfile` & `ouster-sdk-0.9.0/sdk/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/_static/css/ouster_rtd_tweaks.css` & `ouster-sdk-0.9.0/sdk/docs/_static/css/ouster_rtd_tweaks.css`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/conf.py` & `ouster-sdk-0.9.0/sdk/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,17 +61,21 @@
     'sphinx.ext.napoleon',
     'sphinx.ext.viewcode',
     'sphinx.ext.todo',
     'sphinx_autodoc_typehints',
     'sphinx_rtd_theme',
     'sphinx_copybutton',
     'sphinx_tabs.tabs',
-    'breathe'
+    'breathe',
+    'sphinx_rtd_size',
 ]
 
+# Page width
+sphinx_rtd_size_width = "70%"
+
 # Full path generated Doxygen XML dir resolved in do_doxygen_generate_xml()
 # handler below
 breathe_projects = {'cpp_api': "xml"}
 
 breathe_default_project = 'cpp_api'
 breathe_show_include = True
 breathe_default_members = ()
```

### Comparing `ouster-sdk-0.8.1/sdk/docs/cpp/building.rst` & `ouster-sdk-0.9.0/sdk/docs/cpp/building.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 The C++ example code is available `on the Ouster Github
 <https://github.com/ouster-lidar/ouster_example>`_. Follow the instructions for cloning the project.
 
 Building on Linux / macOS
 =========================
 
-To install build dependencies on Ubuntu, run:
+To install build dependencies on Ubuntu:20.04+, run:
 
 .. code:: console
 
    $ sudo apt install build-essential cmake libjsoncpp-dev libeigen3-dev libcurl4-openssl-dev \
                       libtins-dev libpcap-dev libglfw3-dev libglew-dev libspdlog-dev
 
 You may also install curl with a different ssl backend, for example libcurl4-gnutls-dev or
@@ -43,47 +43,62 @@
 CMake build script supports several optional flags. Add any of the following to override the
 defaults:
 
 .. code:: console
 
    -DBUILD_VIZ=OFF                    # Do not build the sample visualizer
    -DBUILD_PCAP=OFF                   # Do not build pcap tools
+   -DBUILD_OSF=OFF                    # Do not build OSF lib
    -DBUILD_EXAMPLES=ON                # Build C++ examples
    -DBUILD_TESTING=ON                 # Build tests
    -DBUILD_SHARED_LIBS=ON             # Build shared instead of static libraries
 
+.. admonition:: Additional dependencies required to build Ouster OSF lib
+
+   To build Ouster OSF library as part of the SDK you need to pass ``BUILD_OSF=ON`` and ensure that
+   ``libpng`` and ``flatbuffers`` packages are available on the system.
+
+   On Ubuntu:20.04+ systems::
+
+      $ sudo apt install libpng-dev libflatbuffers-dev
+
+   On macOS::
+
+      $ brew install libpng flatbuffers
+
+
 Building on Windows
 ===================
 
 The example code can be built on Windows 10 with Visual Studio 2019 using CMake support and vcpkg
 for dependencies. Follow the official documentation to set up your build environment:
 
 * `Visual Studio <https://visualstudio.microsoft.com/downloads/>`_
 * `Visual Studio CMake Support
   <https://docs.microsoft.com/en-us/cpp/build/cmake-projects-in-visual-studio?view=vs-2019>`_
 * `Visual Studio CPP Support
   <https://docs.microsoft.com/en-us/cpp/build/vscpp-step-0-installation?view=vs-2019>`_
-* `Vcpkg, at tag "2022.02.23" installed and integrated with Visual Studio
+* `Vcpkg, at tag "2023.02.24" installed and integrated with Visual Studio
   <https://docs.microsoft.com/en-us/cpp/build/vcpkg?view=msvc-160#installation>`_
 
-**Note** You'll need to run ``git checkout 2022.02.23`` in the vcpkg directory before bootstrapping
+**Note** You'll need to run ``git checkout 2023.02.24`` in the vcpkg directory before bootstrapping
 to use the correct versions of the dependencies. Building may fail unexpectedly if you skip this
 step.
 
 Don't forget to integrate vcpkg with Visual Studio after bootstrapping:
 
 .. code:: powershell
 
    PS > .\vcpkg.exe integrate install
 
 You should be able to install dependencies with
 
 .. code:: powershell
 
-   PS > .\vcpkg.exe install --triplet x64-windows jsoncpp eigen3 curl libtins glfw3 glew spdlog
+   PS > .\vcpkg.exe install --triplet x64-windows jsoncpp eigen3 curl libtins glfw3 glew spdlog libpng flatbuffers
 
 After these steps are complete, you should be able to open, build and run the ``ouster_example``
 project using Visual Studio:
 
 1. Start Visual Studio.
 2. When the prompt opens asking you what type of project to open click **Open a local folder** and
    navigate to the ``ouster_example`` source directory.
```

### Comparing `ouster-sdk-0.8.1/sdk/docs/cpp/examples.rst` & `ouster-sdk-0.9.0/sdk/docs/cpp/examples.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/cpp/ouster_client/client.rst` & `ouster-sdk-0.9.0/sdk/docs/cpp/ouster_client/client.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/cpp/ouster_client/lidar_scan.rst` & `ouster-sdk-0.9.0/sdk/docs/cpp/ouster_client/lidar_scan.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/cpp/ouster_client/types.rst` & `ouster-sdk-0.9.0/sdk/docs/cpp/ouster_client/types.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/cpp/ouster_pcap/os_pcap.rst` & `ouster-sdk-0.9.0/sdk/docs/cpp/ouster_pcap/os_pcap.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/cpp/ouster_viz/point_viz.rst` & `ouster-sdk-0.9.0/sdk/docs/cpp/ouster_viz/point_viz.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/Ouster_Logo_TM_Horiz_Black_RGB_600px.png` & `ouster-sdk-0.9.0/sdk/docs/images/Ouster_Logo_TM_Horiz_Black_RGB_600px.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/Ouster_Logo_TM_Horiz_White_RGB.svg` & `ouster-sdk-0.9.0/sdk/docs/images/Ouster_Logo_TM_Horiz_White_RGB.svg`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/Ouster_Logo_TM_Stacked_White_RGB.svg` & `ouster-sdk-0.9.0/sdk/docs/images/Ouster_Logo_TM_Stacked_White_RGB.svg`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/brooklyn_bridge_ls_50_range_image.png` & `ouster-sdk-0.9.0/sdk/docs/images/brooklyn_bridge_ls_50_range_image.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/brooklyn_bridge_ls_50_xyz_cut.png` & `ouster-sdk-0.9.0/sdk/docs/images/brooklyn_bridge_ls_50_xyz_cut.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/lidar_scan_destaggered.png` & `ouster-sdk-0.9.0/sdk/docs/images/lidar_scan_destaggered.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/lidar_scan_staggered.png` & `ouster-sdk-0.9.0/sdk/docs/images/lidar_scan_staggered.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/lidar_scan_xyz_84.png` & `ouster-sdk-0.9.0/sdk/docs/images/lidar_scan_xyz_84.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/lidar_scan_xyz_84_3d.png` & `ouster-sdk-0.9.0/sdk/docs/images/lidar_scan_xyz_84_3d.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/simple-viz.png` & `ouster-sdk-0.9.0/sdk/docs/images/simple-viz.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/axes_helper_unstructured.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/axes_helper_unstructured.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/empty_point_viz.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/empty_point_viz.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/image_set_pos_bot_right.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/image_set_pos_bot_right.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/image_set_pos_center.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/image_set_pos_center.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/image_set_pos_left.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/image_set_pos_left.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/image_set_pos_right.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/image_set_pos_right.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_fields_images.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_fields_images.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_fields_images_labels.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_fields_images_labels.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_structured.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_structured.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_viz.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_viz.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_viz_checkers.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_viz_checkers.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/images/viz-tutorial/lidar_scan_viz_labels.png` & `ouster-sdk-0.9.0/sdk/docs/images/viz-tutorial/lidar_scan_viz_labels.png`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/index.rst` & `ouster-sdk-0.9.0/sdk/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,24 @@
 
    Lidar Scan API <reference/lidar-scan>
    Python API Reference <python/api/index>
    C++ API Reference <cpp/api>
    Changelog <reference/changelog>
 
 .. toctree::
+   :caption: Command Line Utility Guide
+   :hidden:
+
+   Overview <cli/overview>
+   Getting Started <cli/getting-started>
+   Sample Sessions <cli/sample-sessions>
+   Common Use Cases <cli/common-use-cases>
+   Changelog <cli/changelog>
+
+.. toctree::
    :caption: Migration Guides
    :hidden:
 
     Migrating from 20220927/0.5.1 to 20230114/0.7.1 <migration/migration-20220927-20230114>
     Migrating from 20230114/0.7.1 to 20230403/0.8.1 <migration/migration-20230114-20230403>
 ..
    FAQ <faq>
```

### Comparing `ouster-sdk-0.8.1/sdk/docs/installation.rst` & `ouster-sdk-0.9.0/sdk/docs/installation.rst`

 * *Files 16% similar despite different names*

```diff
@@ -31,19 +31,30 @@
 
 The Ouster Python SDK binary packages require Python >= 3.7 and pip >= 19.0 on most platforms. On
 Ubuntu 18.04, the default Python 3 version is is 3.6, so you'll have to install and use
 ``python3.7`` explicitly. On Apple M1, you'll need need Python >= 3.8.
 
 .. note::
 
-    Using a virtual environment with the Ouster Python SDK is recommended. Users newer to Python should
-    read the official `venv instructions`_ and ensure that they upgrade pip *after* activating their
-    venv. If you're using venv on Windows, you'll want to use ``python`` and ``pip`` instead of ``py
+    Using a virtual environment with the Ouster Python SDK is recommended.
+    Users newer to Python should read the official `venv instructions`_ and
+    ensure that they upgrade pip *after* activating their venv. If you're using
+    venv on Windows, you'll want to use ``python`` and ``pip`` instead of ``py
     -3`` and ``py -3 -m pip`` in the following Powershell snippets.
 
+.. note::
+
+    Python 3 when installed with macOS Developer Tools uses LibreSSL 2.8.3 (or
+    an older version.) OusterSDK, like many Python 3-compatible packages,
+    requires urllib3 which is not compatible with LibreSSL and requires OpenSSL
+    1.1.1 or newer. To account for this, macOS users should install an official
+    distribution of Python 3 or one provided by Homebrew, as these use OpenSSL
+    1.1.1 or newer. In either case, installing OusterSDK into a Python 3
+    virtual enviroment is still recommended.
+
 If you're using an unsupported platform like a non-glibc-based linux distribution, or wish to modify
 the Ouster Python SDK, you will need to build from source. See the `build instructions`_ for
 requirements needed to build from a source distribution or from a clone of the repository.
 
 To install on :ref:`supported platforms<supported-platforms>`, first make sure you have the latest
 version of pip:
```

### Comparing `ouster-sdk-0.8.1/sdk/docs/migration/migration-20220927-20230114.rst` & `ouster-sdk-0.9.0/sdk/docs/migration/migration-20220927-20230114.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/migration/migration-20230114-20230403.rst` & `ouster-sdk-0.9.0/sdk/docs/migration/migration-20230114-20230403.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/overview.rst` & `ouster-sdk-0.9.0/sdk/docs/overview.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 Quick links
 -----------
 
 * :doc:`installation`
 * :doc:`python/quickstart`
 * :doc:`cpp/building`
 * `Ouster ROS 1 driver`_
-
+* :doc:`python/viz/index`
+  :doc:`cli/getting-started`
 .. figure:: /images/simple-viz.png
     :align: center
 
-* :doc:`python/viz/index`
 
 Compatibility with FW
 ---------------------
 
 The Ouster SDK currently provides backwards compatibility with any FW 2.0 and later for all
 releases. Older SDK versions are not, however, generally forward-compatible with later FW relesaes,
 e.g., the SDK version 20210608 (ouster-sdk 0.2.0) is not compatible with FW 3.0.
```

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/api/client.rst` & `ouster-sdk-0.9.0/sdk/docs/python/api/client.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/api/examples.rst` & `ouster-sdk-0.9.0/sdk/docs/python/api/examples.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/api/viz.rst` & `ouster-sdk-0.9.0/sdk/docs/python/api/viz.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/devel.rst` & `ouster-sdk-0.9.0/sdk/docs/python/devel.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 - a C++14-capable compiler
 - `cmake <https://cmake.org/>`_  >= 3.5
 - `eigen <https://eigen.tuxfamily.org>`_ >= 3.3
 - `curl <https://curl.se/libcurl/>`_ >= 7.58
 - `jsoncpp <https://github.com/open-source-parsers/jsoncpp>`_ >= 1.7
 - `libtins <http://libtins.github.io/>`_ >= 3.4
 - `libpcap <https://www.tcpdump.org/>`_
+- `libpng <http://www.libpng.org>`_ >= 1.6
+- `flatbuffers <https://flatbuffers.dev/>`_ >= 1.1
 - `libglfw3 <https://www.glfw.org/>`_ >= 3.2
 - `libglew <http://glew.sourceforge.net/>`_ >= 2.1 or `glad <https://github.com/Dav1dde/glad>`_
 - `spdlog <https://github.com/gabime/spdlog>`_ >= 1.9
 - `Python <https://www.python.org/>`_ >= 3.7 (with headers and development libraries)
 - `pybind11 <https://pybind11.readthedocs.io>`_ >= 2.0
 
 The Python SDK source is available `on the Ouster Github <https://github.com/ouster-lidar/ouster_example>`_. You should clone the whole project.
@@ -29,33 +31,37 @@
 
 On supported Debian-based linux systems, you can install all build dependencies by running:
 
 .. code:: console
 
    $ sudo apt install build-essential cmake \
                       libeigen3-dev libjsoncpp-dev libtins-dev libpcap-dev \
-                      python3-dev python3-pip pybind11-dev libcurl4-openssl-dev \
-                      libglfw3-dev libglew-dev libspdlog-dev
+                      python3-dev python3-pip libcurl4-openssl-dev \
+                      libglfw3-dev libglew-dev libspdlog-dev \
+                      libpng-dev libflatbuffers-dev
 
 On macos >= 10.13, using homebrew, you should be able to run:
 
 .. code:: console
 
-  $ brew install cmake eigen curl jsoncpp libtins python3 pybind11 glfw glew spdlog
+  $ brew install cmake eigen curl jsoncpp libtins python3 glfw glew spdlog libpng flatbuffers
 
 After you have the system dependencies, you can build the SDK with:
 
 .. code:: console
 
    # first, specify the path to the ouster_example repository
    $ export OUSTER_SDK_PATH=<PATH TO OUSTER_EXAMPLE REPO>
 
    # make sure you have an up-to-date version of pip installed
    $ python3 -m pip install --user --upgrade pip
 
+   # install pybind11
+   $ python3 -m pip install pybind11
+
    # then, build an installable "wheel" package
    $ python3 -m pip wheel --no-deps $OUSTER_SDK_PATH/python
 
    # or just install directly (virtualenv recommended)
    $ python3 -m pip install $OUSTER_SDK_PATH/python
 
 
@@ -70,17 +76,17 @@
 ----------
 
 On Windows 10, you'll have to install the Visual Studio 2017 Build Tools, Python and the `vcpkg`_
 package manager and run:
 
 .. code:: powershell
 
-   PS > vcpkg install --triplet=x64-windows eigen3 jsoncpp libtins pybind11 glfw3 glad[gl-api-33] spdlog
+   PS > vcpkg install --triplet=x64-windows eigen3 jsoncpp libtins glfw3 glad[gl-api-33] spdlog libpng flatbuffers
 
-The currently tested vcpkg tag is ``2022.02.23``. After that, using a developer powershell prompt:
+The currently tested vcpkg tag is ``2023.02.24``. After that, using a developer powershell prompt:
 
 .. code:: powershell
 
    # first, specify the path to the ouster_example repository
    PS > $env:OUSTER_SDK_PATH="<PATH TO OUSTER_EXAMPLE>"
 
    # point cmake to the location of vcpkg (make sure to use an absolute path)
@@ -88,14 +94,17 @@
 
    # set the correct vcpkg triplet
    PS > $env:VCPKG_TARGET_TRIPLET="x64-windows"
    
    # set build options related to the compiler
    PS > $env:CMAKE_GENERATOR_PLATFORM="x64"
    PS > $env:CMAKE_GENERATOR="Visual Studio 15 2017"
+
+   # install pybind11
+   PS > py -m pip install pybind11
    
    # then, build an installable "wheel" package
    PS > py -m pip wheel --no-deps "$env:OUSTER_SDK_PATH\python"
 
    # or just install directly (virtualenv recommended)
    PS > py -m pip install "$env:OUSTER_SDK_PATH\python"
 
@@ -112,15 +121,17 @@
 Install in editable mode with pip using ``pip install -e``. For a faster development cycle, you can
 rebuild using ``python3 setup.py build_ext -i`` instead of reinstalling the package after every
 change. For a local debug build, you can also add the ``-g`` flag.
 
 The Ouster SDK package includes configuration for ``flake8`` and ``mypy``. To run:
 
 .. code:: console
-
+   # install pybind11
+   $ python3 -m pip install pybind11
+   
    # install and run flake8 linter
    $ python3 -m pip install flake8
    $ cd ${OUSTER_SDK_PATH}/python
    $ python3 -m flake8
 
    # install and run mypy in an environment with
    $ python3 -m pip install mypy
@@ -165,13 +176,13 @@
 
 .. code:: console
 
    $ docker build ${OUSTER_SDK_PATH} -f ${OUSTER_SDK_PATH}/python/Dockerfile \
        --build-arg BASE=ubuntu:20.04 \
        -t ouster-sdk-tox
 
-the ``BASE`` argument will default to ``ubuntu:18.04``, but can also be set to other docker tags,
-e.g. ``ubuntu:20.04``, ``ubuntu:22.04`` or ``debian:11``. Then, run the container to invoke tox:
+the ``BASE`` argument will default to ``ubuntu:20.04``, but can also be set to other docker tags,
+e.g. ``ubuntu:22.04`` or ``debian:11``. Then, run the container to invoke tox:
 
 .. code:: console
 
    $ docker run -it --rm ouster-sdk-tox
```

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/examples/basics-sensor.rst` & `ouster-sdk-0.9.0/sdk/docs/python/examples/basics-sensor.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/examples/conversion.rst` & `ouster-sdk-0.9.0/sdk/docs/python/examples/conversion.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,17 @@
     .. code-tab:: powershell Windows x64
 
         PS > py -3 -m ouster.sdk.examples.pcap $SAMPLE_DATA_PCAP_PATH $SAMPLE_DATA_JSON_PATH pcap-to-csv --scan-num 5
 
 
 The source code of an example below:
 
-.. literalinclude:: /../python/src/ouster/sdk/examples/pcap.py
+.. literalinclude:: /../python/src/ouster/cli/core/pcap.py
     :start-after: [doc-stag-pcap-to-csv]
     :end-before: [doc-etag-pcap-to-csv]
-    :emphasize-lines: 37-41
     :linenos:
     :dedent:
 
 Because we stored the scan as structured 2D images, we can easily recover it by loading it back into
 a ``numpy.ndarray`` and continuing to use it as a 2D image.
 
 .. code:: python
@@ -108,8 +107,8 @@
     .. code-tab:: powershell Windows x64
 
         PS > py -3 -m ouster.sdk.examples.pcap $SAMPLE_DATA_PCAP_PATH $SAMPLE_DATA_JSON_PATH pcap-to-ply --scan-num 5
 
 Checkout the :func:`.examples.pcap.pcap_to_ply` documentation for the example source code.
 
 .. _Open3d File IO: http://www.open3d.org/docs/release/tutorial/geometry/file_io.html#Point-cloud
-.. _plyfile: https://pypi.org/project/plyfile/
+.. _plyfile: https://pypi.org/project/plyfile/
```

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/examples/index.rst` & `ouster-sdk-0.9.0/sdk/docs/python/examples/index.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/examples/lidar-scan.rst` & `ouster-sdk-0.9.0/sdk/docs/python/examples/lidar-scan.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/examples/record-stream.rst` & `ouster-sdk-0.9.0/sdk/docs/python/examples/record-stream.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/examples/udp-packets.rst` & `ouster-sdk-0.9.0/sdk/docs/python/examples/udp-packets.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/examples/visualizations.rst` & `ouster-sdk-0.9.0/sdk/docs/python/examples/visualizations.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/quickstart.rst` & `ouster-sdk-0.9.0/sdk/docs/python/quickstart.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/viz/index.rst` & `ouster-sdk-0.9.0/sdk/docs/python/viz/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-=======================
+======================
 Point Cloud Visualizer
-=======================
+======================
 
 The Ouster visualization toolkit is written in C++ with Python bindings for Python functionality. It
 consists of the following:
 
 - ``simple-viz`` (:class:`.viz.SimpleViz`): the default Python application visualizer, which can
   also be used as an entrypoint for more sophisticated custom point cloud visualizations
 - ``ouster_viz``: the core C++ library
```

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/viz/viz-api-tutorial.rst` & `ouster-sdk-0.9.0/sdk/docs/python/viz/viz-api-tutorial.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/python/viz/viz-run.rst` & `ouster-sdk-0.9.0/sdk/docs/python/viz/viz-run.rst`

 * *Files 15% similar despite different names*

```diff
@@ -47,21 +47,24 @@
     ``s``           Camera pitch down
     ``a``           Camera yaw left
     ``d``           Camera yaw right
     ``1``           Toggle first return point cloud visibility
     ``2``           Toggle second return point cloud visibility
     ``0``           Toggle orthographic camera
     ``=/-``         Dolly in/out
-    ``(space)``     Toggle pause
+    ``?``           Prints key bindings
+    ``space``       Toggle pause
+    ``esc``         Exit visualization
     ``./,``         Step one frame forward/back
     ``ctrl + ./,``  Step 10 frames forward/back
     ``>/<``         Increase/decrease playback rate (during replay)
     ``shift``       Camera Translation with mouse drag
-    ``shift-z``     Save a screenshot of the current view
-    ``shift-x``     Toggle a continuous saving of screenshots
+    ``shift+z``     Save a screenshot of the current view
+    ``shift+x``     Toggle a continuous saving of screenshots
+    ``?``           Print keys to standard out
     ==============  ===============================================
 
 ..
    [end-simple-viz-keymap]
 
 The visualizer also includes an option to control the orientation of the point cloud in space when
 loaded. If you possess, say, an OS-DOME mounted an upside down, you can start the visualizer with
```

### Comparing `ouster-sdk-0.8.1/sdk/docs/reference/lidar-scan.rst` & `ouster-sdk-0.9.0/sdk/docs/reference/lidar-scan.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/docs/sample-data.rst` & `ouster-sdk-0.9.0/sdk/docs/sample-data.rst`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/examples/client_example.cpp` & `ouster-sdk-0.9.0/sdk/examples/client_example.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,16 @@
                "\n\n<udp_destination> is optional: leave blank for "
                "automatic destination detection"
             << std::endl;
 
         return argc == 1 ? EXIT_SUCCESS : EXIT_FAILURE;
     }
 
-    // Limit ouster_client log statements to "info" and direct the output to log
-    // file rather than the console (default).
-    sensor::init_logger("info", "ouster.log");
+    // Limit ouster_client log statements to "info"
+    sensor::init_logger("info");
 
     std::cerr << "Ouster client example " << ouster::SDK_VERSION << std::endl;
     /*
      * The sensor client consists of the network client and a library for
      * reading and working with data.
      *
      * The network client supports reading and writing a limited number of
```

### Comparing `ouster-sdk-0.8.1/sdk/examples/config_example.cpp` & `ouster-sdk-0.9.0/sdk/examples/config_example.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/examples/helpers.cpp` & `ouster-sdk-0.9.0/sdk/examples/helpers.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/examples/lidar_scan_example.cpp` & `ouster-sdk-0.9.0/sdk/examples/lidar_scan_example.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/examples/mtp_client_example.cpp` & `ouster-sdk-0.9.0/sdk/examples/mtp_client_example.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/examples/representations_example.cpp` & `ouster-sdk-0.9.0/sdk/examples/representations_example.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/examples/viz_example.cpp` & `ouster-sdk-0.9.0/sdk/examples/viz_example.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/CMakeLists.txt` & `ouster-sdk-0.9.0/sdk/ouster_client/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 find_package(jsoncpp REQUIRED)
 find_package(CURL REQUIRED)
 find_package(spdlog REQUIRED)
 
 # ==== Libraries ====
 add_library(ouster_client src/client.cpp src/types.cpp src/netcompat.cpp src/lidar_scan.cpp
   src/image_processing.cpp src/buffered_udp_source.cpp src/parsing.cpp
-  src/sensor_http.cpp src/sensor_http_imp.cpp src/sensor_tcp_imp.cpp src/logging.cpp)
+  src/sensor_http.cpp src/sensor_http_imp.cpp src/sensor_tcp_imp.cpp src/logging.cpp
+  src/profile_extension.cpp)
 target_link_libraries(ouster_client
   PUBLIC
     Eigen3::Eigen
     $<BUILD_INTERFACE:ouster_build>
   PRIVATE
     CURL::libcurl
     jsoncpp_lib
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/include/optional-lite/nonstd/optional.hpp` & `ouster-sdk-0.9.0/sdk/ouster_client/include/optional-lite/nonstd/optional.hpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/buffered_udp_source.h` & `ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/buffered_udp_source.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/client.h` & `ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/client.h`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 #include <cstdint>
 #include <memory>
 #include <string>
 
 #include "ouster/types.h"
 #include "ouster/version.h"
+#include "ouster/defaults.h"
 
 namespace ouster {
 namespace sensor {
 
 struct client;
 
 /** Returned by poll_client. */
@@ -92,15 +93,15 @@
  * @return pointer owning the resources associated with the connection.
  */
 std::shared_ptr<client> init_client(const std::string& hostname,
                                     const std::string& udp_dest_host,
                                     lidar_mode ld_mode = MODE_UNSPEC,
                                     timestamp_mode ts_mode = TIME_FROM_UNSPEC,
                                     int lidar_port = 0, int imu_port = 0,
-                                    int timeout_sec = 60);
+                                    int timeout_sec = DEFAULT_HTTP_REQUEST_TIMEOUT_SECONDS);
 
 /**
  * [BETA] Connect to and configure the sensor and start listening for data via
  * multicast.
  *
  * @param[in] hostname hostname or ip of the sensor.
  * @param[in] config sensor config to set on sensor.
@@ -115,15 +116,15 @@
  * @remarks when main flag is set the config object will be used to configure
  * the sensor, otherwise only the port values within the config object will be
  * used and the rest will be ignored.
  */
 std::shared_ptr<client> mtp_init_client(const std::string& hostname,
                                         const sensor_config& config,
                                         const std::string& mtp_dest_host,
-                                        bool main, int timeout_sec = 60);
+                                        bool main, int timeout_sec = DEFAULT_HTTP_REQUEST_TIMEOUT_SECONDS);
 
 /** @}*/
 
 /**
  * Block for up to timeout_sec until either data is ready or an error occurs.
  *
  * NOTE: will return immediately if LIDAR_DATA or IMU_DATA are set and not
@@ -166,38 +167,40 @@
 /**
  * Get metadata text blob from the sensor.
  *
  * Will attempt to fetch from the network if not already populated.
  *
  * @throw runtime_error if the sensor is in ERROR state, the firmware version
  * used to initialize the HTTP or TCP client is invalid, the metadata could
- * not be retrieved from the sensor, or the response could not be parsed.
+ * not be retrieved from the sensor within the timeout period,
+ * a timeout occured while waiting for the sensor to finish initializing,
+ * or the response could not be parsed.
  *
  * @param[in] cli client returned by init_client associated with the connection.
  * @param[in] timeout_sec how long to wait for the sensor to initialize.
  * @param[in] legacy_format whether to use legacy format of metadata output.
  *
  * @return a text blob of metadata parseable into a sensor_info struct.
  */
-std::string get_metadata(client& cli, int timeout_sec = 60,
+std::string get_metadata(client& cli, int timeout_sec = DEFAULT_HTTP_REQUEST_TIMEOUT_SECONDS,
                          bool legacy_format = false);
 
 /**
  * Get sensor config from the sensor.
  *
  * Populates passed in config with the results of get_config.
  *
  * @param[in] hostname sensor hostname.
  * @param[out] config sensor config to populate.
  * @param[in] active whether to pull active or passive configs.
  *
  * @return true if sensor config successfully populated.
  */
 bool get_config(const std::string& hostname, sensor_config& config,
-                bool active = true);
+                bool active = true, int timeout_sec = DEFAULT_HTTP_REQUEST_TIMEOUT_SECONDS);
 
 // clang-format off
 /**
  * Flags for set_config()
  */
 enum config_flags : uint8_t {
     CONFIG_UDP_DEST_AUTO    = (1 << 0), ///< Set udp_dest automatically
@@ -217,15 +220,15 @@
  * @param[in] hostname sensor hostname.
  * @param[in] config sensor config.
  * @param[in] config_flags flags to pass in.
  *
  * @return true if config params successfuly set on sensor.
  */
 bool set_config(const std::string& hostname, const sensor_config& config,
-                uint8_t config_flags = 0);
+                uint8_t config_flags = 0, int timeout_sec = DEFAULT_HTTP_REQUEST_TIMEOUT_SECONDS);
 
 /**
  * Return the port used to listen for lidar UDP data.
  *
  * @param[in] cli client returned by init_client associated with the connection.
  *
  * @return the port number.
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/image_processing.h` & `ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/image_processing.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/impl/cartesian.h` & `ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/impl/cartesian.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/impl/lidar_scan_impl.h` & `ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/impl/lidar_scan_impl.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/lidar_scan.h` & `ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/lidar_scan.h`

 * *Files 7% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     /** XYZ coordinates with dimensions arranged contiguously in columns. */
     using Points = Eigen::Array<double, Eigen::Dynamic, 3>;
 
    private:
     Header<uint64_t> timestamp_;
     Header<uint16_t> measurement_id_;
     Header<uint32_t> status_;
+    std::vector<mat4d> pose_;
     std::map<sensor::ChanField, impl::FieldSlot> fields_;
     LidarScanFieldTypes field_types_;
 
     LidarScan(size_t w, size_t h, LidarScanFieldTypes field_types);
 
    public:
     /**
@@ -233,14 +234,23 @@
      */
     Eigen::Ref<Header<uint32_t>> status();
 
     /** @copydoc status() */
     Eigen::Ref<const Header<uint32_t>> status() const;
 
     /**
+     * Access the vector of poses (per each timestamp).
+     *
+     * @return a reference to vector with poses (4x4) homogeneous.
+     */
+    std::vector<mat4d>& pose();
+    /** @copydoc pose() */
+    const std::vector<mat4d>& pose() const;
+
+    /**
      * Assess completeness of scan.
      * @param[in] window The column window to use for validity assessment
      * @return whether all columns within given column window were valid
      */
     bool complete(sensor::ColumnWindow window) const;
 
     friend bool operator==(const LidarScan& a, const LidarScan& b);
@@ -478,52 +488,11 @@
      * @param[in] ls lidar scan to populate.
      *
      * @return true when the provided lidar scan is ready to use.
      */
     bool operator()(const uint8_t* packet_buf, LidarScan& ls);
 };
 
-/**
- * Imu Data
- */
-struct Imu {
-    union {
-        std::array<double, 3> angular_vel;
-        struct {
-            double wx, wy, wz;
-        };
-    };
-    union {
-        std::array<double, 3> linear_accel;
-        struct {
-            double ax, ay, az;
-        };
-    };
-    union {
-        std::array<uint64_t, 3> ts;
-        struct {
-            uint64_t sys_ts, accel_ts, gyro_ts;
-        };
-    };
-};
-
-/** Equality for Imu */
-inline bool operator==(const Imu& a, const Imu& b) {
-    return a.angular_vel == b.angular_vel && a.linear_accel == b.linear_accel &&
-           a.ts == b.ts;
-};
-
-/** Not Equality for Imu */
-inline bool operator!=(const Imu& a, const Imu& b) {
-    return !(a == b);
-};
-
-std::string to_string(const Imu& imu);
-
-/// Reconstructs buf with UDP imu_packet to osf::Imu object
-void packet_to_imu(const uint8_t* buf, const ouster::sensor::packet_format& pf,
-                   Imu& imu);
-
 }  // namespace ouster
 
 #include "ouster/impl/cartesian.h"
 #include "ouster/impl/lidar_scan_impl.h"
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/sensor_http.h` & `ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/sensor_http.h`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
  *
  */
 
 #pragma once
 
 #include <json/json.h>
 #include <ouster/version.h>
+#include <ouster/defaults.h>
 
 #include <memory>
 
 namespace ouster {
 namespace sensor {
 namespace util {
 
@@ -118,27 +119,27 @@
     virtual void save_config_params() const = 0;
 
     /**
      * Retrieves sensor firmware version information as a string.
      *
      * @param[in] hostname hostname of the sensor to communicate with.
      */
-    static std::string firmware_version_string(const std::string& hostname);
+    static std::string firmware_version_string(const std::string& hostname, int timeout_sec = DEFAULT_HTTP_REQUEST_TIMEOUT_SECONDS);
 
     /**
      * Retrieves sensor firmware version information.
      *
      * @param[in] hostname hostname of the sensor to communicate with.
      */
-    static ouster::util::version firmware_version(const std::string& hostname);
+    static ouster::util::version firmware_version(const std::string& hostname, int timeout_sec = DEFAULT_HTTP_REQUEST_TIMEOUT_SECONDS);
 
     /**
      * Creates an instance of the SensorHttp interface.
      *
      * @param[in] hostname hostname of the sensor to communicate with.
      */
-    static std::unique_ptr<SensorHttp> create(const std::string& hostname);
+    static std::unique_ptr<SensorHttp> create(const std::string& hostname, int timeout_sec = DEFAULT_HTTP_REQUEST_TIMEOUT_SECONDS);
 };
 
 }  // namespace util
 }  // namespace sensor
-}  // namespace ouster
+}  // namespace ouster
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/types.h` & `ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/types.h`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,15 @@
     uint32_t
         columns_per_frame;  ///< columns per frame, should match with lidar mode
     std::vector<int>
         pixel_shift_by_row;      ///< shift of pixels by row to enable destagger
     ColumnWindow column_window;  ///< window of columns over which sensor fires
     UDPProfileLidar udp_profile_lidar;  ///< profile of lidar packet
     UDPProfileIMU udp_profile_imu;      ///< profile of imu packet
-    uint16_t fps;                ///< frames per second
+    uint16_t fps;                       ///< frames per second
 };
 
 /** Stores necessary information from sensor to parse and project sensor data.
  */
 struct sensor_info {
     [[deprecated("Will be removed in the next version")]] std::string
         name;               ///< @deprecated Will be removed in the next version
@@ -671,29 +671,35 @@
  *
  * String and vector fields will have size 0 if the parameter cannot
  * be found or parsed, while lidar_mode will be set to 0 (invalid).
  *
  * @throw runtime_error if the text is not valid json
  *
  * @param[in] metadata a text blob returned by get_metadata from client.h.
+ * @param[in] skip_beam_validation whether to skip validation on metdata - not
+ * for use on recorded data or metadata from sensors
  *
  * @return a sensor_info struct populated with a subset of the metadata.
  */
-sensor_info parse_metadata(const std::string& metadata);
+sensor_info parse_metadata(const std::string& metadata,
+                           bool skip_beam_validation = false);
 
 /**
  * Parse metadata given path to a json file.
  *
  * @throw runtime_error if json file does not exist or is malformed.
  *
  * @param[in] json_file path to a json file containing sensor metadata.
+ * @param[in] skip_beam_validation whether to skip validation on metadata - not
+ * for use on recorded data or metadata from sensors
  *
  * @return a sensor_info struct populated with a subset of the metadata.
  */
-sensor_info metadata_from_json(const std::string& json_file);
+sensor_info metadata_from_json(const std::string& json_file,
+                               bool skip_beam_validation = false);
 
 /**
  * Get a string representation of the sensor_info. All fields included. Not
  * equivalent or interchangeable with metadata from sensor.
  *
  * @param[in] info sensor_info struct
  *
@@ -1161,9 +1167,16 @@
  *
  * @param[in] info parameters provided by the sensor.
  *
  * @return a packet_format suitable for parsing UDP packets sent by the sensor.
  */
 const packet_format& get_format(const sensor_info& info);
 
+namespace impl {
+
+/** Maximum number of allowed lidar profiles */
+constexpr int MAX_NUM_PROFILES = 32;
+
+}  // namespace impl
+
 }  // namespace sensor
 }  // namespace ouster
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/include/ouster/version.h` & `ouster-sdk-0.9.0/sdk/ouster_client/include/ouster/version.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/buffered_udp_source.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/buffered_udp_source.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/client.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/client.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -241,53 +241,59 @@
     // could not bind() a MTP server socket
     freeaddrinfo(info_start);
     logger().error("failed to bind mtp socket");
     return SOCKET_ERROR;
 }
 
 Json::Value collect_metadata(const std::string& hostname, int timeout_sec) {
-    auto sensor_http = SensorHttp::create(hostname);
+    // Note, this function throws std::runtime_error if
+    // 1. the metadata couldn't be retrieved
+    // 2. the sensor is in the INITIALIZING state when timeout is reached
+    auto sensor_http = SensorHttp::create(hostname, timeout_sec);
     auto timeout_time =
         chrono::steady_clock::now() + chrono::seconds{timeout_sec};
     std::string status;
 
     // TODO: can remove this loop when we drop support for FW 2.4
     do {
-        if (chrono::steady_clock::now() >= timeout_time) return false;
+        if (chrono::steady_clock::now() >= timeout_time) {
+            throw std::runtime_error(
+                "A timeout occurred while waiting for the sensor to initialize."
+            );
+        }
         std::this_thread::sleep_for(1s);
         status = sensor_http->sensor_info()["status"].asString();
     } while (status == "INITIALIZING");
 
-    // not all metadata available when sensor isn't RUNNING
-    if (status != "RUNNING") {
+    try {
+        auto metadata = sensor_http->metadata();
+        // merge extra info into metadata
+        metadata["client_version"] = client_version();
+        return metadata;
+    } catch (const std::runtime_error& e) {
         throw std::runtime_error(
             "Cannot obtain full metadata with sensor status: " + status +
             ". Please ensure that sensor is not in a STANDBY, UNCONFIGURED, "
             "WARMUP, or ERROR state");
     }
-
-    auto metadata = sensor_http->metadata();
-    // merge extra info into metadata
-    metadata["client_version"] = client_version();
-    return metadata;
 }
 
 }  // namespace
 
 bool get_config(const std::string& hostname, sensor_config& config,
-                bool active) {
-    auto sensor_http = SensorHttp::create(hostname);
+                bool active, int timeout_sec) {
+    auto sensor_http = SensorHttp::create(hostname, timeout_sec);
     auto res = sensor_http->get_config_params(active);
     config = parse_config(res);
     return true;
 }
 
 bool set_config(const std::string& hostname, const sensor_config& config,
-                uint8_t config_flags) {
-    auto sensor_http = SensorHttp::create(hostname);
+                uint8_t config_flags, int timeout_sec) {
+    auto sensor_http = SensorHttp::create(hostname, timeout_sec);
 
     // reset staged config to avoid spurious errors
     auto config_params = sensor_http->active_config_params();
     Json::Value config_params_copy = config_params;
 
     // set all desired config parameters
     Json::Value config_json = to_json(config);
@@ -354,14 +360,16 @@
         sensor_http->save_config_params();
     }
 
     return true;
 }
 
 std::string get_metadata(client& cli, int timeout_sec, bool legacy_format) {
+    // Note, this function calls functions that throw std::runtime_error
+    // on timeout.
     try {
         cli.meta = collect_metadata(cli.hostname, timeout_sec);
     } catch (const std::exception& e) {
         logger().warn(std::string("Unable to retrieve sensor metadata: ") +
                       e.what());
         throw;
     }
@@ -383,15 +391,15 @@
 
     // We can't insert this logic into the light init_client since its advantage
     // is that it doesn't make netowrk calls but we need it to run every time
     // there is a valid connection to the sensor So we insert it here
     // TODO: remove after release of FW 3.2/3.3 (sufficient warning)
     sensor_config config;
     get_config(cli.hostname, config);
-    auto fw_version = SensorHttp::firmware_version(cli.hostname);
+    auto fw_version = SensorHttp::firmware_version(cli.hostname, timeout_sec);
     // only warn for people on the latest FW, as people on older FWs may not
     // care
     if (fw_version.major >= 3 &&
         config.udp_profile_lidar == UDPProfileLidar::PROFILE_LIDAR_LEGACY) {
         logger().warn(
             "Please note that the Legacy Lidar Profile will be deprecated "
             "in the sensor FW soon. If you plan to upgrade your FW, we "
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/curl_client.h` & `ouster-sdk-0.9.0/sdk/ouster_client/src/curl_client.h`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 #include <cstring>
 
 #include "http_client.h"
 
 class CurlClient : public ouster::util::HttpClient {
    public:
-    CurlClient(const std::string& base_url_) : HttpClient(base_url_) {
+    CurlClient(const std::string& base_url_, int timeout_seconds) : HttpClient(base_url_) {
         curl_global_init(CURL_GLOBAL_ALL);
         curl_handle = curl_easy_init();
         curl_easy_setopt(curl_handle, CURLOPT_WRITEFUNCTION,
                          &CurlClient::write_memory_callback);
         curl_easy_setopt(curl_handle, CURLOPT_WRITEDATA, this);
+        curl_easy_setopt(curl_handle, CURLOPT_TIMEOUT, timeout_seconds);
     }
 
     virtual ~CurlClient() override {
         curl_easy_cleanup(curl_handle);
         curl_global_cleanup();
     }
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/http_client.h` & `ouster-sdk-0.9.0/sdk/ouster_client/src/http_client.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/image_processing.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/image_processing.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/lidar_scan.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/lidar_scan.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,17 @@
 }};
 
 struct DefaultFieldsEntry {
     const std::pair<ChanField, ChanFieldType>* fields;
     size_t n_fields;
 };
 
-Table<UDPProfileLidar, DefaultFieldsEntry, 32> default_scan_fields{
+using ouster::sensor::impl::MAX_NUM_PROFILES;
+// clang-format off
+Table<UDPProfileLidar, DefaultFieldsEntry, MAX_NUM_PROFILES> default_scan_fields{
     {{UDPProfileLidar::PROFILE_LIDAR_LEGACY,
       {legacy_field_slots.data(), legacy_field_slots.size()}},
      {UDPProfileLidar::PROFILE_RNG19_RFL8_SIG16_NIR16_DUAL,
       {dual_field_slots.data(), dual_field_slots.size()}},
      {UDPProfileLidar::PROFILE_RNG19_RFL8_SIG16_NIR16,
       {single_field_slots.data(), single_field_slots.size()}},
      {UDPProfileLidar::PROFILE_RNG15_RFL8_NIR8,
@@ -122,18 +124,18 @@
 }  // namespace impl
 
 // specify sensor:: namespace for doxygen matching
 LidarScan::LidarScan(size_t w, size_t h, LidarScanFieldTypes field_types)
     : timestamp_{Header<uint64_t>::Zero(w)},
       measurement_id_{Header<uint16_t>::Zero(w)},
       status_{Header<uint32_t>::Zero(w)},
+      pose_(w, mat4d::Identity()),
       field_types_{std::move(field_types)},
       w{static_cast<std::ptrdiff_t>(w)},
       h{static_cast<std::ptrdiff_t>(h)} {
-    // TODO: error on duplicate fields
     for (const auto& ft : field_types_) {
         if (fields_.count(ft.first) > 0)
             throw std::invalid_argument("Duplicated fields found");
         fields_[ft.first] = impl::FieldSlot{ft.second, w, h};
     }
 }
 
@@ -202,14 +204,17 @@
 }
 
 Eigen::Ref<LidarScan::Header<uint32_t>> LidarScan::status() { return status_; }
 Eigen::Ref<const LidarScan::Header<uint32_t>> LidarScan::status() const {
     return status_;
 }
 
+std::vector<mat4d>& LidarScan::pose() { return pose_; }
+const std::vector<mat4d>& LidarScan::pose() const { return pose_; }
+
 bool LidarScan::complete(sensor::ColumnWindow window) const {
     const auto& status = this->status();
     auto start = window.first;
     auto end = window.second;
 
     if (start <= end) {
         return status.segment(start, end - start + 1)
@@ -227,15 +232,15 @@
 
 bool operator==(const LidarScan& a, const LidarScan& b) {
     return a.frame_id == b.frame_id && a.w == b.w && a.h == b.h &&
            a.frame_status == b.frame_status && a.fields_ == b.fields_ &&
            a.field_types_ == b.field_types_ &&
            (a.timestamp() == b.timestamp()).all() &&
            (a.measurement_id() == b.measurement_id()).all() &&
-           (a.status() == b.status()).all();
+           (a.status() == b.status()).all() && a.pose() == b.pose();
 }
 
 LidarScanFieldTypes get_field_types(const LidarScan& ls) {
     return {ls.begin(), ls.end()};
 }
 
 LidarScanFieldTypes get_field_types(const sensor::sensor_info& info) {
@@ -285,15 +290,15 @@
        << ts.maxCoeff() << ")," << std::endl;
     auto mid = ls.measurement_id().cast<uint64_t>();
     ss << "  measurement_id = (" << mid.minCoeff() << "; " << mid.mean() << "; "
        << mid.maxCoeff() << ")," << std::endl;
     auto st = ls.status().cast<uint64_t>();
     ss << "  status = (" << st.minCoeff() << "; " << st.mean() << "; "
        << st.maxCoeff() << ")" << std::endl;
-
+    ss << "  poses = (size: " << ls.pose().size() << ")" << std::endl;
     ss << "}";
     return ss.str();
 }
 
 XYZLut make_xyz_lut(size_t w, size_t h, double range_unit,
                     const mat4d& beam_to_lidar_transform,
                     const mat4d& transform,
@@ -629,50 +634,8 @@
 
         impl::foreach_field(ls, parse_field_col(), m_id, pf, col_buf);
     }
 
     return false;
 }
 
-std::string to_string(const Imu& imu) {
-    std::stringstream ss;
-    ss << "Imu: ";
-    ss << "linear_accel: [";
-    for (size_t i = 0; i < imu.linear_accel.size(); ++i) {
-        if (i > 0) ss << ", ";
-        ss << imu.linear_accel[i];
-    }
-    ss << "]";
-    ss << ", angular_vel = [";
-    for (size_t i = 0; i < imu.angular_vel.size(); ++i) {
-        if (i > 0) ss << ", ";
-        ss << imu.angular_vel[i];
-    }
-    ss << "]";
-    ss << ", ts: [";
-    std::array<std::string, 3> labels{"sys_ts", "accel_ts", "gyro_ts"};
-    for (size_t i = 0; i < imu.ts.size(); ++i) {
-        if (i > 0) ss << ", ";
-        ss << labels[i] << " = ";
-        ss << imu.ts[i];
-    }
-    ss << "]";
-    return ss.str();
-}
-
-void packet_to_imu(const uint8_t* buf, const ouster::sensor::packet_format& pf,
-                   Imu& imu) {
-    // Storing all available timestamps
-    imu.sys_ts = pf.imu_sys_ts(buf);
-    imu.accel_ts = pf.imu_accel_ts(buf);
-    imu.gyro_ts = pf.imu_gyro_ts(buf);
-
-    imu.linear_accel[0] = pf.imu_la_x(buf);
-    imu.linear_accel[1] = pf.imu_la_y(buf);
-    imu.linear_accel[2] = pf.imu_la_z(buf);
-
-    imu.angular_vel[0] = pf.imu_av_x(buf);
-    imu.angular_vel[1] = pf.imu_av_y(buf);
-    imu.angular_vel[2] = pf.imu_av_z(buf);
-}
-
 }  // namespace ouster
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/logging.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/logging.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/logging.h` & `ouster-sdk-0.9.0/sdk/ouster_client/src/logging.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/netcompat.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/netcompat.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/netcompat.h` & `ouster-sdk-0.9.0/sdk/ouster_client/src/netcompat.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/parsing.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/parsing.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     {ChanField::RAW32_WORD1, {UINT32, 0, 0, 0}},
     {ChanField::RAW32_WORD2, {UINT32, 4, 0, 0}},
     {ChanField::RAW32_WORD3, {UINT32, 8, 0, 0}},
     {ChanField::RAW32_WORD4, {UINT32, 12, 0, 0}},
     {ChanField::RAW32_WORD5, {UINT32, 16, 0, 0}},
 }};
 
-Table<UDPProfileLidar, ProfileEntry, 32> profiles{{
+Table<UDPProfileLidar, ProfileEntry, MAX_NUM_PROFILES> profiles{{
     {UDPProfileLidar::PROFILE_LIDAR_LEGACY,
      {legacy_field_info.data(), legacy_field_info.size(), 12}},
     {UDPProfileLidar::PROFILE_RNG19_RFL8_SIG16_NIR16_DUAL,
      {dual_field_info.data(), dual_field_info.size(), 16}},
     {UDPProfileLidar::PROFILE_RNG19_RFL8_SIG16_NIR16,
      {single_field_info.data(), single_field_info.size(), 12}},
     {UDPProfileLidar::PROFILE_RNG15_RFL8_NIR8,
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/sensor_http.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/sensor_http.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 using std::string;
 
 using namespace ouster::util;
 using namespace ouster::sensor;
 using namespace ouster::sensor::util;
 using namespace ouster::sensor::impl;
 
-string SensorHttp::firmware_version_string(const string& hostname) {
-    auto http_client = std::make_unique<CurlClient>("http://" + hostname);
+string SensorHttp::firmware_version_string(const string& hostname, int timeout_sec) {
+    auto http_client = std::make_unique<CurlClient>("http://" + hostname, timeout_sec);
     return http_client->get("api/v1/system/firmware");
 }
 
-version SensorHttp::firmware_version(const string& hostname) {
-    auto result = firmware_version_string(hostname);
+version SensorHttp::firmware_version(const string& hostname, int timeout_sec) {
+    auto result = firmware_version_string(hostname, timeout_sec);
     auto rgx = std::regex(R"(v(\d+).(\d+)\.(\d+))");
     std::smatch matches;
     std::regex_search(result, matches, rgx);
 
     if (matches.size() < 4) return invalid_version;
 
     try {
@@ -32,31 +32,31 @@
                        static_cast<uint16_t>(stoul(matches[2])),
                        static_cast<uint16_t>(stoul(matches[3]))};
     } catch (const std::exception&) {
         return invalid_version;
     }
 }
 
-std::unique_ptr<SensorHttp> SensorHttp::create(const string& hostname) {
-    auto fw = firmware_version(hostname);
+std::unique_ptr<SensorHttp> SensorHttp::create(const string& hostname, int timeout_sec) {
+    auto fw = firmware_version(hostname, timeout_sec);
 
     if (fw == invalid_version || fw.major < 2) {
         throw std::runtime_error(
             "SensorHttp:: create firmware version information unavailable or "
             "not fully supported version. Please upgrade your sensor to FW "
             "2.0 or later.");
     }
 
     if (fw.major == 2) {
         switch (fw.minor) {
             case 0:
                 // FW 2.0 doesn't work properly with http
                 return std::make_unique<SensorTcpImp>(hostname);
             case 1:
-                return std::make_unique<SensorHttpImp_2_1>(hostname);
+                return std::make_unique<SensorHttpImp_2_1>(hostname, timeout_sec);
             case 2:
-                return std::make_unique<SensorHttpImp_2_2>(hostname);
+                return std::make_unique<SensorHttpImp_2_2>(hostname, timeout_sec);
         }
     }
 
-    return std::make_unique<SensorHttpImp>(hostname);
+    return std::make_unique<SensorHttpImp>(hostname, timeout_sec);
 }
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/sensor_http_imp.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/sensor_http_imp.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #include "sensor_http_imp.h"
 
 #include "curl_client.h"
 
 using std::string;
 using namespace ouster::sensor::impl;
 
-SensorHttpImp::SensorHttpImp(const string& hostname)
-    : http_client(std::make_unique<CurlClient>("http://" + hostname)) {}
+SensorHttpImp::SensorHttpImp(const string& hostname, int timeout_sec)
+    : http_client(std::make_unique<CurlClient>("http://" + hostname, timeout_sec)) {}
 
 SensorHttpImp::~SensorHttpImp() = default;
 
 Json::Value SensorHttpImp::metadata() const {
     return get_json("api/v1/sensor/metadata");
 }
 
@@ -92,24 +92,24 @@
     auto result = get(url);
     if (result != validation)
         throw std::runtime_error("SensorHttpImp::execute failed! url: " + url +
                                  " returned [" + result + "], expected [" +
                                  validation + "]");
 }
 
-SensorHttpImp_2_2::SensorHttpImp_2_2(const string& hostname)
-    : SensorHttpImp(hostname) {}
+SensorHttpImp_2_2::SensorHttpImp_2_2(const string& hostname, int timeout_sec)
+    : SensorHttpImp(hostname, timeout_sec) {}
 
 void SensorHttpImp_2_2::set_udp_dest_auto() const {
     return execute("api/v1/sensor/cmd/set_udp_dest_auto",
                    "\"set_config_param\"");
 }
 
-SensorHttpImp_2_1::SensorHttpImp_2_1(const string& hostname)
-    : SensorHttpImp_2_2(hostname) {}
+SensorHttpImp_2_1::SensorHttpImp_2_1(const string& hostname, int timeout_sec)
+    : SensorHttpImp_2_2(hostname, timeout_sec) {}
 
 Json::Value SensorHttpImp_2_1::metadata() const {
     Json::Value root;
     root["sensor_info"] = sensor_info();
     root["beam_intrinsics"] = beam_intrinsics();
     root["imu_intrinsics"] = imu_intrinsics();
     root["lidar_intrinsics"] = lidar_intrinsics();
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/sensor_http_imp.h` & `ouster-sdk-0.9.0/sdk/ouster_client/src/sensor_http_imp.h`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class SensorHttpImp : public util::SensorHttp {
    public:
     /**
      * Constructs an http interface to communicate with the sensor.
      *
      * @param[in] hostname hostname of the sensor to communicate with.
      */
-    SensorHttpImp(const std::string& hostname);
+    SensorHttpImp(const std::string& hostname, int timeout_sec);
 
     /**
      * Deconstruct the sensor http interface.
      */
     ~SensorHttpImp() override;
 
     /**
@@ -126,30 +126,30 @@
    protected:
     std::unique_ptr<ouster::util::HttpClient> http_client;
 };
 
 // TODO: remove when firmware 2.2 has been fully phased out
 class SensorHttpImp_2_2 : public SensorHttpImp {
    public:
-    SensorHttpImp_2_2(const std::string& hostname);
+    SensorHttpImp_2_2(const std::string& hostname, int timeout_sec);
 
     void set_udp_dest_auto() const override;
 };
 
 /**
  * An implementation of the sensor http interface
  */
 class SensorHttpImp_2_1 : public SensorHttpImp_2_2 {
    public:
     /**
      * Constructs an http interface to communicate with the sensor.
      *
      * @param[in] hostname hostname of the sensor to communicate with.
      */
-    SensorHttpImp_2_1(const std::string& hostname);
+    SensorHttpImp_2_1(const std::string& hostname, int timeout_sec);
 
     /**
      * Queries the sensor metadata.
      *
      * @return returns a Json object of the sensor metadata.
      */
     Json::Value metadata() const override;
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/sensor_tcp_imp.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/sensor_tcp_imp.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/sensor_tcp_imp.h` & `ouster-sdk-0.9.0/sdk/ouster_client/src/sensor_tcp_imp.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_client/src/types.cpp` & `ouster-sdk-0.9.0/sdk/ouster_client/src/types.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,16 @@
     {ChanField::RAW32_WORD5, "RAW32_WORD5"},
     {ChanField::RAW32_WORD6, "RAW32_WORD6"},
     {ChanField::RAW32_WORD7, "RAW32_WORD7"},
     {ChanField::RAW32_WORD8, "RAW32_WORD8"},
     {ChanField::RAW32_WORD9, "RAW32_WORD9"},
 }};
 
-Table<UDPProfileLidar, const char*, 5> udp_profile_lidar_strings{{
+// clang-format off
+Table<UDPProfileLidar, const char*, MAX_NUM_PROFILES> udp_profile_lidar_strings{{
     {PROFILE_LIDAR_LEGACY, "LEGACY"},
     {PROFILE_RNG19_RFL8_SIG16_NIR16_DUAL, "RNG19_RFL8_SIG16_NIR16_DUAL"},
     {PROFILE_RNG19_RFL8_SIG16_NIR16, "RNG19_RFL8_SIG16_NIR16"},
     {PROFILE_RNG15_RFL8_NIR8, "RNG15_RFL8_NIR8"},
     {PROFILE_FIVE_WORD_PIXEL, "FIVE_WORD_PIXEL"},
 }};
 
@@ -364,15 +365,15 @@
 
 template <typename K, size_t N>
 static optional<K> rlookup(const impl::Table<K, const char*, N> table,
                            const char* v) {
     auto end = table.end();
     auto res = std::find_if(table.begin(), end,
                             [&](const std::pair<K, const char*>& p) {
-                                return std::strcmp(p.second, v) == 0;
+                                return p.second && std::strcmp(p.second, v) == 0;
                             });
 
     return res == end ? nullopt : make_optional<K>(res->first);
 }
 
 std::string to_string(lidar_mode mode) {
     auto res = lookup(impl::lidar_mode_strings, mode);
@@ -756,15 +757,16 @@
         // GCC 8.3.1
         optional<UDPProfileLidar> profile{nullopt};
         profile =
             udp_profile_lidar_of_string(root["udp_profile_lidar"].asString());
         if (profile) {
             format.udp_profile_lidar = profile.value();
         } else {
-            throw std::runtime_error{"Unexpected udp lidar profile"};
+            throw std::runtime_error{"Unexpected udp lidar profile: " +
+                                     root["udp_profile_lidar"].asString()};
         }
     } else {
         logger().warn("No lidar profile found. Using LEGACY lidar profile");
         format.udp_profile_lidar = PROFILE_LIDAR_LEGACY;
     }
 
     if (root.isMember("udp_profile_imu")) {
@@ -787,15 +789,15 @@
         // 0)");
         format.fps = 0;
     }
 
     return format;
 }  // namespace sensor
 
-static sensor_info parse_legacy(const std::string& meta) {
+static sensor_info parse_legacy(const std::string& meta, bool skip_beam_validation) {
     Json::Value root{};
     Json::CharReaderBuilder builder{};
     std::string errors{};
     std::stringstream ss{meta};
 
     if (meta.size()) {
         if (!Json::parseFromStream(builder, ss, &root, &errors))
@@ -1026,16 +1028,20 @@
                                      [](double k) { return k == 0.0; });
         if (all_zeros) {
             throw std::runtime_error{"Field " + name +
                                      " in the metadata cannot all be zeros."};
         }
     };
 
-    zero_check(info.beam_altitude_angles, "beam_altitude_angles");
-    zero_check(info.beam_azimuth_angles, "beam_azimuth_angles");
+    if (!skip_beam_validation) {
+        zero_check(info.beam_altitude_angles, "beam_altitude_angles");
+        zero_check(info.beam_azimuth_angles, "beam_azimuth_angles");
+    } else {
+        logger().warn("Skipping all 0 beam angle check");
+    }
 
     info.extrinsic = mat4d::Identity();
 
     // default to 0 if keys are not present
     info.init_id = root["initialization_id"].asInt();
     info.udp_port_lidar = root["udp_port_lidar"].asInt();
     info.udp_port_imu = root["udp_port_imu"].asInt();
@@ -1097,51 +1103,51 @@
     Json::StreamWriterBuilder write_builder;
     write_builder["enableYAMLCompatibility"] = true;
     write_builder["precision"] = 6;
     write_builder["indentation"] = "    ";
     return Json::writeString(write_builder, result);
 }
 
-sensor_info parse_metadata(const std::string& metadata) {
+sensor_info parse_metadata(const std::string& metadata, bool skip_beam_validation) {
     Json::Value root{};
     Json::CharReaderBuilder builder{};
     std::string errors{};
     std::stringstream ss{metadata};
 
     if (metadata.size()) {
         if (!Json::parseFromStream(builder, ss, &root, &errors))
             throw std::runtime_error{
                 "Errors parsing metadata for parse_metadata: " + errors};
     }
 
     sensor_info info{};
     if (is_new_format(metadata)) {
         logger().debug("parsing non-legacy metadata format");
-        info = parse_legacy(convert_to_legacy(metadata));
+        info = parse_legacy(convert_to_legacy(metadata), skip_beam_validation);
     } else {
         logger().debug("parsing legacy metadata format");
-        info = parse_legacy(metadata);
+        info = parse_legacy(metadata, skip_beam_validation);
     }
     return info;
 }
 
-sensor_info metadata_from_json(const std::string& json_file) {
+sensor_info metadata_from_json(const std::string& json_file, bool skip_beam_validation) {
     std::stringstream buf{};
     std::ifstream ifs{};
     ifs.open(json_file);
     buf << ifs.rdbuf();
     ifs.close();
 
     if (!ifs) {
         std::stringstream ss;
         ss << "Failed to read metadata file: " << json_file;
         throw std::runtime_error{ss.str()};
     }
 
-    return parse_metadata(buf.str());
+    return parse_metadata(buf.str(), skip_beam_validation);
 }
 
 std::string to_string(const sensor_info& info) {
     Json::Value root{};
 
     root["client_version"] = client_version();
     root["hostname"] = "";
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_pcap/CMakeLists.txt` & `ouster-sdk-0.9.0/sdk/ouster_pcap/CMakeLists.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 if(WIN32)
   target_compile_options(ouster_pcap PRIVATE /wd4200)
   target_link_libraries(ouster_pcap PUBLIC ws2_32)
 endif()
 target_link_libraries(ouster_pcap
   PUBLIC
     OusterSDK::ouster_client
-  PRIVATE ${PCAP_LIBRARY} libtins)
+  PRIVATE libpcap::libpcap libtins::libtins)
 add_library(OusterSDK::ouster_pcap ALIAS ouster_pcap)
 
 # ==== Install ====
 install(TARGETS ouster_pcap
   EXPORT ouster-sdk-targets
   LIBRARY DESTINATION lib
   ARCHIVE DESTINATION lib
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_pcap/include/ouster/indexed_pcap_reader.h` & `ouster-sdk-0.9.0/sdk/ouster_pcap/include/ouster/indexed_pcap_reader.h`

 * *Files 18% similar despite different names*

```diff
@@ -7,34 +7,55 @@
 #include "ouster/pcap.h"
 #include "ouster/os_pcap.h"
 #include "ouster/types.h"
 
 namespace ouster {
 namespace sensor_utils {
 
+
+struct PcapIndex {
+    using frame_index = std::vector<uint64_t>;                      ///< Maps a frame number to a file offset
+    std::vector<frame_index> frame_indices_;                        ///< frame index for each sensor
+
+    PcapIndex(size_t num_sensors)
+    : frame_indices_(num_sensors) {}
+
+    /**
+     * Returns the number of frames in the frame index for the given sensor index.
+     *
+     * @param sensor_index[in] The position of the sensor for which to retrieve the desired frame count.
+     * @return The number of frames in the sensor's frame index.
+     */
+    size_t frame_count(size_t sensor_index) const;
+
+    /**
+     * Seeks the given reader to the given frame number for the given sensor index
+     */
+    void seek_to_frame(PcapReader& reader, size_t sensor_index, unsigned int frame_number);
+};
+
 /**
  * A PcapReader that allows seeking to the start of a lidar frame.
- * To do this, the constructor calls `get_stream_info`, which in turn calls
- * IndexedPcapReader::update_index_for_current_packet for each packet.
- * This allows us to compute the index and obtain the stream_info while reading
- * the PCAP file only once.
+ *
+ * The index must be computed by iterating through all packets and calling
+ * `update_index_for_current_packet()` for each one.
  */
 struct IndexedPcapReader : public PcapReader {
-    using frame_index = std::vector<uint64_t>;                      ///< Maps a frame number to a file offset
 
     /**
      * @param pcap_filename[in] A file path of the pcap to read
      * @param metadata_filenames[in] A vector of sensor metadata file paths
      */
     IndexedPcapReader(
         const std::string& pcap_filename,
-        const std::vector<std::string>& metadata_filenames,
-        std::function<void(uint64_t, uint64_t, uint64_t)> progress_callback
+        const std::vector<std::string>& metadata_filenames
     );
 
+    const PcapIndex& get_index() const;
+
     /**
      * Attempts to match the current packet to one of the sensor info objects
      * and returns the appropriate packet format if there is one
      *
      * @return An optional packet format for the current packet
      */
     nonstd::optional<size_t> sensor_idx_for_current_packet() const;
@@ -43,46 +64,27 @@
      * @return the current packet's frame_id
      * if the packet is associated with a sensor (and its corresponding packet format)
      */
     nonstd::optional<uint16_t> current_frame_id() const;
 
     /**
      * Updates the frame index for the current packet
-     *
-     * Important: this method is only meant to be invoked from `get_stream_info`!
-     */
-    void update_index_for_current_packet();
-
-    /**
-     * @return The stream_info associated with this PcapReader
-     */
-    std::shared_ptr<stream_info> get_stream_info() const; // TODO move to parent class
-
-    /**
-     * Seeks to the given frame number for the given sensor index
-     */
-    void seek_to_frame(size_t sensor_index, unsigned int frame_number);
-
-    /**
-     * Returns the number of frames in the frame index for the given sensor index.
-     *
-     * @param sensor_index[in] The position of the sensor for which to retrieve the desired frame count.
-     * @return The number of frames in the sensor's frame index.
+     * @return the progress of indexing as an int from [0, 100]
      */
-    size_t frame_count(size_t sensor_index) const;
+    int update_index_for_current_packet();
 
     /**
      * Return true if the frame_id from the packet stream has rolled over,
      * hopefully avoiding spurious result that could occur from out of order or dropped packets.
      *
      * @return true if the frame id has rolled over.
      */
     static bool frame_id_rolled_over(uint16_t previous, uint16_t current);
 
+
     std::vector<ouster::sensor::sensor_info> sensor_infos_;         ///< A vector of sensor_info that correspond to the provided metadata files
-    std::shared_ptr<stream_info> stream_info_;                      ///< TODO: move to parent class
-    std::vector<frame_index> frame_indices_;                        ///< frame index for each sensor
+    PcapIndex index_;
     std::vector<nonstd::optional<uint16_t>> previous_frame_ids_;  ///< previous frame id for each sensor
 };
 
 } // namespace sensor_utils
 } // namespace ouster
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_pcap/include/ouster/os_pcap.h` & `ouster-sdk-0.9.0/sdk/ouster_pcap/include/ouster/os_pcap.h`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,44 @@
 #pragma once
 
 #include <chrono>
 #include <cstdint>
 #include <memory>
 #include <string>
 #include <map>
+#include <unordered_map>
 #include <vector>
 #include <functional>
 
 #include "ouster/types.h"
 #include "ouster/pcap.h"
+namespace ouster {
+namespace sensor_utils {
+/**
+ * Structure representing a hash key/sorting key for a udp stream
+ */
+struct stream_key {
+    std::string dst_ip;          ///< The destination IP
+    std::string src_ip;          ///< The source IP
+    int src_port;                ///< The src port
+    int dst_port;                ///< The destination port
+
+    bool operator==(const struct stream_key &other) const;
+};
+}}
+
+template<>
+struct std::hash<ouster::sensor_utils::stream_key> {
+    std::size_t operator()(const ouster::sensor_utils::stream_key& key) const noexcept {
+        return std::hash<std::string>{}(key.src_ip) ^
+               (std::hash<std::string>{}(key.src_ip) << 1) ^
+               (std::hash<int>{}(key.src_port << 2)) ^
+               (std::hash<int>{}(key.dst_port << 3));
+    }
+};
 
 namespace ouster {
 namespace sensor_utils {
 
 using ts = std::chrono::microseconds;  ///< Microsecond timestamp
 
 /**
@@ -30,30 +55,15 @@
  * @param[inout] stream_in The pre-existing ostream to concat with data.
  * @param[in] data The packet_info to output.
  *
  * @return The new output stream containing concatted stream_in and data.
  */
 std::ostream& operator<<(std::ostream& stream_in, const packet_info& data);
 
-/**
- * Structure representing a hash key/sorting key for a udp stream
- */
-struct stream_key {
-    std::string dst_ip;          ///< The destination IP
-    std::string src_ip;          ///< The source IP
-    int src_port;                ///< The src port
-    int dst_port;                ///< The destination port
 
-    bool operator==(const struct stream_key &other) const;
-    bool operator!=(const struct stream_key &other) const;
-    bool operator<(const struct stream_key &other) const;
-    bool operator>(const struct stream_key &other) const;
-    bool operator<=(const struct stream_key &other) const;
-    bool operator>=(const struct stream_key &other) const;
-};
 
 /**
  * Structure representing a hash key/sorting key for a udp stream
  */
 struct guessed_ports {
     int lidar;                   ///< Guessed lidar port
     int imu;                     ///< Guessed imu port
@@ -98,15 +108,15 @@
 struct stream_info {
     uint64_t total_packets;             ///< The total number of packets detected
     uint32_t encapsulation_protocol;    ///< The encapsulation protocol for the pcap file
 
     ts timestamp_max;                   ///< The latest timestamp detected
     ts timestamp_min;                   ///< The earliest timestamp detected
 
-    std::map<stream_key, stream_data> udp_streams; ///< Datastructure containing info on all of the different streams
+    std::unordered_map<stream_key, stream_data> udp_streams; ///< Datastructure containing info on all of the different streams
 };
 
 /**
  * To string method for stream info structs.
  *
  * @param[inout] stream_in The pre-existing ostream to concat with data.
  * @param[in] data The stream_info to output.
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_pcap/include/ouster/pcap.h` & `ouster-sdk-0.9.0/sdk/ouster_pcap/include/ouster/pcap.h`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
      * @return A packet_info object on the current packet
      */
     const packet_info& current_info() const;
 
     /**
      * @return The size of the PCAP file in bytes
      */
-    uint64_t file_size() const;
+    int64_t file_size() const;
 
     /**
      * Return the read position to the start of the PCAP file
      */
     void reset();
 
     /**
@@ -109,17 +109,19 @@
      * @pre \paramname{offset} must be the offset of a PCAP
      * record header. If any other value is provided,
      * subsequent packet reads from this PcapReader will be
      * invalid until \functionname{reset} is called.
      */
     void seek(uint64_t offset);
 
+    int64_t current_offset() const;
+
    private:
-    uint64_t file_size_{};
-    uint64_t file_start_{};
+    int64_t file_size_{};
+    int64_t file_start_{};
 };
 
 /**
  * Class for dealing with writing udp pcap files
  */
 class PcapWriter {
    public:
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_pcap/src/indexed_pcap_reader.cpp` & `ouster-sdk-0.9.0/sdk/ouster_pcap/src/indexed_pcap_reader.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,24 @@
 #include "ouster/indexed_pcap_reader.h"
 
 namespace ouster {
 namespace sensor_utils {
 
 IndexedPcapReader::IndexedPcapReader(
     const std::string& pcap_filename,
-    const std::vector<std::string>& metadata_filenames,
-    std::function<void(uint64_t, uint64_t, uint64_t)> progress_callback)
+    const std::vector<std::string>& metadata_filenames)
     : PcapReader(pcap_filename)
-    , frame_indices_(metadata_filenames.size())
+    , index_(metadata_filenames.size())
     , previous_frame_ids_(metadata_filenames.size())
 {
     for(const std::string& metadata_filename : metadata_filenames) {
         sensor_infos_.push_back(
             ouster::sensor::metadata_from_json(metadata_filename)
         );
     }
-    stream_info_ = ouster::sensor_utils::get_stream_info(*this, progress_callback, 256, -1);
-    if(sensor_infos_.size() == 1 && sensor_infos_[0].udp_port_lidar == 0) {
-        // guess lidar port for a single sensor if it is unspecified in sensor info
-        const ouster::sensor::packet_format& pf = ouster::sensor::packet_format(sensor_infos_[0]);
-        std::vector<guessed_ports> ports = guess_ports(
-            *stream_info_,
-            pf.lidar_packet_size, pf.imu_packet_size,
-            sensor_infos_[0].udp_port_lidar, sensor_infos_[0].udp_port_imu
-        );
-        if(ports.empty()) {
-            throw std::runtime_error("IndexedPcapReader: unable to determine lidar UDP port");
-        }
-        sensor_infos_[0].udp_port_lidar = ports[0].lidar;
-        sensor_infos_[0].udp_port_imu = ports[0].imu;
-    }
 }
 
 nonstd::optional<size_t> IndexedPcapReader::sensor_idx_for_current_packet() const {
     const auto& pkt_info = current_info();
     for(size_t i = 0; i < sensor_infos_.size(); i++) {
         if(pkt_info.dst_port == sensor_infos_[i].udp_port_lidar) {
             // TODO use the packet format and match serial number if it's available
@@ -56,37 +40,38 @@
 }
 
 bool IndexedPcapReader::frame_id_rolled_over(uint16_t previous, uint16_t current) {
     static_assert(sizeof(uint16_t) == 2, "expected frame_id to be two bytes");
     return previous > 0xff00 && current < 0x00ff;
 }
 
-void IndexedPcapReader::update_index_for_current_packet() {
+int IndexedPcapReader::update_index_for_current_packet() {
     if(nonstd::optional<size_t> sensor_info_idx = sensor_idx_for_current_packet()) {
         if(nonstd::optional<uint16_t> frame_id = current_frame_id()) {
             if(!previous_frame_ids_[*sensor_info_idx]
                 || *previous_frame_ids_[*sensor_info_idx] < *frame_id  // frame_id is greater than previous
                 || frame_id_rolled_over(*previous_frame_ids_[*sensor_info_idx], *frame_id)
             ) {
-                frame_indices_[*sensor_info_idx].push_back(current_info().file_offset);
+                index_.frame_indices_[*sensor_info_idx].push_back(current_info().file_offset);
                 previous_frame_ids_[*sensor_info_idx] = *frame_id;
             }
         }
     }
+    return static_cast<int>(100 * static_cast<float>(current_offset())/file_size());
 }
 
-void IndexedPcapReader::seek_to_frame(size_t sensor_index, unsigned int frame_number) {
-    seek(frame_indices_.at(sensor_index).at(frame_number));
+const PcapIndex& IndexedPcapReader::get_index() const {
+    return index_;
 }
 
-
-size_t IndexedPcapReader::frame_count(size_t sensor_index) const {
-    return frame_indices_.at(sensor_index).size();
+void PcapIndex::seek_to_frame(PcapReader& reader, size_t sensor_index, unsigned int frame_number) {
+    reader.seek(frame_indices_.at(sensor_index).at(frame_number));
 }
 
-std::shared_ptr<stream_info> IndexedPcapReader::get_stream_info() const {
-    return stream_info_;
+
+size_t PcapIndex::frame_count(size_t sensor_index) const {
+    return frame_indices_.at(sensor_index).size();
 }
 
 } // namespace sensor_utils
 } // namespace ouster
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_pcap/src/os_pcap.cpp` & `ouster-sdk-0.9.0/sdk/ouster_pcap/src/os_pcap.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -65,40 +65,14 @@
 bool stream_key::operator==(const struct stream_key &other) const {
     return dst_ip == other.dst_ip &&
         src_ip == other.src_ip &&
         src_port == other.src_port &&
         dst_port == other.dst_port;
 }
 
-bool stream_key::operator!=(const struct stream_key &other) const {
-    return !(*this == other);
-}
-
-bool stream_key::operator<=(const struct stream_key &other) const {
-    return dst_ip <= other.dst_ip &&
-        src_ip <= other.src_ip &&
-        dst_port <= other.dst_port &&
-        src_port <= other.src_port;
-}
-
-bool stream_key::operator>=(const struct stream_key &other) const {
-    return dst_ip >= other.dst_ip &&
-        src_ip >= other.src_ip &&
-        dst_port >= other.dst_port &&
-        src_port >= other.src_port;
-}
-
-bool stream_key::operator<(const struct stream_key &other) const {
-    return *this <= other && *this != other;
-}
-
-bool stream_key::operator>(const struct stream_key &other) const {
-    return *this >= other && *this != other;
-}
-
 std::ostream& operator<<(std::ostream& stream_in, const stream_key& data) {
     stream_in << "Source IP: \"" << data.src_ip << "\" " << std::endl;
     stream_in << "Destination IP: \"" << data.dst_ip << "\" " << std::endl;
     stream_in << "Source Port: " << data.src_port << std::endl;
     stream_in << "Destination Port: " << data.dst_port << std::endl;
     return stream_in;
 }
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_pcap/src/pcap.cpp` & `ouster-sdk-0.9.0/sdk/ouster_pcap/src/pcap.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,26 @@
  * @TODO check that the header casting is idiomatic libpcap
  * @TODO warn on dropped packets when pcap contains garbage, when fragments
  * missing, buffer reused before sending
  * @TODO split up reading / playback
  * @TODO improve error reporting
  */
 
+#define _FILE_OFFSET_BITS 64
 #include "ouster/pcap.h"
 
 #if defined _WIN32
 #include <winsock2.h>
+#define FTELL ftell
+#define FSEEK fseek
 #else
 #include <arpa/inet.h>  // inet_ntop
 #include <sys/time.h>   // timeval
+#define FTELL ftello
+#define FSEEK fseeko
 #endif
 
 #include <pcap.h>
 #if defined _WIN32
 #include <pcap/bpf.h>
 #else
 #include <pcap/dlt.h>
@@ -69,50 +74,60 @@
         fileSizeStream.seekg(0, std::ios::end);
         file_size_ = fileSizeStream.tellg();
     }
     impl->pcap_reader = std::make_unique<Tins::FileSniffer>(file);
     impl->encap_proto = impl->pcap_reader->link_type();
     impl->pcap_reader_internals =
         pcap_file(impl->pcap_reader->get_pcap_handle());
-    file_start_ = ftell(impl->pcap_reader_internals);
+    file_start_ = FTELL(impl->pcap_reader_internals);
 }
 
 PcapReader::~PcapReader() {}
 
 const uint8_t* PcapReader::current_data() const { return data; }
 
 size_t PcapReader::current_length() const { return info.payload_size; }
 
 const packet_info& PcapReader::current_info() const { return info; }
 
 void PcapReader::seek(uint64_t offset) {
     if(offset < sizeof(struct pcap_file_header)) {
         offset = sizeof(struct pcap_file_header);
     }
-    if(fseek(impl->pcap_reader_internals, offset, SEEK_SET)) {
+    if(FSEEK(impl->pcap_reader_internals, offset, SEEK_SET)) {
         throw std::runtime_error("pcap seek failed");
     }
 }
 
-uint64_t PcapReader::file_size() const {
+int64_t PcapReader::file_size() const {
     return file_size_;
 }
 
+int64_t PcapReader::current_offset() const {
+    int64_t ret = FTELL(impl->pcap_reader_internals);
+
+    if(ret == -1L) {
+        fclose(impl->pcap_reader_internals);
+        throw std::runtime_error("ftell error: errno " + std::to_string(errno));
+    }
+    return ret;
+}
+
 void PcapReader::reset() {
     seek(file_start_);
 }
 
 size_t PcapReader::next_packet() {
     size_t result = 0;
 
     bool reassm = false;
     int reassm_packets = 0;
     while (!reassm) {
         reassm_packets++;
-        info.file_offset = ftell(impl->pcap_reader_internals);
+        info.file_offset = current_offset();
         impl->packet_cache = impl->pcap_reader->next_packet();
         if (impl->packet_cache) {
             auto pdu = impl->packet_cache.pdu();
             if (pdu) {
                 info.packet_size = pdu->size();
                 IP* ip = pdu->find_pdu<IP>();
                 IPv6* ipv6 = pdu->find_pdu<IPv6>();
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/CMakeLists.txt` & `ouster-sdk-0.9.0/sdk/ouster_viz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/include/ouster/point_viz.h` & `ouster-sdk-0.9.0/sdk/ouster_viz/include/ouster/point_viz.h`

 * *Files 2% similar despite different names*

```diff
@@ -748,14 +748,24 @@
      * @param[in] translation translation vector array, column major, where each
      * row is a translation vector. That is, the vth translation is t[v], t[w +
      * v], t[2 * w + v]
      */
     void set_column_poses(const float* rotation, const float* translation);
 
     /**
+     * Set the per-column poses, so that the point corresponding to the
+     * pixel at row u, column v in the staggered lidar scan is transformed
+     * by the vth pose, given as a homogeneous transformation matrix.
+     *
+     * @param[in] column_poses array of 4x4 pose elements and length w
+     * (i.e. [wx4x4]) column-storage
+     */
+    void set_column_poses(const float* column_poses);
+
+    /**
      * Set the point cloud color palette.
      *
      * @param[in] palette the new palette to use, must have size 3*palette_size
      * @param[in] palette_size the number of colors in the new palette
      */
     void set_palette(const float* palette, size_t palette_size);
 
@@ -965,14 +975,21 @@
      * Clear dirty flags.
      *
      * Resets any changes since the last call to PointViz::update()
      */
     void clear();
 
     /**
+     * Set all dirty flags.
+     *
+     * Re-sets everything so the object is always redrawn.
+     */
+    void dirty();
+
+    /**
      * Update label text.
      *
      * @param[in] text new text to display
      */
     void set_text(const std::string& text);
 
     /**
```

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/camera.cpp` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/camera.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/camera.h` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/camera.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/cloud.cpp` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/cloud.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/cloud.h` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/cloud.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/colormaps.h` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/colormaps.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/common.h` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/common.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/glfw.cpp` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/glfw.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/glfw.h` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/glfw.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/gltext.h` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/gltext.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/image.cpp` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/image.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/image.h` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/image.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/misc.cpp` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/misc.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/misc.h` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/misc.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/ouster_viz/src/point_viz.cpp` & `ouster-sdk-0.9.0/sdk/ouster_viz/src/point_viz.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -379,14 +379,15 @@
 }
 
 void PointViz::add(const std::shared_ptr<Cuboid>& cuboid) {
     pimpl->cuboids.add(cuboid);
 }
 
 void PointViz::add(const std::shared_ptr<Label>& label) {
+    label->dirty();
     pimpl->labels.add(label);
 }
 
 void PointViz::add(const std::shared_ptr<Image>& image) {
     pimpl->images.add(image);
 }
 
@@ -587,14 +588,31 @@
         for (size_t rgb = 0; rgb < 3; rgb++) {
             transform_data_[9 * w_ + 3 * v + rgb] = translation[v + rgb * w_];
         }
     }
     transform_changed_ = true;
 }
 
+void Cloud::set_column_poses(const float* column_poses) {
+    // columns_poses: is [Wx4x4] and column-major storage
+    for (size_t v = 0; v < w_; v++) {
+        for (size_t u = 0; u < 3; u++) {
+            for (size_t r = 0; r < 3; r++) {
+                transform_data_[(r * w_ + v) * 3 + u] =
+                    column_poses[(r * 4 + u) * w_ + v];
+            }
+        }
+        for (size_t u = 0; u < 3; u++) {
+            transform_data_[9 * w_ + 3 * v + u] =
+                column_poses[(3 * 4 + u) * w_ + v];
+        }
+    }
+    transform_changed_ = true;
+}
+
 void Cloud::set_palette(const float* palette, size_t palette_size) {
     palette_data_.resize(palette_size * 3);
     std::copy(palette, palette + (palette_size * 3), palette_data_.begin());
     palette_changed_ = true;
 }
 
 Image::Image() = default;
@@ -722,14 +740,21 @@
 void Label::clear() {
     text_changed_ = false;
     pos_changed_ = false;
     scale_changed_ = false;
     rgba_changed_ = false;
 }
 
+void Label::dirty() {
+    text_changed_ = true;
+    pos_changed_ = true;
+    scale_changed_ = true;
+    rgba_changed_ = true;
+}
+
 void Label::set_position(const vec3d& position) {
     position_ = position;
     pos_changed_ = true;
     is_3d_ = true;
 }
 
 void Label::set_position(float x, float y, bool align_right, bool align_top) {
```

### Comparing `ouster-sdk-0.8.1/sdk/tests/CMakeLists.txt` & `ouster-sdk-0.9.0/sdk/tests/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -24,28 +24,28 @@
 add_executable(lidar_scan_test lidar_scan_test.cpp)
 
 target_link_libraries(lidar_scan_test OusterSDK::ouster_client GTest::gtest GTest::gtest_main)
 
 add_test(NAME lidar_scan_test COMMAND lidar_scan_test --gtest_output=xml:lidar_scan_test.xml)
 set_tests_properties(
     lidar_scan_test
-        PROPERTIES 
-        ENVIRONMENT 
+        PROPERTIES
+        ENVIRONMENT
         DATA_DIR=${CMAKE_CURRENT_LIST_DIR}/metadata/
 )
 
 add_executable(cartesian_test cartesian_test.cpp)
 
 target_link_libraries(cartesian_test OusterSDK::ouster_client GTest::gtest GTest::gtest_main)
 
 add_test(NAME cartesian_test COMMAND cartesian_test --gtest_output=xml:cartesian_test.xml)
 set_tests_properties(
   cartesian_test
-        PROPERTIES 
-        ENVIRONMENT 
+        PROPERTIES
+        ENVIRONMENT
         DATA_DIR=${CMAKE_CURRENT_LIST_DIR}/metadata/
 )
 
 add_executable(metadata_errors_test metadata_errors_test.cpp)
 
 target_link_libraries(metadata_errors_test OusterSDK::ouster_client GTest::gtest GTest::gtest_main)
 
@@ -64,7 +64,13 @@
 add_test(NAME pcap_test COMMAND pcap_test --gtest_output=xml:pcap_test.xml)
 set_tests_properties(
     pcap_test
         PROPERTIES
         ENVIRONMENT
         DATA_DIR=${CMAKE_CURRENT_LIST_DIR}/pcaps/
 )
+
+add_executable(profile_extension_test profile_extension_test.cpp)
+
+target_link_libraries(profile_extension_test OusterSDK::ouster_client GTest::gtest GTest::gtest_main)
+
+add_test(NAME profile_extension_test COMMAND profile_extension_test --gtest_output=xml:profile_extension_test.xml)
```

### Comparing `ouster-sdk-0.8.1/sdk/tests/bcompat_meta_json_test.cpp` & `ouster-sdk-0.9.0/sdk/tests/bcompat_meta_json_test.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/bcompat_sensor_info_data.h` & `ouster-sdk-0.9.0/sdk/tests/bcompat_sensor_info_data.h`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/cartesian_test.cpp` & `ouster-sdk-0.9.0/sdk/tests/cartesian_test.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/lidar_scan_test.cpp` & `ouster-sdk-0.9.0/sdk/tests/lidar_scan_test.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_12_os1-991913000010-64.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_12_os1-991913000010-64.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_12_os1-991937000062-16A0_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_12_os1-991937000062-16A0_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_12_os1-991937000062-64_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_12_os1-991937000062-64_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_13_os1-991913000010-64.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_13_os1-991913000010-64.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_13_os1-991937000062-16A0_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_13_os1-991937000062-16A0_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_13_os1-991937000062-32A02_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_13_os1-991937000062-32A02_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_13_os1-991937000062-64_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_13_os1-991937000062-64_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_14_6cccd_os-882002000138-128_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_14_6cccd_os-882002000138-128_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_14_6cccd_os-882002000138-32U0_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_14_6cccd_os-882002000138-32U0_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_14_6cccd_os-882002000138-64U02_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_14_6cccd_os-882002000138-64U02_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_14_beta_os-882004000055-128_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_14_beta_os-882004000055-128_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_14_beta_os1-991937000062-16A0_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_14_beta_os1-991937000062-16A0_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_14_beta_os1-991937000062-32A02_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_14_beta_os1-991937000062-32A02_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/1_14_beta_os1-991937000062-64_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/1_14_beta_os1-991937000062-64_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_0_0_os1-991913000010-64.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_0_0_os1-991913000010-64.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_0_0_os1-992008000494-128_col_win_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_0_0_os1-992008000494-128_col_win_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_0_rc2_os-992011000121-32U0_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_0_rc2_os-992011000121-32U0_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_1_2_os1-991913000010-64.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_1_2_os1-991913000010-64.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_1_2_os1-991913000010-64_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_1_2_os1-991913000010-64_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_2_os-992119000444-128.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_2_os-992119000444-128.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_2_os-992119000444-128_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_2_os-992119000444-128_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_3_1_os-992146000760-128.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_3_1_os-992146000760-128.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_3_1_os-992146000760-128_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_3_1_os-992146000760-128_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_3_os-992146000760-128.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_3_os-992146000760-128.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_3_os-992146000760-128_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_3_os-992146000760-128_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_4_0_os-992146000760-128.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_4_0_os-992146000760-128.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_4_0_os-992146000760-128_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_4_0_os-992146000760-128_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_5_0_os-992146000760-128.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_5_0_os-992146000760-128.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/2_5_0_os-992146000760-128_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/2_5_0_os-992146000760-128_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/3_0_1_os-122246000293-128.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/3_0_1_os-122246000293-128.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/3_0_1_os-122246000293-128_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/3_0_1_os-122246000293-128_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/malformed/complete_but_all_zeros_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/malformed/complete_but_all_zeros_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/malformed/garbled_legacy_and_nonlegacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/malformed/garbled_legacy_and_nonlegacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/malformed/incomplete_data_format_legacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/malformed/incomplete_data_format_legacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/malformed/incomplete_data_format_nonlegacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/malformed/incomplete_data_format_nonlegacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/malformed/incomplete_no_calref_nonlegacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/malformed/incomplete_no_calref_nonlegacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/malformed/incomplete_no_sensor_info_nonlegacy.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/malformed/incomplete_no_sensor_info_nonlegacy.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/malformed/incorrect_nbeam_angles_legacy_113.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/malformed/incorrect_nbeam_angles_legacy_113.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/malformed/legacy_with_calibration_status.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/malformed/legacy_with_calibration_status.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata/ouster-studio-reduced-config-v1.json` & `ouster-sdk-0.9.0/sdk/tests/metadata/ouster-studio-reduced-config-v1.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/metadata_errors_test.cpp` & `ouster-sdk-0.9.0/sdk/tests/metadata_errors_test.cpp`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcap_test.cpp` & `ouster-sdk-0.9.0/sdk/tests/pcap_test.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -102,53 +102,65 @@
     PcapReader pcap(filename);
     pcap.seek(file_size(filename) + 1);
 
     // attempting to read past end of file is not an error, either
     EXPECT_EQ(pcap.next_packet(), 0);
 }
 
-void progress_callback(uint64_t, uint64_t, uint64_t) {}
-
-
 TEST(IndexedPcapReader, constructor) {
     // it should be constructed with the correct number of indices
     // and previous frame counts (one for each metadata file)
     auto data_dir = getenvs("DATA_DIR");
     std::string filename = data_dir + "/OS-0-32-U1_v2.2.0_1024x10-single-packet.pcap";
     std::string meta_filename = data_dir + "/OS-0-32-U1_v2.2.0_1024x10.json";
 
-    IndexedPcapReader pcap(filename, {meta_filename, meta_filename, meta_filename}, progress_callback);
-    EXPECT_EQ(pcap.frame_indices_.size(), 3);
+    IndexedPcapReader pcap(filename, {meta_filename, meta_filename, meta_filename});
+    EXPECT_EQ(pcap.index_.frame_indices_.size(), 3);
     EXPECT_EQ(pcap.previous_frame_ids_.size(), 3);
 }
 
 TEST(IndexedPcapReader, frame_count) {
     // it should raise std::out_of_range if there is no sensor at that position
     auto data_dir = getenvs("DATA_DIR");
     std::string filename = data_dir + "/OS-0-32-U1_v2.2.0_1024x10-single-packet.pcap";
-    IndexedPcapReader pcap(filename, {}, progress_callback);
-    pcap.frame_indices_.push_back(IndexedPcapReader::frame_index());
-    pcap.frame_indices_.at(0).push_back(0);
+    IndexedPcapReader pcap(filename, {});
+    pcap.index_.frame_indices_.push_back(PcapIndex::frame_index());
+    pcap.index_.frame_indices_.at(0).push_back(0);
 
-    EXPECT_EQ(pcap.frame_count(0), 1);
-    EXPECT_THROW(pcap.frame_count(1), std::out_of_range);
+    EXPECT_EQ(pcap.index_.frame_count(0), 1);
+    EXPECT_THROW(pcap.index_.frame_count(1), std::out_of_range);
 }
 
 TEST(IndexedPcapReader, seek_to_frame) {
     // it should raise std::out_of_range if there is no sensor or frame at that position
     auto data_dir = getenvs("DATA_DIR");
-    std::string filename = data_dir + "/OS-0-32-U1_v2.2.0_1024x10-single-packet.pcap";
-    std::string meta_filename = data_dir + "/OS-0-32-U1_v2.2.0_1024x10.json";
-    IndexedPcapReader pcap(filename, {meta_filename}, progress_callback);
-    pcap.frame_indices_.push_back(IndexedPcapReader::frame_index());
-
-    EXPECT_EQ(pcap.frame_count(0), 1);
-    EXPECT_NO_THROW(pcap.seek_to_frame(0, 0));
-    EXPECT_THROW(pcap.seek_to_frame(0, 1), std::out_of_range);
-    EXPECT_THROW(pcap.seek_to_frame(1, 1), std::out_of_range);
+    std::string filename = data_dir + "/OS-2-128-U1_v2.3.0_1024x10.pcap";
+    std::string meta_filename = data_dir + "/OS-2-128-U1_v2.3.0_1024x10.json";
+    IndexedPcapReader pcap(filename, {meta_filename});
+
+    std::vector<int> progress;
+    while(pcap.next_packet()) {
+        progress.push_back(pcap.update_index_for_current_packet());
+    }
+    ASSERT_GT(progress.size(), 2);
+    // progress values are in the range and are increasing [1, 100]
+    int prev_progress = 0l;
+    for(size_t i = 0; i < progress.size(); i++) {
+        EXPECT_GE(progress[i], 1);
+        EXPECT_LE(progress[i], 100);
+        EXPECT_GE(progress[i], prev_progress);
+        prev_progress = progress[i];
+    }
+    EXPECT_EQ(progress[progress.size() - 1], 100); // last progress value is 100
+    pcap.index_.frame_indices_.push_back(PcapIndex::frame_index());
+
+    EXPECT_EQ(pcap.index_.frame_count(0), 1);
+    EXPECT_NO_THROW(pcap.index_.seek_to_frame(pcap, 0, 0));
+    EXPECT_THROW(pcap.index_.seek_to_frame(pcap, 0, 1), std::out_of_range);
+    EXPECT_THROW(pcap.index_.seek_to_frame(pcap, 1, 1), std::out_of_range);
 }
 
 TEST(IndexedPcapReader, frame_id_rolled_over) {
     EXPECT_TRUE(IndexedPcapReader::frame_id_rolled_over(65535, 0));
     EXPECT_TRUE(IndexedPcapReader::frame_id_rolled_over(65290, 100));
     EXPECT_FALSE(IndexedPcapReader::frame_id_rolled_over(65000, 65535));
     EXPECT_FALSE(IndexedPcapReader::frame_id_rolled_over(1, 0));
```

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10.json` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10.pcap` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10.pcap`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10_digest.json` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-128-U1_v2.3.0_1024x10_digest.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10-single-packet.pcap` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10-single-packet.pcap`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10.json` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10.pcap` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10.pcap`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10_digest.json` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-0-32-U1_v2.2.0_1024x10_digest.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10.json` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10.pcap` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10.pcap`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10_digest.json` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-1-32-G_v2.1.1_1024x10_digest.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10.json` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10.pcap` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10.pcap`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10_digest.json` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-128-U1_v2.3.0_1024x10_digest.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10.json` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10.pcap` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10.pcap`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10_digest.json` & `ouster-sdk-0.9.0/sdk/tests/pcaps/OS-2-32-U0_v2.0.0_1024x10_digest.json`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/setup.cfg` & `ouster-sdk-0.9.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries
 	Topic :: System :: Hardware :: Hardware Drivers
 	Topic :: Scientific/Engineering
 	Topic :: Scientific/Engineering :: Image Processing
 
 [egg_info]
 tag_build =
```

### Comparing `ouster-sdk-0.8.1/setup.py` & `ouster-sdk-0.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -77,19 +77,34 @@
         env = os.environ.copy()
         extra_args = env.get('OUSTER_SDK_CMAKE_ARGS')
         if extra_args:
             cmake_args += shlex.split(extra_args)
 
         if not os.path.exists(self.build_temp):
             os.makedirs(self.build_temp)
-        subprocess.check_call(['cmake', ext.sourcedir] + cmake_args,
-                              cwd=self.build_temp,
-                              env=env)
-        subprocess.check_call(['cmake', '--build', '.'] + build_args,
-                              cwd=self.build_temp)
+        output1 = subprocess.run(['cmake', ext.sourcedir] + cmake_args,
+                                 cwd=self.build_temp,
+                                 stdout=subprocess.PIPE,
+                                 stderr=subprocess.STDOUT,
+                                 env=env, text=True)
+
+        print("CMAKE CONFIG OUTPUT")
+        print(output1.stdout)
+        if output1.returncode != 0:
+            raise "Error running cmake"
+
+        output2 = subprocess.run(['cmake', '--build', '.'] + build_args,
+                                 cwd=self.build_temp,
+                                 stdout=subprocess.PIPE,
+                                 stderr=subprocess.STDOUT,
+                                 env=env, text=True)
+        print("CMAKE BUILD OUTPUT")
+        print(output2.stdout)
+        if output2.returncode != 0:
+            raise "Error running cmake --build"
 
 
 class sdk_sdist(sdist):
     """Allow including files from parent directory via symlink."""
     def run(self):
         created = False
         try:
@@ -124,38 +139,53 @@
     # read from top-level sdk CMakeLists.txt
     version=parse_version(),
     package_dir={'': 'src'},
     packages=find_namespace_packages(where='src', include='ouster.*'),
     package_data={
         'ouster.client': ['py.typed', '_client.pyi'],
         'ouster.pcap': ['py.typed', '_pcap.pyi'],
+        'ouster.osf': ['py.typed', '_osf.pyi'],
         'ouster.sdk': ['py.typed', '_viz.pyi'],
+        'ouster.sdkx': ['py.typed'],
     },
     author='Ouster Sensor SDK Developers',
     author_email='oss@ouster.io',
-    description='Ouster sensor SDK',
+    description='Ouster Sensor SDK',
     license='BSD 3-Clause License',
     ext_modules=[
         CMakeExtension('ouster.*'),
     ],
     cmdclass={
         'build_ext': CMakeBuild,
         'sdist': sdk_sdist,
         'bdist_wheel': sdk_bdist_wheel,
     },
     zip_safe=False,
     python_requires='>=3.7, <4',
     install_requires=[
+        'psutil >=5.9.5, <6',
+        'zeroconf ==0.58.2',
+        'click >=8.1.3, <9',
+        'python-magic ==0.4.27',
+        'importlib_metadata ==6.6.0',
+        'prettytable >= 2.1.0',
+        'requests >=2.0, <3',
         'more-itertools >=8.6',
         'numpy >=1.19, <2, !=1.19.4',
+        # scipy is not supported on Mac M1 with Mac OS < 12.0
+        'scipy >=1.7, <2;platform_system != "Darwin" or platform_machine != "arm64" or platform_version >= "21.0.0"',
         'typing-extensions >=3.7.4.3',
-        'Pillow >=9.2'
+        'Pillow >=9.2',
+        'packaging',
     ],
     extras_require={
-        'test': ['pytest >=7.0, <8'],
+        'test': [
+            'pytest >=7.0, <8',
+            'flask==2.2.5'
+        ],
         'dev': ['flake8', 'mypy', 'pylsp-mypy', 'python-lsp-server', 'yapf'],
         'docs': [
             'Sphinx >=3.5',
             'sphinx-autodoc-typehints ==1.17.0',
             'sphinx-rtd-theme ==1.0.0',
             'sphinx-copybutton ==0.5.0',
             'docutils <0.18',
@@ -164,10 +194,21 @@
         ],
         'examples': [
             'matplotlib',
             'opencv-python',
             'laspy',
             'PyQt5; platform_system=="Windows"',
         ],
+        'mapping': [
+            'kiss-icp >=0.2.10, <1',
+            'open3d >=0, <1',
+            'laspy >=2.0, <3',
+        ],
     },
-    entry_points={'console_scripts': ['simple-viz=ouster.sdk.simple_viz:main',
-        'convert-meta-to-legacy=ouster.sdk.convert_to_legacy:main']})
+    entry_points={'console_scripts':
+        [
+            'simple-viz=ouster.sdk.simple_viz:main',
+            'convert-meta-to-legacy=ouster.sdk.convert_to_legacy:main',
+            'ouster-cli=ouster.cli.core:run'
+        ]
+    }
+)
```

### Comparing `ouster-sdk-0.8.1/src/cpp/_client.cpp` & `ouster-sdk-0.9.0/src/cpp/_client.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 #include <string>
 #include <utility>
 
 #include "ouster/buffered_udp_source.h"
 #include "ouster/client.h"
 #include "ouster/image_processing.h"
 #include "ouster/impl/build.h"
+#include "ouster/impl/profile_extension.h"
 #include "ouster/lidar_scan.h"
 #include "ouster/types.h"
 
 namespace py = pybind11;
 namespace chrono = std::chrono;
 using spdlog::sinks::base_sink;
 
@@ -80,15 +81,16 @@
 extern const Table<timestamp_mode, const char*, 4> timestamp_mode_strings;
 extern const Table<OperatingMode, const char*, 2> operating_mode_strings;
 extern const Table<MultipurposeIOMode, const char*, 6>
     multipurpose_io_mode_strings;
 extern const Table<Polarity, const char*, 2> polarity_strings;
 extern const Table<NMEABaudRate, const char*, 2> nmea_baud_rate_strings;
 extern Table<ChanField, const char*, 29> chanfield_strings;
-extern Table<UDPProfileLidar, const char*, 5> udp_profile_lidar_strings;
+extern Table<UDPProfileLidar, const char*, MAX_NUM_PROFILES>
+    udp_profile_lidar_strings;
 extern Table<UDPProfileIMU, const char*, 1> udp_profile_imu_strings;
 extern Table<ShotLimitingStatus, const char*, 10> shot_limiting_status_strings;
 extern Table<ThermalShutdownStatus, const char*, 2>
     thermal_shutdown_status_strings;
 
 }  // namespace impl
 }  // namespace sensor
@@ -110,43 +112,48 @@
 /*
  * Define an enum from a table of strings, along with some properties to make
  * the class behave more like a Python enum
  */
 template <typename C, typename E, size_t N>
 void def_enum(C& Enum, const Table<E, const char*, N>& strings_table,
               const std::string& enum_prefix = "") {
+    // weed out empty profiles
+    auto end = std::find_if(
+        strings_table.begin(), strings_table.end(),
+        [](const std::pair<E, const char*>& p) { return p.second == nullptr; });
+
     // in pybind11 2.0, calling enum.value(const char* name, val) doesn't make a
     // copy of the name argument. When value names aren't statically allocated,
     // we have to keep them alive. Use deque for stability of c_str() pointers
     static std::deque<std::string> enumerator_names;
 
     // module imports
     py::object MappingProxy =
         py::module::import("types").attr("MappingProxyType");
 
     // declare enumerators
-    for (const auto& p : strings_table) {
-        enumerator_names.push_back(enum_prefix + p.second);
-        Enum.value(enumerator_names.back().c_str(), p.first);
+    for (auto it = strings_table.begin(); it != end; ++it) {
+        enumerator_names.push_back(enum_prefix + it->second);
+        Enum.value(enumerator_names.back().c_str(), it->first);
     }
 
     // use immutable MappingProxy to return members dict
     std::map<std::string, E> members;
-    for (const auto& p : strings_table) members[p.second] = p.first;
+    for (auto it = strings_table.begin(); it != end; ++it)
+        members[it->second] = it->first;
     py::object py_members = MappingProxy(members);
     Enum.def_property_readonly_static(
         "__members__", [=](py::object) { return py_members; },
         "Returns a mapping of member name->value.");
 
     // can't make the class iterable itself easily
     Enum.def_property_readonly_static(
         "values",
-        [&](py::object) {
-            return py::make_key_iterator(strings_table.begin(),
-                                         strings_table.end());
+        [&, end](py::object) {
+            return py::make_key_iterator(strings_table.begin(), end);
         },
         "Returns an iterator of all enum members.");
 
     // support name / value properties like regular enums
     Enum.def_property_readonly(
         "value", [](const E& self) { return static_cast<int>(self); },
         "The value of the Enum member.");
@@ -194,14 +201,34 @@
         return sensor::ChanFieldType::UINT32;
     else if (dt == py::dtype::of<uint64_t>())
         return sensor::ChanFieldType::UINT64;
     else
         throw std::invalid_argument("Invalid dtype for a channel field");
 }
 
+/*
+ * Map a channel field type to a dtype
+ */
+static py::dtype dtype_of_field_type(const sensor::ChanFieldType& ftype) {
+    switch (ftype) {
+        case sensor::ChanFieldType::UINT8:
+            return py::dtype::of<uint8_t>();
+        case sensor::ChanFieldType::UINT16:
+            return py::dtype::of<uint16_t>();
+        case sensor::ChanFieldType::UINT32:
+            return py::dtype::of<uint32_t>();
+        case sensor::ChanFieldType::UINT64:
+            return py::dtype::of<uint64_t>();
+        default:
+            throw std::invalid_argument(
+                "Invalid field_type for convertion to dtype");
+    }
+    return py::dtype();  // unreachable ...
+}
+
 #if (SPDLOG_VER_MAJOR >= 1)  // don't include for spdlog < 1.x.x
 
 /*
  * Forward spdlog to python logging module
  */
 class PySink : public base_sink<std::mutex> {
    protected:
@@ -436,18 +463,18 @@
 
         See the sensor documentation for the meaning of each property.
         )")
         .def(py::init<>(), R"(
         Args:
             raw (str): json string to parse
         )")
-        .def("__init__", [](sensor_info& self, const std::string& s) {
+        .def("__init__", [](sensor_info& self, const std::string& s, bool skip_beam_validation) {
             new (&self) sensor_info{};
-            self = sensor::parse_metadata(s);
-        })
+            self = sensor::parse_metadata(s, skip_beam_validation);
+        }, py::arg("s"), py::arg("skip_beam_validation") = false)
         .def_readwrite("hostname", &sensor_info::name, "Sensor hostname.")
         .def_readwrite("sn", &sensor_info::sn, "Sensor serial number.")
         .def_readwrite("fw_rev", &sensor_info::fw_rev, "Sensor firmware revision.")
         .def_readwrite("mode", &sensor_info::mode, "Lidar mode, e.g., 1024x10.")
         .def_readwrite("prod_line", &sensor_info::prod_line, "Product line, e.g., 'OS-1-128'.")
         .def_readwrite("format", &sensor_info::format,  "Describes the structure of a lidar packet.")
         .def_readwrite("beam_azimuth_angles", &sensor_info::beam_azimuth_angles, "Beam azimuth angles, useful for XYZ projection.")
@@ -525,14 +552,30 @@
     auto ChanField = py::enum_<sensor::ChanField>(m, "ChanField", R"(
     Channel data block fields
     )", py::metaclass());
     def_enum(ChanField, sensor::impl::chanfield_strings);
 
     auto UDPProfileLidar = py::enum_<sensor::UDPProfileLidar>(m, "UDPProfileLidar", "UDP lidar profile.", py::metaclass());
     def_enum(UDPProfileLidar, sensor::impl::udp_profile_lidar_strings, "PROFILE_LIDAR_");
+    UDPProfileLidar.attr("from_string") = py::cpp_function(
+        [](const std::string& s) {
+            return sensor::udp_profile_lidar_of_string(s);
+        },
+        py::name("from_string"), "Create UDPProfileLidar from string.");
+    UDPProfileLidar.def_property_readonly_static(
+        "values",
+        [](py::object) {
+            return py::make_key_iterator(
+                sensor::impl::udp_profile_lidar_strings.begin(),
+                std::find_if(
+                    sensor::impl::udp_profile_lidar_strings.begin(),
+                    sensor::impl::udp_profile_lidar_strings.end(),
+                    [](const auto& p) { return p.second == nullptr; }));
+        },
+        "Returns an iterator of all UDPProfileLidar enum members.");
 
     auto UDPProfileIMU = py::enum_<sensor::UDPProfileIMU>(m, "UDPProfileIMU", "UDP imu profile.", py::metaclass());
     def_enum(UDPProfileIMU, sensor::impl::udp_profile_imu_strings, "PROFILE_IMU_");
 
     auto ShotLimitingStatus = py::enum_<sensor::ShotLimitingStatus>(m, "ShotLimitingStatus", "Shot Limiting Status.", py::metaclass());
     def_enum(ShotLimitingStatus, sensor::impl::shot_limiting_status_strings);
 
@@ -696,17 +739,17 @@
         .def(py::init<std::string, std::string, sensor::lidar_mode,
                       sensor::timestamp_mode, int, int, int, size_t>(),
              py::arg("hostname"), py::arg("udp_dest_host"),
              py::arg("mode") = sensor::lidar_mode::MODE_1024x10,
              py::arg("timestamp_mode") =
                  sensor::timestamp_mode::TIME_FROM_INTERNAL_OSC,
              py::arg("lidar_port") = 0, py::arg("imu_port") = 0,
-             py::arg("timeout_sec") = 30, py::arg("capacity") = 128)
+             py::arg("timeout_sec") = 10, py::arg("capacity") = 128)
         .def("get_metadata", &BufferedUDPSource::get_metadata,
-             py::arg("timeout_sec") = 60, py::arg("legacy") = true)
+             py::arg("timeout_sec") = 10, py::arg("legacy") = true)
         .def("shutdown", &BufferedUDPSource::shutdown)
         .def("consume",
              [](BufferedUDPSource& self, py::buffer buf, float timeout_sec) {
                  using fsec = chrono::duration<float>;
 
                  auto info = buf.request();
 
@@ -882,14 +925,24 @@
             "status",
             [](LidarScan& self) {
                 return py::array(py::dtype::of<uint32_t>(), self.w,
                                  self.status().data(), py::cast(self));
             },
             "The measurement status header as a W-element numpy array.")
         .def_property_readonly(
+            "pose",
+            [](LidarScan& self) {
+                return py::array(
+                    py::dtype::of<double>(),
+                    std::vector<size_t>{
+                        static_cast<size_t>(self.timestamp().size()), 4, 4},
+                    self.pose().data()->data(), py::cast(self));
+            },
+            "The pose vector of 4x4 homogeneous matrices (per each timestamp).")
+        .def_property_readonly(
             "fields",
             // NOTE: keep_alive seems to be ignored without cpp_function wrapper
             py::cpp_function(
                 [](LidarScan& self) {
                     return py::make_key_iterator(self.begin(), self.end());
                 },
                 py::keep_alive<0, 1>()),
@@ -981,83 +1034,74 @@
     py::class_<viz::BeamUniformityCorrector>(m, "BeamUniformityCorrector")
         .def(py::init<>())
         .def("__call__", &image_proc_call<viz::BeamUniformityCorrector, float>,
              py::arg("image"), py::arg("update_state") = true)
         .def("__call__", &image_proc_call<viz::BeamUniformityCorrector, double>,
              py::arg("image"), py::arg("update_state") = true);
 
-    // Imu
-    py::class_<ouster::Imu>(m, "Imu")
-        .def(
-            "__init__",
-            [](ouster::Imu& self, py::buffer& buf,
-               const sensor::packet_format& pf) {
-                new (&self) ouster::Imu{};
-                ouster::packet_to_imu(getptr(pf.imu_packet_size, buf), pf,
-                                      self);
-            },
-            py::arg("buf"), py::arg("pf"),
-            "Creates imu object from ``buf`` and ``pf``")
-        .def(
-            "__init__",
-            [](ouster::Imu& self, py::array_t<double>& accel,
-               py::array_t<double>& angular_vel, uint64_t sys_ts,
-               uint64_t accel_ts, uint64_t gyro_ts) {
-                py::buffer_info accel_buf = accel.request();
-                py::buffer_info angular_buf = angular_vel.request();
-
-                if (accel_buf.ndim != 1 || angular_buf.ndim != 1) {
-                    throw std::invalid_argument(
-                        "Expect number of dimensions 1");
-                }
-                new (&self) ouster::Imu{};
-                if (accel_buf.size == 3) {
-                    double* ptr = static_cast<double*>(accel_buf.ptr);
-                    self.linear_accel[0] = *ptr;
-                    self.linear_accel[1] = *(ptr + 1);
-                    self.linear_accel[2] = *(ptr + 2);
-                }
-                if (angular_buf.size == 3) {
-                    double* ptr = static_cast<double*>(angular_buf.ptr);
-                    self.angular_vel[0] = *ptr;
-                    self.angular_vel[1] = *(ptr + 1);
-                    self.angular_vel[2] = *(ptr + 2);
-                }
-                self.sys_ts = sys_ts;
-                self.accel_ts = accel_ts;
-                self.gyro_ts = gyro_ts;
-            },
-            py::arg("accel"), py::arg("angular_vel"), py::arg("sys_ts") = 0,
-            py::arg("accel_ts") = 0, py::arg("gyro_ts") = 0,
-            "Creates ``client.Imu`` object from imu data.")
-        .def_property_readonly(
-            "sys_ts", [](const ouster::Imu& imu) { return imu.sys_ts; },
-            "System timestamp (ns)")
-        .def_property_readonly(
-            "accel_ts", [](const ouster::Imu& imu) { return imu.accel_ts; },
-            "Accelerometer timestamp (ns)")
-        .def_property_readonly(
-            "gyro_ts", [](const ouster::Imu& imu) { return imu.gyro_ts; },
-            "Gyroscope timestamp (ns)")
-        .def_property_readonly(
-            "accel",
-            [](const ouster::Imu& imu) {
-                return py::array(py::dtype::of<double>(),
-                                 imu.linear_accel.size(),
-                                 imu.linear_accel.data());
-            },
-            "Accelerometer data")
-        .def_property_readonly(
-            "angular_vel",
-            [](const ouster::Imu& imu) {
-                return py::array(py::dtype::of<double>(),
-                                 imu.angular_vel.size(),
-                                 imu.angular_vel.data());
-            },
-            "Angular velocity data")
-        .def("__repr__", [](ouster::Imu& p) { return ouster::to_string(p); })
-        .def("__str__", [](ouster::Imu& p) { return ouster::to_string(p); });
+    m.def(
+        "get_field_types",
+        [](const sensor::sensor_info& info) {
+            auto field_types = ouster::get_field_types(info);
+            std::map<sensor::ChanField, py::dtype> field_types_res{};
+            for (const auto& f : field_types) {
+                auto dtype = dtype_of_field_type(f.second);
+                field_types_res.emplace(f.first, dtype);
+            }
+            return field_types_res;
+        },
+        R"(
+        Extracts LidarScan fields with types for a given SensorInfo
+
+        Args:
+            info: sensor metadata for which to find fields types
+
+        Returns:
+            returns field types
+            )",
+        py::arg("info"));
+
+    m.def(
+        "get_field_types",
+        [](const LidarScan& ls) {
+            auto field_types = ouster::get_field_types(ls);
+            std::map<sensor::ChanField, py::dtype> field_types_res{};
+            for (const auto& f : field_types) {
+                auto dtype = dtype_of_field_type(f.second);
+                field_types_res.emplace(f.first, dtype);
+            }
+            return field_types_res;
+        },
+        R"(
+        Extracts LidarScan fields with types for a given lidar scan ``ls``
+
+        Args:
+            ls: lidar scan from which to get field types
+
+        Returns:
+            returns field types
+            )",
+        py::arg("lidar_scan"));
+
+    using ouster::sensor::impl::FieldInfo;
+    py::class_<FieldInfo>(m, "FieldInfo")
+        .def("__init__",
+             [](FieldInfo& self, py::object dt, size_t offset, uint64_t mask,
+                int shift) {
+                 new (&self)
+                     FieldInfo{field_type_of_dtype(py::dtype::from_args(dt)),
+                               offset, mask, shift};
+             })
+        .def_property_readonly("ty_tag",
+                               [](const FieldInfo& self) {
+                                   return dtype_of_field_type(self.ty_tag);
+                               })
+        .def_readwrite("offset", &FieldInfo::offset)
+        .def_readwrite("mask", &FieldInfo::mask)
+        .def_readwrite("shift", &FieldInfo::shift);
+
+    m.def("add_custom_profile", &ouster::sensor::add_custom_profile);
 
     m.attr("__version__") = ouster::SDK_VERSION;
 
     return m.ptr();
 }
```

### Comparing `ouster-sdk-0.8.1/src/cpp/_pcap.cpp` & `ouster-sdk-0.9.0/src/cpp/_pcap.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 PYBIND11_MAKE_OPAQUE(std::shared_ptr<playback_handle>);
 PYBIND11_MAKE_OPAQUE(std::shared_ptr<record_handle>);
 PYBIND11_MAKE_OPAQUE(std::vector<stream_key>);
 PYBIND11_MAKE_OPAQUE(std::vector<int>);
 PYBIND11_MAKE_OPAQUE(std::vector<guessed_ports>);
 PYBIND11_MAKE_OPAQUE(std::vector<uint64_t>);
 PYBIND11_MAKE_OPAQUE(std::vector<uint8_t>);
-using stream_map = std::map<stream_key, stream_data>;
+using stream_map = std::unordered_map<stream_key, stream_data>;
 PYBIND11_MAKE_OPAQUE(stream_map);
 using count_map = std::map<uint64_t, uint64_t>;
 PYBIND11_MAKE_OPAQUE(count_map);
 PYBIND11_PLUGIN(_pcap) {
     py::module m("_pcap", R"(Pcap bindings generated by pybind11.
 
 This module is generated from the C++ code and not meant to be used directly.
@@ -45,15 +45,15 @@
     py::options options;
     options.disable_function_signatures();
     py::bind_vector<std::vector<stream_key>>(m, "VectorStreamKey");
     py::bind_vector<std::vector<int>>(m, "VectorInt");
     py::bind_vector<std::vector<guessed_ports>>(m, "VectorGuessedPorts");
     py::bind_vector<std::vector<uint64_t>>(m, "VectorUint64");
     py::bind_vector<std::vector<uint8_t>>(m, "VectorUint8");
-    py::bind_map<std::map<stream_key, stream_data>>(m, "MapUdpStreams");
+    py::bind_map<std::unordered_map<stream_key, stream_data>>(m, "MapUdpStreams");
     py::bind_map<std::map<uint64_t, uint64_t>>(m, "CountMap");
     py::class_<packet_info, std::shared_ptr<packet_info>>(m, "packet_info")
         .def(py::init<>())
         .def("__repr__",
              [](const packet_info& data) {
                  std::stringstream result;
                  result << data;
@@ -220,29 +220,34 @@
         }
         record_packet(*handle, info, static_cast<uint8_t*>(buf_info.ptr),
                       buf_info.size);
     });
 
     py::class_<PcapReader>(m, "PcapReader"); // TODO add more complete bindings
 
+    py::class_<PcapIndex>(m, "PcapIndex")
+        .def(py::init<int>())
+        .def("frame_count", &PcapIndex::frame_count)
+        .def("seek_to_frame", &PcapIndex::seek_to_frame)
+        .def_readonly("frame_indices", &PcapIndex::frame_indices_);
+
     py::class_<IndexedPcapReader, PcapReader>(m, "IndexedPcapReader")
-        .def(py::init<const std::string&, const std::vector<std::string>&, std::function<void(uint64_t, uint64_t, uint64_t)>>())
-        .def("frame_count", &IndexedPcapReader::frame_count)
-        .def("seek_to_frame", &IndexedPcapReader::seek_to_frame)
-        .def("get_stream_info", &IndexedPcapReader::get_stream_info)
+        .def(py::init<const std::string&, const std::vector<std::string>&>())
         .def("current_info", &IndexedPcapReader::current_info)
         .def("next_packet", &IndexedPcapReader::next_packet)
+        .def("update_index_for_current_packet", &IndexedPcapReader::update_index_for_current_packet)
         .def("current_frame_id",[](IndexedPcapReader& reader) -> py::object {
             if(auto frame_id = reader.current_frame_id()) {
                 return py::int_(*frame_id);
             }
             return py::none();
         })
+        .def("reset", &IndexedPcapReader::reset) // TODO move to PcapReader binding?
+        .def("get_index", &IndexedPcapReader::get_index)
         .def("current_data", [](IndexedPcapReader& reader) -> py::array {
             uint8_t* data = const_cast<uint8_t*>(reader.current_data());
             size_t data_size = reader.current_length();
             return py::array(py::dtype::of<uint8_t>(), data_size, data, py::cast(reader));
-        })
-        .def_readonly("frame_indices", &IndexedPcapReader::frame_indices_);
+        });
 
     return m.ptr();
 }
```

### Comparing `ouster-sdk-0.8.1/src/cpp/_viz.cpp` & `ouster-sdk-0.9.0/src/cpp/_viz.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -495,34 +495,24 @@
                          that the xyz position of the ith point is ``i``,
                          ``i + n``, ``i + 2n``
              )")
         .def(
             "set_column_poses",
             [](viz::Cloud& self,
                py::array_t<float, py::array::f_style | py::array::forcecast>
-                   rotation,
-               py::array_t<float, py::array::f_style | py::array::forcecast>
-                   translation) {
-                check_array(rotation, self.get_cols() * 9, 0, 'F');
-                check_array(translation, self.get_cols() * 3, 0, 'F');
-                self.set_column_poses(rotation.data(), translation.data());
+                   column_poses) {
+                check_array(column_poses, self.get_cols() * 16, 0, 'F');
+                self.set_column_poses(column_poses.data());
             },
-            py::arg("rotation"), py::arg("translation"),
+            py::arg("column_poses"),
             R"(
-                 Set the rotation and translation values per column.
+                 Set scan poses (per every column).
 
                  Args:
-                    rotation: array of exactly 9n where n is number of columns,
-                         so that the rotation of the ith column is ``i``,
-                         ``i + 3n``, ``i + 6n``, ``i + n``, ``i + n + 3n``,
-                         ``i + n + 6n``, ``i + 2n``, ``i + 2n + 3n``,
-                         ``i + 2n + 6n``
-                    translation: array of exactly 3n where n is number of
-                         columns, so that the translation of the ith column is
-                         ``i``, ``i + n``, ``i + 2n``
+                    column_poses: array of poses (Wx4x4) per every column.
              )")
         .def(
             "set_pose",
             [](viz::Cloud& self, pymatrixd pose) {
                 check_array(pose, 16, 2, 'F');
                 viz::mat4d posea;
                 std::copy(pose.data(), pose.data() + 16, posea.data());
```

### Comparing `ouster-sdk-0.8.1/src/ouster/client/_client.pyi` & `ouster-sdk-0.9.0/src/ouster/client/_client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 Note:
     This file should be updated whenever the bindings are modified.
 
 """
 # flake8: noqa (linter complains about scoping, but afaict mypy doesn't care)
 
 from numpy import ndarray
-from typing import (Callable, ClassVar, Dict, Iterator, List, Optional,
-                    overload, Tuple, Union)
+from typing import (ClassVar, Dict, Iterator, List, Optional, overload, Tuple)
 
-from .data import (BufferT, ColHeader, FieldDType)
+from .data import (BufferT, ColHeader, FieldDType, FieldTypes)
 
 
 class Client:
     @overload
     def __init__(self,
                  hostname: str = ...,
                  lidar_port: int = ...,
@@ -129,14 +128,18 @@
     def __init__(self) -> None:
         ...
 
     @overload
     def __init__(self, metadata: str) -> None:
         ...
 
+    @overload
+    def __init__(self, metadata: str, skip_beam_validation: bool) -> None:
+        ...
+
 
 class DataFormat:
     columns_per_frame: int
     columns_per_packet: int
     pixel_shift_by_row: List[int]
     pixels_per_column: int
     column_window: Tuple[int, int]
@@ -158,14 +161,34 @@
     def columns_per_packet(self) -> int:
         ...
 
     @property
     def pixels_per_column(self) -> int:
         ...
 
+    @property
+    def packet_header_size(self) -> int:
+        ...
+
+    @property
+    def col_header_size(self) -> int:
+        ...
+
+    @property
+    def col_footer_size(self) -> int:
+        ...
+
+    @property
+    def col_size(self) -> int:
+        ...
+
+    @property
+    def packet_footer_size(self) -> int:
+        ...
+
     def packet_type(self, buf: BufferT) -> int:
         ...
 
     def frame_id(self, buf: BufferT) -> int:
         ...
 
     def prod_sn(self, buf: BufferT) -> int:
@@ -628,14 +651,18 @@
     def measurement_id(self) -> ndarray:
         ...
 
     @property
     def status(self) -> ndarray:
         ...
 
+    @property
+    def pose(self) -> ndarray:
+        ...
+
     def complete(self, window: Optional[Tuple[int, int]] = ...) -> bool:
         ...
 
     @property
     def fields(self) -> Iterator[ChanField]:
         ...
 
@@ -729,36 +756,43 @@
         ...
 
     @overload
     def __init__(self, lo_percentile: float, hi_percentile: float,
                  update_every: int) -> None:
         ...
 
-    def __call__(self, image: ndarray, update_state: Optional[bool] = True) -> None:
+    def __call__(self,
+                 image: ndarray,
+                 update_state: Optional[bool] = True) -> None:
         ...
 
 
 class BeamUniformityCorrector:
     def __init__(self) -> None:
         ...
 
     def __call__(self, image: ndarray) -> None:
         ...
 
-class Imu:
-    @overload
-    def __init__(self, buf: BufferT, pf) -> None: ...
+class FieldInfo:
+    @property
+    def ty_tag(self) -> FieldDType:
+        ...
 
-    @overload
-    def __init__(self, accel: ndarray, angular_vel: ndarray,
-                 sys_ts: int = ..., accel_ts: int = ..., gyro_ts: int = ...) -> None: ...
+    def __init__(self, ty_tag: FieldDType, offset: int, mask: int, shift: int) -> None:
+        ...
 
-    @property
-    def accel(self) -> ndarray: ...
-    @property
-    def accel_ts(self) -> int: ...
-    @property
-    def angular_vel(self) -> ndarray: ...
-    @property
-    def gyro_ts(self) -> int: ...
-    @property
-    def sys_ts(self) -> int: ...
+    offset: int
+    mask:   int
+    shift:  int
+
+def add_custom_profile(profile_nr: int,
+                       name: str,
+                       fields: List[Tuple[int, FieldInfo]],
+                       chan_data_size: int) -> None:
+    ...
+
+@overload
+def get_field_types(scan: LidarScan) -> FieldTypes: ...
+
+@overload
+def get_field_types(info: SensorInfo) -> FieldTypes: ...
```

### Comparing `ouster-sdk-0.8.1/src/ouster/client/_digest.py` & `ouster-sdk-0.9.0/src/ouster/client/_digest.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/src/ouster/client/core.py` & `ouster-sdk-0.9.0/src/ouster/client/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 This module contains more idiomatic wrappers around the lower-level module
 generated using pybind11.
 """
 from contextlib import closing
 from typing import cast, Dict, Iterable, Iterator, List, Optional, Tuple, Union
 from threading import Thread
 import time
+from math import ceil
 
 from more_itertools import take
 from typing_extensions import Protocol
 
 from . import _client
 from ._client import (SensorInfo, LidarScan, UDPProfileLidar)
 from .data import (ChanField, FieldDType, ImuPacket, LidarPacket, Packet,
                    PacketIdError)
+import numpy as np
 
 
 class ClientError(Exception):
     """Base class for client errors."""
     pass
 
 
@@ -130,15 +132,16 @@
                  metadata: Optional[SensorInfo] = None,
                  buf_size: int = 128,
                  timeout: Optional[float] = 2.0,
                  _overflow_err: bool = False,
                  _flush_before_read: bool = True,
                  _flush_frames: int = 5,
                  _legacy_format: bool = False,
-                 _soft_id_check: bool = False) -> None:
+                 _soft_id_check: bool = False,
+                 _skip_metadata_beam_validation: bool = False) -> None:
         """
         Neither the ports nor udp destination configuration on the sensor will
         be updated. The metadata will be fetched over the network from the
         sensor unless explicitly provided using the ``metadata`` parameter.
 
         Args:
             hostname: hostname or IP address of the sensor
@@ -146,16 +149,17 @@
             imu_port: UDP port to listen on for imu data
             metadata: explicitly provide metadata for the stream
             buf_size: number of packets to buffer before dropping data
             timeout: seconds to wait for packets before signaling error or None
             _overflow_err: if True, raise ClientOverflow
             _flush_before_read: if True, try to clear buffers before reading
             _legacy_format: if True, use legacy metadata format
-            _soft_id_check: if True, don't skip lidar packets buffers on
-            id mismatch (init_id/sn pair)
+            _soft_id_check: if True, don't skip lidar packets buffers on,
+            id mismatch (init_id/sn pair),
+            _skip_metadata_beam_validation: if True, skip metadata beam angle check
 
         Raises:
             ClientError: If initializing the client fails.
         """
         self._cli = _client.Client(hostname, lidar_port, imu_port, buf_size)
         self._timeout = timeout
         self._overflow_err = _overflow_err
@@ -163,32 +167,36 @@
         self._cache = None
         self._fetched_meta = ""
         self._flush_frames = _flush_frames
         self._legacy_format = _legacy_format
 
         self._soft_id_check = _soft_id_check
         self._id_error_count = 0
+        self._skip_metadata_beam_validation = _skip_metadata_beam_validation
 
         # Fetch from sensor if not explicitly provided
         if metadata:
             self._metadata = metadata
         else:
             self._fetch_metadata()
-            self._metadata = SensorInfo(self._fetched_meta)
+            self._metadata = SensorInfo(self._fetched_meta, self._skip_metadata_beam_validation)
         self._pf = _client.PacketFormat.from_info(self._metadata)
 
         # Use args to avoid capturing self causing circular reference
         self._producer = Thread(target=lambda cli, pf: cli.produce(pf),
                                 args=(self._cli, self._pf))
         self._producer.start()
 
-    def _fetch_metadata(self) -> None:
+    def _fetch_metadata(self, timeout: Optional[float] = None) -> None:
+        timeout_sec = 45
+        if timeout:
+            timeout_sec = ceil(timeout)
         if not self._fetched_meta:
             self._fetched_meta = self._cli.get_metadata(
-                legacy=self._legacy_format)
+                legacy=self._legacy_format, timeout_sec = timeout_sec)
             if not self._fetched_meta:
                 raise ClientError("Failed to collect metadata")
 
     def write_metadata(self, path: str) -> None:
         """Save metadata to disk.
 
         Args:
@@ -372,14 +380,15 @@
             timeout: seconds to wait for a scan before error or None
             fields: specify which channel fields to populate on LidarScans
             _max_latency: (experimental) approximate max number of frames to buffer
         """
         self._source = source
         self._complete = complete
         self._timeout = timeout
+        self._timed_out = False
         self._max_latency = _max_latency
         # used to initialize LidarScan
         self._fields: Union[Dict[ChanField, FieldDType], UDPProfileLidar] = (
             fields if fields is not None else
             self._source.metadata.format.udp_profile_lidar)
 
     def __iter__(self) -> Iterator[LidarScan]:
@@ -398,34 +407,42 @@
         pf = _client.PacketFormat.from_info(self._source.metadata)
         batch = _client.ScanBatcher(w, pf)
 
         # Time from which to measure timeout
         start_ts = time.monotonic()
 
         it = iter(self._source)
+        self._packets_consumed = 0
+        self._scans_produced = 0
         while True:
             try:
                 packet = next(it)
+                self._packets_consumed += 1
             except StopIteration:
                 if ls_write is not None:
                     if not self._complete or ls_write.complete(column_window):
                         yield ls_write
                 return
+            except ClientTimeout:
+                self._timed_out = True
+                return
 
             if self._timeout is not None and (time.monotonic() >=
                                               start_ts + self._timeout):
-                raise ClientTimeout(f"No lidar scans within {self._timeout}s")
+                self._timed_out = True
+                return
 
             if isinstance(packet, LidarPacket):
                 ls_write = ls_write or LidarScan(h, w, self._fields)
 
                 if batch(packet._data, ls_write):
                     # Got a new frame, return it and start another
                     if not self._complete or ls_write.complete(column_window):
                         yield ls_write
+                        self._scans_produced += 1
                         start_ts = time.monotonic()
                     ls_write = None
 
                     # Drop data along frame boundaries to maintain _max_latency and
                     # clear out already-batched first packet of next frame
                     if self._max_latency and sensor is not None:
                         buf_frames = sensor.buf_use() // packets_per_frame
@@ -518,7 +535,37 @@
                         _flush_before_read=True)
 
         return cls(source,
                    timeout=timeout,
                    complete=complete,
                    fields=fields,
                    _max_latency=2)
+
+
+def first_valid_column(scan: LidarScan) -> int:
+    """Return first valid column of a LidarScan"""
+    return int(np.bitwise_and(scan.status, 1).argmax())
+
+
+def last_valid_column(scan: LidarScan) -> int:
+    """Return last valid column of a LidarScan"""
+    return int(scan.w - 1 - np.bitwise_and(scan.status, 1)[::-1].argmax())
+
+
+def first_valid_column_ts(scan: LidarScan) -> int:
+    """Return first valid column timestamp of a LidarScan"""
+    return scan.timestamp[first_valid_column(scan)]
+
+
+def last_valid_column_ts(scan: LidarScan) -> int:
+    """Return last valid column timestamp of a LidarScan"""
+    return scan.timestamp[last_valid_column(scan)]
+
+
+def first_valid_column_pose(scan: LidarScan) -> np.ndarray:
+    """Return first valid column pose of a LidarScan"""
+    return scan.pose[first_valid_column(scan)]
+
+
+def last_valid_column_pose(scan: LidarScan) -> np.ndarray:
+    """Return last valid column pose of a LidarScan"""
+    return scan.pose[last_valid_column(scan)]
```

### Comparing `ouster-sdk-0.8.1/src/ouster/client/data.py` & `ouster-sdk-0.9.0/src/ouster/client/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """
 Copyright (c) 2021, Ouster, Inc.
 All rights reserved.
 """
 
 from copy import deepcopy
 from enum import Enum
-from typing import Callable, Iterator, Type, List, Optional, Union
+from typing import Callable, Iterator, Type, List, Optional, Union, Dict
 import logging
 import warnings
 
 import numpy as np
 
 from . import _client
-from ._client import (ChanField, LidarScan, SensorInfo, Imu)
+from ._client import (ChanField, LidarScan, SensorInfo)
 
 BufferT = Union[bytes, bytearray, memoryview, np.ndarray]
 """Types that support the buffer protocol."""
 
 FieldDType = Type[np.unsignedinteger]
 """Numpy dtype of fields."""
 
 Packet = Union['ImuPacket', 'LidarPacket']
 """Packets emitted by a sensor."""
 
+FieldTypes = Dict[ChanField, FieldDType]
+"""LidarScan chan fields with types"""
+
 logger = logging.getLogger("ouster.client.data")
 
 
 class ImuPacket:
     """Read IMU Packet data from a bufer."""
     _pf: _client.PacketFormat
     _data: np.ndarray
@@ -111,19 +114,67 @@
     STATUS = 3
     FRAME_ID = 4
 
     def __int__(self) -> int:
         return self.value
 
 
-class PacketIdError(Exception):
+class PacketValidationFailure(Exception):
+    def __eq__(self, other):
+        return type(self) == type(other) and self.args == other.args
+
+    def __hash__(self):
+        return hash((type(self), self.args))
+
+
+class PacketIdError(PacketValidationFailure):
     """Exception raised when init_id/sn from metadata and packet doesn't match."""
     pass
 
 
+class PacketSizeError(PacketValidationFailure):
+    """Exception raised when the packet size wrong for the given metadata."""
+    pass
+
+
+class LidarPacketValidator:
+    """A utility class for validating lidar packets for a given sensor info."""
+    def __init__(self, metadata: SensorInfo, checks=['id_and_sn_valid', 'packet_size_valid']):
+        self._metadata = metadata
+        self._metadata_init_id = metadata.init_id
+        self._metadata_sn = int(metadata.sn)
+        self._pf = _client.PacketFormat.from_info(metadata)
+        self._checks = [getattr(self, check) for check in checks]
+
+    def check_packet(self, data: BufferT, n_bytes: int) -> List[PacketValidationFailure]:
+        errors = []
+        for check in self._checks:
+            error = check(data, n_bytes)
+            if error:
+                errors.append(error)
+        return errors
+
+    def id_and_sn_valid(self, data: BufferT, n_bytes: int) -> Optional[PacketValidationFailure]:
+        """Check the metadata init_id/sn and packet init_id/sn mismatch."""
+        init_id = self._pf.init_id(data)
+        sn = self._pf.prod_sn(data)
+        if bool(init_id and (init_id != self._metadata_init_id or sn != self._metadata_sn)):
+            error_msg = f"Metadata init_id/sn does not match: " \
+                    f"expected by metadata - {self._metadata_init_id}/{self._metadata_sn}, " \
+                    f"but got from packet buffer - {init_id}/{sn}"
+            return PacketIdError(error_msg)
+        return None
+
+    def packet_size_valid(self, data: BufferT, n_bytes: int) -> Optional[PacketValidationFailure]:
+        if self._pf.lidar_packet_size != n_bytes:
+            return PacketSizeError(
+                f"Expected a packet of size {self._pf.lidar_packet_size} but got a buffer of size {n_bytes}")
+        return None
+
+
 class LidarPacket:
     """Read lidar packet data as numpy arrays.
 
     The dimensions of returned arrays depend on the sensor product line and
     configuration. Measurement headers will be arrays of size matching the
     configured ``columns_per_packet``, while measurement fields will be 2d
     arrays of size ``pixels_per_column`` by ``columns_per_packet``.
@@ -395,11 +446,11 @@
 
         return xyz.reshape(info.format.pixels_per_column,
                            info.format.columns_per_frame, 3)
 
     return res
 
 
-def imu_from_packet(packet: ImuPacket) -> Imu:
-    """Transform ImuPacket to client.Imu data type"""
-    return Imu(packet.accel, packet.angular_vel, packet.sys_ts, packet.accel_ts,
-               packet.gyro_ts)
+def packet_ts(packet: Packet) -> int:
+    """Return the packet timestamp in nanoseconds"""
+    return int(packet.capture_timestamp *
+               10**9) if packet.capture_timestamp else 0
```

### Comparing `ouster-sdk-0.8.1/src/ouster/pcap/_pcap.pyi` & `ouster-sdk-0.9.0/src/ouster/pcap/_pcap.pyi`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/src/ouster/pcap/pcap.py` & `ouster-sdk-0.9.0/src/ouster/pcap/pcap.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 All rights reserved.
 """
 from copy import copy
 import os
 import socket
 import time
 from threading import Lock
-from typing import (Iterable, Iterator, Optional, Tuple)
+from collections import defaultdict
+from typing import (Iterable, Iterator, Optional, Tuple, Dict)  # noqa: F401
 
-from ouster.client import (LidarPacket, ImuPacket, Packet, PacketSource,
-                           SensorInfo, _client, PacketIdError)
+from ouster.client import (LidarPacketValidator, LidarPacket, ImuPacket, Packet, PacketSource,  # noqa: F401
+                           SensorInfo, _client, PacketValidationFailure, PacketIdError)         # noqa: F401
 from . import _pcap
 
 MTU_SIZE = 1500
 
 
 def _guess_ports(stream_info, sensor_info):
     pf = _client.PacketFormat.from_info(sensor_info)
@@ -45,14 +46,15 @@
     def __init__(self,
                  pcap_path: str,
                  info: SensorInfo,
                  *,
                  rate: float = 0.0,
                  lidar_port: Optional[int] = None,
                  imu_port: Optional[int] = None,
+                 loop: bool = False,
                  _soft_id_check: bool = False):
         """Read a single sensor data stream from a packet capture.
 
         Packet captures can contain arbitrary network traffic or even multiple
         valid sensor data streans. To avoid passing invalid data to the user,
         this class assumes that lidar and/or imu packets are associated with
         distinct destination ports, which may be recorded in the sensor metadata
@@ -71,29 +73,31 @@
 
         Args:
             info: Sensor metadata
             pcap_path: File path of recorded pcap
             rate: Output packets in real time, if non-zero
             lidar_port: Specify the destination port of lidar packets
             imu_port: Specify the destination port of imu packets
-            _soft_id_check: if True, don't skip lidar packets buffers on
-            init_id/sn mismatch
+            loop: Specify whether to reload the PCAP file when the end is reached
+            _soft_id_check: if True, don't skip lidar packets buffers on init_id/sn mismatch
         """
 
         # prefer explicitly specified ports (can probably remove the args?)
         lidar_port = info.udp_port_lidar if lidar_port is None else lidar_port
         imu_port = info.udp_port_imu if imu_port is None else imu_port
 
         # override ports in metadata, if explicitly specified
         self._metadata = copy(info)
         self._metadata.udp_port_lidar = lidar_port
         self._metadata.udp_port_imu = imu_port
 
+        self.loop = loop
         self._soft_id_check = _soft_id_check
-        self._id_error_count = 0
+        self._id_error_count = 0    # TWS 20230615 TODO generialize error counting and reporting
+        self._errors = defaultdict(int)  # type: Dict[PacketValidationFailure,int]
 
         # sample pcap and attempt to find UDP ports consistent with metadata
         n_packets = 1000
         stats = _packet_info_stream(pcap_path, n_packets)
         self._guesses = _guess_ports(stats, self._metadata)
 
         # fill in unspecified (0) ports with inferred values
@@ -113,19 +117,25 @@
                 raise ValueError("I/O operation on closed packet source")
 
         buf = bytearray(2**16)
         packet_info = _pcap.packet_info()
 
         real_start_ts = time.monotonic()
         pcap_start_ts = None
+        validator = LidarPacketValidator(self.metadata)
         while True:
             with self._lock:
-                if not (self._handle
-                        and _pcap.next_packet_info(self._handle, packet_info)):
+                if not self._handle:
                     break
+                if not _pcap.next_packet_info(self._handle, packet_info):
+                    if self.loop:
+                        _pcap.replay_reset(self._handle)
+                        _pcap.next_packet_info(self._handle, packet_info)
+                    else:
+                        break
                 n = _pcap.read_packet(self._handle, buf)
 
             # if rate is set, read in 'real time' simulating UDP stream
             # TODO: factor out into separate packet iterator utility
             timestamp = packet_info.timestamp
             if self._rate:
                 if not pcap_start_ts:
@@ -133,14 +143,16 @@
                 real_delta = time.monotonic() - real_start_ts
                 pcap_delta = (timestamp - pcap_start_ts) / self._rate
                 delta = max(0, pcap_delta - real_delta)
                 time.sleep(delta)
 
             try:
                 if (packet_info.dst_port == self._metadata.udp_port_lidar):
+                    for error in validator.check_packet(buf, n):
+                        self._errors[error] += 1  # accumulate counts of errors
                     lp = LidarPacket(
                         buf[0:n],
                         self._metadata,
                         timestamp,
                         _raise_on_id_check=not self._soft_id_check)
                     if lp.id_error:
                         self._id_error_count += 1
```

### Comparing `ouster-sdk-0.8.1/src/ouster/sdk/_viz.pyi` & `ouster-sdk-0.9.0/src/ouster/sdk/_viz.pyi`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/src/ouster/sdk/convert_to_legacy.py` & `ouster-sdk-0.9.0/src/ouster/sdk/convert_to_legacy.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/src/ouster/sdk/examples/client.py` & `ouster-sdk-0.9.0/src/ouster/sdk/examples/client.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/src/ouster/sdk/examples/colormaps.py` & `ouster-sdk-0.9.0/src/ouster/sdk/examples/colormaps.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/src/ouster/sdk/examples/open3d.py` & `ouster-sdk-0.9.0/src/ouster/sdk/examples/open3d.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/src/ouster/sdk/examples/pcap.py` & `ouster-sdk-0.9.0/src/ouster/sdk/examples/pcap.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 This module has a rudimentary command line interface. For usage, run::
 
     $ python -m ouster.sdk.examples.pcap -h
 """
 import os
 import argparse
 from contextlib import closing
-from typing import Tuple, List
-
 import numpy as np
 
 from ouster import client, pcap
 from .colormaps import normalize
 
 
 def pcap_3d_one_scan(source: client.PacketSource,
@@ -110,129 +108,14 @@
 
     [x, y, z] = [c.flatten() for c in np.dsplit(xyz, 3)]
     ax.scatter(x, y, z, c=normalize(key.flatten()), s=0.2)
     plt.show()
     # [doc-etag-pcap-plot-xyz-points]
 
 
-def pcap_to_csv(source: client.PacketSource,
-                metadata: client.SensorInfo,
-                num: int = 0,
-                csv_dir: str = ".",
-                csv_base: str = "pcap_out",
-                csv_ext: str = "csv") -> None:
-    """Write scans from a pcap to csv files (one per lidar scan).
-
-    The number of saved lines per csv file is always H x W, which corresponds to
-    a full 2D image representation of a lidar scan.
-
-    Each line in a csv file is (for LEGACY profile):
-
-        TIMESTAMP, RANGE (mm), SIGNAL, NEAR_IR, REFLECTIVITY, X (mm), Y (mm), Z (mm)
-
-    If ``csv_ext`` ends in ``.gz``, the file is automatically saved in
-    compressed gzip format. :func:`.numpy.loadtxt` can be used to read gzipped
-    files transparently back to :class:`.numpy.ndarray`.
-
-    Args:
-        source: PacketSource from pcap
-        metadata: associated SensorInfo for PacketSource
-        num: number of scans to save from pcap to csv files
-        csv_dir: path to the directory where csv files will be saved
-        csv_base: string to use as the base of the filename for pcap output
-        csv_ext: file extension to use, "csv" by default
-    """
-
-    dual = False
-    if metadata.format.udp_profile_lidar == client.UDPProfileLidar.PROFILE_LIDAR_RNG19_RFL8_SIG16_NIR16_DUAL:
-        dual = True
-        print("Note: You've selected to convert a dual returns pcap to CSV. Each row "
-              "will represent a single pixel, so that both returns for that pixel will "
-              "be on a single row. As this is an example we provide for getting "
-              "started, we realize that you may have conversion needs which are not met "
-              "by this function. You can find the source code on the Python SDK "
-              "documentation website to modify it for your own needs.")
-
-    # ensure that base csv_dir exists
-    if not os.path.exists(csv_dir):
-        os.makedirs(csv_dir)
-
-    # construct csv header and data format
-    def get_fields_info(scan: client.LidarScan) -> Tuple[str, List[str]]:
-        field_names = 'TIMESTAMP (ns)'
-        field_fmts = ['%d']
-        for chan_field in scan.fields:
-            field_names += f', {chan_field}'
-            if chan_field in [client.ChanField.RANGE, client.ChanField.RANGE2]:
-                field_names += ' (mm)'
-            field_fmts.append('%d')
-        field_names += ', X (mm), Y (mm), Z (mm)'
-        field_fmts.extend(3 * ['%d'])
-        if dual:
-            field_names += ', X2 (mm), Y2 (mm), Z2 (mm)'
-            field_fmts.extend(3 * ['%d'])
-        return field_names, field_fmts
-
-    field_names: str = ''
-    field_fmts: List[str] = []
-
-    # [doc-stag-pcap-to-csv]
-    from itertools import islice
-    # precompute xyzlut to save computation in a loop
-    xyzlut = client.XYZLut(metadata)
-
-    # create an iterator of LidarScans from pcap and bound it if num is specified
-    scans = iter(client.Scans(source))
-    if num:
-        scans = islice(scans, num)
-
-    for idx, scan in enumerate(scans):
-
-        # initialize the field names for csv header
-        if not field_names or not field_fmts:
-            field_names, field_fmts = get_fields_info(scan)
-
-        # copy per-column timestamps for each channel
-        timestamps = np.tile(scan.timestamp, (scan.h, 1))
-
-        # grab channel data
-        fields_values = [scan.field(ch) for ch in scan.fields]
-
-        # use integer mm to avoid loss of precision casting timestamps
-        xyz = (xyzlut(scan.field(client.ChanField.RANGE)) * 1000).astype(
-            np.int64)
-
-        if dual:
-            xyz2 = (xyzlut(scan.field(client.ChanField.RANGE2)) * 1000).astype(
-                np.int64)
-
-            # get all data as one H x W x num fields int64 array for savetxt()
-            frame = np.dstack((timestamps, *fields_values, xyz, xyz2))
-
-        else:
-            # get all data as one H x W x num fields int64 array for savetxt()
-            frame = np.dstack((timestamps, *fields_values, xyz))
-
-        # not necessary, but output points in "image" vs. staggered order
-        frame = client.destagger(metadata, frame)
-
-        # write csv out to file
-        csv_path = os.path.join(csv_dir, f'{csv_base}_{idx:06d}.{csv_ext}')
-        print(f'write frame #{idx}, to file: {csv_path}')
-
-        header = '\n'.join([f'frame num: {idx}', field_names])
-
-        np.savetxt(csv_path,
-                   frame.reshape(-1, frame.shape[2]),
-                   fmt=field_fmts,
-                   delimiter=',',
-                   header=header)
-    # [doc-etag-pcap-to-csv]
-
-
 def pcap_to_las(source: client.PacketSource,
                 metadata: client.SensorInfo,
                 num: int = 0,
                 las_dir: str = ".",
                 las_base: str = "las_out",
                 las_ext: str = "las") -> None:
     "Write scans from a pcap to las files (one per lidar scan)."
@@ -381,23 +264,33 @@
         elif isinstance(packet, client.ImuPacket):
             # and access ImuPacket content
             print(f'  acceleration = {packet.accel}')
             print(f'  angular_velocity = {packet.angular_vel}')
     # [doc-etag-pcap-read-packets]
 
 
+def pcap_to_csv(
+        source: client.PacketSource,
+        metadata: client.SensorInfo,
+        num: int = 0) -> None:
+    # leave comment directing users to ouster-cli
+    print("NOTICE: The pcap-to-csv example has been retired in favor of "
+          "the ouster-cli utility installed with the Python Ouster SDK.\n"
+          "To try: ouster-cli source <PCAP> convert <OUT.CSV>")
+
+
 def main():
     """Pcap examples runner."""
     examples = {
         "open3d-one-scan": pcap_3d_one_scan,
         "plot-xyz-points": pcap_display_xyz_points,
-        "pcap-to-csv": pcap_to_csv,
         "pcap-to-las": pcap_to_las,
         "pcap-to-pcd": pcap_to_pcd,
         "pcap-to-ply": pcap_to_ply,
+        "pcap-to-csv": pcap_to_csv,
         "query-scan": pcap_query_scan,
         "read-packets": pcap_read_packets,
     }
 
     description = "Ouster Python SDK Pcap examples. The EXAMPLE must be one of:\n  " + str.join(
         '\n  ', examples.keys())
```

### Comparing `ouster-sdk-0.8.1/src/ouster/sdk/examples/reference.py` & `ouster-sdk-0.9.0/src/ouster/sdk/examples/reference.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/src/ouster/sdk/examples/viz.py` & `ouster-sdk-0.9.0/src/ouster/sdk/examples/viz.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/src/ouster/sdk/util.py` & `ouster-sdk-0.9.0/src/ouster/sdk/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Miscellaneous utilites."""
 
 import os
-from typing import Optional, List
+from typing import Optional, List, Any
+from packaging import version
+import requests
+import re
 
 
 def resolve_metadata_multi_with_prefix_guess(data_path: str) -> List[str]:
     """Look for best-matching metadata files from all json files in the same dir
 
     Args:
         data_path: filename location with the data, usually .pcap or .bag
@@ -74,7 +77,24 @@
     Args:
         data_path: filename location with the data, usually .pcap or .bag
 
     Returns:
         list of metadata json paths guessed with the most common prefix match
     """
     return resolve_metadata_multi_with_prefix_guess(data_path)
+
+
+def firmware_version(hostname: str) -> Any:
+    firmware_version_endpoint = f"http://{hostname}/api/v1/system/firmware"
+    response = requests.get(firmware_version_endpoint)
+    if response.status_code != requests.codes.ok:
+        raise RuntimeError("Could not get sensor firmware version")
+
+    match = re.search("v(\\d+).(\\d+)\\.(\\d+)", response.text)
+    if match:
+        return version.Version(".".join(
+            [match.group(1), match.group(2),
+             match.group(3)]))
+    else:
+        raise RuntimeError(
+            f"Could not get sensor firmware version from {response.text}")
+    return None
```

### Comparing `ouster-sdk-0.8.1/src/ouster/sdk/viz.py` & `ouster-sdk-0.9.0/src/ouster/sdk/viz.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,43 +3,70 @@
 All rights reserved.
 
 Sensor data visualization tools.
 
 Visualize lidar data using OpenGL.
 """
 
-from collections import (deque)
+from collections import deque
 from dataclasses import dataclass
 from functools import partial
+from enum import Enum
 import os
 import threading
 import time
 from datetime import datetime
 from typing import (Callable, ClassVar, Deque, Dict, Generic, Iterable, List,
-                    Optional, Tuple, TypeVar, Union, Any)
+                    Optional, Tuple, TypeVar, Union, Any, cast)
 from typing_extensions import Protocol, runtime_checkable
 import weakref
 import logging
+import click
 
 import numpy as np
 from PIL import Image as PILImage
 
 from ouster import client
-from ouster.client import _utils, ChanField
+from ouster.client import _utils, ChanField, first_valid_column_pose
 from ..client._client import Version
 from ._viz import (PointViz, Cloud, Image, Cuboid, Label, WindowCtx, Camera,
                    TargetDisplay, add_default_controls, calref_palette,
                    spezia_palette, grey_palette, viridis_palette, magma_palette)
 
-logger = logging.getLogger("viz-logger")
+from ouster.sdkx.util import img_aspect_ratio  # type:ignore
+import platform
 
-# limit ouster_client log statements to "debug" and direct the output to log file
-# rather than the console (default).
-# TODO uncomment when we figure out where we want to write it everywhere, have more useful logs
-# client.init_logger("info", "ouster-python.log")
+logger = logging.getLogger("viz-logger")
+client_log_location = None
+if platform.system() == "Windows":
+    client_log_dir = os.getenv("LOCALAPPDATA")
+
+    if not client_log_dir:
+        client_log_dir = os.getenv("TMP")
+        if not client_log_dir:
+            client_log_dir = "C:"
+    client_log_dir = os.path.join(client_log_dir, "ouster-cli")
+    client_log_location = os.path.join(client_log_dir, "ouster-sdk.log")
+
+else:
+    client_log_dir = os.path.join(os.path.expanduser("~"), ".ouster-cli")
+    client_log_location = os.path.join(client_log_dir, "ouster-sdk.log")
+
+logging_enabled = True
+if not os.path.exists(client_log_dir):
+    try:
+        os.makedirs(client_log_dir)
+    except Exception as e:
+        click.echo(f"Can't enable logging: {e}")
+        logging_enabled = False
+if not os.access(client_log_dir, os.W_OK):
+    click.echo("Can't enable logging")
+    logging_enabled = False
+if logging_enabled:
+    client.init_logger("info", client_log_location)
 
 T = TypeVar('T')
 
 
 def push_point_viz_handler(
         viz: PointViz, arg: T, handler: Callable[[T, WindowCtx, int, int],
                                                  bool]) -> None:
@@ -94,14 +121,16 @@
     """LidarScan field processor
 
     View modes define the process of getting the key data for
     the scan and return number as well as checks the possibility
     of showing data in that mode, see `enabled()`.
     """
 
+    _info: Optional[client.SensorInfo]
+
     @property
     def name(self) -> str:
         """Name of the view mode"""
         ...
 
     @property
     def names(self) -> List[str]:
@@ -118,28 +147,31 @@
         """Checks the view mode availability for a scan and return number"""
         ...
 
 
 @runtime_checkable
 class ImageMode(FieldViewMode, Protocol):
     """Applies the view mode key to the viz.Image"""
+
     def set_image(self,
                   img: Image,
                   ls: client.LidarScan,
                   return_num: int = 0) -> None:
         """Prepares the key data and sets the image key to it."""
         ...
 
 
 @runtime_checkable
 class CloudMode(FieldViewMode, Protocol):
     """Applies the view mode key to the viz.Cloud"""
+
     def set_cloud_color(self,
                         cloud: Cloud,
                         ls: client.LidarScan,
+                        *,
                         return_num: int = 0) -> None:
         """Prepares the key data and sets the cloud key to it."""
         ...
 
 
 class ImageCloudMode(ImageMode, CloudMode, Protocol):
     """Applies the view mode to viz.Cloud and viz.Image"""
@@ -164,17 +196,17 @@
 
     Handles single and dual returns scans.
 
     When AutoExposure is enabled its state updates only for return_num=0 but
     applies for both returns.
     """
     def __init__(self,
-                 info: client.SensorInfo,
                  field: client.ChanField,
                  *,
+                 info: Optional[client.SensorInfo] = None,
                  prefix: Optional[str] = "",
                  suffix: Optional[str] = "",
                  use_ae: bool = True,
                  use_buc: bool = False) -> None:
         """
         Args:
             info: sensor metadata used mainly for destaggering here
@@ -224,14 +256,17 @@
 
         return key_data
 
     def set_image(self,
                   img: Image,
                   ls: client.LidarScan,
                   return_num: int = 0) -> None:
+        if self._info is None:
+            raise ValueError(
+                f"VizMode[{self.name}] requires metadata to make a 2D image")
         key_data = self._prepare_data(ls, return_num)
         if key_data is not None:
             img.set_image(client.destagger(self._info, key_data))
 
     def set_cloud_color(self,
                         cloud: Cloud,
                         ls: client.LidarScan,
@@ -244,21 +279,27 @@
         return (self._fields[return_num] in ls.fields
                 if return_num < len(self._fields) else False)
 
 
 class ReflMode(SimpleMode, ImageCloudMode):
     """Prepares image/cloud data for REFLECTIVITY channel"""
 
-    def __init__(self, info: client.SensorInfo) -> None:
-        super().__init__(info, client.ChanField.REFLECTIVITY, use_ae=True)
+    def __init__(self, *, info: Optional[client.SensorInfo] = None) -> None:
+        super().__init__(client.ChanField.REFLECTIVITY, info=info, use_ae=True)
         # used only for uncalibrated reflectivity in FW prior v2.1.0
         # TODO: should we check for calibrated reflectivity status from
         # metadata too?
-        self._normalized_refl = (Version.from_string(self._info.fw_rev) >=
-                                 Version.from_string("v2.1.0"))
+        if info is not None:
+            self._info = cast(client.SensorInfo, self._info)
+            self._normalized_refl = (Version.from_string(self._info.fw_rev) >=
+                                     Version.from_string("v2.1.0"))
+        else:
+            # NOTE/TODO[pb]: ReflMode added through viz extra mode mechanism
+            # may not have a correct normalized_refl set ... need a refactor.
+            self._normalized_refl = True
 
     def _prepare_data(self,
                       ls: client.LidarScan,
                       return_num: int = 0) -> Optional[np.ndarray]:
         if not self.enabled(ls, return_num):
             return None
 
@@ -276,15 +317,15 @@
 
 def is_norm_reflectivity_mode(mode: FieldViewMode) -> bool:
     """Checks whether the image/cloud mode is a normalized REFLECTIVITY mode
 
     NOTE[pb]: This is highly implementation specific and doesn't look nicely,
     i.e. it's more like duck/duct plumbing .... but suits the need.
     """
-    return (hasattr(mode, "_normalized_refl") and mode._normalized_refl)
+    return (isinstance(mode, ReflMode) and mode._normalized_refl)
 
 
 @dataclass
 class ImgModeItem:
     """Image mode for specific return with explicit name."""
     mode: ImageMode
     name: str
@@ -298,22 +339,53 @@
     palette: np.ndarray
 
 
 LidarScanVizMode = Union[ImageCloudMode, ImageMode, CloudMode]
 """Field view mode types"""
 
 
+@dataclass
+class VizExtraMode:
+    """Image/Cloud mode factory func
+
+    Used to embed viz modes from external plugins.
+    """
+    func: Callable[[], LidarScanVizMode]
+
+    def create(self,
+               info: Optional[client.SensorInfo] = None) -> LidarScanVizMode:
+        extra_mode = self.func()
+        if info and hasattr(extra_mode, "_info") and extra_mode._info is None:
+            extra_mode._info = info
+        return extra_mode
+
+
+# Viz modes added externally
+_viz_extra_modes: List[VizExtraMode]
+_viz_extra_modes = []
+
+# Viz palettes added externally
+_viz_extra_palettes: List[CloudPaletteItem]
+_viz_extra_palettes = []
+
+
 class LidarScanViz:
     """Visualize LidarScan data.
 
     Uses the supplied PointViz instance to easily display the contents of a
     LidarScan. Sets up key bindings to toggle which channel fields and returns
     are displayed, and change 2D image and point size.
     """
 
+    class FlagsMode(Enum):
+        NONE = 0
+        HIGHLIGHT_SECOND = 1
+        HIGHLIGHT_BLOOM = 2
+        HIDE_BLOOM = 3
+
     _cloud_palette: Optional[CloudPaletteItem]
 
     def __init__(
             self,
             meta: client.SensorInfo,
             viz: Optional[PointViz] = None,
             *,
@@ -339,53 +411,68 @@
         self._cloud_palettes: List[CloudPaletteItem]
         self._cloud_palettes = [
             CloudPaletteItem("Ouster Colors", spezia_palette),
             CloudPaletteItem("Greyscale", grey_palette),
             CloudPaletteItem("Viridis", viridis_palette),
             CloudPaletteItem("Magma", magma_palette),
         ]
+
+        # Add extra color palettes, usually inserted through plugins
+        self._cloud_palettes.extend(_viz_extra_palettes)
+
         self._cloud_palettes.extend(_ext_palettes or [])
 
         self._cloud_palette_ind = 0
         self._cloud_palette = self._cloud_palettes[self._cloud_palette_ind]
         self._cloud_palette_name = self._cloud_palette.name
 
         # image display state
         self._img_ind = [0, 1]  # index of field to display
         self._img_refl_mode = [False, False]
-        self._img_size_fraction = 6
-        self._img_aspect = _img_aspect_ratio or (
-            max(meta.beam_altitude_angles) -
-            min(meta.beam_altitude_angles)) / 360.0
+        self._img_size_fraction = 4
+        self._img_aspect = _img_aspect_ratio or img_aspect_ratio(meta)
 
         # misc display state
         self._ring_size = 1
         self._ring_line_width = 1
         self._osd_enabled = True
+        self._scan_poses_enabled = False
 
         self._modes: List[LidarScanVizMode]
         self._modes = [
-            SimpleMode(meta, ChanField.NEAR_IR, use_ae=True, use_buc=True),
-            ReflMode(meta),
-            SimpleMode(meta, ChanField.SIGNAL),
-            SimpleMode(meta, ChanField.RANGE),
+            ReflMode(info=meta),
+            SimpleMode(ChanField.NEAR_IR, info=meta, use_ae=True, use_buc=True),
+            SimpleMode(ChanField.SIGNAL, info=meta),
+            SimpleMode(ChanField.RANGE, info=meta),
         ]
 
+        # Add extra viz mode, usually inserted through plugins
+        self._modes.extend([vm.create(meta) for vm in _viz_extra_modes])
+
         self._modes.extend(_ext_modes or [])
 
         self._image_modes: List[ImgModeItem]
         self._image_modes = [
             ImgModeItem(mode, name, num) for mode in self._modes
             if isinstance(mode, ImageMode)
             for num, name in enumerate(mode.names)
         ]
 
         self._cloud_modes: List[CloudMode]
         self._cloud_modes = [m for m in self._modes if isinstance(m, CloudMode)]
 
+        # TODO[pb]: Extract FlagsMode to custom processor (TBD the whole thing)
+        # initialize masks to just green with zero opacity
+        mask = np.zeros(
+            (meta.format.pixels_per_column, meta.format.columns_per_frame, 4),
+            dtype=np.float32)
+        mask[:, :, 1] = 1.0
+        self._cloud_masks = (mask, mask.copy())
+        self._flags_mode = LidarScanViz.FlagsMode.NONE
+
         self._viz = viz or PointViz("Ouster Viz")
 
         self._metadata = meta
         self._clouds = (Cloud(meta), Cloud(meta))
         self._viz.add(self._clouds[0])
         self._viz.add(self._clouds[1])
 
@@ -399,14 +486,21 @@
         self._viz.target_display.set_ring_size(self._ring_size)
         self._viz.target_display.enable_rings(True)
 
         # initialize osd
         self._osd = Label("", 0, 1)
         self._viz.add(self._osd)
 
+        self._scan_ind = -1
+
+        # scan identity poses to re-use
+        self._scan_column_poses_identity = np.array(
+            [np.eye(4) for _ in range(self._metadata.format.columns_per_frame)],
+            dtype=np.float32)
+
         # key bindings. will be called from rendering thread, must be synchronized
         key_bindings: Dict[Tuple[int, int], Callable[[LidarScanViz], None]] = {
             (ord('E'), 0): partial(LidarScanViz.update_image_size, amount=1),
             (ord('E'), 1): partial(LidarScanViz.update_image_size, amount=-1),
             (ord('P'), 0): partial(LidarScanViz.update_point_size, amount=1),
             (ord('P'), 1): partial(LidarScanViz.update_point_size, amount=-1),
             (ord('1'), 0): partial(LidarScanViz.toggle_cloud, i=0),
@@ -415,23 +509,52 @@
             (ord('N'), 0): partial(LidarScanViz.cycle_img_mode, i=1),
             (ord('M'), 0): LidarScanViz.cycle_cloud_mode,
             (ord('F'), 0): LidarScanViz.cycle_cloud_palette,
             (ord("'"), 0): partial(LidarScanViz.update_ring_size, amount=1),
             (ord("'"), 1): partial(LidarScanViz.update_ring_size, amount=-1),
             (ord("'"), 2): LidarScanViz.cicle_ring_line_width,
             (ord("O"), 0): LidarScanViz.toggle_osd,
+            (ord('T'), 0): LidarScanViz.toggle_scan_poses,
+            # TODO[pb]: Extract FlagsMode to custom processor (TBD the whole thing)
+            (ord('C'), 0): LidarScanViz.update_flags_mode,
+            (ord('/'), 1): LidarScanViz.print_keys,
         }
 
         def handle_keys(self: LidarScanViz, ctx: WindowCtx, key: int,
                         mods: int) -> bool:
             if (key, mods) in key_bindings:
                 key_bindings[key, mods](self)
                 self.draw()
             return True
 
+        key_definitions: Dict[str, str] = {
+            'w': "Camera pitch up",
+            's': "Camera pitch down",
+            'a': "Camera yaw left",
+            'd': "Camera yaw right",
+            "e / E": "Increase/decrease size of displayed 2D images",
+            "p / P": "Increase/decrease point size",
+            "R": "Reset camera orientation",
+            "0": "Toggle orthographic camera",
+            "1": "Toggle point cloud 1 visibility",
+            "2": "Toggle point cloud 2 visibility",
+            "b": "Cycle top 2D image",
+            "n": "Cycle bottom 2D image",
+            'm': "Cycle through point cloud coloring mode",
+            'f': "Cycle through point cloud color palette",
+            't': "Toggle scan poses",
+            '?': "Print keys to standard out",
+            "= / -": "Dolly in and out",
+            "' / \"": "Increase/decrease spacing in range markers",
+            'SHIFT': "Camera Translation with mouse drag",
+            'ESC': "Exit the application",
+        }
+        self._key_definitions = key_definitions
+        print("Press \'?\' while viz window is focused to print key bindings")
+
         push_point_viz_handler(self._viz, self, handle_keys)
         add_default_controls(self._viz)
 
     def cycle_img_mode(self, i: int) -> None:
         """Change the displayed field of the i'th image."""
         with self._lock:
             self._img_ind[i] += 1
@@ -497,24 +620,80 @@
             self._viz.target_display.set_ring_line_width(self._ring_line_width)
 
     def toggle_osd(self, state: Optional[bool] = None) -> None:
         """Show or hide the on-screen display."""
         with self._lock:
             self._osd_enabled = not self._osd_enabled if state is None else state
 
+    def toggle_scan_poses(self) -> None:
+        """Toggle the per column poses use."""
+        with self._lock:
+            if self._scan_poses_enabled:
+                self._scan_poses_enabled = False
+                print("LidarScanViz: Key T: Scan Poses: OFF")
+            else:
+                self._scan_poses_enabled = True
+                print("LidarScanViz: Key T: Scan Poses: ON")
+
+    # TODO[pb]: Extract FlagsMode to custom processor (TBD the whole thing)
+    def update_flags_mode(self,
+                          mode: 'Optional[LidarScanViz.FlagsMode]' = None) -> None:
+        with self._lock:
+            # cycle between flag mode enum values
+            if mode is None:
+                self._flags_mode = LidarScanViz.FlagsMode(
+                    (self._flags_mode.value + 1) %
+                    len(LidarScanViz.FlagsMode.__members__))
+            else:
+                self._flags_mode = mode
+
+            # set mask on all points in the second cloud, clear other mask
+            if self._flags_mode == LidarScanViz.FlagsMode.HIGHLIGHT_SECOND:
+                self._cloud_masks[0][:, :, 3] = 0.0
+                self._cloud_masks[1][:, :, 3] = 1.0
+                self._clouds[0].set_mask(self._cloud_masks[0])
+                self._clouds[1].set_mask(self._cloud_masks[1])
+            # clear masks on both clouds, expected to be set dynamically in _draw()
+            else:
+                self._cloud_masks[0][:, :, 3] = 0.0
+                self._cloud_masks[1][:, :, 3] = 0.0
+                self._clouds[0].set_mask(self._cloud_masks[0])
+                self._clouds[1].set_mask(self._cloud_masks[1])
+
+            # not bothering with OSD
+            # TODO[pb]: hmm, probably should bother with OSD somehow
+            print("Flags mode:", self._flags_mode.name)
+
+    def print_keys(self) -> None:
+        with self._lock:
+            print(">---------------- Key Bindings --------------<")
+            for key_binding in self._key_definitions:
+                print(f"{key_binding:^7}: {self._key_definitions[key_binding]}")
+            print(">--------------------------------------------<")
+
     @property
     def scan(self) -> client.LidarScan:
         """The currently displayed scan."""
         return self._scan
 
     @scan.setter
     def scan(self, scan: client.LidarScan) -> None:
         """Set the scan to display"""
         self._scan = scan
 
+    @property
+    def scan_ind(self) -> int:
+        """The currently displayed scan number (-1 if was never set)"""
+        return self._scan_ind
+
+    @scan_ind.setter
+    def scan_ind(self, scan_ind: int) -> None:
+        """Set the scan number of the currently displayed scan"""
+        self._scan_ind = scan_ind
+
     def draw(self, update: bool = True) -> bool:
         """Process and draw the latest state to the screen."""
         with self._lock:
             self._draw()
 
         if update:
             return self._viz.update()
@@ -612,14 +791,56 @@
                 f"profile: {str(meta.format.udp_profile_lidar)}\n"
                 f"{meta.prod_line} {meta.fw_rev} {meta.mode}\n"
                 f"shot limiting status: {str(scan.shot_limiting())}\n"
                 f"thermal shutdown status: {str(scan.thermal_shutdown())}")
         else:
             self._osd.set_text("")
 
+        self._draw_update_scan_poses()
+
+        # TODO[pb]: Extract FlagsMode to custom processor (TBD the whole thing)
+        self._draw_update_flags_mode()
+
+    def _draw_update_scan_poses(self) -> None:
+        """Apply poses from the scan to the cloud"""
+
+        column_poses = (self._scan.pose if self._scan_poses_enabled else
+                        self._scan_column_poses_identity)
+
+        for cloud in self._clouds:
+            cloud.set_column_poses(column_poses)
+
+        # with poses camera tracks the scan position
+        camera_target = (np.linalg.inv(first_valid_column_pose(self._scan))
+                         if self._scan_poses_enabled else np.eye(4))
+
+        self._viz.camera.set_target(camera_target)
+
+    def _draw_update_flags_mode(self) -> None:
+        """Apply selected FlagsMode to the cloud"""
+        # set a cloud mask based where first flags bit is set
+        if self._flags_mode == LidarScanViz.FlagsMode.HIGHLIGHT_BLOOM:
+            for i, flag_field in ((0, ChanField.FLAGS), (1, ChanField.FLAGS2)):
+                if flag_field in self._scan.fields:
+                    mask_opacity = (self._scan.field(flag_field) & 0x1) * 1.0
+                    self._cloud_masks[i][:, :, 3] = mask_opacity
+                    self._clouds[i].set_mask(self._cloud_masks[i])
+
+        # set range to zero where first flags bit is set
+        elif self._flags_mode == LidarScanViz.FlagsMode.HIDE_BLOOM:
+            for i, flag_field, range_field in ((0, ChanField.FLAGS,
+                                                ChanField.RANGE),
+                                               (1, ChanField.FLAGS2,
+                                                ChanField.RANGE2)):
+                if flag_field in self._scan.fields and range_field in self._scan.fields:
+                    # modifying the scan in-place would break cycling modes while paused
+                    range = self._scan.field(range_field).copy()
+                    range[self._scan.field(flag_field) & 0x1 == 0x1] = 0
+                    self._clouds[i].set_range(range)
+
 
 class _Seekable(Generic[T]):
     """Wrap an iterable to support seeking by index.
 
     Similar to `more_itertools.seekable` but keeps indexes stable even values
     are evicted from the cache.
 
@@ -724,14 +945,15 @@
     _playback_rates: ClassVar[Tuple[float, ...]]
     _playback_rates = (0.25, 0.5, 0.75, 1.0, 1.5, 2.0, 3.0, 0.0)
 
     def __init__(self,
                  arg: Union[client.SensorInfo, AnyScanViz],
                  rate: Optional[float] = None,
                  pause_at: int = -1,
+                 on_eof: str = 'exit',
                  _buflen: int = 50) -> None:
         """
         Args:
             arg: Metadata associated with the scans to be visualized or a
                  LidarScanViz instance to use.
             rate: Playback rate. One of 0.25, 0.5, 0.75, 1.0, 1.5, 2.0, 3.0 or
                   None for "live" playback (the default).
@@ -756,14 +978,15 @@
             self._scan_viz = arg
 
         self._lock = threading.Lock()
         self._live = (rate is None)
         self._rate_ind = SimpleViz._playback_rates.index(rate or 0.0)
         self._buflen = _buflen
         self._pause_at = pause_at
+        self._on_eof = on_eof
 
         # pausing and stepping
         self._cv = threading.Condition()
         self._paused = False
         self._step = 0
         self._proc_exit = False
 
@@ -783,14 +1006,25 @@
             (ord('.'), 2): partial(SimpleViz.seek_relative, n_frames=10),
             (ord(' '), 0): SimpleViz.toggle_pause,
             (ord('O'), 0): SimpleViz.toggle_osd,
             (ord('X'), 1): SimpleViz.toggle_img_recording,
             (ord('Z'), 1): SimpleViz.screenshot,
         }
 
+        key_definitions: Dict[str, str] = {
+            'o': "Toggle information overlay",
+            'shift+x': "Toggle a continuous saving of screenshots",
+            'shift+z': "Take a screenshot!",
+            ". / ,": "Step forward one frame",
+            "> / <": "Increase/decrease playback rate (during replay)",
+            'SPACE': "Pause and unpause",
+        }
+        if hasattr(self._scan_viz, "_key_definitions"):
+            self._scan_viz._key_definitions.update(key_definitions)
+
         # only allow changing rate when not in "live" mode
         if not self._live:
             key_bindings.update({
                 (ord(','), 1):
                 partial(SimpleViz.modify_rate, amount=-1),
                 (ord('.'), 1):
                 partial(SimpleViz.modify_rate, amount=1),
@@ -894,47 +1128,49 @@
     def _process(self, seekable: _Seekable[client.LidarScan]) -> None:
 
         last_ts = time.monotonic()
         scan_idx = -1
         try:
             while True:
                 # wait until unpaused, step, or quit
-                with self._cv:
-                    self._cv.wait_for(lambda: not self._paused or self._step or
-                                      self._proc_exit)
-                    if self._proc_exit:
+                try:
+                    with self._cv:
+                        self._cv.wait_for(lambda: not self._paused or self._step or
+                                          self._proc_exit)
+                        if self._proc_exit:
+                            break
+                        if self._step:
+                            seek_ind = seekable.next_ind + self._step - 1
+                            self._step = 0
+                            if not seekable.seek(seek_ind):
+                                continue
+                        period = self._frame_period()
+
+                    # process new data
+                    scan_idx = seekable.next_ind
+                    self._scan_viz.scan = next(seekable)
+                    self._scan_viz.scan_ind = scan_idx
+                    self._scan_viz.draw(update=False)
+
+                    if self._pause_at == scan_idx:
+                        self._paused = True
+                        self._update_playback_osd()
+
+                    # sleep for remainder of scan period
+                    to_sleep = max(0.0, period - (time.monotonic() - last_ts))
+                    if scan_idx > 0:
+                        time.sleep(to_sleep)
+
+                    last_ts = time.monotonic()
+
+                    # show new data
+                    self._viz.update()
+                except StopIteration:
+                    if self._on_eof == 'exit':
                         break
-                    if self._step:
-                        seek_ind = seekable.next_ind + self._step - 1
-                        self._step = 0
-                        if not seekable.seek(seek_ind):
-                            continue
-                    period = self._frame_period()
-
-                # process new data
-                scan_idx = seekable.next_ind
-                self._scan_viz.scan = next(seekable)
-                self._scan_viz.draw(update=False)
-
-                if self._pause_at == scan_idx:
-                    self._paused = True
-                    self._update_playback_osd()
-
-                # sleep for remainder of scan period
-                to_sleep = max(0.0, period - (time.monotonic() - last_ts))
-                if scan_idx > 0:
-                    time.sleep(to_sleep)
-
-                last_ts = time.monotonic()
-
-                # show new data
-                self._viz.update()
-
-        except StopIteration:
-            pass
 
         finally:
             # signal rendering (main) thread to exit, with a delay
             # because the viz in main thread may not have been started
             # and on Mac it was observed that it fails to set a flag if
             # _process fails immediately after start
             time.sleep(0.5)
@@ -951,22 +1187,22 @@
 
         Returns:
             When the stream is consumed or the visualizer window is closed.
         """
 
         seekable = _Seekable(scans, maxlen=self._buflen)
         try:
-            logger.warn("Starting processing thread...")
+            logger.info("Starting processing thread...")
             self._proc_exit = False
             proc_thread = threading.Thread(name="Viz processing",
                                            target=self._process,
                                            args=(seekable, ))
             proc_thread.start()
 
-            logger.warn("Starting rendering loop...")
+            logger.info("Starting rendering loop...")
             self._viz.run()
             logger.info("Done rendering loop")
         except KeyboardInterrupt:
             pass
         finally:
             try:
                 # some scan sources may be waiting on IO, blocking the
@@ -984,9 +1220,9 @@
             proc_thread.join()
 
 
 __all__ = [
     'PointViz', 'Cloud', 'Image', 'Cuboid', 'Label', 'WindowCtx', 'Camera',
     'TargetDisplay', 'add_default_controls', 'calref_palette', 'spezia_palette',
     'grey_palette', 'viridis_palette', 'magma_palette', 'ImageMode',
-    'CloudMode', 'ImageCloudMode', 'CloudPaletteItem'
+    'CloudMode', 'ImageCloudMode', 'CloudPaletteItem', 'VizExtraMode'
 ]
```

### Comparing `ouster-sdk-0.8.1/src/ouster_sdk.egg-info/PKG-INFO` & `ouster-sdk-0.9.0/src/ouster_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ouster-sdk
-Version: 0.8.1
-Summary: Ouster sensor SDK
+Version: 0.9.0
+Summary: Ouster Sensor SDK
 Home-page: https://github.com/ouster-lidar/ouster_example
 Author: Ouster Sensor SDK Developers
 Author-email: oss@ouster.io
 License: BSD 3-Clause License
 Project-URL: Ouster SDK Documentation, https://static.ouster.dev/sdk-docs/index.html
 Project-URL: Bug Tracker, https://github.com/ouster-lidar/ouster_example/issues
 Project-URL: Ouster Customer Support, https://ouster.atlassian.net/servicedesk/customer/portal/8
@@ -20,24 +20,26 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: examples
+Provides-Extra: mapping
 
 =================
 Ouster Python SDK
 =================
 
 ..
     [sdk-overview-start]
@@ -74,15 +76,15 @@
   ``manylinux2014_aarch64``)
 - macOS >= 10.13 on x86_64 platforms (``macosx_10_13_x86_64``)
 - macOS >= 11.0 on Apple M1 for Python >= 3.8 (``macosx_11_0_arm64``)
 - Windows 10 on x86_64 platforms (``win_amd64``)
 
 Building from source is supported on:
 
-- Ubuntu 18.04, 20.04, 22.04, and Debian 10 (x86-64, aarch64)
+- Ubuntu 20.04, 22.04, and Debian 11 (x86-64, aarch64)
 - macOS >= 10.13 (x86-64), >= 11.0 (arm64)
 - Windows 10 (x86-64)
 
 .. _PyPI: https://pypi.org/project/ouster-sdk/
 
 ..
     [python-supported-platforms-end]
```

### Comparing `ouster-sdk-0.8.1/tests/conftest.py` & `ouster-sdk-0.9.0/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Copyright (c) 2021, Ouster, Inc.
 All rights reserved.
 """
 
 from contextlib import closing
 from os import path
 from typing import Iterator
+from pathlib import Path
 
 from more_itertools import partition
 import pytest
 
 from ouster import client, pcap
 
 pytest.register_assert_rewrite('ouster.client._digest')
@@ -42,15 +43,17 @@
 
     config.hook.pytest_deselected(items=deselect)
     items[:] = select
 
 
 # test data
 # TODO: add OS-DOME-32/64 in 1024x10 mode pcap with digest
-DATA_DIR = path.join(path.dirname(path.abspath(__file__)), "../../tests/pcaps")
+PCAPS_DATA_DIR = path.join(path.dirname(path.abspath(__file__)), "../../tests/pcaps")
+METADATA_DATA_DIR = path.join(path.dirname(path.abspath(__file__)), "../../tests/metadata")
+OSFS_DATA_DIR = path.join(path.dirname(path.abspath(__file__)), "../../tests/osfs")
 
 TESTS = {
     'legacy-2.0': 'OS-2-32-U0_v2.0.0_1024x10',
     'legacy-2.1': 'OS-1-32-G_v2.1.1_1024x10',
     'dual-2.2': 'OS-0-32-U1_v2.2.0_1024x10',
     'single-2.3': 'OS-2-128-U1_v2.3.0_1024x10',
     'low-data-rate-2.3': 'OS-0-128-U1_v2.3.0_1024x10',
@@ -65,36 +68,36 @@
 @pytest.fixture
 def base_name(test_key: str) -> str:
     return TESTS[test_key]
 
 
 @pytest.fixture
 def stream_digest(base_name: str):
-    digest_path = path.join(DATA_DIR, f"{base_name}_digest.json")
+    digest_path = path.join(PCAPS_DATA_DIR, f"{base_name}_digest.json")
     with open(digest_path, 'r') as f:
         return digest.StreamDigest.from_json(f.read())
 
 
 @pytest.fixture
 def meta(base_name: str):
-    meta_path = path.join(DATA_DIR, f"{base_name}.json")
+    meta_path = path.join(PCAPS_DATA_DIR, f"{base_name}.json")
     with open(meta_path, 'r') as f:
         return client.SensorInfo(f.read())
 
 
 @pytest.fixture
 def meta_2_0():
-    meta_path = path.join(DATA_DIR, f"{TESTS['legacy-2.0']}.json")
+    meta_path = path.join(PCAPS_DATA_DIR, f"{TESTS['legacy-2.0']}.json")
     with open(meta_path, 'r') as f:
         return client.SensorInfo(f.read())
 
 
 @pytest.fixture
 def real_pcap_path(base_name: str, meta: client.SensorInfo) -> str:
-    return path.join(DATA_DIR, f"{base_name}.pcap")
+    return path.join(PCAPS_DATA_DIR, f"{base_name}.pcap")
 
 
 @pytest.fixture
 def real_pcap(real_pcap_path: str,
               meta: client.SensorInfo) -> Iterator[pcap.Pcap]:
     pcap_obj = pcap.Pcap(real_pcap_path, meta)
     yield pcap_obj
@@ -120,7 +123,12 @@
         return client.Packets(ps, meta)
 
 
 @pytest.fixture
 def scan(packets: client.PacketSource) -> client.LidarScan:
     scans = client.Scans(packets)
     return next(iter(scans))
+
+
+@pytest.fixture(scope="package")
+def test_data_dir():
+    return Path(path.dirname(path.abspath(__file__))) / ".." / ".." / "tests"
```

### Comparing `ouster-sdk-0.8.1/tests/test_batching.py` & `ouster-sdk-0.9.0/tests/test_batching.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/tests/test_config.py` & `ouster-sdk-0.9.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/tests/test_core.py` & `ouster-sdk-0.9.0/tests/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,19 +187,24 @@
 
 
 @pytest.mark.parametrize('test_key', ['legacy-2.0'])
 def test_scans_timeout(packets: client.PacketSource) -> None:
     """A zero timeout should deterministically throw.
 
     TODO: should it, though?
+
+    TWS 20230609: a timeout no longer raises an exception...
+    instead it stops iteration and sets _timed_out=True.
     """
-    scans = iter(client.Scans(packets, timeout=0.0))
+    scans = client.Scans(packets, timeout=0.0)
+    scans_itr = iter(scans)
 
-    with pytest.raises(client.ClientTimeout):
-        next(scans)
+    with pytest.raises(StopIteration):
+        next(scans_itr)
+    assert scans._timed_out
 
 
 def test_scans_digest(stream_digest, packets: client.PacketSource) -> None:
     """Test that parsing packets produces expected results.
 
     Checks hashes of all packet and scans fields and headers against
     known-good values.
```

### Comparing `ouster-sdk-0.8.1/tests/test_data.py` & `ouster-sdk-0.9.0/tests/test_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,21 +2,26 @@
 Copyright (c) 2021, Ouster, Inc.
 All rights reserved.
 
 Tests for lidar data parsing.
 
 Checks that the output of parsing hasn't changed unexpectedly.
 """
+import os
+import json
 from copy import deepcopy
 
 import numpy as np
 import pytest
 
 from ouster import client
 from ouster.client import _client
+from ouster.pcap import _pcap
+
+from tests.conftest import PCAPS_DATA_DIR
 
 
 def test_make_packets(meta: client.SensorInfo) -> None:
     pf = _client.PacketFormat.from_info(meta)
 
     client.ImuPacket(bytes(pf.imu_packet_size), meta)
     client.ImuPacket(bytearray(pf.imu_packet_size), meta)
@@ -170,14 +175,20 @@
 
     ls.status[-1] = 0xffff
     assert ls.status[-1] == 0xffff
 
     ls.status[:] = 0x1
     assert np.all(ls.status == 0x1)
 
+    assert np.all(ls.pose == np.eye(4))
+
+    ls.pose[1][0, 2] = 8
+    assert np.all(ls.pose[1] == np.array([[1, 0, 8, 0], [0, 1, 0, 0],
+                                          [0, 0, 1, 0], [0, 0, 0, 1]]))
+
 
 def test_scan_from_native() -> None:
     ls = client.LidarScan(1024, 32)
     ls2 = client.LidarScan.from_native(ls)
 
     assert ls is ls2
 
@@ -432,14 +443,15 @@
 
 def test_scan_copy_eq() -> None:
     """Test equality with a copy."""
 
     ls0 = client.LidarScan(32, 512)
     ls0.status[:] = 0x1
     ls0.field(client.ChanField.REFLECTIVITY)[:] = 100
+    ls0.pose[:, 0, 3] = 8
 
     ls1 = deepcopy(ls0)
 
     assert ls0 is not ls1
     assert ls0 == ls1
 
     ls0.frame_id = 9
@@ -462,14 +474,20 @@
 
     ls0.field(client.ChanField.RANGE)[0, 0] = 42
     assert ls0 != ls1
 
     ls1.field(client.ChanField.RANGE)[0, 0] = 42
     assert ls0 == ls1
 
+    ls0.pose[1] = np.eye(4)
+    assert ls0 != ls1
+
+    ls0.pose[1, 0, 3] = 8
+    assert ls0 == ls1
+
 
 def test_scan_eq_with_custom_fields() -> None:
     """Test equality with custom fields."""
 
     ls0 = client.LidarScan(32, 512, {
         client.ChanField.CUSTOM0: np.uint32,
         client.ChanField.CUSTOM4: np.uint8
@@ -484,7 +502,120 @@
     assert np.count_nonzero(
         ls2.field(client.ChanField.CUSTOM0) == 100) == ls0.h * ls0.w
     assert np.count_nonzero(ls2.field(client.ChanField.CUSTOM4) == 100) == 0
 
     assert ls1 is not ls0
     assert ls1 != ls0
     assert ls2 == ls0
+
+
+def test_error_eq() -> None:
+    assert client.PacketSizeError("abc") == client.PacketSizeError("abc")
+
+
+def test_lidar_packet_validator() -> None:
+    """LidarPacketValidator should be capable of the same init_id/sn check as LidarPacket."""
+    meta_file_path = os.path.join(PCAPS_DATA_DIR, 'OS-0-128-U1_v2.3.0_1024x10.json')
+    pcap_file_path = os.path.join(PCAPS_DATA_DIR, 'OS-0-128-U1_v2.3.0_1024x10.pcap')
+    metadata = client.SensorInfo(open(meta_file_path).read())
+
+    metadata2 = deepcopy(metadata)
+    metadata2.init_id = 1234
+    metadata2.sn = "5678"
+
+    validator = client.LidarPacketValidator(metadata2)
+    pcap_handle = _pcap.replay_initialize(pcap_file_path)
+    buf = bytearray(2**16)
+    info = _pcap.packet_info()
+    _pcap.next_packet_info(pcap_handle, info)
+    n_bytes = _pcap.read_packet(pcap_handle, buf)
+    errors = validator.check_packet(buf, n_bytes)
+    assert n_bytes == 8448
+    try:
+        # LidarPacket constructor should throw the same error if _raise_on_id_check is True
+        client.LidarPacket(buf, metadata2, None, _raise_on_id_check=True)
+    except client.data.PacketIdError as e:
+        assert type(errors) == list
+        assert len(errors) == 1
+        assert str(e) == str(errors[0])
+        assert str(e) == "Metadata init_id/sn does not match: expected by metadata \
+- 1234/5678, but got from packet buffer - 5431292/122150000150"
+        pass
+    else:
+        assert False, "Expected an exception to be raised by client.LidarPacket."
+    finally:
+        _pcap.replay_uninitialize(pcap_handle)
+
+
+def test_lidar_packet_validator_2() -> None:
+    """LidarPacketValidator check_packet should return None if there are no issues."""
+    meta_file_path = os.path.join(PCAPS_DATA_DIR, 'OS-0-128-U1_v2.3.0_1024x10.json')
+    pcap_file_path = os.path.join(PCAPS_DATA_DIR, 'OS-0-128-U1_v2.3.0_1024x10.pcap')
+    metadata = client.SensorInfo(open(meta_file_path).read())
+
+    metadata2 = deepcopy(metadata)
+
+    validator = client.LidarPacketValidator(metadata2)
+    pcap_handle = _pcap.replay_initialize(pcap_file_path)
+    buf = bytearray(2**16)
+    info = _pcap.packet_info()
+    _pcap.next_packet_info(pcap_handle, info)
+    n_bytes = _pcap.read_packet(pcap_handle, buf)
+    assert n_bytes == 8448
+    assert validator.check_packet(buf, n_bytes) == []
+    _pcap.replay_uninitialize(pcap_handle)
+
+
+def test_lidar_packet_validator_3() -> None:
+    """LidarPacketValidator check_packet should identify a packet
+    that's the wrong size according to the lidar UDP profile."""
+    meta_file_path = os.path.join(PCAPS_DATA_DIR, 'OS-0-128-U1_v2.3.0_1024x10.json')
+    pcap_file_path = os.path.join(PCAPS_DATA_DIR, 'OS-0-128-U1_v2.3.0_1024x10.pcap')
+    metadata = client.SensorInfo(open(meta_file_path).read())
+
+    metadata2 = deepcopy(metadata)
+    metadata2.format.udp_profile_lidar = client.UDPProfileLidar.PROFILE_LIDAR_FIVE_WORD_PIXEL
+
+    validator = client.LidarPacketValidator(metadata2)
+    pcap_handle = _pcap.replay_initialize(pcap_file_path)
+    buf = bytearray(2**16)
+    info = _pcap.packet_info()
+    _pcap.next_packet_info(pcap_handle, info)
+    n_bytes = _pcap.read_packet(pcap_handle, buf)
+    assert n_bytes == 8448
+    errors = validator.check_packet(buf, n_bytes)
+    assert len(errors) == 1
+    assert type(errors[0]) == client.PacketSizeError
+    assert str(errors[0]) == 'Expected a packet of size 41216 but got a buffer of size 8448'
+    _pcap.replay_uninitialize(pcap_handle)
+
+
+def test_lidar_packet_validator_4() -> None:
+    """LidarPacketValidator check_packet should identify a packet
+    that's the wrong size according to the data format."""
+    meta_file_path = os.path.join(PCAPS_DATA_DIR, 'OS-0-128-U1_v2.3.0_1024x10.json')
+    pcap_file_path = os.path.join(PCAPS_DATA_DIR, 'OS-0-128-U1_v2.3.0_1024x10.pcap')
+    meta_json = json.load(open(meta_file_path))
+    meta_json['data_format']['columns_per_frame'] = 4096
+    meta_json['data_format']['pixels_per_column'] = 16
+    meta_json['data_format']['pixel_shift_by_row'] = [0] * 16
+    meta_json['beam_altitude_angles'] = [1] * 16
+    meta_json['beam_azimuth_angles'] = [1] * 16
+    meta_json['prod_sn'] = '1234'
+    metadata2 = client.SensorInfo(json.dumps(meta_json))
+
+    validator = client.LidarPacketValidator(metadata2)
+    pcap_handle = _pcap.replay_initialize(pcap_file_path)
+    buf = bytearray(2**16)
+    info = _pcap.packet_info()
+    _pcap.next_packet_info(pcap_handle, info)
+    n_bytes = _pcap.read_packet(pcap_handle, buf)
+    assert n_bytes == 8448
+    errors = validator.check_packet(buf, n_bytes)
+    assert len(errors) == 2
+    assert type(errors[0]) == client.PacketIdError
+    assert str(
+        errors[0]) == 'Metadata init_id/sn does not match: expected by metadata - \
+5431292/1234, but got from packet buffer - 5431292/122150000150'
+    assert type(errors[1]) == client.PacketSizeError
+    assert str(errors[1]) == 'Expected a packet of size 1280 but got a buffer of size 8448'
+    _pcap.replay_uninitialize(pcap_handle)
```

### Comparing `ouster-sdk-0.8.1/tests/test_destagger.py` & `ouster-sdk-0.9.0/tests/test_destagger.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/tests/test_metadata.py` & `ouster-sdk-0.9.0/tests/test_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 
 from copy import copy
 
 import json
 import numpy
 import pytest
 import inspect
+from pathlib import Path
 
 from ouster import client
 
+from tests.conftest import METADATA_DATA_DIR
+
 
 @pytest.mark.parametrize("mode, string", [
     (client.TimestampMode.TIME_FROM_UNSPEC, "UNKNOWN"),
     (client.TimestampMode.TIME_FROM_INTERNAL_OSC, "TIME_FROM_INTERNAL_OSC"),
     (client.TimestampMode.TIME_FROM_SYNC_PULSE_IN, "TIME_FROM_SYNC_PULSE_IN"),
     (client.TimestampMode.TIME_FROM_PTP_1588, "TIME_FROM_PTP_1588"),
 ])
@@ -210,7 +213,28 @@
 def test_equality_format() -> None:
     """Check length of data format to ensure we've added appropriately to the == operator"""
 
     data_format_attributes = inspect.getmembers(client.DataFormat, lambda a: not inspect.isroutine(a))
     data_format_properties = [a for a in data_format_attributes if not (a[0].startswith('__') and a[0].endswith('__'))]
 
     assert len(data_format_properties) == 8, "Don't forget to update tests and the data_format == operator!"
+
+
+def test_skip_metadata_beam_validation() -> None:
+    """Check that skipping beam validation works"""
+
+    all_zeros_metadata = str(Path(METADATA_DATA_DIR) / "malformed/complete_but_all_zeros_legacy.json")
+
+    # test that you can simply initialize without any metadata specified
+    client.SensorInfo()
+
+    with open(all_zeros_metadata, 'r') as f:
+
+        # test that by default it raises an error
+        with pytest.raises(RuntimeError):
+            client.SensorInfo(f.read())
+
+        # reset
+        f.seek(0)
+
+        # test that specifying skip doesn't raise error
+        client.SensorInfo(f.read(), skip_beam_validation = True)
```

### Comparing `ouster-sdk-0.8.1/tests/test_pcap.py` & `ouster-sdk-0.9.0/tests/test_pcap.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 from collections import defaultdict
 from copy import copy
 from os import path
 from random import getrandbits, shuffle, random
 from typing import (Dict, Iterable, Iterator, List, Callable)
 from itertools import chain
+from more_itertools import consume
 
 import pytest
 import time
 
 from ouster import pcap
 from ouster.pcap import _pcap
 from ouster import client
 from ouster.client import _client
-from tests.conftest import DATA_DIR, TESTS
+from tests.conftest import PCAPS_DATA_DIR, TESTS
 from tests.test_batching import _patch_frame_id
 
 SLL_PROTO = 113
 ETH_PROTO = 1
 UDP_PROTO = 17
 
 
@@ -495,120 +496,141 @@
         i += 1
 
     _pcap.replay_uninitialize(playback)
 
 
 def test_indexed_pcap_reader(tmpdir):
     """It should correctly locate the start of frames in a PCAP file"""
-    meta_path = path.join(DATA_DIR, f"{TESTS['dual-2.2']}.json")
+    meta_path = path.join(PCAPS_DATA_DIR, f"{TESTS['dual-2.2']}.json")
 
-    def progress_callback(offset, delta, filesize):
-        pass
     sensor_info = client.SensorInfo(open(meta_path).read())
     num_frames = 10
     in_packets = list(fake_packet_stream_with_frame_id(sensor_info, num_frames, 3, 3, lambda frame_num: frame_num))
     assert len(in_packets) > 0
     file_path = path.join(tmpdir, "pcap_index_test.pcap")
     pcap.record(in_packets, file_path)
-    reader = _pcap.IndexedPcapReader(file_path, [meta_path], progress_callback)
+    reader = _pcap.IndexedPcapReader(file_path, [meta_path])
+    while reader.next_packet():
+        reader.update_index_for_current_packet()
+    reader.reset()
 
     # the index should contain the number of frames from the file
-    assert reader.frame_count(0) == num_frames
-    assert len(reader.frame_indices[0]) == num_frames
+    assert reader.get_index().frame_count(0) == num_frames
+    assert len(reader.get_index().frame_indices[0]) == num_frames
 
     # make sure that the file offset for a frame in the index corresponds to the offset of the first packet of the frame
     frame_num = 0
     previous_frame_id = None
     while reader.next_packet():
         info = reader.current_info()
         if info.dst_port == sensor_info.udp_port_lidar:
             packet_frame_id = reader.current_frame_id()
             if previous_frame_id is None or packet_frame_id > previous_frame_id:
-                assert reader.frame_indices[0][frame_num] == info.file_offset
+                assert reader.get_index().frame_indices[0][frame_num] == info.file_offset
                 previous_frame_id = packet_frame_id
                 frame_num += 1
 
 
 def test_indexed_pcap_reader_seek(tmpdir):
     """After seeking to the start of a frame, next_packet should return the first packet of that frame"""
-    meta_path = path.join(DATA_DIR, f"{TESTS['dual-2.2']}.json")
+    meta_path = path.join(PCAPS_DATA_DIR, f"{TESTS['dual-2.2']}.json")
 
-    def progress_callback(offset, delta, filesize):
-        pass
     sensor_info = client.SensorInfo(open(meta_path).read())
     packet_format = _client.PacketFormat.from_info(sensor_info)
     num_frames = 10
     packets_per_frame = 3
     in_packets = list(fake_packet_stream_with_frame_id(sensor_info, num_frames,
                       packets_per_frame, 3, lambda frame_num: frame_num))
     assert len(in_packets) > 0
     file_path = path.join(tmpdir, "pcap_index_test.pcap")
     pcap.record(in_packets, file_path)
-    reader = _pcap.IndexedPcapReader(file_path, [meta_path], progress_callback)
+    reader = _pcap.IndexedPcapReader(file_path, [meta_path])
+    while reader.next_packet():
+        reader.update_index_for_current_packet()
+    reader.reset()
 
     for frame in range(num_frames):
-        reader.seek_to_frame(0, frame)
+        reader.get_index().seek_to_frame(reader, 0, frame)
         assert packet_format.lidar_packet_size == reader.next_packet()
-        assert reader.current_info().file_offset == reader.frame_indices[0][frame]
+        assert reader.current_info().file_offset == reader.get_index().frame_indices[0][frame]
         assert reader.current_frame_id() == frame
         assert reader.current_frame_id() == packet_format.frame_id(reader.current_data().tobytes())
 
 
 def test_out_of_order_frames(tmpdir):
     """Frames that are out of order are skipped"""
-    meta_path = path.join(DATA_DIR, f"{TESTS['dual-2.2']}.json")
+    meta_path = path.join(PCAPS_DATA_DIR, f"{TESTS['dual-2.2']}.json")
 
-    def progress_callback(offset, delta, filesize):
-        pass
     sensor_info = client.SensorInfo(open(meta_path).read())
     packet_format = _client.PacketFormat.from_info(sensor_info)
     num_frames = 10
     packets_per_frame = 3
 
     # odd number frames are out of order in this dataset
     # frame ids are 2, 1, 4, 3, 6, ...
     in_packets = list(fake_packet_stream_with_frame_id(sensor_info, num_frames,
                       packets_per_frame, 3, lambda f: f + 1 + (1 - f % 2) - f % 2))
 
     assert len(in_packets) > 0
     file_path = path.join(tmpdir, "pcap_index_test.pcap")
     pcap.record(in_packets, file_path)
-    reader = _pcap.IndexedPcapReader(file_path, [meta_path], progress_callback)
+    reader = _pcap.IndexedPcapReader(file_path, [meta_path])
+    while reader.next_packet():
+        reader.update_index_for_current_packet()
+    reader.reset()
 
     # since odd number frames are out of order, there should be half as many in the index as in the input
-    assert len(reader.frame_indices[0]) == num_frames // 2
+    assert len(reader.get_index().frame_indices[0]) == num_frames // 2
 
-    for frame in range(len(reader.frame_indices[0])):
-        reader.seek_to_frame(0, frame)
+    for frame in range(len(reader.get_index().frame_indices[0])):
+        reader.get_index().seek_to_frame(reader, 0, frame)
         assert packet_format.lidar_packet_size == reader.next_packet()
-        assert reader.current_info().file_offset == reader.frame_indices[0][frame]
+        assert reader.current_info().file_offset == reader.get_index().frame_indices[0][frame]
         assert reader.current_frame_id() == (frame + 1) * 2
         assert reader.current_frame_id() == packet_format.frame_id(reader.current_data().tobytes())
 
 
 def test_current_data(fake_meta, tmpdir):
     """It should provide access to current packet data as a memory view"""
-    meta_path = path.join(DATA_DIR, f"{TESTS['dual-2.2']}.json")
+    meta_path = path.join(PCAPS_DATA_DIR, f"{TESTS['dual-2.2']}.json")
 
-    def progress_callback(offset, delta, filesize):
-        pass
     sensor_info = client.SensorInfo(open(meta_path).read())
     packet_format = _client.PacketFormat.from_info(sensor_info)
     num_frames = 10
     packets_per_frame = 1
 
     # odd number frames are out of order in this dataset
     # frame ids are 2, 1, 4, 3, 6, ...
     in_packets = list(fake_packet_stream_with_frame_id(sensor_info, num_frames,
                       packets_per_frame, 3, lambda f: f + 1 + (1 - f % 2) - f % 2))
 
     assert len(in_packets) > 0
     file_path = path.join(tmpdir, "pcap_index_test.pcap")
     pcap.record(in_packets, file_path)
-    reader = _pcap.IndexedPcapReader(file_path, [meta_path], progress_callback)
+    reader = _pcap.IndexedPcapReader(file_path, [meta_path])
+    while reader.next_packet():
+        reader.update_index_for_current_packet()
+    reader.reset()
+
     frame_ids = []
     while reader.next_packet():
         info = reader.current_info()
         if info.dst_port == sensor_info.udp_port_lidar:
             packet_data = reader.current_data()
             frame_ids.append(packet_format.frame_id(packet_data.tobytes()))
     assert frame_ids == [2, 1, 4, 3, 6, 5, 8, 7, 10, 9]
+
+
+def test_validation():
+    """The Pcap class should accumlate errors detected by LidarPacketValidator"""
+    meta_file_path = path.join(PCAPS_DATA_DIR, 'OS-0-128-U1_v2.3.0_1024x10.json')
+    pcap_file_path = path.join(PCAPS_DATA_DIR, 'OS-0-128-U1_v2.3.0_1024x10.pcap')
+    metadata = client.SensorInfo(open(meta_file_path).read())
+    metadata.init_id = 123
+    metadata.format.udp_profile_lidar = client.UDPProfileLidar.PROFILE_LIDAR_FIVE_WORD_PIXEL
+    reader = pcap.Pcap(pcap_file_path, metadata)
+    consume(reader)
+    assert reader._errors == {
+        client.PacketIdError('Metadata init_id/sn does not match: expected by metadata - \
+123/122150000150, but got from packet buffer - 5431292/122150000150'): 64,
+        client.PacketSizeError('Expected a packet of size 41216 but got a buffer of size 8448'): 64
+    }
```

### Comparing `ouster-sdk-0.8.1/tests/test_viz.py` & `ouster-sdk-0.9.0/tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/tests/test_xyzlut.py` & `ouster-sdk-0.9.0/tests/test_xyzlut.py`

 * *Files identical despite different names*

### Comparing `ouster-sdk-0.8.1/tox.ini` & `ouster-sdk-0.9.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py{37,38,39,310}
+envlist = py{37,38,39,310,311}
 isolated_build = true
 skip_missing_interpreters = true
 
 [testenv]
 extras = test
 allowlist_externals = mkdir
 passenv = ARTIFACT_DIR, ID, VERSION_ID
@@ -12,20 +12,20 @@
     ID = {env:ID:none}
     VERSION_ID = {env:VERSION_ID:none}
 commands =
     pytest tests/ -o junit_suite_name="ouster-sdk-{env:ID}-{env:VERSION_ID}-{envname}" \
            --junit-prefix="{env:ID}__{env:VERSION_ID}__{envname}" \
            --junitxml="{env:ARTIFACT_DIR}/tox-tests/ouster-sdk-{env:ID}-{env:VERSION_ID}-{envname}.xml"
 
-[testenv:py{37,38,39,310}-use_wheels]
+[testenv:py{37,38,39,310,311}-use_wheels]
 description = installs ouster-sdk-python from wheels and runs tests
 passenv = WHEELS_DIR
 skipsdist = true
 skip_install = true
-commands = 
+commands =
     pip install --force-reinstall --upgrade --pre -f {env:WHEELS_DIR} --no-index ouster-sdk[test]
     pytest tests/ -o junit_suite_name="ouster-sdk-{env:ID}-{env:VERSION_ID}-{envname}" \
            --junit-prefix="{env:ID}__{env:VERSION_ID}__{envname}" \
            --junitxml="{env:ARTIFACT_DIR}/tox-tests/ouster-sdk-{env:ID}-{env:VERSION_ID}-{envname}.xml"
 
 [testenv:docs]
 description = generating Ouster SDK documentaion html page (sphinx based)
```

