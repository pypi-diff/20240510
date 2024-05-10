# Comparing `tmp/mpi4jax-0.4.1.tar.gz` & `tmp/mpi4jax-0.4.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpi4jax-0.4.1.tar", last modified: Sat May  4 08:54:19 2024, max compression
+gzip compressed data, was "mpi4jax-0.4.1.post1.tar", last modified: Fri May 10 17:01:53 2024, max compression
```

## Comparing `mpi4jax-0.4.1.tar` & `mpi4jax-0.4.1.post1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.740313 mpi4jax-0.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    16700 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/examples/shallow_water.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/mpi4jax/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.744313 mpi4jax-0.4.1/mpi4jax/_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/_latest_jax_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.748313 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/allgather.py
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/allreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/alltoall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/recv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/send.py
--rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/collective_ops/sendrecv.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/flush.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/jax_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.748313 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/device_descriptors.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/device_descriptors.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    22934 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_xpu.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/sycl_runtime_api.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/mpi4jax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.748313 mpi4jax-0.4.1/mpi4jax/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.748313 mpi4jax-0.4.1/mpi4jax/experimental/notoken/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.752313 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/allgather.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/allreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/alltoall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/recv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/send.py
--rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/sendrecv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/mpi4jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 08:54:19.000000 mpi4jax-0.4.1/mpi4jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.752313 mpi4jax-0.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/tests/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_allgather.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_allreduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_allreduce_matvec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_alltoall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_bcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_send_and_recv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/collective_ops/test_sendrecv.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:54:19.756313 mpi4jax-0.4.1/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/experimental/test_notoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_flush.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_has_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_has_sycl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_jax_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    81295 2024-05-04 08:53:11.000000 mpi4jax-0.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.922197 mpi4jax-0.4.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-10 17:01:53.922197 mpi4jax-0.4.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.906197 mpi4jax-0.4.1.post1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    16700 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/examples/shallow_water.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.922197 mpi4jax-0.4.1.post1/mpi4jax/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.910198 mpi4jax-0.4.1.post1/mpi4jax/_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/_latest_jax_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.914198 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/allgather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/recv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11988 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/sendrecv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/flush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/jax_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.914198 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/device_descriptors.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/device_descriptors.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    22934 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    21542 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_xpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/sycl_runtime_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-10 17:01:53.922197 mpi4jax-0.4.1.post1/mpi4jax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.914198 mpi4jax-0.4.1.post1/mpi4jax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.914198 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.918197 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/allgather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/recv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/send.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/sendrecv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.922197 mpi4jax-0.4.1.post1/mpi4jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-05-10 17:01:53.000000 mpi4jax-0.4.1.post1/mpi4jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-10 17:01:53.000000 mpi4jax-0.4.1.post1/mpi4jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:01:53.000000 mpi4jax-0.4.1.post1/mpi4jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:01:53.000000 mpi4jax-0.4.1.post1/mpi4jax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-10 17:01:53.000000 mpi4jax-0.4.1.post1/mpi4jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-10 17:01:53.000000 mpi4jax-0.4.1.post1/mpi4jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-10 17:01:53.922197 mpi4jax-0.4.1.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.918197 mpi4jax-0.4.1.post1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.922197 mpi4jax-0.4.1.post1/tests/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_allgather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_allreduce_matvec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_bcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_send_and_recv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/collective_ops/test_sendrecv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:01:53.922197 mpi4jax-0.4.1.post1/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/experimental/test_notoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/test_flush.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/test_has_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/test_has_sycl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/test_jax_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81295 2024-05-10 17:00:37.000000 mpi4jax-0.4.1.post1/versioneer.py
```

### Comparing `mpi4jax-0.4.1/LICENSE.md` & `mpi4jax-0.4.1.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/PKG-INFO` & `mpi4jax-0.4.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpi4jax
-Version: 0.4.1
+Version: 0.4.1.post1
 Summary: Zero-copy MPI communication of JAX arrays, for turbo-charged HPC applications in Python ⚡
 Home-page: https://github.com/mpi4jax/mpi4jax
 Author: Filippo Vicentini
 Author-email: filippovicentini@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
```

### Comparing `mpi4jax-0.4.1/README.rst` & `mpi4jax-0.4.1.post1/README.rst`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/examples/shallow_water.py` & `mpi4jax-0.4.1.post1/examples/shallow_water.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/__init__.py` & `mpi4jax-0.4.1.post1/mpi4jax/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/__init__.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/allgather.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/allgather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/allreduce.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/allreduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/alltoall.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/alltoall.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/barrier.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/barrier.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/bcast.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/bcast.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/gather.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/gather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/recv.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/recv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/reduce.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/reduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/scan.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/scan.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/scatter.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/scatter.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/send.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/send.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/collective_ops/sendrecv.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/collective_ops/sendrecv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/decorators.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/decorators.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/jax_compat.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/jax_compat.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/utils.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/utils.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/validation.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/validation.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/__init__.py` & `mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd` & `mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/device_descriptors.pxd` & `mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/device_descriptors.pxd`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/device_descriptors.pyx` & `mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/device_descriptors.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd` & `mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx` & `mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx` & `mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx` & `mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_xpu.pyx` & `mpi4jax-0.4.1.post1/mpi4jax/_src/xla_bridge/mpi_xla_bridge_xpu.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/__init__.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/allgather.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/allgather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/allreduce.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/allreduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/alltoall.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/alltoall.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/barrier.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/barrier.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/bcast.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/bcast.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/gather.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/gather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/recv.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/recv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/reduce.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/reduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/scan.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/scan.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/scatter.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/scatter.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/send.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/send.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax/experimental/notoken/collective_ops/sendrecv.py` & `mpi4jax-0.4.1.post1/mpi4jax/experimental/notoken/collective_ops/sendrecv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/mpi4jax.egg-info/PKG-INFO` & `mpi4jax-0.4.1.post1/mpi4jax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpi4jax
-Version: 0.4.1
+Version: 0.4.1.post1
 Summary: Zero-copy MPI communication of JAX arrays, for turbo-charged HPC applications in Python ⚡
 Home-page: https://github.com/mpi4jax/mpi4jax
 Author: Filippo Vicentini
 Author-email: filippovicentini@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
```

### Comparing `mpi4jax-0.4.1/mpi4jax.egg-info/SOURCES.txt` & `mpi4jax-0.4.1.post1/mpi4jax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/pyproject.toml` & `mpi4jax-0.4.1.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/setup.py` & `mpi4jax-0.4.1.post1/setup.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_allgather.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_allgather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_allreduce.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_allreduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_allreduce_matvec.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_allreduce_matvec.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_alltoall.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_alltoall.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_barrier.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_barrier.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_bcast.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_bcast.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_common.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_common.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_gather.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_gather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_reduce.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_reduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_scan.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_scan.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_scatter.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_scatter.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_send_and_recv.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_send_and_recv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/collective_ops/test_sendrecv.py` & `mpi4jax-0.4.1.post1/tests/collective_ops/test_sendrecv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/experimental/test_notoken.py` & `mpi4jax-0.4.1.post1/tests/experimental/test_notoken.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/test_decorators.py` & `mpi4jax-0.4.1.post1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/test_jax_compat.py` & `mpi4jax-0.4.1.post1/tests/test_jax_compat.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/tests/test_validation.py` & `mpi4jax-0.4.1.post1/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.4.1/versioneer.py` & `mpi4jax-0.4.1.post1/versioneer.py`

 * *Files identical despite different names*

