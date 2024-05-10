# Comparing `tmp/small_gicp-0.0.3.tar.gz` & `tmp/small_gicp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "small_gicp-0.0.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "small_gicp-0.0.6.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `small_gicp-0.0.3.tar` & `small_gicp-0.0.6.tar`

### file list

```diff
@@ -1,127 +1,128 @@
--rw-r--r--   0        0        0     4540 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.clang-format
--rw-r--r--   0        0        0      954 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.github/workflows/build-linux.yml
--rw-r--r--   0        0        0      624 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.github/workflows/build-windows.yml
--rw-r--r--   0        0        0     1576 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1075 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.gitignore
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.pytest_cache/README.md
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 small_gicp-0.0.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     5238 2022-11-09 12:37:21.000000 small_gicp-0.0.3/BENCHMARK.md
--rw-r--r--   0        0        0     9946 2022-11-09 12:37:21.000000 small_gicp-0.0.3/CMakeLists.txt
--rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 small_gicp-0.0.3/LICENSE
--rw-r--r--   0        0        0    20170 2022-11-09 12:37:21.000000 small_gicp-0.0.3/README.md
--rw-r--r--   0        0        0      840 2022-11-09 12:37:21.000000 small_gicp-0.0.3/cmake/FindIridescence.cmake
--rw-r--r--   0        0        0      710 2022-11-09 12:37:21.000000 small_gicp-0.0.3/cmake/small_gicp-config.cmake.in
--rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 small_gicp-0.0.3/codecov.yml
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 small_gicp-0.0.3/data/T_target_source.txt
--rw-r--r--   0        0        0  1116940 2022-11-09 12:37:21.000000 small_gicp-0.0.3/data/source.ply
--rw-r--r--   0        0        0  1105676 2022-11-09 12:37:21.000000 small_gicp-0.0.3/data/target.ply
--rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 small_gicp-0.0.3/docker/Dockerfile.build.gcc
--rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 small_gicp-0.0.3/docker/Dockerfile.build.llvm
--rw-r--r--   0        0        0      818 2022-11-09 12:37:21.000000 small_gicp-0.0.3/docker/Dockerfile.test.gcc
--rw-r--r--   0        0        0     1101 2022-11-09 12:37:21.000000 small_gicp-0.0.3/docker/Dockerfile.test.llvm
--rw-r--r--   0        0        0   217132 2022-11-09 12:37:21.000000 small_gicp-0.0.3/docs/assets/downsampling_comp.png
--rw-r--r--   0        0        0    94855 2022-11-09 12:37:21.000000 small_gicp-0.0.3/docs/assets/downsampling_threads.png
--rw-r--r--   0        0        0   239925 2022-11-09 12:37:21.000000 small_gicp-0.0.3/docs/assets/kdtree_time.png
--rw-r--r--   0        0        0    31849 2022-11-09 12:37:21.000000 small_gicp-0.0.3/docs/assets/odometry_native.png
--rw-r--r--   0        0        0   452009 2022-11-09 12:37:21.000000 small_gicp-0.0.3/docs/assets/odometry_time.png
--rw-r--r--   0        0        0     5590 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/ann/flat_container.hpp
--rw-r--r--   0        0        0     2777 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/ann/gaussian_voxelmap.hpp
--rw-r--r--   0        0        0     9543 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/ann/incremental_voxelmap.hpp
--rw-r--r--   0        0        0     4250 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/ann/kdtree.hpp
--rw-r--r--   0        0        0      940 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/ann/kdtree_omp.hpp
--rw-r--r--   0        0        0      934 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/ann/kdtree_tbb.hpp
--rw-r--r--   0        0        0    73571 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/ann/nanoflann.hpp
--rw-r--r--   0        0        0    25681 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/ann/nanoflann_omp.hpp
--rw-r--r--   0        0        0    25212 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/ann/nanoflann_tbb.hpp
--rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/ann/traits.hpp
--rw-r--r--   0        0        0     4045 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/benchmark/benchmark.hpp
--rw-r--r--   0        0        0     3531 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/benchmark/benchmark_odom.hpp
--rw-r--r--   0        0        0     3635 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/benchmark/read_points.hpp
--rw-r--r--   0        0        0     3229 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/factors/general_factor.hpp
--rw-r--r--   0        0        0     3718 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/factors/gicp_factor.hpp
--rw-r--r--   0        0        0     2390 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/factors/icp_factor.hpp
--rw-r--r--   0        0        0     2808 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/factors/plane_icp_factor.hpp
--rw-r--r--   0        0        0      945 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/pcl/pcl_point.hpp
--rw-r--r--   0        0        0     1756 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/pcl/pcl_point_traits.hpp
--rw-r--r--   0        0        0     1292 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/pcl/pcl_proxy.hpp
--rw-r--r--   0        0        0     5314 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/pcl/pcl_registration.hpp
--rw-r--r--   0        0        0     8664 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/pcl/pcl_registration_impl.hpp
--rw-r--r--   0        0        0      611 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/points/eigen.hpp
--rw-r--r--   0        0        0     3191 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/points/point_cloud.hpp
--rw-r--r--   0        0        0     2269 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/points/traits.hpp
--rw-r--r--   0        0        0     5484 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/registration/optimizer.hpp
--rw-r--r--   0        0        0     2350 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/registration/reduction.hpp
--rw-r--r--   0        0        0     2297 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/registration/reduction_omp.hpp
--rw-r--r--   0        0        0     4169 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/registration/reduction_tbb.hpp
--rw-r--r--   0        0        0     2169 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/registration/registration.hpp
--rw-r--r--   0        0        0     4036 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/registration/registration_helper.hpp
--rw-r--r--   0        0        0      957 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/registration/registration_result.hpp
--rw-r--r--   0        0        0     1013 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/registration/rejector.hpp
--rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/registration/termination_criteria.hpp
--rw-r--r--   0        0        0     4118 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/util/downsampling.hpp
--rw-r--r--   0        0        0     3652 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/util/downsampling_omp.hpp
--rw-r--r--   0        0        0     3516 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/util/downsampling_tbb.hpp
--rw-r--r--   0        0        0      499 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/util/fast_floor.hpp
--rw-r--r--   0        0        0     3357 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/util/lie.hpp
--rw-r--r--   0        0        0     5842 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/util/normal_estimation.hpp
--rw-r--r--   0        0        0     3969 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/util/normal_estimation_omp.hpp
--rw-r--r--   0        0        0     3635 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/util/normal_estimation_tbb.hpp
--rw-r--r--   0        0        0     2456 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/util/sort_omp.hpp
--rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 small_gicp-0.0.3/include/small_gicp/util/vector3i_hash.hpp
--rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 small_gicp-0.0.3/package.xml
--rw-r--r--   0        0        0      980 2022-11-09 12:37:21.000000 small_gicp-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4772 2022-11-09 12:37:21.000000 small_gicp-0.0.3/scripts/plot_downsampling.py
--rw-r--r--   0        0        0     2875 2022-11-09 12:37:21.000000 small_gicp-0.0.3/scripts/plot_kdtree.py
--rw-r--r--   0        0        0     3731 2022-11-09 12:37:21.000000 small_gicp-0.0.3/scripts/plot_odometry.py
--rw-r--r--   0        0        0     2915 2022-11-09 12:37:21.000000 small_gicp-0.0.3/scripts/plot_odometry_accuracy.py
--rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 small_gicp-0.0.3/scripts/plot_odometry_native.py
--rwxr-xr-x   0        0        0      345 2022-11-09 12:37:21.000000 small_gicp-0.0.3/scripts/run_downsampling_benchmark.sh
--rwxr-xr-x   0        0        0      573 2022-11-09 12:37:21.000000 small_gicp-0.0.3/scripts/run_kdtree_benchmark.sh
--rwxr-xr-x   0        0        0      786 2022-11-09 12:37:21.000000 small_gicp-0.0.3/scripts/run_odometry_benchmark.sh
--rwxr-xr-x   0        0        0      698 2022-11-09 12:37:21.000000 small_gicp-0.0.3/scripts/run_odometry_benchmark_native.sh
--rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/downsampling_benchmark.cpp
--rw-r--r--   0        0        0     5472 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/kdtree_benchmark.cpp
--rw-r--r--   0        0        0     3447 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark.cpp
--rw-r--r--   0        0        0     2014 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_fast_gicp.cpp
--rw-r--r--   0        0        0     2172 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_fast_vgicp.cpp
--rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_pcl.cpp
--rw-r--r--   0        0        0     1918 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp.cpp
--rw-r--r--   0        0        0     2597 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp_model_tbb.cpp
--rw-r--r--   0        0        0     2554 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp_omp.cpp
--rw-r--r--   0        0        0     1957 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp_pcl.cpp
--rw-r--r--   0        0        0     2131 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp_tbb.cpp
--rw-r--r--   0        0        0     6645 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp_tbb_flow.cpp
--rw-r--r--   0        0        0     2540 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_vgicp_model_tbb.cpp
--rw-r--r--   0        0        0     2191 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_vgicp_omp.cpp
--rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_vgicp_tbb.cpp
--rw-r--r--   0        0        0     3711 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/example/01_basic_registration.cpp
--rw-r--r--   0        0        0     5331 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/example/02_basic_registration_pcl.cpp
--rw-r--r--   0        0        0    16394 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/example/03_registration_template.cpp
--rwxr-xr-x   0        0        0     7189 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/example/basic_registration.py
--rwxr-xr-x   0        0        0     3550 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/example/kitti_odometry.py
--rw-r--r--   0        0        0     5479 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/python/align.cpp
--rw-r--r--   0        0        0     3323 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/python/factors.cpp
--rw-r--r--   0        0        0     1469 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/python/kdtree.cpp
--rw-r--r--   0        0        0      665 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/python/misc.cpp
--rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/python/pointcloud.cpp
--rw-r--r--   0        0        0     5679 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/python/preprocess.cpp
--rw-r--r--   0        0        0      662 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/python/python.cpp
--rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/python/result.cpp
--rw-r--r--   0        0        0     2844 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/python/voxelmap.cpp
--rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/small_gicp/benchmark/benchmark_odom.cpp
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/small_gicp/registration/registration.cpp
--rw-r--r--   0        0        0     7225 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/small_gicp/registration/registration_helper.cpp
--rw-r--r--   0        0        0     3993 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/test/downsampling_test.cpp
--rw-r--r--   0        0        0     9331 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/test/kdtree_test.cpp
--rw-r--r--   0        0        0    10072 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/test/normal_estimation_test.cpp
--rw-r--r--   0        0        0     2325 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/test/points_test.cpp
--rwxr-xr-x   0        0        0     7468 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/test/python_test.py
--rw-r--r--   0        0        0    14258 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/test/registration_test.cpp
--rw-r--r--   0        0        0     3217 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/test/sort_omp_test.cpp
--rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 small_gicp-0.0.3/src/test/vector_test.cpp
--rw-r--r--   0        0        0    20554 2022-11-09 12:37:21.000000 small_gicp-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4540 2022-11-09 12:37:21.000000 small_gicp-0.0.6/.clang-format
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 small_gicp-0.0.6/.github/workflows/build-linux.yml
+-rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 small_gicp-0.0.6/.github/workflows/build-macos.yml
+-rw-r--r--   0        0        0      617 2022-11-09 12:37:21.000000 small_gicp-0.0.6/.github/workflows/build-windows.yml
+-rw-r--r--   0        0        0     1576 2022-11-09 12:37:21.000000 small_gicp-0.0.6/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1075 2022-11-09 12:37:21.000000 small_gicp-0.0.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1783 2022-11-09 12:37:21.000000 small_gicp-0.0.6/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       84 2022-11-09 12:37:21.000000 small_gicp-0.0.6/.gitignore
+-rw-r--r--   0        0        0     5416 2022-11-09 12:37:21.000000 small_gicp-0.0.6/BENCHMARK.md
+-rw-r--r--   0        0        0     9960 2022-11-09 12:37:21.000000 small_gicp-0.0.6/CMakeLists.txt
+-rw-r--r--   0        0        0     1068 2022-11-09 12:37:21.000000 small_gicp-0.0.6/LICENSE
+-rw-r--r--   0        0        0    21588 2022-11-09 12:37:21.000000 small_gicp-0.0.6/README.md
+-rw-r--r--   0        0        0      840 2022-11-09 12:37:21.000000 small_gicp-0.0.6/cmake/FindIridescence.cmake
+-rw-r--r--   0        0        0      710 2022-11-09 12:37:21.000000 small_gicp-0.0.6/cmake/small_gicp-config.cmake.in
+-rw-r--r--   0        0        0      137 2022-11-09 12:37:21.000000 small_gicp-0.0.6/codecov.yml
+-rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 small_gicp-0.0.6/data/T_target_source.txt
+-rw-r--r--   0        0        0  1116940 2022-11-09 12:37:21.000000 small_gicp-0.0.6/data/source.ply
+-rw-r--r--   0        0        0  1105676 2022-11-09 12:37:21.000000 small_gicp-0.0.6/data/target.ply
+-rw-r--r--   0        0        0      643 2022-11-09 12:37:21.000000 small_gicp-0.0.6/docker/Dockerfile.pytest.gcc
+-rw-r--r--   0        0        0      871 2022-11-09 12:37:21.000000 small_gicp-0.0.6/docker/Dockerfile.pytest.llvm
+-rw-r--r--   0        0        0   217132 2022-11-09 12:37:21.000000 small_gicp-0.0.6/docs/assets/downsampling_comp.png
+-rw-r--r--   0        0        0    94855 2022-11-09 12:37:21.000000 small_gicp-0.0.6/docs/assets/downsampling_threads.png
+-rw-r--r--   0        0        0   189313 2022-11-09 12:37:21.000000 small_gicp-0.0.6/docs/assets/kdtree_time.png
+-rw-r--r--   0        0        0    31849 2022-11-09 12:37:21.000000 small_gicp-0.0.6/docs/assets/odometry_native.png
+-rw-r--r--   0        0        0   452009 2022-11-09 12:37:21.000000 small_gicp-0.0.6/docs/assets/odometry_time.png
+-rw-r--r--   0        0        0     4250 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/deprecated/kdtree.hpp
+-rw-r--r--   0        0        0      940 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/deprecated/kdtree_omp.hpp
+-rw-r--r--   0        0        0      934 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/deprecated/kdtree_tbb.hpp
+-rw-r--r--   0        0        0    73571 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/deprecated/nanoflann.hpp
+-rw-r--r--   0        0        0    25681 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/deprecated/nanoflann_omp.hpp
+-rw-r--r--   0        0        0    25212 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/deprecated/nanoflann_tbb.hpp
+-rw-r--r--   0        0        0     5590 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/flat_container.hpp
+-rw-r--r--   0        0        0     2777 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/gaussian_voxelmap.hpp
+-rw-r--r--   0        0        0     9543 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/incremental_voxelmap.hpp
+-rw-r--r--   0        0        0    13006 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/kdtree.hpp
+-rw-r--r--   0        0        0     3838 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/kdtree_omp.hpp
+-rw-r--r--   0        0        0     3095 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/kdtree_tbb.hpp
+-rw-r--r--   0        0        0     3091 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/knn_result.hpp
+-rw-r--r--   0        0        0     3865 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/projection.hpp
+-rw-r--r--   0        0        0     2362 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/ann/traits.hpp
+-rw-r--r--   0        0        0     4045 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/benchmark/benchmark.hpp
+-rw-r--r--   0        0        0     3531 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/benchmark/benchmark_odom.hpp
+-rw-r--r--   0        0        0     3635 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/benchmark/read_points.hpp
+-rw-r--r--   0        0        0     3231 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/factors/general_factor.hpp
+-rw-r--r--   0        0        0     3720 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/factors/gicp_factor.hpp
+-rw-r--r--   0        0        0     2390 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/factors/icp_factor.hpp
+-rw-r--r--   0        0        0     2808 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/factors/plane_icp_factor.hpp
+-rw-r--r--   0        0        0      945 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/pcl/pcl_point.hpp
+-rw-r--r--   0        0        0     1756 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/pcl/pcl_point_traits.hpp
+-rw-r--r--   0        0        0     1292 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/pcl/pcl_proxy.hpp
+-rw-r--r--   0        0        0     5308 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/pcl/pcl_registration.hpp
+-rw-r--r--   0        0        0     8694 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/pcl/pcl_registration_impl.hpp
+-rw-r--r--   0        0        0      611 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/points/eigen.hpp
+-rw-r--r--   0        0        0     3191 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/points/point_cloud.hpp
+-rw-r--r--   0        0        0     2269 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/points/traits.hpp
+-rw-r--r--   0        0        0     5484 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/registration/optimizer.hpp
+-rw-r--r--   0        0        0     2352 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/registration/reduction.hpp
+-rw-r--r--   0        0        0     2297 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/registration/reduction_omp.hpp
+-rw-r--r--   0        0        0     4169 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/registration/reduction_tbb.hpp
+-rw-r--r--   0        0        0     2169 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/registration/registration.hpp
+-rw-r--r--   0        0        0     4036 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/registration/registration_helper.hpp
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/registration/registration_result.hpp
+-rw-r--r--   0        0        0     1013 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/registration/rejector.hpp
+-rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/registration/termination_criteria.hpp
+-rw-r--r--   0        0        0     4118 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/util/downsampling.hpp
+-rw-r--r--   0        0        0     3652 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/util/downsampling_omp.hpp
+-rw-r--r--   0        0        0     3516 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/util/downsampling_tbb.hpp
+-rw-r--r--   0        0        0      499 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/util/fast_floor.hpp
+-rw-r--r--   0        0        0     3357 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/util/lie.hpp
+-rw-r--r--   0        0        0     5842 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/util/normal_estimation.hpp
+-rw-r--r--   0        0        0     3969 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/util/normal_estimation_omp.hpp
+-rw-r--r--   0        0        0     3635 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/util/normal_estimation_tbb.hpp
+-rw-r--r--   0        0        0     2806 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/util/sort_omp.hpp
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 small_gicp-0.0.6/include/small_gicp/util/vector3i_hash.hpp
+-rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 small_gicp-0.0.6/package.xml
+-rw-r--r--   0        0        0     1444 2022-11-09 12:37:21.000000 small_gicp-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4772 2022-11-09 12:37:21.000000 small_gicp-0.0.6/scripts/plot_downsampling.py
+-rw-r--r--   0        0        0     2891 2022-11-09 12:37:21.000000 small_gicp-0.0.6/scripts/plot_kdtree.py
+-rw-r--r--   0        0        0     3731 2022-11-09 12:37:21.000000 small_gicp-0.0.6/scripts/plot_odometry.py
+-rw-r--r--   0        0        0     2915 2022-11-09 12:37:21.000000 small_gicp-0.0.6/scripts/plot_odometry_accuracy.py
+-rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 small_gicp-0.0.6/scripts/plot_odometry_native.py
+-rwxr-xr-x   0        0        0      345 2022-11-09 12:37:21.000000 small_gicp-0.0.6/scripts/run_downsampling_benchmark.sh
+-rwxr-xr-x   0        0        0      576 2022-11-09 12:37:21.000000 small_gicp-0.0.6/scripts/run_kdtree_benchmark.sh
+-rwxr-xr-x   0        0        0      786 2022-11-09 12:37:21.000000 small_gicp-0.0.6/scripts/run_odometry_benchmark.sh
+-rwxr-xr-x   0        0        0      698 2022-11-09 12:37:21.000000 small_gicp-0.0.6/scripts/run_odometry_benchmark_native.sh
+-rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/downsampling_benchmark.cpp
+-rw-r--r--   0        0        0     5536 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/kdtree_benchmark.cpp
+-rw-r--r--   0        0        0     3447 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark.cpp
+-rw-r--r--   0        0        0     2014 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_fast_gicp.cpp
+-rw-r--r--   0        0        0     2172 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_fast_vgicp.cpp
+-rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_pcl.cpp
+-rw-r--r--   0        0        0     1918 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp.cpp
+-rw-r--r--   0        0        0     2597 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp_model_tbb.cpp
+-rw-r--r--   0        0        0     2563 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp_omp.cpp
+-rw-r--r--   0        0        0     1957 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp_pcl.cpp
+-rw-r--r--   0        0        0     2145 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp_tbb.cpp
+-rw-r--r--   0        0        0     6645 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp_tbb_flow.cpp
+-rw-r--r--   0        0        0     2540 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_vgicp_model_tbb.cpp
+-rw-r--r--   0        0        0     2206 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_vgicp_omp.cpp
+-rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_vgicp_tbb.cpp
+-rw-r--r--   0        0        0     3711 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/example/01_basic_registration.cpp
+-rw-r--r--   0        0        0     5361 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/example/02_basic_registration_pcl.cpp
+-rw-r--r--   0        0        0    16426 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/example/03_registration_template.cpp
+-rwxr-xr-x   0        0        0     7189 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/example/basic_registration.py
+-rwxr-xr-x   0        0        0     3550 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/example/kitti_odometry.py
+-rw-r--r--   0        0        0     8924 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/python/align.cpp
+-rw-r--r--   0        0        0     3314 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/python/factors.cpp
+-rw-r--r--   0        0        0     1592 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/python/kdtree.cpp
+-rw-r--r--   0        0        0      665 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/python/misc.cpp
+-rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/python/pointcloud.cpp
+-rw-r--r--   0        0        0     5739 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/python/preprocess.cpp
+-rw-r--r--   0        0        0      662 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/python/python.cpp
+-rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/python/result.cpp
+-rw-r--r--   0        0        0     2844 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/python/voxelmap.cpp
+-rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/small_gicp/benchmark/benchmark_odom.cpp
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/small_gicp/registration/registration.cpp
+-rw-r--r--   0        0        0     7225 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/small_gicp/registration/registration_helper.cpp
+-rw-r--r--   0        0        0     5632 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/test/downsampling_test.cpp
+-rw-r--r--   0        0        0     5493 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/test/helper_test.cpp
+-rw-r--r--   0        0        0    10513 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/test/kdtree_synthetic_test.cpp
+-rw-r--r--   0        0        0     9395 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/test/kdtree_test.cpp
+-rw-r--r--   0        0        0    10066 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/test/normal_estimation_test.cpp
+-rw-r--r--   0        0        0     2325 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/test/points_test.cpp
+-rwxr-xr-x   0        0        0     7468 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/test/python_test.py
+-rw-r--r--   0        0        0    14258 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/test/registration_test.cpp
+-rw-r--r--   0        0        0     3217 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/test/sort_omp_test.cpp
+-rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 small_gicp-0.0.6/src/test/vector_test.cpp
+-rw-r--r--   0        0        0    21907 2022-11-09 12:37:21.000000 small_gicp-0.0.6/PKG-INFO
```

### Comparing `small_gicp-0.0.3/.clang-format` & `small_gicp-0.0.6/.clang-format`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/.github/workflows/build-linux.yml` & `small_gicp-0.0.6/.github/workflows/build-linux.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Build(Linux)
+name: linux
 
 on:
   push:
     branches: [ master ]
     paths-ignore: '**.md'
   pull_request:
     branches: [ master ]
@@ -30,11 +30,11 @@
         with:
           username: ${{ secrets.DOCKER_USERNAME }}
           password: ${{ secrets.DOCKER_TOKEN }}
 
       - name: Docker build
         uses: docker/build-push-action@v2
         with:
-          file: ${{github.workspace}}/docker/Dockerfile.build.${{ matrix.TOOLCHAIN }}
+          file: ${{github.workspace}}/docker/Dockerfile.pytest.${{ matrix.TOOLCHAIN }}
           build-args: BASE_IMAGE=ubuntu:${{ matrix.DISTRO }}
           context: .
           push: false
```

### Comparing `small_gicp-0.0.3/.github/workflows/build-windows.yml` & `small_gicp-0.0.6/.github/workflows/build-windows.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Build(Windows)
+name: windows
 
 on:
   push:
     branches: [ master ]
     paths-ignore: '**.md'
   pull_request:
     branches: [ master ]
```

### Comparing `small_gicp-0.0.3/.github/workflows/coverage.yml` & `small_gicp-0.0.6/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/.github/workflows/test.yml` & `small_gicp-0.0.6/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Test
+name: test
 
 on:
   push:
     branches: [ master ]
     paths-ignore: '**.md'
   pull_request:
     branches: [ master ]
```

### Comparing `small_gicp-0.0.3/BENCHMARK.md` & `small_gicp-0.0.6/BENCHMARK.md`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 All benchmarks were conducted on the KITTI 00 sequence.
 
 ### Downsampling
 
 ```bash
 cd small_gicp/scripts
-./run_downsampling_benchmark.sh
+./run_downsampling_benchmark.sh /path/to/kitti/velodyne
 python3 plot_downsampling.py
 ```
 
 - Single-threaded `small_gicp::voxelgrid_sampling` is about **1.3x faster** than `pcl::VoxelGrid`.
 - Multi-threaded `small_gicp::voxelgrid_sampling_tbb` (6 threads) is about **3.2x faster** than `pcl::VoxelGrid`.
 - `small_gicp::voxelgrid_sampling` gives accurate downsampling results (almost identical to those of `pcl::VoxelGrid`) while `pcl::ApproximateVoxelGrid` yields spurious points (up to 2x points).
 - `small_gicp::voxelgrid_sampling` can process a larger point cloud with a fine voxel resolution compared to `pcl::VoxelGrid` (for a point cloud of 1000m width, minimum voxel resolution can be 0.5 mm).
@@ -63,29 +63,30 @@
 
 ![downsampling_threads](docs/assets/downsampling_threads.png)
 
 ### KdTree construction
 
 ```bash
 cd small_gicp/scripts
-./run_kdtree_benchmark.sh
+./run_kdtree_benchmark.sh /path/to/kitti/velodyne
 python3 plot_kdtree.py
 ```
 
 - Multi-threaded implementation (TBB and OMP) can be up to **4x faster** than the single-threaded one (All the implementations are based on nanoflann).
-- The processing speed gets faster as the number of threads increases, but the speed gain is not monotonic sometimes (because of the scheduling algorithm or some CPU(AMD 5995WX)-specific issues?).
+- ~~The processing speed gets faster as the number of threads increases, but the speed gain is not monotonic sometimes (because of the scheduling algorithm or some CPU(AMD 5995WX)-specific issues?)~~.
+- The new KdTree implementation shows a good scalability thanks to its well balanced task assignment.
 - This benchmark only compares the construction time (query time is not included). 
 
 ![kdtree_time](docs/assets/kdtree_time.png)
 
 ### Odometry estimation
 
 ```bash
 cd small_gicp/scripts
-./run_odometry_benchmark.sh
+./run_odometry_benchmark.sh /path/to/kitti/velodyne
 python3 plot_odometry.py
 ```
 
 - Single-thread `small_gicp::GICP` is about **2.4x and 1.9x faster** than `pcl::GICP` and `fast_gicp::GICP`, respectively.
 - `small_gicp::(GICP|VGICP)` shows a better multi-thread scalability compared to `fast_gicp::(GICP|VGICP)`.
 - `small_gicp::GICP` parallelized with [TBB flow graph](src/odometry_benchmark_small_gicp_tbb_flow.cpp) shows an excellent scalability to many-threads situations (**~128 threads**) but with latency degradation.
```

### Comparing `small_gicp-0.0.3/CMakeLists.txt` & `small_gicp-0.0.6/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.16)
-project(small_gicp VERSION 0.0.3 LANGUAGES C CXX)
+project(small_gicp VERSION 0.0.6 LANGUAGES C CXX)
 
 set(CMAKE_CXX_STANDARD 17)
 list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/cmake")
 
 if(NOT CMAKE_BUILD_TYPE AND NOT CMAKE_CONFIGURATION_TYPES)
   set(CMAKE_BUILD_TYPE "Release" CACHE STRING "Choose the type of build." FORCE)
   set_property(CACHE CMAKE_BUILD_TYPE PROPERTY STRINGS "Debug" "Release" "MinSizeRel" "RelWithDebInfo")
@@ -36,26 +36,26 @@
 if(BUILD_TESTS OR BUILD_EXAMPLES)
   set(BUILD_HELPER ON CACHE BOOL "Helper library is required" FORCE)
   set(BUILD_WITH_TBB ON CACHE BOOL "TBB is required" FORCE)
   set(BUILD_WITH_PCL ON CACHE BOOL "PCL is required" FORCE)
 endif()
 
 # Eigen is the sole mandatory dependency
-find_package(Eigen3)
+find_package(Eigen3 CONFIG)
 
-if(NOT EIGEN3_FOUND)
-  message(STATUS "System Eigen not found. Download Eigen 3.3.9.")
+if(NOT Eigen3_FOUND)
+  message(STATUS "System Eigen not found. Download Eigen 3.4.0.")
   include(FetchContent)
   FetchContent_Populate(
     Eigen3
-    URL https://gitlab.com/libeigen/eigen/-/archive/3.3.9/eigen-3.3.9.tar.gz
+    URL https://gitlab.com/libeigen/eigen/-/archive/3.4.0/eigen-3.4.0.tar.gz
   )
   add_library(Eigen3::Eigen INTERFACE IMPORTED GLOBAL)
   set_target_properties(Eigen3::Eigen PROPERTIES
-    INTERFACE_INCLUDE_DIRECTORIES "${CMAKE_BINARY_DIR}/Eigen3-src"
+    INTERFACE_INCLUDE_DIRECTORIES "${eigen3_SOURCE_DIR}"
   )
 endif()
 
 if(BUILD_WITH_OPENMP STREQUAL "auto")
   find_package(OpenMP)
   set(BUILD_WITH_OPENMP ${OpenMP_FOUND})
 elseif(BUILD_WITH_OPENMP)
@@ -93,15 +93,15 @@
 
 if(BUILD_WITH_MARCH_NATIVE)
   add_compile_options(-march=native)
 endif()
 
 if(MSVC)
   add_compile_definitions(_USE_MATH_DEFINES)
-  add_compile_options(/openmp:llvm)
+  # add_compile_options(/openmp:llvm)
 endif()
 
 ##############
 ## Coverage ##
 ##############
 if(ENABLE_COVERAGE)
   # https://danielsieger.com/blog/2022/03/06/code-coverage-for-cpp.html
@@ -137,15 +137,15 @@
     Eigen3::Eigen
     $<TARGET_NAME_IF_EXISTS:OpenMP::OpenMP_CXX>
   )
 endif()
 
 # Python bindings
 if(BUILD_PYTHON_BINDINGS)
-  find_package(Python COMPONENTS Interpreter Development REQUIRED)
+  find_package(Python COMPONENTS Interpreter Development)
   find_package(pybind11 CONFIG REQUIRED)
 
   pybind11_add_module(small_gicp_python
     src/small_gicp/registration/registration.cpp
     src/small_gicp/registration/registration_helper.cpp
 
     src/python/pointcloud.cpp
@@ -263,21 +263,21 @@
     target_link_libraries(${TEST_NAME} PRIVATE
       small_gicp
       fmt::fmt
       GTest::gtest_main
       TBB::tbb
       TBB::tbbmalloc
       PCL::PCL
+      OpenMP::OpenMP_CXX
     )
 
     gtest_discover_tests(${TEST_NAME} WORKING_DIRECTORY ${CMAKE_SOURCE_DIR})
   endforeach()
 endif()
 
-
 #############
 ## Install ##
 #############
 
 include(GNUInstallDirs)
 install(DIRECTORY include/ DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
```

### Comparing `small_gicp-0.0.3/LICENSE` & `small_gicp-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/README.md` & `small_gicp-0.0.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # small_gicp (fast_gicp2)
 
 **small_gicp** is a header-only C++ library that offers efficient and parallelized algorithms for fine point cloud registration (ICP, Point-to-Plane ICP, GICP, VGICP, etc.). It is a refined and optimized version of its predecessor, [fast_gicp](https://github.com/SMRT-AIST/fast_gicp), re-written from scratch with the following features.
 
-- **Highly Optimized** : The implementation of the core registration algorithm is further optimized from that in fast_gicp. It enables up to **2x speed gain** compared to fast_gicp.
-- **All parallerized** : small_gicp offers parallelized implementations of several preprocessing algorithms to make the entire registration process parallelized (Downsampling, KdTree construction, Normal/covariance estimation). As a parallelism backend, either (or both) [OpenMP](https://www.openmp.org/) and [Intel TBB](https://github.com/oneapi-src/oneTBB) can be used. 
-- **Minimum dependency** : Only [Eigen](https://eigen.tuxfamily.org/) (and bundled [nanoflann](https://github.com/jlblancoc/nanoflann) and [Sophus](https://github.com/strasdat/Sophus)) are required at a minimum. Optionally, it provides the [PCL](https://pointclouds.org/) registration interface so that it can be used as a drop-in replacement in many systems.
+- **Highly Optimized** : The implementation of the core registration algorithm is further optimized from that in fast_gicp. It enables up to **2x speed gain**.
+- **All parallerized** : small_gicp offers parallel implementations of several preprocessing algorithms to make the entire registration process parallelized (Downsampling, KdTree construction, Normal/covariance estimation). As a parallelism backend, either (or both) [OpenMP](https://www.openmp.org/) and [Intel TBB](https://github.com/oneapi-src/oneTBB) can be used. 
+- **Minimum dependency** : Only [Eigen](https://eigen.tuxfamily.org/) (and bundled [nanoflann](https://github.com/jlblancoc/nanoflann) and [Sophus](https://github.com/strasdat/Sophus)) are required at a minimum. Optionally, it provides the [PCL](https://pointclouds.org/) registration interface so that it can be used as a drop-in replacement.
 - **Customizable** : small_gicp allows feeding any custom point cloud class to the registration algorithm via traits. Furthermore, the template-based implementation enables customizing the registration process with your original correspondence estimator and registration factors.
-- **Python bindings** : The isolation from PCL makes small_gicp's python bindings more portable and connectable to other libraries (e.g., Open3D) without problems. 
+- **Python bindings** : The isolation from PCL makes small_gicp's python bindings more portable and usable with other libraries (e.g., Open3D) without problems. 
 
 Note that GPU-based implementations are NOT included in this package.
 
 If you find this package useful for your project, please consider leaving a comment [here](https://github.com/koide3/small_gicp/issues/3). It would help the author receive recognition in his organization and keep working on this project.
 
 
-[![Build(Linux)](https://github.com/koide3/small_gicp/actions/workflows/build-linux.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/build-linux.yml) [![Build(Windows)](https://github.com/koide3/small_gicp/actions/workflows/build-windows.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/build-windows.yml) [![Test](https://github.com/koide3/small_gicp/actions/workflows/test.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/koide3/small_gicp/graph/badge.svg?token=PCVIUP2Z33)](https://codecov.io/gh/koide3/small_gicp)
+[![Build(Linux)](https://github.com/koide3/small_gicp/actions/workflows/build-linux.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/build-linux.yml) [![macos](https://github.com/koide3/small_gicp/actions/workflows/build-macos.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/build-macos.yml) [![Build(Windows)](https://github.com/koide3/small_gicp/actions/workflows/build-windows.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/build-windows.yml) [![Test](https://github.com/koide3/small_gicp/actions/workflows/test.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/koide3/small_gicp/graph/badge.svg?token=PCVIUP2Z33)](https://codecov.io/gh/koide3/small_gicp)
 
 ## Requirements
 
 This library uses some C++17 features. The PCL interface is not compatible with PCL older than 1.11 that uses `boost::shared_ptr`.
 
 ## Dependencies
 
-- [Mandatory] [Eigen](https://eigen.tuxfamily.org/), [nanoflann](https://github.com/jlblancoc/nanoflann) ([bundled1](include/small_gicp/ann/nanoflann.hpp), [bundled2](include/small_gicp/ann/nanoflann_omp.hpp), [bundled3](include/small_gicp/ann/nanoflann_tbb.hpp)), [Sophus](https://github.com/strasdat/Sophus) ([bundled](include/small_gicp/util/lie.hpp))
-- [Optional] [OpenMP](https://www.openmp.org/), [Intel TBB](https://www.intel.com/content/www/us/en/developer/tools/oneapi/onetbb.html), [PCL](https://pointclouds.org/), [Iridescence](https://github.com/koide3/iridescence)
+- [Mandatory] [Eigen](https://eigen.tuxfamily.org/), [nanoflann](https://github.com/jlblancoc/nanoflann) ([bundled](include/small_gicp/ann/kdtree.hpp)), [Sophus](https://github.com/strasdat/Sophus) ([bundled](include/small_gicp/util/lie.hpp))
+- [Optional] [OpenMP](https://www.openmp.org/), [Intel TBB](https://www.intel.com/content/www/us/en/developer/tools/oneapi/onetbb.html), [PCL](https://pointclouds.org/)
 
 ## Installation
 
 ### C++
 
 small_gicp is a header-only library. You can just download and drop it in your project directory to use it.
 
@@ -167,16 +167,16 @@
 // Estimate covariances of points.
 const int num_threads = 4;
 const int num_neighbors = 20;
 estimate_covariances_omp(*target, num_neighbors, num_threads);
 estimate_covariances_omp(*source, num_neighbors, num_threads);
 
 // Create KdTree for target and source.
-auto target_tree = std::make_shared<KdTreeOMP<pcl::PointCloud<pcl::PointCovariance>>>(target, num_threads);
-auto source_tree = std::make_shared<KdTreeOMP<pcl::PointCloud<pcl::PointCovariance>>>(source, num_threads);
+auto target_tree = std::make_shared<KdTree<pcl::PointCloud<pcl::PointCovariance>>>(target, KdTreeBuilderOMP(num_threads));
+auto source_tree = std::make_shared<KdTree<pcl::PointCloud<pcl::PointCovariance>>>(source, KdTreeBuilderOMP(num_threads));
 
 Registration<GICPFactor, ParallelReductionOMP> registration;
 registration.reduction.num_threads = num_threads;
 registration.rejector.max_dist_sq = 1.0;
 
 // Align point clouds. Note that the input point clouds are pcl::PointCloud<pcl::PointCovariance>.
 auto result = registration.align(*target, *source, *target_tree, Eigen::Isometry3d::Identity());
@@ -210,16 +210,16 @@
 auto source = std::make_shared<PointCloud>(source_points);
 
 // Downsampling
 target = voxelgrid_sampling_omp(*target, downsampling_resolution, num_threads);
 source = voxelgrid_sampling_omp(*source, downsampling_resolution, num_threads);
 
 // Create KdTree
-auto target_tree = std::make_shared<KdTreeOMP<PointCloud>>(target, num_threads);
-auto source_tree = std::make_shared<KdTreeOMP<PointCloud>>(source, num_threads);
+auto target_tree = std::make_shared<KdTree<PointCloud>>(target, KdTreeBuilderOMP(num_threads));
+auto source_tree = std::make_shared<KdTree<PointCloud>>(source, KdTreeBuilderOMP(num_threads));
 
 // Estimate point covariances
 estimate_covariances_omp(*target, *target_tree, num_neighbors, num_threads);
 estimate_covariances_omp(*source, *source_tree, num_neighbors, num_threads);
 
 // GICP + OMP-based parallel reduction
 Registration<GICPFactor, ParallelReductionOMP> registration;
@@ -249,63 +249,104 @@
 ## Usage (Python) [basic_registration.py](src/example/basic_registration.py)
 
 <details><summary>Expand</summary>
 
 Example A : Perform registration with numpy arrays
 
 ```python
-# Arguments
-# - target_points               : Nx4 or Nx3 numpy array of the target point cloud
-# - source_points               : Nx4 or Nx3 numpy array of the source point cloud
-# Optional arguments
-# - init_T_target_source        : Initial guess of the transformation matrix (4x4 numpy array)
-# - registration_type           : Registration type ("ICP", "PLANE_ICP", "GICP", "VGICP")
-# - voxel_resolution            : Voxel resolution for VGICP
-# - downsampling_resolution     : Downsampling resolution
-# - max_correspondence_distance : Maximum correspondence distance
-# - num_threads                 : Number of threads
+# Align two point clouds using various ICP-like algorithms.
+# 
+# Parameters
+# ----------
+# target_points : NDArray[np.float64]
+#     Nx3 or Nx4 matrix representing the target point cloud.
+# source_points : NDArray[np.float64]
+#     Nx3 or Nx4 matrix representing the source point cloud.
+# init_T_target_source : np.ndarray[np.float64]
+#     4x4 matrix representing the initial transformation from target to source.
+# registration_type : str = 'GICP'
+#     Type of registration algorithm to use ('ICP', 'PLANE_ICP', 'GICP', 'VGICP').
+# voxel_resolution : float = 1.0
+#     Resolution of voxels used for downsampling.
+# downsampling_resolution : float = 0.25
+#     Resolution for downsampling the point clouds.
+# max_correspondence_distance : float = 1.0
+#     Maximum distance for matching points between point clouds.
+# num_threads : int = 1
+#     Number of threads to use for parallel processing.
+# 
+# Returns
+# -------
+# RegistrationResult
+#     Object containing the final transformation matrix and convergence status.
 result = small_gicp.align(target_raw_numpy, source_raw_numpy, downsampling_resolution=0.25)
 
 result.T_target_source  # Estimated transformation (4x4 numpy array)
 result.converged        # If true, the optimization converged successfully
 result.iterations       # Number of iterations the optimization took
 result.num_inliers      # Number of inlier points
 result.H                # Final Hessian matrix (6x6 matrix)
 result.b                # Final information vector (6D vector)
 result.e                # Final error (float)
 ```
 
 Example B : Perform preprocessing and registration separately
 
 ```python
-# Preprocess point clouds
-# Arguments
-# - points                      : Nx4 or Nx3 numpy array of the target point cloud
-# Optional arguments
-# - downsampling_resolution     : Downsampling resolution
-# - num_neighbors               : Number of neighbors for normal and covariance estimation
-# - num_threads                 : Number of threads
+# Preprocess point cloud (downsampling, kdtree construction, and normal/covariance estimation)
+#
+# Parameters
+# ----------
+# points : NDArray[np.float64]
+#     Nx3 or Nx4 matrix representing the point cloud.
+# downsampling_resolution : float = 0.1
+#     Resolution for downsampling the point clouds.
+# num_neighbors : int = 20
+#     Number of neighbor points to usefor point normal/covariance estimation.
+# num_threads : int = 1
+#     Number of threads to use for parallel processing.
+# 
+# Returns
+# -------
+# PointCloud
+#     Downsampled point cloud with estimated normals and covariances.
+# KdTree
+#     KdTree for the downsampled point cloud
 target, target_tree = small_gicp.preprocess_points(target_raw_numpy, downsampling_resolution=0.25)
 source, source_tree = small_gicp.preprocess_points(source_raw_numpy, downsampling_resolution=0.25)
 
 # `target` and `source` are small_gicp.PointCloud with the following methods
 target.size()           # Number of points
 target.points()         # Nx4 numpy array   [x, y, z, 1] x N
 target.normals()        # Nx4 numpy array   [nx, ny, nz, 0] x N
 target.covs()           # Array of 4x4 covariance matrices
 
-# Align point clouds
-# Arguments
-# - target                      : Target point cloud (small_gicp.PointCloud)
-# - source                      : Source point cloud (small_gicp.PointCloud)
-# - target_tree                 : KD-tree of the target point cloud (small_gicp.KdTree)
-# Optional arguments
-# - init_T_target_source        : Initial guess of the transformation matrix (4x4 numpy array)
-# - max_correspondence_distance : Maximum correspondence distance
-# - num_threads                 : Number of threads
+#  Align two point clouds using specified ICP-like algorithms, utilizing point cloud and KD-tree inputs.
+#
+#  Parameters
+#  ----------
+#  target : PointCloud::ConstPtr
+#      Pointer to the target point cloud.
+#  source : PointCloud::ConstPtr
+#      Pointer to the source point cloud.
+#  target_tree : KdTree<PointCloud>::ConstPtr, optional
+#      Pointer to the KD-tree of the target for nearest neighbor search. If nullptr, a new tree is built.
+#  init_T_target_source : NDArray[np.float64]
+#      4x4 matrix representing the initial transformation from target to source.
+#  registration_type : str = 'GICP'
+#      Type of registration algorithm to use ('ICP', 'PLANE_ICP', 'GICP').
+#  max_correspondence_distance : float = 1.0
+#      Maximum distance for corresponding point pairs.
+#  num_threads : int = 1
+#      Number of threads to use for computation.
+# 
+#  Returns
+#  -------
+#  RegistrationResult
+#      Object containing the final transformation matrix and convergence status.
 result = small_gicp.align(target, source, target_tree)
 ```
 
 Example C : Perform each of preprocessing steps one-by-one
 
 ```python
 # Convert numpy arrays (Nx3 or Nx4) to small_gicp.PointCloud
@@ -330,24 +371,29 @@
 
 Example D: Example with Open3D
 
 ```python
 target_o3d = open3d.io.read_point_cloud('small_gicp/data/target.ply').paint_uniform_color([0, 1, 0])
 source_o3d = open3d.io.read_point_cloud('small_gicp/data/source.ply').paint_uniform_color([0, 0, 1])
 
-target, target_tree = small_gicp.preprocess_points(points_numpy=numpy.asarray(target_o3d.points), downsampling_resolution=0.25)
-source, source_tree = small_gicp.preprocess_points(points_numpy=numpy.asarray(source_o3d.points), downsampling_resolution=0.25)
+target, target_tree = small_gicp.preprocess_points(numpy.asarray(target_o3d.points), downsampling_resolution=0.25)
+source, source_tree = small_gicp.preprocess_points(numpy.asarray(source_o3d.points), downsampling_resolution=0.25)
 result = small_gicp.align(target, source, target_tree)
 
 source_o3d.transform(result.T_target_source)
 open3d.visualization.draw_geometries([target_o3d, source_o3d])
 ```
 
 </details>
 
+
+### Cookbook
+
+- [Scan-to-scan and scan-to-model GICP matching odometry on KITTI](src/example/kitti_odometry.py)
+
 ## [Benchmark](BENCHMARK.md)
 
 Processing speed comparison between small_gicp and Open3D ([youtube]((https://youtu.be/LNESzGXPr4c?feature=shared))).
 [![small_comp](https://github.com/koide3/small_gicp/assets/31344317/7959edd6-f0e4-4318-b4c1-a3f8755c407f)](https://youtu.be/LNESzGXPr4c?feature=shared)
 
 ### Downsampling
 
@@ -356,16 +402,17 @@
 - `small_gicp::voxelgrid_sampling` gives accurate downsampling results (almost identical to those of `pcl::VoxelGrid`) while `pcl::ApproximateVoxelGrid` yields spurious points (up to 2x points).
 - `small_gicp::voxelgrid_sampling` can process a larger point cloud with a fine voxel resolution compared to `pcl::VoxelGrid` (for a point cloud of 1000m width, the minimum voxel resolution can be **0.5 mm**).
 
 ![downsampling_comp](docs/assets/downsampling_comp.png)
 
 ### KdTree construction
 
-- Multi-threaded implementation (TBB and OMP) can be up to **4x faster** than the single-threaded one (All the implementations are based on nanoflann).
-- The processing speed gets faster as the number of threads increases, but the speed gain is not monotonic sometimes (because of the scheduling algorithm or some CPU(AMD 5995WX)-specific issues?).
+- Multi-threaded implementation (TBB and OMP) can be up to **6x faster** than the single-threaded one. The single-thread version shows almost equivalent performance with nanoflann.
+- ~~The processing speed gets faster as the number of threads increases, but the speed gain is not monotonic sometimes (because of the scheduling algorithm or some CPU(AMD 5995WX)-specific issues?)~~.
+- The new KdTree implementation shows a good scalability thanks to its well balanced task assignment.
 - This benchmark only compares the construction time (query time is not included). 
 
 ![kdtree_time](docs/assets/kdtree_time.png)
 
 ### Odometry estimation
 
 - Single-thread `small_gicp::GICP` is about **2.4x and 1.9x faster** than `pcl::GICP` and `fast_gicp::GICP`, respectively.
```

### Comparing `small_gicp-0.0.3/cmake/FindIridescence.cmake` & `small_gicp-0.0.6/cmake/FindIridescence.cmake`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/cmake/small_gicp-config.cmake.in` & `small_gicp-0.0.6/cmake/small_gicp-config.cmake.in`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/data/source.ply` & `small_gicp-0.0.6/data/source.ply`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/data/target.ply` & `small_gicp-0.0.6/data/target.ply`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/docs/assets/downsampling_comp.png` & `small_gicp-0.0.6/docs/assets/downsampling_comp.png`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/docs/assets/downsampling_threads.png` & `small_gicp-0.0.6/docs/assets/downsampling_threads.png`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/docs/assets/odometry_native.png` & `small_gicp-0.0.6/docs/assets/odometry_native.png`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/docs/assets/odometry_time.png` & `small_gicp-0.0.6/docs/assets/odometry_time.png`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/ann/flat_container.hpp` & `small_gicp-0.0.6/include/small_gicp/ann/flat_container.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/ann/gaussian_voxelmap.hpp` & `small_gicp-0.0.6/include/small_gicp/ann/gaussian_voxelmap.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/ann/incremental_voxelmap.hpp` & `small_gicp-0.0.6/include/small_gicp/ann/incremental_voxelmap.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/ann/kdtree.hpp` & `small_gicp-0.0.6/include/small_gicp/ann/deprecated/kdtree.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/ann/kdtree_omp.hpp` & `small_gicp-0.0.6/include/small_gicp/ann/deprecated/kdtree_omp.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/ann/kdtree_tbb.hpp` & `small_gicp-0.0.6/include/small_gicp/ann/deprecated/kdtree_tbb.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/ann/nanoflann.hpp` & `small_gicp-0.0.6/include/small_gicp/ann/deprecated/nanoflann.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/ann/nanoflann_omp.hpp` & `small_gicp-0.0.6/include/small_gicp/ann/deprecated/nanoflann_omp.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/ann/nanoflann_tbb.hpp` & `small_gicp-0.0.6/include/small_gicp/ann/deprecated/nanoflann_tbb.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/ann/traits.hpp` & `small_gicp-0.0.6/include/small_gicp/ann/traits.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/benchmark/benchmark.hpp` & `small_gicp-0.0.6/include/small_gicp/benchmark/benchmark.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/benchmark/benchmark_odom.hpp` & `small_gicp-0.0.6/include/small_gicp/benchmark/benchmark_odom.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/benchmark/read_points.hpp` & `small_gicp-0.0.6/include/small_gicp/benchmark/read_points.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/factors/general_factor.hpp` & `small_gicp-0.0.6/include/small_gicp/factors/general_factor.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   NullFactor() = default;
 
   /// @brief Update linearized system consisting of linearized per-point factors.
   /// @param target       Target point cloud
   /// @param source       Source point cloud
   /// @param target_tree  Nearest neighbor search for the target point cloud
   /// @param T            Linearization point
-  /// @param H            [in/out] Linearized precision matrix.
+  /// @param H            [in/out] Linearized information matrix.
   /// @param b            [in/out] Linearized information vector.
   /// @param e            [in/out] Error at the linearization point.
   template <typename TargetPointCloud, typename SourcePointCloud, typename TargetTree>
   void update_linearized_system(
     const TargetPointCloud& target,
     const SourcePointCloud& source,
     const TargetTree& target_tree,
```

### Comparing `small_gicp-0.0.3/include/small_gicp/factors/gicp_factor.hpp` & `small_gicp-0.0.6/include/small_gicp/factors/gicp_factor.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   /// @brief Linearize the factor
   /// @param target       Target point cloud
   /// @param source       Source point cloud
   /// @param target_tree  Nearest neighbor search for the target point cloud
   /// @param T            Linearization point
   /// @param source_index Source point index
   /// @param rejector     Correspondence rejector
-  /// @param H            Linearized precision matrix
+  /// @param H            Linearized information matrix
   /// @param b            Linearized information vector
   /// @param e            Error at the linearization point
   /// @return
   template <typename TargetPointCloud, typename SourcePointCloud, typename TargetTree, typename CorrespondenceRejector>
   bool linearize(
     const TargetPointCloud& target,
     const SourcePointCloud& source,
```

### Comparing `small_gicp-0.0.3/include/small_gicp/factors/icp_factor.hpp` & `small_gicp-0.0.6/include/small_gicp/factors/icp_factor.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/factors/plane_icp_factor.hpp` & `small_gicp-0.0.6/include/small_gicp/factors/plane_icp_factor.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/pcl/pcl_point.hpp` & `small_gicp-0.0.6/include/small_gicp/pcl/pcl_point.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/pcl/pcl_point_traits.hpp` & `small_gicp-0.0.6/include/small_gicp/pcl/pcl_point_traits.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/pcl/pcl_proxy.hpp` & `small_gicp-0.0.6/include/small_gicp/pcl/pcl_proxy.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/pcl/pcl_registration.hpp` & `small_gicp-0.0.6/include/small_gicp/pcl/pcl_registration.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -95,16 +95,16 @@
   int num_threads_;                ///< Number of threads to use.
   int k_correspondences_;          ///< Number of neighbors for covariance estimation.
   double rotation_epsilon_;        ///< Rotation epsilon for convergence check.
   double voxel_resolution_;        ///< Voxel resolution for VGICP.
   std::string registration_type_;  ///< Registration type ("GICP" or "VGICP").
   bool verbose_;                   ///< Verbosity flag.
 
-  std::shared_ptr<KdTreeOMP<pcl::PointCloud<PointSource>>> target_tree_;  ///< KdTree for target point cloud.
-  std::shared_ptr<KdTreeOMP<pcl::PointCloud<PointSource>>> source_tree_;  ///< KdTree for source point cloud.
+  std::shared_ptr<KdTree<pcl::PointCloud<PointSource>>> target_tree_;  ///< KdTree for target point cloud.
+  std::shared_ptr<KdTree<pcl::PointCloud<PointSource>>> source_tree_;  ///< KdTree for source point cloud.
 
   std::shared_ptr<GaussianVoxelMap> target_voxelmap_;  ///< VoxelMap for target point cloud.
   std::shared_ptr<GaussianVoxelMap> source_voxelmap_;  ///< VoxelMap for source point cloud.
 
   std::vector<Eigen::Matrix4d> target_covs_;  ///< Covariances of target points
   std::vector<Eigen::Matrix4d> source_covs_;  ///< Covariances of source points.
```

### Comparing `small_gicp-0.0.3/include/small_gicp/pcl/pcl_registration_impl.hpp` & `small_gicp-0.0.6/include/small_gicp/pcl/pcl_registration_impl.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,27 @@
 template <typename PointSource, typename PointTarget>
 void RegistrationPCL<PointSource, PointTarget>::setInputSource(const PointCloudSourceConstPtr& cloud) {
   if (input_ == cloud) {
     return;
   }
 
   pcl::Registration<PointSource, PointTarget, Scalar>::setInputSource(cloud);
-  source_tree_ = std::make_shared<KdTreeOMP<pcl::PointCloud<PointSource>>>(input_, num_threads_);
+  source_tree_ = std::make_shared<KdTree<pcl::PointCloud<PointSource>>>(input_, KdTreeBuilderOMP(num_threads_));
   source_covs_.clear();
   source_voxelmap_.reset();
 }
 
 template <typename PointSource, typename PointTarget>
 void RegistrationPCL<PointSource, PointTarget>::setInputTarget(const PointCloudTargetConstPtr& cloud) {
   if (target_ == cloud) {
     return;
   }
 
   pcl::Registration<PointSource, PointTarget, Scalar>::setInputTarget(cloud);
-  target_tree_ = std::make_shared<KdTreeOMP<pcl::PointCloud<PointTarget>>>(target_, num_threads_);
+  target_tree_ = std::make_shared<KdTree<pcl::PointCloud<PointTarget>>>(target_, KdTreeBuilderOMP(num_threads_));
   target_covs_.clear();
   target_voxelmap_.reset();
 }
 
 template <typename PointSource, typename PointTarget>
 void RegistrationPCL<PointSource, PointTarget>::setSourceCovariances(const std::vector<Eigen::Matrix4d>& covs) {
   if (input_ == nullptr) {
```

### Comparing `small_gicp-0.0.3/include/small_gicp/points/eigen.hpp` & `small_gicp-0.0.6/include/small_gicp/points/eigen.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/points/point_cloud.hpp` & `small_gicp-0.0.6/include/small_gicp/points/point_cloud.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/points/traits.hpp` & `small_gicp-0.0.6/include/small_gicp/points/traits.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/registration/optimizer.hpp` & `small_gicp-0.0.6/include/small_gicp/registration/optimizer.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/registration/reduction.hpp` & `small_gicp-0.0.6/include/small_gicp/registration/reduction.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   /// @brief Sum up linearized systems
   /// @param target       Target point cloud
   /// @param source       Source point cloud
   /// @param target_tree  Nearest neighbor search for the target point cloud
   /// @param rejector     Correspondence rejector
   /// @param T            Linearization point
   /// @param factors      Factors to be linearized
-  /// @return             Sum of the linearized systems (Precision matrix, information vector, and error)
+  /// @return             Sum of the linearized systems (information matrix, information vector, and error)
   template <typename TargetPointCloud, typename SourcePointCloud, typename TargetTree, typename CorrespondenceRejector, typename Factor>
   std::tuple<Eigen::Matrix<double, 6, 6>, Eigen::Matrix<double, 6, 1>, double> linearize(
     const TargetPointCloud& target,
     const SourcePointCloud& source,
     const TargetTree& target_tree,
     const CorrespondenceRejector& rejector,
     const Eigen::Isometry3d& T,
```

### Comparing `small_gicp-0.0.3/include/small_gicp/registration/reduction_omp.hpp` & `small_gicp-0.0.6/include/small_gicp/registration/reduction_omp.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/registration/reduction_tbb.hpp` & `small_gicp-0.0.6/include/small_gicp/registration/reduction_tbb.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/registration/registration.hpp` & `small_gicp-0.0.6/include/small_gicp/registration/registration.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/registration/registration_helper.hpp` & `small_gicp-0.0.6/include/small_gicp/registration/registration_helper.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/registration/registration_result.hpp` & `small_gicp-0.0.6/include/small_gicp/registration/registration_result.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -20,13 +20,13 @@
 
   Eigen::Isometry3d T_target_source;  ///<  Estimated transformation
 
   bool converged;      ///< If the optimization converged
   size_t iterations;   ///< Number of optimization iterations
   size_t num_inliers;  ///< Number of inliear points
 
-  Eigen::Matrix<double, 6, 6> H;  ///< Final precision matrix
+  Eigen::Matrix<double, 6, 6> H;  ///< Final information matrix
   Eigen::Matrix<double, 6, 1> b;  ///< Final information vector
   double error;                   ///< Final error
 };
 
 }  // namespace small_gicp
```

### Comparing `small_gicp-0.0.3/include/small_gicp/registration/rejector.hpp` & `small_gicp-0.0.6/include/small_gicp/registration/rejector.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/registration/termination_criteria.hpp` & `small_gicp-0.0.6/include/small_gicp/registration/termination_criteria.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/util/downsampling.hpp` & `small_gicp-0.0.6/include/small_gicp/util/downsampling.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/util/downsampling_omp.hpp` & `small_gicp-0.0.6/include/small_gicp/util/downsampling_omp.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/util/downsampling_tbb.hpp` & `small_gicp-0.0.6/include/small_gicp/util/downsampling_tbb.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/util/lie.hpp` & `small_gicp-0.0.6/include/small_gicp/util/lie.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/util/normal_estimation.hpp` & `small_gicp-0.0.6/include/small_gicp/util/normal_estimation.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/util/normal_estimation_omp.hpp` & `small_gicp-0.0.6/include/small_gicp/util/normal_estimation_omp.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/util/normal_estimation_tbb.hpp` & `small_gicp-0.0.6/include/small_gicp/util/normal_estimation_tbb.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/include/small_gicp/util/sort_omp.hpp` & `small_gicp-0.0.6/include/small_gicp/util/sort_omp.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 // SPDX-FileCopyrightText: Copyright 2024 Kenji Koide
 // SPDX-License-Identifier: MIT
 #pragma once
 
 #include <algorithm>
 
+#ifdef _MSC_VER
+#pragma message("warning: Task-based OpenMP parallelism is not well supported on windows.")
+#pragma message("warning: Thus, OpenMP-based downsampling is only partially parallelized on windows.")
+#endif
+
 namespace small_gicp {
 
 template <typename RandomAccessIterator, typename Compare>
 void merge_sort_omp_impl(RandomAccessIterator first, RandomAccessIterator last, const Compare& comp) {
   const size_t n = std::distance(first, last);
   if (n < 1024) {
     std::sort(first, last, comp);
@@ -24,19 +29,23 @@
 
 #pragma omp taskwait
   std::inplace_merge(first, center, last, comp);
 }
 
 template <typename RandomAccessIterator, typename Compare>
 void merge_sort_omp(RandomAccessIterator first, RandomAccessIterator last, const Compare& comp, int num_threads) {
+#ifndef _MSC_VER
 #pragma omp parallel num_threads(num_threads)
   {
 #pragma omp single nowait
     { merge_sort_omp_impl(first, last, comp); }
   }
+#else
+  std::stable_sort(first, last, comp);
+#endif
 }
 
 template <typename RandomAccessIterator, typename Compare>
 void quick_sort_omp_impl(RandomAccessIterator first, RandomAccessIterator last, const Compare& comp) {
   const std::ptrdiff_t n = std::distance(first, last);
   if (n < 1024) {
     std::sort(first, last, comp);
@@ -61,15 +70,19 @@
 
 #pragma omp task
   quick_sort_omp_impl(middle2, last, comp);
 }
 
 template <typename RandomAccessIterator, typename Compare>
 void quick_sort_omp(RandomAccessIterator first, RandomAccessIterator last, const Compare& comp, int num_threads) {
+#ifndef _MSC_VER
 #pragma omp parallel num_threads(num_threads)
   {
 #pragma omp single nowait
     { quick_sort_omp_impl(first, last, comp); }
   }
+#else
+  std::sort(first, last, comp);
+#endif
 }
 
 }  // namespace small_gicp
```

### Comparing `small_gicp-0.0.3/include/small_gicp/util/vector3i_hash.hpp` & `small_gicp-0.0.6/include/small_gicp/util/vector3i_hash.hpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/package.xml` & `small_gicp-0.0.6/package.xml`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/scripts/plot_downsampling.py` & `small_gicp-0.0.6/scripts/plot_downsampling.py`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/scripts/plot_kdtree.py` & `small_gicp-0.0.6/scripts/plot_kdtree.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,22 +50,22 @@
 
     num_threads, num_points, rets = parse_result(results_path + '/' + filename)
     results[method] = rets[list(rets.keys())[0]] 
 
   fig, axes = pyplot.subplots(1, 2, figsize=(12, 3))
   
   num_threads = [1, 2, 3, 4, 5, 6, 7, 8, 16, 32, 64, 128]
-  axes[0].plot(num_points, results['small_1'], label='kdtree (nanoflann)', marker='o', linestyle='--')
-  for idx in [1, 3, 5, 7, 8]:
+  axes[0].plot(num_points, results['small_1'], label='kdtree (single-thread)', marker='o', linestyle='--')
+  for idx in [1, 2, 3, 5, 7, 8, 9]:
     N = num_threads[idx]
     axes[0].plot(num_points, results['omp_{}'.format(N)], label='kdtree_omp (%d threads)' % N, marker='s')
-    axes[0].plot(num_points, results['tbb_{}'.format(N)], label='kdtree_tbb (%d threads)' % N, marker='^')
+    # axes[0].plot(num_points, results['tbb_{}'.format(N)], label='kdtree_tbb (%d threads)' % N, marker='^')
 
   baseline = numpy.array(results['small_1'])
-  axes[1].plot([num_threads[0], num_threads[-1]], [1.0, 1.0], label='kdtree (nanoflann)', linestyle='--')
+  axes[1].plot([num_threads[0], num_threads[-1]], [1.0, 1.0], label='kdtree (single-thread)', linestyle='--')
   for idx in [5]:
     threads = num_threads[idx]
     N = num_points[idx]
     
     axes[1].plot(num_threads, baseline[idx] / [results['omp_{}'.format(threads)][idx] for threads in num_threads], label='omp (num_points=%d)' % N, marker='s')
     axes[1].plot(num_threads, baseline[idx] / [results['tbb_{}'.format(threads)][idx] for threads in num_threads], label='tbb (num_points=%d)' % N, marker='^')
```

### Comparing `small_gicp-0.0.3/scripts/plot_odometry.py` & `small_gicp-0.0.6/scripts/plot_odometry.py`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/scripts/plot_odometry_accuracy.py` & `small_gicp-0.0.6/scripts/plot_odometry_accuracy.py`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/scripts/plot_odometry_native.py` & `small_gicp-0.0.6/scripts/plot_odometry_native.py`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/scripts/run_kdtree_benchmark.sh` & `small_gicp-0.0.6/scripts/run_kdtree_benchmark.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/bin/bash
 dataset_path=$1
 exe_path=../build/kdtree_benchmark
 
 mkdir results
-num_threads=(1 2 3 4 5 6 7 8 16 32 64 128)
+num_threads=(1 2 3 4 5 6 7 8 16 32 64 92 128)
 
 $exe_path $dataset_path --num_threads 1 --num_trials 1000 --method small | tee results/kdtree_benchmark_small_$N.txt
 
 for N in ${num_threads[@]}; do
     sleep 1
     $exe_path $dataset_path --num_threads $N --num_trials 1000 --method tbb | tee results/kdtree_benchmark_tbb_$N.txt
 done
```

### Comparing `small_gicp-0.0.3/scripts/run_odometry_benchmark.sh` & `small_gicp-0.0.6/scripts/run_odometry_benchmark.sh`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/scripts/run_odometry_benchmark_native.sh` & `small_gicp-0.0.6/scripts/run_odometry_benchmark_native.sh`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/downsampling_benchmark.cpp` & `small_gicp-0.0.6/src/benchmark/downsampling_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/kdtree_benchmark.cpp` & `small_gicp-0.0.6/src/benchmark/kdtree_benchmark.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -104,19 +104,19 @@
   auto t1 = std::chrono::high_resolution_clock::now();
   while (std::chrono::duration_cast<std::chrono::seconds>(std::chrono::high_resolution_clock::now() - t1).count() < 1) {
     auto downsampled = voxelgrid_sampling(*raw_points, 0.1);
 
     if (method == "small") {
       UnsafeKdTree<PointCloud> tree(*downsampled);
     } else if (method == "omp") {
-      UnsafeKdTreeOMP<PointCloud> tree(*downsampled, num_threads);
+      UnsafeKdTree<PointCloud> tree(*downsampled, KdTreeBuilderOMP(num_threads));
     }
 #ifdef BUILD_WITH_TBB
     else if (method == "tbb") {
-      UnsafeKdTreeTBB<PointCloud> tree(*downsampled);
+      UnsafeKdTree<PointCloud> tree(*downsampled, KdTreeBuilderTBB());
     }
 #endif
   }
 
   Stopwatch sw;
 
   if (method == "small") {
@@ -135,29 +135,29 @@
       std::cout << "kdtree_times=" << kdtree_times.str() << " [msec]" << std::endl;
     }
   } else if (method == "omp") {
     for (size_t i = 0; i < downsampling_resolutions.size(); i++) {
       Summarizer kdtree_omp_times(true);
       sw.start();
       for (size_t j = 0; j < num_trials; j++) {
-        UnsafeKdTreeOMP<PointCloud> tree(*downsampled[i], num_threads);
+        UnsafeKdTree<PointCloud> tree(*downsampled[i], KdTreeBuilderOMP(num_threads));
         sw.lap();
         kdtree_omp_times.push(sw.msec());
       }
 
       std::cout << "kdtree_omp_times=" << kdtree_omp_times.str() << " [msec]" << std::endl;
     }
   }
 #ifdef BUILD_WITH_TBB
   else if (method == "tbb") {
     for (size_t i = 0; i < downsampling_resolutions.size(); i++) {
       Summarizer kdtree_tbb_times(true);
       sw.start();
       for (size_t j = 0; j < num_trials; j++) {
-        UnsafeKdTreeTBB<PointCloud> tree(*downsampled[i]);
+        UnsafeKdTree<PointCloud> tree(*downsampled[i], KdTreeBuilderTBB());
         sw.lap();
         kdtree_tbb_times.push(sw.msec());
       }
 
       std::cout << "kdtree_tbb_times=" << kdtree_tbb_times.str() << " [msec]" << std::endl;
     }
   }
```

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_fast_gicp.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_fast_gicp.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_fast_vgicp.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_fast_vgicp.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_pcl.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_pcl.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp_model_tbb.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp_model_tbb.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp_omp.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp_tbb.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,70 @@
+#ifdef BUILD_WITH_TBB
+
 #include <small_gicp/benchmark/benchmark_odom.hpp>
 
+#include <tbb/tbb.h>
 #include <small_gicp/factors/gicp_factor.hpp>
 #include <small_gicp/points/point_cloud.hpp>
-#include <small_gicp/ann/kdtree_omp.hpp>
-#include <small_gicp/util/normal_estimation_omp.hpp>
-#include <small_gicp/registration/reduction_omp.hpp>
+#include <small_gicp/ann/kdtree_tbb.hpp>
+#include <small_gicp/util/normal_estimation_tbb.hpp>
+#include <small_gicp/registration/reduction_tbb.hpp>
 #include <small_gicp/registration/registration.hpp>
 
 namespace small_gicp {
 
-class SmallGICPOnlineOdometryEstimationOMP : public OnlineOdometryEstimation {
+class SmallGICPOnlineOdometryEstimationTBB : public OnlineOdometryEstimation {
 public:
-  explicit SmallGICPOnlineOdometryEstimationOMP(const OdometryEstimationParams& params) : OnlineOdometryEstimation(params), T_world_lidar(Eigen::Isometry3d::Identity()) {}
+  explicit SmallGICPOnlineOdometryEstimationTBB(const OdometryEstimationParams& params)
+  : OnlineOdometryEstimation(params),
+    control(tbb::global_control::max_allowed_parallelism, params.num_threads),
+    T(Eigen::Isometry3d::Identity()) {}
 
   Eigen::Isometry3d estimate(const PointCloud::Ptr& points) override {
     Stopwatch sw;
     sw.start();
 
-    // Preprocess input points (kdtree construction & covariance estimation)
-    // Note that input points here is already downsampled
-    auto tree = std::make_shared<KdTreeOMP<PointCloud>>(points, params.num_threads);
-    estimate_covariances_omp(*points, *tree, params.num_neighbors, params.num_threads);
+    auto tree = std::make_shared<KdTree<PointCloud>>(points, KdTreeBuilderTBB());
+    estimate_covariances_tbb(*points, *tree, params.num_neighbors);
 
     if (target_points == nullptr) {
-      // This is the very first frame
       target_points = points;
       target_tree = tree;
-      return T_world_lidar;
+      return T;
     }
 
-    // Registration using GICP + OMP-based parallel reduction
-    Registration<GICPFactor, ParallelReductionOMP> registration;
+    Registration<GICPFactor, ParallelReductionTBB> registration;
     registration.rejector.max_dist_sq = params.max_correspondence_distance * params.max_correspondence_distance;
-    registration.reduction.num_threads = params.num_threads;
 
-    // Perform registration
     auto result = registration.align(*target_points, *points, *target_tree, Eigen::Isometry3d::Identity());
 
-    // Update T_world_lidar and target points
-    T_world_lidar = T_world_lidar * result.T_target_source;
-    target_points = points;
-    target_tree = tree;
-
     sw.stop();
     reg_times.push(sw.msec());
 
-    return T_world_lidar;
+    T = T * result.T_target_source;
+    target_points = points;
+    target_tree = tree;
+
+    return T;
   }
 
   void report() override {  //
     std::cout << "registration_time_stats=" << reg_times.str() << " [msec/scan]  total_throughput=" << total_times.str() << " [msec/scan]" << std::endl;
   }
 
 private:
+  tbb::global_control control;
+
   Summarizer reg_times;
 
-  PointCloud::Ptr target_points;           // Last point cloud to be registration target
-  KdTreeOMP<PointCloud>::Ptr target_tree;  // KdTree of the last point cloud
+  PointCloud::Ptr target_points;
+  KdTree<PointCloud>::Ptr target_tree;
 
-  Eigen::Isometry3d T_world_lidar;  // T_world_lidar
+  Eigen::Isometry3d T;
 };
 
-static auto small_gicp_omp_registry =
-  register_odometry("small_gicp_omp", [](const OdometryEstimationParams& params) { return std::make_shared<SmallGICPOnlineOdometryEstimationOMP>(params); });
+static auto small_gicp_tbb_registry =
+  register_odometry("small_gicp_tbb", [](const OdometryEstimationParams& params) { return std::make_shared<SmallGICPOnlineOdometryEstimationTBB>(params); });
 
 }  // namespace small_gicp
+
+#endif
```

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp_pcl.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp_pcl.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp_tbb.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_vgicp_tbb.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 #ifdef BUILD_WITH_TBB
 
 #include <small_gicp/benchmark/benchmark_odom.hpp>
 
 #include <tbb/tbb.h>
 #include <small_gicp/factors/gicp_factor.hpp>
 #include <small_gicp/points/point_cloud.hpp>
-#include <small_gicp/ann/kdtree_tbb.hpp>
+#include <small_gicp/ann/gaussian_voxelmap.hpp>
 #include <small_gicp/util/normal_estimation_tbb.hpp>
 #include <small_gicp/registration/reduction_tbb.hpp>
 #include <small_gicp/registration/registration.hpp>
 
 namespace small_gicp {
 
-class SmallGICPOnlineOdometryEstimationTBB : public OnlineOdometryEstimation {
+class SmallVGICPOnlineOdometryEstimationTBB : public OnlineOdometryEstimation {
 public:
-  explicit SmallGICPOnlineOdometryEstimationTBB(const OdometryEstimationParams& params)
+  explicit SmallVGICPOnlineOdometryEstimationTBB(const OdometryEstimationParams& params)
   : OnlineOdometryEstimation(params),
     control(tbb::global_control::max_allowed_parallelism, params.num_threads),
     T(Eigen::Isometry3d::Identity()) {}
 
   Eigen::Isometry3d estimate(const PointCloud::Ptr& points) override {
     Stopwatch sw;
     sw.start();
 
-    auto tree = std::make_shared<KdTreeTBB<PointCloud>>(points);
-    estimate_covariances_tbb(*points, *tree, params.num_neighbors);
+    estimate_covariances_tbb(*points, params.num_neighbors);
+
+    auto voxelmap = std::make_shared<GaussianVoxelMap>(params.voxel_resolution);
+    voxelmap->insert(*points);
 
     if (target_points == nullptr) {
       target_points = points;
-      target_tree = tree;
+      target_voxelmap = voxelmap;
       return T;
     }
 
     Registration<GICPFactor, ParallelReductionTBB> registration;
     registration.rejector.max_dist_sq = params.max_correspondence_distance * params.max_correspondence_distance;
 
-    auto result = registration.align(*target_points, *points, *target_tree, Eigen::Isometry3d::Identity());
+    auto result = registration.align(*target_voxelmap, *points, *target_voxelmap, Eigen::Isometry3d::Identity());
 
     sw.stop();
     reg_times.push(sw.msec());
 
     T = T * result.T_target_source;
+
     target_points = points;
-    target_tree = tree;
+    target_voxelmap = voxelmap;
 
     return T;
   }
 
   void report() override {  //
     std::cout << "registration_time_stats=" << reg_times.str() << " [msec/scan]  total_throughput=" << total_times.str() << " [msec/scan]" << std::endl;
   }
 
 private:
   tbb::global_control control;
 
   Summarizer reg_times;
 
   PointCloud::Ptr target_points;
-  KdTreeTBB<PointCloud>::Ptr target_tree;
+  GaussianVoxelMap::Ptr target_voxelmap;
 
   Eigen::Isometry3d T;
 };
 
 static auto small_gicp_tbb_registry =
-  register_odometry("small_gicp_tbb", [](const OdometryEstimationParams& params) { return std::make_shared<SmallGICPOnlineOdometryEstimationTBB>(params); });
+  register_odometry("small_vgicp_tbb", [](const OdometryEstimationParams& params) { return std::make_shared<SmallVGICPOnlineOdometryEstimationTBB>(params); });
 
 }  // namespace small_gicp
 
 #endif
```

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_gicp_tbb_flow.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_gicp_tbb_flow.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_vgicp_model_tbb.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_vgicp_model_tbb.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/benchmark/odometry_benchmark_small_vgicp_omp.cpp` & `small_gicp-0.0.6/src/benchmark/odometry_benchmark_small_vgicp_omp.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 public:
   explicit SmallVGICPOnlineOdometryEstimationOMP(const OdometryEstimationParams& params) : OnlineOdometryEstimation(params), T(Eigen::Isometry3d::Identity()) {}
 
   Eigen::Isometry3d estimate(const PointCloud::Ptr& points) override {
     Stopwatch sw;
     sw.start();
 
-    auto tree = std::make_shared<KdTreeOMP<PointCloud>>(points, params.num_threads);
+    auto tree = std::make_shared<KdTree<PointCloud>>(points, KdTreeBuilderOMP(params.num_threads));
     estimate_covariances_omp(*points, *tree, params.num_neighbors, params.num_threads);
 
     auto voxelmap = std::make_shared<GaussianVoxelMap>(params.voxel_resolution);
     voxelmap->insert(*points);
 
     if (target_points == nullptr) {
       target_points = points;
```

### Comparing `small_gicp-0.0.3/src/example/01_basic_registration.cpp` & `small_gicp-0.0.6/src/example/01_basic_registration.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/example/02_basic_registration_pcl.cpp` & `small_gicp-0.0.6/src/example/02_basic_registration_pcl.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,16 @@
   // Estimate covariances of points.
   const int num_threads = 4;
   const int num_neighbors = 20;
   estimate_covariances_omp(*target, num_neighbors, num_threads);
   estimate_covariances_omp(*source, num_neighbors, num_threads);
 
   // Create KdTree for target and source.
-  auto target_tree = std::make_shared<KdTreeOMP<pcl::PointCloud<pcl::PointCovariance>>>(target, num_threads);
-  auto source_tree = std::make_shared<KdTreeOMP<pcl::PointCloud<pcl::PointCovariance>>>(source, num_threads);
+  auto target_tree = std::make_shared<KdTree<pcl::PointCloud<pcl::PointCovariance>>>(target, KdTreeBuilderOMP(num_threads));
+  auto source_tree = std::make_shared<KdTree<pcl::PointCloud<pcl::PointCovariance>>>(source, KdTreeBuilderOMP(num_threads));
 
   Registration<GICPFactor, ParallelReductionOMP> registration;
   registration.reduction.num_threads = num_threads;
   registration.rejector.max_dist_sq = 1.0;
 
   // Align point clouds. Note that the input point clouds are pcl::PointCloud<pcl::PointCovariance>.
   auto result = registration.align(*target, *source, *target_tree, Eigen::Isometry3d::Identity());
```

### Comparing `small_gicp-0.0.3/src/example/03_registration_template.cpp` & `small_gicp-0.0.6/src/example/03_registration_template.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
   auto source = std::make_shared<PointCloud>(source_points);
 
   // Downsampling
   target = voxelgrid_sampling_omp(*target, downsampling_resolution, num_threads);
   source = voxelgrid_sampling_omp(*source, downsampling_resolution, num_threads);
 
   // Create KdTree
-  auto target_tree = std::make_shared<KdTreeOMP<PointCloud>>(target, num_threads);
-  auto source_tree = std::make_shared<KdTreeOMP<PointCloud>>(source, num_threads);
+  auto target_tree = std::make_shared<KdTree<PointCloud>>(target, KdTreeBuilderOMP(num_threads));
+  auto source_tree = std::make_shared<KdTree<PointCloud>>(source, KdTreeBuilderOMP(num_threads));
 
   // Estimate point covariances
   estimate_covariances_omp(*target, *target_tree, num_neighbors, num_threads);
   estimate_covariances_omp(*source, *source_tree, num_neighbors, num_threads);
 
   // GICP + OMP-based parallel reduction
   Registration<GICPFactor, ParallelReductionOMP> registration;
@@ -215,15 +215,15 @@
   /// @brief Update linearized system.
   /// @note  This method is  called just before the linearized system is solved.
   ///        By modifying the linearized system (H, b, e), you can inject arbitrary constraints.
   /// @param target       Target point cloud
   /// @param source       Source point cloud
   /// @param target_tree  Nearest neighbor search for the target point cloud
   /// @param T            Linearization point
-  /// @param H            [in/out] Linearized precision matrix.
+  /// @param H            [in/out] Linearized information matrix.
   /// @param b            [in/out] Linearized information vector.
   /// @param e            [in/out] Error at the linearization point.
   template <typename TargetPointCloud, typename SourcePointCloud, typename TargetTree>
   void update_linearized_system(
     const TargetPointCloud& target,
     const SourcePointCloud& source,
     const TargetTree& target_tree,
```

### Comparing `small_gicp-0.0.3/src/example/basic_registration.py` & `small_gicp-0.0.6/src/example/basic_registration.py`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/example/kitti_odometry.py` & `small_gicp-0.0.6/src/example/kitti_odometry.py`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/python/factors.cpp` & `small_gicp-0.0.6/src/python/factors.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     .def(py::init<>())
     .def(
       "linearize",
       [](
         ICPFactor& factor,
         const PointCloud& target,
         const PointCloud& source,
-        const KdTreeOMP<PointCloud>& kdtree,
+        const KdTree<PointCloud>& kdtree,
         const Eigen::Matrix4d& T,
         size_t source_index,
         const DistanceRejector& rejector) -> std::tuple<bool, Eigen::Matrix<double, 6, 6>, Eigen::Matrix<double, 6, 1>, double> {
         Eigen::Matrix<double, 6, 6> H = Eigen::Matrix<double, 6, 6>::Zero();
         Eigen::Matrix<double, 6, 1> b = Eigen::Matrix<double, 6, 1>::Zero();
         double e = 0.0;
         bool succ = factor.linearize(target, source, kdtree, Eigen::Isometry3d(T), source_index, rejector, &H, &b, &e);
@@ -49,15 +49,15 @@
     .def(py::init<>())
     .def(
       "linearize",
       [](
         PointToPlaneICPFactor& factor,
         const PointCloud& target,
         const PointCloud& source,
-        const KdTreeOMP<PointCloud>& kdtree,
+        const KdTree<PointCloud>& kdtree,
         const Eigen::Matrix4d& T,
         size_t source_index,
         const DistanceRejector& rejector) -> std::tuple<bool, Eigen::Matrix<double, 6, 6>, Eigen::Matrix<double, 6, 1>, double> {
         Eigen::Matrix<double, 6, 6> H = Eigen::Matrix<double, 6, 6>::Zero();
         Eigen::Matrix<double, 6, 1> b = Eigen::Matrix<double, 6, 1>::Zero();
         double e = 0.0;
         bool succ = factor.linearize(target, source, kdtree, Eigen::Isometry3d(T), source_index, rejector, &H, &b, &e);
@@ -69,15 +69,15 @@
     .def(py::init<>())
     .def(
       "linearize",
       [](
         GICPFactor& factor,
         const PointCloud& target,
         const PointCloud& source,
-        const KdTreeOMP<PointCloud>& kdtree,
+        const KdTree<PointCloud>& kdtree,
         const Eigen::Matrix4d& T,
         size_t source_index,
         const DistanceRejector& rejector) -> std::tuple<bool, Eigen::Matrix<double, 6, 6>, Eigen::Matrix<double, 6, 1>, double> {
         Eigen::Matrix<double, 6, 6> H = Eigen::Matrix<double, 6, 6>::Zero();
         Eigen::Matrix<double, 6, 1> b = Eigen::Matrix<double, 6, 1>::Zero();
         double e = 0.0;
         bool succ = factor.linearize(target, source, kdtree, Eigen::Isometry3d(T), source_index, rejector, &H, &b, &e);
```

### Comparing `small_gicp-0.0.3/src/python/kdtree.cpp` & `small_gicp-0.0.6/src/python/kdtree.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -12,24 +12,27 @@
 #include <small_gicp/ann/kdtree_omp.hpp>
 
 namespace py = pybind11;
 using namespace small_gicp;
 
 void define_kdtree(py::module& m) {
   // KdTree
-  py::class_<KdTreeOMP<PointCloud>, std::shared_ptr<KdTreeOMP<PointCloud>>>(m, "KdTree")  //
-    .def(py::init<PointCloud::ConstPtr, int>(), py::arg("points"), py::arg("num_threads") = 1)
+  py::class_<KdTree<PointCloud>, std::shared_ptr<KdTree<PointCloud>>>(m, "KdTree")  //
+    .def(
+      py::init([](const PointCloud::ConstPtr& points, int num_threads) { return std::make_shared<KdTree<PointCloud>>(points, KdTreeBuilderOMP(num_threads)); }),
+      py::arg("points"),
+      py::arg("num_threads") = 1)
     .def(
       "nearest_neighbor_search",
-      [](const KdTreeOMP<PointCloud>& kdtree, const Eigen::Vector3d& pt) {
+      [](const KdTree<PointCloud>& kdtree, const Eigen::Vector3d& pt) {
         size_t k_index = -1;
         double k_sq_dist = std::numeric_limits<double>::max();
         const size_t found = traits::nearest_neighbor_search(kdtree, Eigen::Vector4d(pt.x(), pt.y(), pt.z(), 1.0), &k_index, &k_sq_dist);
         return std::make_tuple(found, k_index, k_sq_dist);
       })
-    .def("knn_search", [](const KdTreeOMP<PointCloud>& kdtree, const Eigen::Vector3d& pt, int k) {
+    .def("knn_search", [](const KdTree<PointCloud>& kdtree, const Eigen::Vector3d& pt, int k) {
       std::vector<size_t> k_indices(k, -1);
       std::vector<double> k_sq_dists(k, std::numeric_limits<double>::max());
       const size_t found = traits::knn_search(kdtree, Eigen::Vector4d(pt.x(), pt.y(), pt.z(), 1.0), k, k_indices.data(), k_sq_dists.data());
       return std::make_pair(k_indices, k_sq_dists);
     });
 }
```

### Comparing `small_gicp-0.0.3/src/python/misc.cpp` & `small_gicp-0.0.6/src/python/misc.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/python/pointcloud.cpp` & `small_gicp-0.0.6/src/python/pointcloud.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/python/preprocess.cpp` & `small_gicp-0.0.6/src/python/preprocess.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -53,17 +53,17 @@
     py::arg("points"),
     py::arg("downsampling_resolution"),
     py::arg("num_threads") = 1);
 
   // estimate_normals
   m.def(
     "estimate_normals",
-    [](PointCloud::Ptr points, std::shared_ptr<KdTreeOMP<PointCloud>> tree, int num_neighbors, int num_threads) {
+    [](PointCloud::Ptr points, std::shared_ptr<KdTree<PointCloud>> tree, int num_neighbors, int num_threads) {
       if (tree == nullptr) {
-        tree = std::make_shared<KdTreeOMP<PointCloud>>(points, num_threads);
+        tree = std::make_shared<KdTree<PointCloud>>(points, KdTreeBuilderOMP(num_threads));
       }
 
       if (num_threads == 1) {
         estimate_normals(*points, *tree, num_neighbors);
       } else {
         estimate_normals_omp(*points, *tree, num_neighbors, num_threads);
       }
@@ -72,17 +72,17 @@
     py::arg("tree") = nullptr,
     py::arg("num_neighbors") = 20,
     py::arg("num_threads") = 1);
 
   // estimate_covariances
   m.def(
     "estimate_covariances",
-    [](PointCloud::Ptr points, std::shared_ptr<KdTreeOMP<PointCloud>> tree, int num_neighbors, int num_threads) {
+    [](PointCloud::Ptr points, std::shared_ptr<KdTree<PointCloud>> tree, int num_neighbors, int num_threads) {
       if (tree == nullptr) {
-        tree = std::make_shared<KdTreeOMP<PointCloud>>(points, num_threads);
+        tree = std::make_shared<KdTree<PointCloud>>(points, KdTreeBuilderOMP(num_threads));
       }
 
       if (num_threads == 1) {
         estimate_covariances(*points, *tree, num_neighbors);
       } else {
         estimate_covariances_omp(*points, *tree, num_neighbors, num_threads);
       }
@@ -91,17 +91,17 @@
     py::arg("tree") = nullptr,
     py::arg("num_neighbors") = 20,
     py::arg("num_threads") = 1);
 
   // estimate_normals_covariances
   m.def(
     "estimate_normals_covariances",
-    [](PointCloud::Ptr points, std::shared_ptr<KdTreeOMP<PointCloud>> tree, int num_neighbors, int num_threads) {
+    [](PointCloud::Ptr points, std::shared_ptr<KdTree<PointCloud>> tree, int num_neighbors, int num_threads) {
       if (tree == nullptr) {
-        tree = std::make_shared<KdTreeOMP<PointCloud>>(points, num_threads);
+        tree = std::make_shared<KdTree<PointCloud>>(points, KdTreeBuilderOMP(num_threads));
       }
 
       if (num_threads == 1) {
         estimate_normals_covariances(*points, *tree, num_neighbors);
       } else {
         estimate_normals_covariances_omp(*points, *tree, num_neighbors, num_threads);
       }
@@ -110,15 +110,15 @@
     py::arg("tree") = nullptr,
     py::arg("num_neighbors") = 20,
     py::arg("num_threads") = 1);
 
   // preprocess_points (numpy)
   m.def(
     "preprocess_points",
-    [](const Eigen::MatrixXd& points_numpy, double downsampling_resolution, int num_neighbors, int num_threads) -> std::pair<PointCloud::Ptr, KdTreeOMP<PointCloud>::Ptr> {
+    [](const Eigen::MatrixXd& points_numpy, double downsampling_resolution, int num_neighbors, int num_threads) -> std::pair<PointCloud::Ptr, KdTree<PointCloud>::Ptr> {
       if (points_numpy.cols() != 3 && points_numpy.cols() != 4) {
         std::cerr << "points_numpy must be Nx3 or Nx4" << std::endl;
         return {nullptr, nullptr};
       }
 
       auto points = std::make_shared<PointCloud>();
       points->resize(points_numpy.rows());
@@ -127,34 +127,34 @@
           points->point(i) << points_numpy.row(i).transpose(), 1.0;
         } else {
           points->point(i) << points_numpy.row(i).transpose();
         }
       }
 
       auto downsampled = voxelgrid_sampling_omp(*points, downsampling_resolution, num_threads);
-      auto kdtree = std::make_shared<KdTreeOMP<PointCloud>>(downsampled, num_threads);
+      auto kdtree = std::make_shared<KdTree<PointCloud>>(downsampled, KdTreeBuilderOMP(num_threads));
       estimate_normals_covariances_omp(*downsampled, *kdtree, num_neighbors, num_threads);
       return {downsampled, kdtree};
     },
     py::arg("points"),
     py::arg("downsampling_resolution") = 0.25,
     py::arg("num_neighbors") = 10,
     py::arg("num_threads") = 1);
 
   // preprocess_points
   m.def(
     "preprocess_points",
-    [](const PointCloud& points, double downsampling_resolution, int num_neighbors, int num_threads) -> std::pair<PointCloud::Ptr, KdTreeOMP<PointCloud>::Ptr> {
+    [](const PointCloud& points, double downsampling_resolution, int num_neighbors, int num_threads) -> std::pair<PointCloud::Ptr, KdTree<PointCloud>::Ptr> {
       if (points.empty()) {
         std::cerr << "warning: points is empty" << std::endl;
         return {nullptr, nullptr};
       }
 
       auto downsampled = voxelgrid_sampling_omp(points, downsampling_resolution, num_threads);
-      auto kdtree = std::make_shared<KdTreeOMP<PointCloud>>(downsampled, num_threads);
+      auto kdtree = std::make_shared<KdTree<PointCloud>>(downsampled, KdTreeBuilderOMP(num_threads));
       estimate_normals_covariances_omp(*downsampled, *kdtree, num_neighbors, num_threads);
       return {downsampled, kdtree};
     },
     py::arg("points"),
     py::arg("downsampling_resolution") = 0.25,
     py::arg("num_neighbors") = 10,
     py::arg("num_threads") = 1);
```

### Comparing `small_gicp-0.0.3/src/python/python.cpp` & `small_gicp-0.0.6/src/python/python.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/python/result.cpp` & `small_gicp-0.0.6/src/python/result.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/python/voxelmap.cpp` & `small_gicp-0.0.6/src/python/voxelmap.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/small_gicp/benchmark/benchmark_odom.cpp` & `small_gicp-0.0.6/src/small_gicp/benchmark/benchmark_odom.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/small_gicp/registration/registration_helper.cpp` & `small_gicp-0.0.6/src/small_gicp/registration/registration_helper.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/test/downsampling_test.cpp` & `small_gicp-0.0.6/src/test/downsampling_test.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#include <unordered_set>
+
 #include <gtest/gtest.h>
 #include <pcl/point_types.h>
 #include <pcl/point_cloud.h>
 #include <pcl/filters/voxel_grid.h>
 
 #include <small_gicp/points/point_cloud.hpp>
 #include <small_gicp/pcl/pcl_point.hpp>
@@ -71,24 +73,65 @@
 
 INSTANTIATE_TEST_SUITE_P(DownsamplingTest, DownsamplingTest, testing::Values("SMALL", "TBB", "OMP"), [](const auto& info) { return info.param; });
 
 // Check if downsampling works correctly for empty points
 TEST_P(DownsamplingTest, EmptyTest) {
   auto empty_points = std::make_shared<PointCloud>();
   auto empty_downsampled = downsample(*empty_points, 0.1);
-  EXPECT_EQ(empty_downsampled && empty_downsampled->size(), 0) << "Empty test small: " + GetParam();
+  EXPECT_TRUE(empty_downsampled);
+  EXPECT_EQ(empty_downsampled->size(), 0) << "Empty test small: " + GetParam();
 
   auto empty_points_pcl = pcl::make_shared<pcl::PointCloud<pcl::PointXYZ>>();
   auto empty_downsampled_pcl = downsample(*empty_points_pcl, 0.1);
-  EXPECT_EQ(empty_downsampled_pcl && empty_downsampled_pcl->size(), 0) << "Empty test pcl: " + GetParam();
+  EXPECT_TRUE(empty_downsampled_pcl);
+  EXPECT_EQ(empty_downsampled_pcl->size(), 0) << "Empty test pcl: " + GetParam();
 }
 
 // Check if downsampling results are mostly identical to those of pcl::VoxelGrid
 TEST_P(DownsamplingTest, DownsampleTest) {
   for (size_t i = 0; i < resolutions.size(); i++) {
     auto result = downsample(*points, resolutions[i]);
     EXPECT_LT(std::abs(1.0 - static_cast<double>(result->size()) / downsampled_pcl[i]->size()), 0.9) << "Downsampled size check (small): " + GetParam();
     auto result_pcl = downsample(*points_pcl, resolutions[i]);
     EXPECT_LT(std::abs(1.0 - static_cast<double>(result_pcl->size()) / downsampled_pcl[i]->size()), 0.9) << "Downsampled size check (pcl): " + GetParam();
     EXPECT_EQ(result->size(), result_pcl->size()) << "Size check (small vs pcl): " + GetParam();
   }
 }
+
+// Check if random sampling works correctly for empty points
+TEST_P(DownsamplingTest, EmptyRandamSamplingTest) {
+  std::mt19937 mt;
+
+  auto empty_points = std::make_shared<PointCloud>();
+  auto empty_downsampled = random_sampling(*empty_points, 1000, mt);
+  EXPECT_TRUE(empty_downsampled);
+  EXPECT_EQ(empty_downsampled->size(), 0) << "Empty test small: " + GetParam();
+
+  auto empty_points_pcl = pcl::make_shared<pcl::PointCloud<pcl::PointXYZ>>();
+  auto empty_downsampled_pcl = random_sampling(*empty_points_pcl, 1000, mt);
+  EXPECT_TRUE(empty_downsampled_pcl);
+  EXPECT_EQ(empty_downsampled_pcl->size(), 0) << "Empty test pcl: " + GetParam();
+}
+
+// Test random sampling
+TEST_P(DownsamplingTest, RandamSamplingTest) {
+  std::mt19937 mt;
+
+  auto downsampled = voxelgrid_sampling(*points, 0.1);
+
+  const std::vector<size_t> num_points = {0, 100, 1000};
+  for (size_t N : num_points) {
+    auto result = random_sampling(*downsampled, N, mt);
+    EXPECT_TRUE(result);
+    EXPECT_EQ(result->size(), N) << "Size check (small): " + GetParam();
+
+    std::unordered_set<size_t> indices;
+    for (size_t i = 0; i < N; i++) {
+      const auto found = std::find_if(downsampled->points.begin(), downsampled->points.end(), [&](const auto& p) { return (p - result->points[i]).norm() < 1.0e-6; });
+      EXPECT_NE(found, downsampled->points.end()) << "Existence check (small): " + GetParam();
+
+      const size_t index = std::distance(downsampled->points.begin(), found);
+      EXPECT_EQ(indices.count(index), 0) << "Uniqueness check (small): " + GetParam();
+      indices.insert(index);
+    }
+  }
+}
```

### Comparing `small_gicp-0.0.3/src/test/kdtree_test.cpp` & `small_gicp-0.0.6/src/test/kdtree_test.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -181,24 +181,24 @@
   if (method == "SMALL") {
     auto kdtree = std::make_shared<KdTree<PointCloud>>(points);
     test_kdtree(*points, *kdtree);
 
     auto kdtree_pcl = std::make_shared<KdTree<pcl::PointCloud<pcl::PointXYZ>>>(points_pcl);
     test_kdtree(*points_pcl, *kdtree_pcl);
   } else if (method == "TBB") {
-    auto kdtree = std::make_shared<KdTreeTBB<PointCloud>>(points);
+    auto kdtree = std::make_shared<KdTree<PointCloud>>(points, KdTreeBuilderTBB());
     test_kdtree(*points, *kdtree);
 
-    auto kdtree_pcl = std::make_shared<KdTreeTBB<pcl::PointCloud<pcl::PointXYZ>>>(points_pcl);
+    auto kdtree_pcl = std::make_shared<KdTree<pcl::PointCloud<pcl::PointXYZ>>>(points_pcl, KdTreeBuilderTBB());
     test_kdtree(*points_pcl, *kdtree_pcl);
   } else if (method == "OMP") {
-    auto kdtree = std::make_shared<KdTreeOMP<PointCloud>>(points, 4);
+    auto kdtree = std::make_shared<KdTree<PointCloud>>(points, KdTreeBuilderOMP(4));
     test_kdtree(*points, *kdtree);
 
-    auto kdtree_pcl = std::make_shared<KdTreeOMP<pcl::PointCloud<pcl::PointXYZ>>>(points_pcl, 4);
+    auto kdtree_pcl = std::make_shared<KdTree<pcl::PointCloud<pcl::PointXYZ>>>(points_pcl, KdTreeBuilderOMP(4));
     test_kdtree(*points_pcl, *kdtree_pcl);
   } else if (method == "IVOX") {
     auto voxelmap = std::make_shared<IncrementalVoxelMap<FlatContainerNormalCov>>(1.0);
     voxelmap->insert(*points);
     test_voxelmap(*points, *voxelmap);
 
     auto indices = traits::point_indices(*voxelmap);
```

### Comparing `small_gicp-0.0.3/src/test/normal_estimation_test.cpp` & `small_gicp-0.0.6/src/test/normal_estimation_test.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -233,15 +233,15 @@
   EXPECT_TRUE(check_normals(*point_normals));
   estimate_normals_tbb(*point_normals, num_neighbors);
   EXPECT_TRUE(check_normals(*point_normals));
   estimate_normals_omp(*point_normals, num_neighbors, 2);
   EXPECT_TRUE(check_normals(*point_normals));
 
   // Covariance estimation
-  auto point_covs = pcl::make_shared<pcl::PointCloud<pcl::PointNormalCovariance>>();
+  auto point_covs = pcl::make_shared<pcl::PointCloud<pcl::PointCovariance>>();
   copy_points(*point_covs);
 
   estimate_covariances(*point_covs, num_neighbors);
   EXPECT_TRUE(check_covs(*point_covs));
   estimate_covariances_tbb(*point_covs, num_neighbors);
   EXPECT_TRUE(check_covs(*point_covs));
   estimate_covariances_omp(*point_covs, num_neighbors, 2);
```

### Comparing `small_gicp-0.0.3/src/test/points_test.cpp` & `small_gicp-0.0.6/src/test/points_test.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/test/python_test.py` & `small_gicp-0.0.6/src/test/python_test.py`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/test/registration_test.cpp` & `small_gicp-0.0.6/src/test/registration_test.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/test/sort_omp_test.cpp` & `small_gicp-0.0.6/src/test/sort_omp_test.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/src/test/vector_test.cpp` & `small_gicp-0.0.6/src/test/vector_test.cpp`

 * *Files identical despite different names*

### Comparing `small_gicp-0.0.3/PKG-INFO` & `small_gicp-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 Metadata-Version: 2.1
 Name: small_gicp
-Version: 0.0.3
+Version: 0.0.6
 Summary: Efficient and parallelized algorithms for fine point cloud registration
 Author-Email: Kenji Koide <k.koide@aist.go.jp>
 License: MIT
 Project-URL: Homepage, https://github.com/koide3/small_gicp
 Requires-Python: >=3.7
-Provides-Extra: test
-Requires-Dist: pytest>=6.0; extra == "test"
 Description-Content-Type: text/markdown
 
 # small_gicp (fast_gicp2)
 
 **small_gicp** is a header-only C++ library that offers efficient and parallelized algorithms for fine point cloud registration (ICP, Point-to-Plane ICP, GICP, VGICP, etc.). It is a refined and optimized version of its predecessor, [fast_gicp](https://github.com/SMRT-AIST/fast_gicp), re-written from scratch with the following features.
 
-- **Highly Optimized** : The implementation of the core registration algorithm is further optimized from that in fast_gicp. It enables up to **2x speed gain** compared to fast_gicp.
-- **All parallerized** : small_gicp offers parallelized implementations of several preprocessing algorithms to make the entire registration process parallelized (Downsampling, KdTree construction, Normal/covariance estimation). As a parallelism backend, either (or both) [OpenMP](https://www.openmp.org/) and [Intel TBB](https://github.com/oneapi-src/oneTBB) can be used. 
-- **Minimum dependency** : Only [Eigen](https://eigen.tuxfamily.org/) (and bundled [nanoflann](https://github.com/jlblancoc/nanoflann) and [Sophus](https://github.com/strasdat/Sophus)) are required at a minimum. Optionally, it provides the [PCL](https://pointclouds.org/) registration interface so that it can be used as a drop-in replacement in many systems.
+- **Highly Optimized** : The implementation of the core registration algorithm is further optimized from that in fast_gicp. It enables up to **2x speed gain**.
+- **All parallerized** : small_gicp offers parallel implementations of several preprocessing algorithms to make the entire registration process parallelized (Downsampling, KdTree construction, Normal/covariance estimation). As a parallelism backend, either (or both) [OpenMP](https://www.openmp.org/) and [Intel TBB](https://github.com/oneapi-src/oneTBB) can be used. 
+- **Minimum dependency** : Only [Eigen](https://eigen.tuxfamily.org/) (and bundled [nanoflann](https://github.com/jlblancoc/nanoflann) and [Sophus](https://github.com/strasdat/Sophus)) are required at a minimum. Optionally, it provides the [PCL](https://pointclouds.org/) registration interface so that it can be used as a drop-in replacement.
 - **Customizable** : small_gicp allows feeding any custom point cloud class to the registration algorithm via traits. Furthermore, the template-based implementation enables customizing the registration process with your original correspondence estimator and registration factors.
-- **Python bindings** : The isolation from PCL makes small_gicp's python bindings more portable and connectable to other libraries (e.g., Open3D) without problems. 
+- **Python bindings** : The isolation from PCL makes small_gicp's python bindings more portable and usable with other libraries (e.g., Open3D) without problems. 
 
 Note that GPU-based implementations are NOT included in this package.
 
 If you find this package useful for your project, please consider leaving a comment [here](https://github.com/koide3/small_gicp/issues/3). It would help the author receive recognition in his organization and keep working on this project.
 
 
-[![Build(Linux)](https://github.com/koide3/small_gicp/actions/workflows/build-linux.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/build-linux.yml) [![Build(Windows)](https://github.com/koide3/small_gicp/actions/workflows/build-windows.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/build-windows.yml) [![Test](https://github.com/koide3/small_gicp/actions/workflows/test.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/koide3/small_gicp/graph/badge.svg?token=PCVIUP2Z33)](https://codecov.io/gh/koide3/small_gicp)
+[![Build(Linux)](https://github.com/koide3/small_gicp/actions/workflows/build-linux.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/build-linux.yml) [![macos](https://github.com/koide3/small_gicp/actions/workflows/build-macos.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/build-macos.yml) [![Build(Windows)](https://github.com/koide3/small_gicp/actions/workflows/build-windows.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/build-windows.yml) [![Test](https://github.com/koide3/small_gicp/actions/workflows/test.yml/badge.svg)](https://github.com/koide3/small_gicp/actions/workflows/test.yml) [![codecov](https://codecov.io/gh/koide3/small_gicp/graph/badge.svg?token=PCVIUP2Z33)](https://codecov.io/gh/koide3/small_gicp)
 
 ## Requirements
 
 This library uses some C++17 features. The PCL interface is not compatible with PCL older than 1.11 that uses `boost::shared_ptr`.
 
 ## Dependencies
 
-- [Mandatory] [Eigen](https://eigen.tuxfamily.org/), [nanoflann](https://github.com/jlblancoc/nanoflann) ([bundled1](include/small_gicp/ann/nanoflann.hpp), [bundled2](include/small_gicp/ann/nanoflann_omp.hpp), [bundled3](include/small_gicp/ann/nanoflann_tbb.hpp)), [Sophus](https://github.com/strasdat/Sophus) ([bundled](include/small_gicp/util/lie.hpp))
-- [Optional] [OpenMP](https://www.openmp.org/), [Intel TBB](https://www.intel.com/content/www/us/en/developer/tools/oneapi/onetbb.html), [PCL](https://pointclouds.org/), [Iridescence](https://github.com/koide3/iridescence)
+- [Mandatory] [Eigen](https://eigen.tuxfamily.org/), [nanoflann](https://github.com/jlblancoc/nanoflann) ([bundled](include/small_gicp/ann/kdtree.hpp)), [Sophus](https://github.com/strasdat/Sophus) ([bundled](include/small_gicp/util/lie.hpp))
+- [Optional] [OpenMP](https://www.openmp.org/), [Intel TBB](https://www.intel.com/content/www/us/en/developer/tools/oneapi/onetbb.html), [PCL](https://pointclouds.org/)
 
 ## Installation
 
 ### C++
 
 small_gicp is a header-only library. You can just download and drop it in your project directory to use it.
 
@@ -179,16 +177,16 @@
 // Estimate covariances of points.
 const int num_threads = 4;
 const int num_neighbors = 20;
 estimate_covariances_omp(*target, num_neighbors, num_threads);
 estimate_covariances_omp(*source, num_neighbors, num_threads);
 
 // Create KdTree for target and source.
-auto target_tree = std::make_shared<KdTreeOMP<pcl::PointCloud<pcl::PointCovariance>>>(target, num_threads);
-auto source_tree = std::make_shared<KdTreeOMP<pcl::PointCloud<pcl::PointCovariance>>>(source, num_threads);
+auto target_tree = std::make_shared<KdTree<pcl::PointCloud<pcl::PointCovariance>>>(target, KdTreeBuilderOMP(num_threads));
+auto source_tree = std::make_shared<KdTree<pcl::PointCloud<pcl::PointCovariance>>>(source, KdTreeBuilderOMP(num_threads));
 
 Registration<GICPFactor, ParallelReductionOMP> registration;
 registration.reduction.num_threads = num_threads;
 registration.rejector.max_dist_sq = 1.0;
 
 // Align point clouds. Note that the input point clouds are pcl::PointCloud<pcl::PointCovariance>.
 auto result = registration.align(*target, *source, *target_tree, Eigen::Isometry3d::Identity());
@@ -222,16 +220,16 @@
 auto source = std::make_shared<PointCloud>(source_points);
 
 // Downsampling
 target = voxelgrid_sampling_omp(*target, downsampling_resolution, num_threads);
 source = voxelgrid_sampling_omp(*source, downsampling_resolution, num_threads);
 
 // Create KdTree
-auto target_tree = std::make_shared<KdTreeOMP<PointCloud>>(target, num_threads);
-auto source_tree = std::make_shared<KdTreeOMP<PointCloud>>(source, num_threads);
+auto target_tree = std::make_shared<KdTree<PointCloud>>(target, KdTreeBuilderOMP(num_threads));
+auto source_tree = std::make_shared<KdTree<PointCloud>>(source, KdTreeBuilderOMP(num_threads));
 
 // Estimate point covariances
 estimate_covariances_omp(*target, *target_tree, num_neighbors, num_threads);
 estimate_covariances_omp(*source, *source_tree, num_neighbors, num_threads);
 
 // GICP + OMP-based parallel reduction
 Registration<GICPFactor, ParallelReductionOMP> registration;
@@ -261,63 +259,104 @@
 ## Usage (Python) [basic_registration.py](src/example/basic_registration.py)
 
 <details><summary>Expand</summary>
 
 Example A : Perform registration with numpy arrays
 
 ```python
-# Arguments
-# - target_points               : Nx4 or Nx3 numpy array of the target point cloud
-# - source_points               : Nx4 or Nx3 numpy array of the source point cloud
-# Optional arguments
-# - init_T_target_source        : Initial guess of the transformation matrix (4x4 numpy array)
-# - registration_type           : Registration type ("ICP", "PLANE_ICP", "GICP", "VGICP")
-# - voxel_resolution            : Voxel resolution for VGICP
-# - downsampling_resolution     : Downsampling resolution
-# - max_correspondence_distance : Maximum correspondence distance
-# - num_threads                 : Number of threads
+# Align two point clouds using various ICP-like algorithms.
+# 
+# Parameters
+# ----------
+# target_points : NDArray[np.float64]
+#     Nx3 or Nx4 matrix representing the target point cloud.
+# source_points : NDArray[np.float64]
+#     Nx3 or Nx4 matrix representing the source point cloud.
+# init_T_target_source : np.ndarray[np.float64]
+#     4x4 matrix representing the initial transformation from target to source.
+# registration_type : str = 'GICP'
+#     Type of registration algorithm to use ('ICP', 'PLANE_ICP', 'GICP', 'VGICP').
+# voxel_resolution : float = 1.0
+#     Resolution of voxels used for downsampling.
+# downsampling_resolution : float = 0.25
+#     Resolution for downsampling the point clouds.
+# max_correspondence_distance : float = 1.0
+#     Maximum distance for matching points between point clouds.
+# num_threads : int = 1
+#     Number of threads to use for parallel processing.
+# 
+# Returns
+# -------
+# RegistrationResult
+#     Object containing the final transformation matrix and convergence status.
 result = small_gicp.align(target_raw_numpy, source_raw_numpy, downsampling_resolution=0.25)
 
 result.T_target_source  # Estimated transformation (4x4 numpy array)
 result.converged        # If true, the optimization converged successfully
 result.iterations       # Number of iterations the optimization took
 result.num_inliers      # Number of inlier points
 result.H                # Final Hessian matrix (6x6 matrix)
 result.b                # Final information vector (6D vector)
 result.e                # Final error (float)
 ```
 
 Example B : Perform preprocessing and registration separately
 
 ```python
-# Preprocess point clouds
-# Arguments
-# - points                      : Nx4 or Nx3 numpy array of the target point cloud
-# Optional arguments
-# - downsampling_resolution     : Downsampling resolution
-# - num_neighbors               : Number of neighbors for normal and covariance estimation
-# - num_threads                 : Number of threads
+# Preprocess point cloud (downsampling, kdtree construction, and normal/covariance estimation)
+#
+# Parameters
+# ----------
+# points : NDArray[np.float64]
+#     Nx3 or Nx4 matrix representing the point cloud.
+# downsampling_resolution : float = 0.1
+#     Resolution for downsampling the point clouds.
+# num_neighbors : int = 20
+#     Number of neighbor points to usefor point normal/covariance estimation.
+# num_threads : int = 1
+#     Number of threads to use for parallel processing.
+# 
+# Returns
+# -------
+# PointCloud
+#     Downsampled point cloud with estimated normals and covariances.
+# KdTree
+#     KdTree for the downsampled point cloud
 target, target_tree = small_gicp.preprocess_points(target_raw_numpy, downsampling_resolution=0.25)
 source, source_tree = small_gicp.preprocess_points(source_raw_numpy, downsampling_resolution=0.25)
 
 # `target` and `source` are small_gicp.PointCloud with the following methods
 target.size()           # Number of points
 target.points()         # Nx4 numpy array   [x, y, z, 1] x N
 target.normals()        # Nx4 numpy array   [nx, ny, nz, 0] x N
 target.covs()           # Array of 4x4 covariance matrices
 
-# Align point clouds
-# Arguments
-# - target                      : Target point cloud (small_gicp.PointCloud)
-# - source                      : Source point cloud (small_gicp.PointCloud)
-# - target_tree                 : KD-tree of the target point cloud (small_gicp.KdTree)
-# Optional arguments
-# - init_T_target_source        : Initial guess of the transformation matrix (4x4 numpy array)
-# - max_correspondence_distance : Maximum correspondence distance
-# - num_threads                 : Number of threads
+#  Align two point clouds using specified ICP-like algorithms, utilizing point cloud and KD-tree inputs.
+#
+#  Parameters
+#  ----------
+#  target : PointCloud::ConstPtr
+#      Pointer to the target point cloud.
+#  source : PointCloud::ConstPtr
+#      Pointer to the source point cloud.
+#  target_tree : KdTree<PointCloud>::ConstPtr, optional
+#      Pointer to the KD-tree of the target for nearest neighbor search. If nullptr, a new tree is built.
+#  init_T_target_source : NDArray[np.float64]
+#      4x4 matrix representing the initial transformation from target to source.
+#  registration_type : str = 'GICP'
+#      Type of registration algorithm to use ('ICP', 'PLANE_ICP', 'GICP').
+#  max_correspondence_distance : float = 1.0
+#      Maximum distance for corresponding point pairs.
+#  num_threads : int = 1
+#      Number of threads to use for computation.
+# 
+#  Returns
+#  -------
+#  RegistrationResult
+#      Object containing the final transformation matrix and convergence status.
 result = small_gicp.align(target, source, target_tree)
 ```
 
 Example C : Perform each of preprocessing steps one-by-one
 
 ```python
 # Convert numpy arrays (Nx3 or Nx4) to small_gicp.PointCloud
@@ -342,24 +381,29 @@
 
 Example D: Example with Open3D
 
 ```python
 target_o3d = open3d.io.read_point_cloud('small_gicp/data/target.ply').paint_uniform_color([0, 1, 0])
 source_o3d = open3d.io.read_point_cloud('small_gicp/data/source.ply').paint_uniform_color([0, 0, 1])
 
-target, target_tree = small_gicp.preprocess_points(points_numpy=numpy.asarray(target_o3d.points), downsampling_resolution=0.25)
-source, source_tree = small_gicp.preprocess_points(points_numpy=numpy.asarray(source_o3d.points), downsampling_resolution=0.25)
+target, target_tree = small_gicp.preprocess_points(numpy.asarray(target_o3d.points), downsampling_resolution=0.25)
+source, source_tree = small_gicp.preprocess_points(numpy.asarray(source_o3d.points), downsampling_resolution=0.25)
 result = small_gicp.align(target, source, target_tree)
 
 source_o3d.transform(result.T_target_source)
 open3d.visualization.draw_geometries([target_o3d, source_o3d])
 ```
 
 </details>
 
+
+### Cookbook
+
+- [Scan-to-scan and scan-to-model GICP matching odometry on KITTI](src/example/kitti_odometry.py)
+
 ## [Benchmark](BENCHMARK.md)
 
 Processing speed comparison between small_gicp and Open3D ([youtube]((https://youtu.be/LNESzGXPr4c?feature=shared))).
 [![small_comp](https://github.com/koide3/small_gicp/assets/31344317/7959edd6-f0e4-4318-b4c1-a3f8755c407f)](https://youtu.be/LNESzGXPr4c?feature=shared)
 
 ### Downsampling
 
@@ -368,16 +412,17 @@
 - `small_gicp::voxelgrid_sampling` gives accurate downsampling results (almost identical to those of `pcl::VoxelGrid`) while `pcl::ApproximateVoxelGrid` yields spurious points (up to 2x points).
 - `small_gicp::voxelgrid_sampling` can process a larger point cloud with a fine voxel resolution compared to `pcl::VoxelGrid` (for a point cloud of 1000m width, the minimum voxel resolution can be **0.5 mm**).
 
 ![downsampling_comp](docs/assets/downsampling_comp.png)
 
 ### KdTree construction
 
-- Multi-threaded implementation (TBB and OMP) can be up to **4x faster** than the single-threaded one (All the implementations are based on nanoflann).
-- The processing speed gets faster as the number of threads increases, but the speed gain is not monotonic sometimes (because of the scheduling algorithm or some CPU(AMD 5995WX)-specific issues?).
+- Multi-threaded implementation (TBB and OMP) can be up to **6x faster** than the single-threaded one. The single-thread version shows almost equivalent performance with nanoflann.
+- ~~The processing speed gets faster as the number of threads increases, but the speed gain is not monotonic sometimes (because of the scheduling algorithm or some CPU(AMD 5995WX)-specific issues?)~~.
+- The new KdTree implementation shows a good scalability thanks to its well balanced task assignment.
 - This benchmark only compares the construction time (query time is not included). 
 
 ![kdtree_time](docs/assets/kdtree_time.png)
 
 ### Odometry estimation
 
 - Single-thread `small_gicp::GICP` is about **2.4x and 1.9x faster** than `pcl::GICP` and `fast_gicp::GICP`, respectively.
```

