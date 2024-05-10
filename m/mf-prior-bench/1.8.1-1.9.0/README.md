# Comparing `tmp/mf-prior-bench-1.8.1.tar.gz` & `tmp/mf_prior_bench-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mf-prior-bench-1.8.1.tar", last modified: Tue Dec 19 13:40:52 2023, max compression
+gzip compressed data, was "mf_prior_bench-1.9.0.tar", last modified: Fri May 10 09:39:47 2024, max compression
```

## Comparing `mf-prior-bench-1.8.1.tar` & `mf_prior_bench-1.9.0.tar`

### file list

```diff
@@ -1,702 +1,721 @@
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.206063 mf-prior-bench-1.8.1/
--rw-r--r--   0 skantify  (1000) skantify  (1000)    11355 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/LICENSE.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)      308 2023-09-11 06:16:14.000000 mf-prior-bench-1.8.1/MANIFEST.in
--rw-r--r--   0 skantify  (1000) skantify  (1000)    15143 2023-12-19 13:40:52.202730 mf-prior-bench-1.8.1/PKG-INFO
--rw-r--r--   0 skantify  (1000) skantify  (1000)      127 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/README.md
--rw-r--r--   0 skantify  (1000) skantify  (1000)     6046 2023-12-19 13:40:31.000000 mf-prior-bench-1.8.1/pyproject.toml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       38 2023-12-19 13:40:52.206063 mf-prior-bench-1.8.1/setup.cfg
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.049395 mf-prior-bench-1.8.1/src/
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.199396 mf-prior-bench-1.8.1/src/mf_prior_bench.egg-info/
--rw-r--r--   0 skantify  (1000) skantify  (1000)    15143 2023-12-19 13:40:52.000000 mf-prior-bench-1.8.1/src/mf_prior_bench.egg-info/PKG-INFO
--rw-r--r--   0 skantify  (1000) skantify  (1000)    27724 2023-12-19 13:40:52.000000 mf-prior-bench-1.8.1/src/mf_prior_bench.egg-info/SOURCES.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)        1 2023-12-19 13:40:52.000000 mf-prior-bench-1.8.1/src/mf_prior_bench.egg-info/dependency_links.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)      418 2023-12-19 13:40:52.000000 mf-prior-bench-1.8.1/src/mf_prior_bench.egg-info/requires.txt
--rw-r--r--   0 skantify  (1000) skantify  (1000)       29 2023-12-19 13:40:52.000000 mf-prior-bench-1.8.1/src/mf_prior_bench.egg-info/top_level.txt
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.052729 mf-prior-bench-1.8.1/src/mfpbench/
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2607 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/__init__.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)    10274 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/__main__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.062729 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2074 2023-12-19 13:38:00.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5395 2023-01-17 18:00:17.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     8555 2023-09-11 05:17:42.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/__main__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5571 2023-01-18 23:57:37.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/__main__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)    13287 2023-12-19 13:38:00.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/benchmark.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     6513 2023-02-21 11:38:36.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/benchmark.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     8862 2023-12-19 13:38:00.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     7579 2023-02-21 11:37:18.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     8905 2023-09-07 11:40:45.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/download.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5358 2023-01-17 17:54:08.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/download.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5820 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/get.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5493 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/metric.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     4729 2023-09-11 05:17:42.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/priors.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3900 2023-01-18 23:57:38.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/priors.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3914 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/result.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2660 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/result.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5244 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/resultframe.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5149 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/resultframe.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)    12409 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/setup_benchmark.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2588 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/stats.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2532 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/stats.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)    14871 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/tabular.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)    14675 2023-09-06 17:46:17.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/tabular_benchmark.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     7358 2023-11-24 10:16:37.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/util.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     6910 2023-01-27 15:16:35.000000 mf-prior-bench-1.8.1/src/mfpbench/__pycache__/util.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)    15923 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/benchmark.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     8441 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/config.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)    11466 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/correlations.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     6066 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/get.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.062729 mf-prior-bench-1.8.1/src/mfpbench/jahs/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.066062 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      296 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      474 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     8033 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/benchmark.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     7940 2023-02-21 11:37:18.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/benchmark.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1665 2023-08-24 14:38:12.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1667 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1747 2023-09-06 17:46:17.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/result.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1885 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/result.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3628 2023-09-06 17:46:17.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/spaces.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3458 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/spaces.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)    10960 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/jahs/benchmark.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.066062 mf-prior-bench-1.8.1/src/mfpbench/lcbench_tabular/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      270 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/lcbench_tabular/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.066062 mf-prior-bench-1.8.1/src/mfpbench/lcbench_tabular/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      394 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/lcbench_tabular/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     7062 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/lcbench_tabular/__pycache__/benchmark.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     9870 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/lcbench_tabular/benchmark.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5098 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/metric.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.069395 mf-prior-bench-1.8.1/src/mfpbench/pd1/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      445 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.069395 mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      484 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      496 2023-01-17 17:54:08.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     7375 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/benchmark.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     7051 2023-02-21 11:37:19.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/benchmark.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      649 2023-09-06 11:06:32.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      641 2023-01-18 22:45:33.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2890 2023-09-06 17:46:17.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/result.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2829 2023-01-27 15:16:36.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/result.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     7104 2023-12-19 13:40:01.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmark.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.072728 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      538 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.072728 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      625 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      633 2023-01-17 17:54:08.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1237 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/cifar100.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2060 2023-01-27 15:16:36.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/cifar100.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1222 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/imagenet.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2035 2023-01-18 19:57:06.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/imagenet.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1224 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/lm1b.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2040 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/lm1b.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1240 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/translate_wmt.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2072 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/translate_wmt.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1237 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/uniref50.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2060 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/uniref50.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1318 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/cifar100.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1306 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/imagenet.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1324 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/lm1b.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1344 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/translate_wmt.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1346 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/uniref50.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.072728 mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/
--rw-r--r--   0 skantify  (1000) skantify  (1000)        0 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.076062 mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      161 2023-01-16 15:42:15.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     4542 2023-01-17 16:48:50.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/__pycache__/columns.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     8996 2023-01-17 17:23:34.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/__pycache__/process_script.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     6635 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/columns.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)    13226 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/process_script.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.076062 mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/
--rw-r--r--   0 skantify  (1000) skantify  (1000)        0 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.079395 mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      160 2023-01-17 17:54:08.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5014 2023-01-17 17:54:08.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/__pycache__/training.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1038 2023-01-17 17:54:24.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/__pycache__/xgboost_space.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3243 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/train_xgboost.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     6767 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/training.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1853 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/xgboost_space.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5580 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/priors.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3380 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/result.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     4590 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/resultframe.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)    12570 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/setup_benchmark.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2389 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/stats.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.079395 mf-prior-bench-1.8.1/src/mfpbench/synthetic/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      963 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.079395 mf-prior-bench-1.8.1/src/mfpbench/synthetic/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      820 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      944 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.079395 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1028 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.082729 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      891 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1111 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     8246 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/benchmark.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)    10827 2023-02-21 11:37:19.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/benchmark.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1652 2023-09-06 11:27:34.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1574 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5251 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/generators.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5468 2023-01-16 15:30:59.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/generators.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1834 2023-08-24 14:40:54.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/result.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1805 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/result.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     7935 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/benchmark.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5882 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/generators.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)    18429 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/tabular.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     8553 2023-11-13 07:28:25.000000 mf-prior-bench-1.8.1/src/mfpbench/util.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.082729 mf-prior-bench-1.8.1/src/mfpbench/yahpo/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      829 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.086062 mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      761 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      809 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)    10149 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/benchmark.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     7604 2023-02-21 11:37:19.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/benchmark.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      572 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/config.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      564 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      646 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/result.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      638 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/result.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)    12688 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmark.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.086062 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      967 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.089395 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      903 2023-09-11 05:17:40.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      955 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2460 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/lcbench.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3857 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/lcbench.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     4160 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/nb301.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     5936 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/nb301.cpython-38.pyc
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.089395 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      938 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.092729 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      937 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1156 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2963 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3478 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      937 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_glmnet.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1461 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_glmnet.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1245 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_ranger.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2003 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_ranger.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)      983 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_rpart.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1572 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_rpart.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2283 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_super.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     4643 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_super.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1499 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_xgboost.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2700 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_xgboost.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2698 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)      513 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml_glmnet.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)      769 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml_ranger.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)      547 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml_rpart.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1968 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml_super.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1071 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml_xgboost.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2821 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/lcbench.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3927 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/nb301.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.092729 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1227 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__init__.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.099396 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1168 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1470 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3016 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3446 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1822 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_aknn.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2977 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_aknn.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1722 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_glmnet.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2764 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_glmnet.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2009 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_ranger.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3301 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_ranger.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1782 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_rpart.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2897 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_rpart.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3364 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_super.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     6806 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_super.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     1856 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_svm.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3124 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_svm.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2287 2023-12-19 13:38:01.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_xgboost.cpython-310.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     4009 2023-01-11 23:02:12.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_xgboost.cpython-38.pyc
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2544 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2597 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_aknn.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2489 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_glmnet.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2777 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_ranger.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2563 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_rpart.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     4804 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_super.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     2720 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_svm.py
--rw-r--r--   0 skantify  (1000) skantify  (1000)     3337 2023-12-05 15:34:32.000000 mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_xgboost.py
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.199396 mf-prior-bench-1.8.1/src/priors/
--rw-r--r--   0 skantify  (1000) skantify  (1000)      127 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/cifar100-wide_resnet-2048-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      137 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/cifar100-wide_resnet-2048-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      129 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/cifar100-wide_resnet-2048-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       74 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/cifar100-wide_resnet-2048-gpt.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      129 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/cifar100-wide_resnet-2048-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       47 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/iaml_glmnet-1067-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       52 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/iaml_glmnet-1489-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       52 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/iaml_glmnet-40981-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       51 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/iaml_glmnet-41146-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       64 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/iaml_rpart-1067-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       65 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/iaml_rpart-1489-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       65 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/iaml_rpart-40981-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       67 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/iaml_rpart-41146-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/imagenet-resnet-512-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      134 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/imagenet-resnet-512-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      130 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/imagenet-resnet-512-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       77 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/imagenet-resnet-512-gpt.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      129 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/imagenet-resnet-512-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      191 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_CIFAR10-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      189 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_CIFAR10-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      191 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_CIFAR10-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      190 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_CIFAR10-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      194 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_ColorectalHistology-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      190 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_ColorectalHistology-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      192 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_ColorectalHistology-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      192 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_ColorectalHistology-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      192 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_FashionMNIST-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      191 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_FashionMNIST-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      191 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_FashionMNIST-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      192 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/jahs_FashionMNIST-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-126025-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-126026-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      180 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-126026-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-126026-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      117 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-126026-gpt.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-126026-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-126029-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      179 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-146212-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      175 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167104-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      175 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167149-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167152-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167161-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167168-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167181-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167184-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167185-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167190-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      180 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167190-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      173 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167190-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      117 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167190-gpt.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      174 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167190-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167200-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-167201-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168329-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168330-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      173 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168330-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168330-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      117 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168330-gpt.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168330-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168331-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168335-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168868-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168908-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168910-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      175 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168910-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168910-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      117 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168910-gpt.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-168910-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189354-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189862-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      175 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189865-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189866-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189873-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189905-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189906-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      182 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189906-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189906-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      117 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189906-gpt.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189906-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189908-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-189909-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-34539-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-3945-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      179 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lcbench-7593-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      134 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lm1b-transformer-2048-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      138 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lm1b-transformer-2048-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lm1b-transformer-2048-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       78 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lm1b-transformer-2048-gpt.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/lm1b-transformer-2048-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       71 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_bad-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       72 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_bad-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_bad-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_bad-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       71 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_good-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       72 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_good-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       42 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_good-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_good-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       71 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_moderate-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       72 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_moderate-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_moderate-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_moderate-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       71 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_terrible-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       72 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_terrible-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       42 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_terrible-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh3_terrible-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      143 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_bad-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      145 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_bad-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      147 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_bad-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      149 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_bad-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      143 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_good-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      145 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_good-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       81 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_good-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      146 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_good-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      143 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_moderate-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      145 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_moderate-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      147 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_moderate-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      149 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_moderate-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      143 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_terrible-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      145 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_terrible-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       81 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_terrible-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      146 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/mfh6_terrible-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1040-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1049-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1050-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1053-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1056-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1063-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1067-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1068-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-11-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1111-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-12-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1220-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-14-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1457-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1461-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1462-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1464-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1468-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1475-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1476-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1478-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1479-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1480-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1485-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1486-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1487-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1489-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1493-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1494-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1497-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-15-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1501-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-151-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1510-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1515-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-1590-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-16-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-18-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-181-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-182-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-188-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-22-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-23-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-23381-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-23512-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-23517-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-24-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-28-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-29-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-3-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-300-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-307-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-31-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-312-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-32-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-334-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-37-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-375-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-377-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-38-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40496-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40498-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40499-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40536-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40668-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40670-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40685-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40701-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40900-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40923-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40927-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40966-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40975-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40978-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40979-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40981-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40982-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40983-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40984-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40994-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-40996-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41027-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41138-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41142-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41143-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41146-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41150-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41156-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41157-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41159-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41161-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41162-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41163-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       90 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41164-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41165-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41166-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41168-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41169-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41212-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41216-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-41278-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-4134-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-4154-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-42-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-44-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-4534-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-4538-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-4541-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-458-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-46-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       90 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-469-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-470-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-50-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-54-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-554-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-6-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-60-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_aknn-6332-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1040-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1049-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1050-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1053-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1056-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1063-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1067-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1068-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-11-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1111-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-12-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1220-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-14-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1457-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1461-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1462-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1464-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1468-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1475-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1476-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1478-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1479-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1480-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       90 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1485-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1486-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1487-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1489-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1493-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1494-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1497-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-15-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1501-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-151-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1510-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1515-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-1590-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-16-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-18-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-181-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-182-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-188-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-22-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-23-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-23381-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-23512-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-23517-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-24-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-28-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-29-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-3-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-300-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-307-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-31-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-312-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-32-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       84 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-334-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-37-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-375-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-377-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-38-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40496-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40498-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40499-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40536-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40668-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40670-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40685-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40701-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40900-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40966-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40975-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40978-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40979-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40981-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40982-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40983-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40984-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-40994-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41027-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41138-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41142-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41143-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41146-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41150-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41156-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41157-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41159-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41161-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41162-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41163-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41164-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41166-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41168-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41169-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41212-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41216-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-41278-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-4134-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-4135-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-4154-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-42-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-44-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-4534-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-4538-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-4541-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-458-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-46-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-469-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-470-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-50-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-54-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-554-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-6-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-60-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_glmnet-6332-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1040-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1049-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1050-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1053-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       99 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1056-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1063-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1067-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1068-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-11-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1111-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-12-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1220-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-14-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1457-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1461-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1462-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1464-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1468-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1475-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1476-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1478-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1479-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1480-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1485-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1486-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1487-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1489-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1493-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1494-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1497-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       99 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-15-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1501-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-151-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1510-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1515-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-1590-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-16-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-18-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-181-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-182-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-188-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-22-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-23-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-23381-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-23512-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-23517-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-24-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-28-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-29-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-3-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-300-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-307-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-31-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-312-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-32-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-334-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-37-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-375-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-377-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-38-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40496-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40498-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40499-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40536-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40668-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40670-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40685-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40701-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40900-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40923-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40927-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40966-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40975-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40978-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40979-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40981-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40982-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      100 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40983-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40984-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40994-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-40996-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41027-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41138-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41142-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41143-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41146-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41150-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41156-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41157-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41159-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41161-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41162-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41163-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41164-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41165-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41166-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41168-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41169-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-41212-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       99 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-4134-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-4135-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       99 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-4154-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-42-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-44-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      100 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-4534-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-4538-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-4541-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-458-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-46-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-469-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-470-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-50-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-54-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-554-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-6-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-60-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/rbv2_rpart-6332-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      128 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/translate_wmt-xformer_translate-64-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      136 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/translate_wmt-xformer_translate-64-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      130 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/translate_wmt-xformer_translate-64-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)       81 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/translate_wmt-xformer_translate-64-gpt.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/translate_wmt-xformer_translate-64-medium.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      129 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/uniref50-transformer-128-at25.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/uniref50-transformer-128-bad.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      132 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/uniref50-transformer-128-good.yaml
--rw-r--r--   0 skantify  (1000) skantify  (1000)      125 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/priors/uniref50-transformer-128-medium.yaml
-drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2023-12-19 13:40:52.199396 mf-prior-bench-1.8.1/src/requirements/
--rw-r--r--   0 skantify  (1000) skantify  (1000)        5 2023-09-11 05:16:51.000000 mf-prior-bench-1.8.1/src/requirements/yahpo.txt
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.227407 mf_prior_bench-1.9.0/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    11355 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/LICENSE.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      308 2023-09-11 06:16:14.000000 mf_prior_bench-1.9.0/MANIFEST.in
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    15143 2024-05-10 09:39:47.227407 mf_prior_bench-1.9.0/PKG-INFO
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      127 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/README.md
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     6046 2024-05-10 09:38:41.000000 mf_prior_bench-1.9.0/pyproject.toml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       38 2024-05-10 09:39:47.227407 mf_prior_bench-1.9.0/setup.cfg
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.070741 mf_prior_bench-1.9.0/src/
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.224074 mf_prior_bench-1.9.0/src/mf_prior_bench.egg-info/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    15143 2024-05-10 09:39:47.000000 mf_prior_bench-1.9.0/src/mf_prior_bench.egg-info/PKG-INFO
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    28464 2024-05-10 09:39:47.000000 mf_prior_bench-1.9.0/src/mf_prior_bench.egg-info/SOURCES.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        1 2024-05-10 09:39:47.000000 mf_prior_bench-1.9.0/src/mf_prior_bench.egg-info/dependency_links.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      418 2024-05-10 09:39:47.000000 mf_prior_bench-1.9.0/src/mf_prior_bench.egg-info/requires.txt
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       29 2024-05-10 09:39:47.000000 mf_prior_bench-1.9.0/src/mf_prior_bench.egg-info/top_level.txt
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.077407 mf_prior_bench-1.9.0/src/mfpbench/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2607 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/__init__.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    10274 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/__main__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.084074 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2074 2023-12-19 13:38:00.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5395 2023-01-17 18:00:17.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     8555 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/__main__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5571 2023-01-18 23:57:37.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/__main__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    13287 2024-05-10 09:36:02.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/benchmark.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     6513 2023-02-21 11:38:36.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/benchmark.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     8862 2023-12-19 13:38:00.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     7579 2023-02-21 11:37:18.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     8905 2023-09-07 11:40:45.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/download.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5358 2023-01-17 17:54:08.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/download.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5820 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/get.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5493 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/metric.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4729 2023-09-11 05:17:42.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/priors.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3900 2023-01-18 23:57:38.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/priors.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3914 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/result.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2660 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/result.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5244 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/resultframe.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5149 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/resultframe.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    12409 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/setup_benchmark.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2588 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/stats.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2532 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/stats.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    14871 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/tabular.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    14675 2023-09-06 17:46:17.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/tabular_benchmark.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     7358 2023-11-24 10:16:37.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     6910 2023-01-27 15:16:35.000000 mf_prior_bench-1.9.0/src/mfpbench/__pycache__/util.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    15923 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/benchmark.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     8441 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/config.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    11466 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/correlations.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     6066 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/get.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.084074 mf_prior_bench-1.9.0/src/mfpbench/jahs/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.087407 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      296 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      474 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     8031 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/benchmark.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     7940 2023-02-21 11:37:18.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/benchmark.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1665 2023-08-24 14:38:12.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1667 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1747 2023-09-06 17:46:17.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/result.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1885 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/result.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3628 2023-09-06 17:46:17.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/spaces.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3458 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/spaces.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    10952 2024-05-10 09:35:44.000000 mf_prior_bench-1.9.0/src/mfpbench/jahs/benchmark.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.087407 mf_prior_bench-1.9.0/src/mfpbench/lcbench_tabular/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      270 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/lcbench_tabular/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.087407 mf_prior_bench-1.9.0/src/mfpbench/lcbench_tabular/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      394 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/lcbench_tabular/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     7062 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/lcbench_tabular/__pycache__/benchmark.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     9870 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/lcbench_tabular/benchmark.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5098 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/metric.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.067407 mf_prior_bench-1.9.0/src/mfpbench/nb201_tabular/
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.090741 mf_prior_bench-1.9.0/src/mfpbench/nb201_tabular/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      166 2024-01-25 19:38:33.000000 mf_prior_bench-1.9.0/src/mfpbench/nb201_tabular/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5738 2024-02-01 14:56:57.000000 mf_prior_bench-1.9.0/src/mfpbench/nb201_tabular/__pycache__/benchmark.cpython-310.pyc
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.090741 mf_prior_bench-1.9.0/src/mfpbench/pd1/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      445 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.090741 mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      484 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      496 2023-01-17 17:54:08.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     7396 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/benchmark.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     7051 2023-02-21 11:37:19.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/benchmark.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      649 2023-09-06 11:06:32.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      641 2023-01-18 22:45:33.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2890 2023-09-06 17:46:17.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/result.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2829 2023-01-27 15:16:36.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/result.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     7166 2024-05-10 09:35:44.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmark.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.094074 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      538 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.097407 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      625 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      633 2023-01-17 17:54:08.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1238 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/cifar100.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2060 2023-01-27 15:16:36.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/cifar100.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1222 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/imagenet.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2035 2023-01-18 19:57:06.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/imagenet.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1224 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/lm1b.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2040 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/lm1b.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1250 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/translate_wmt.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2072 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/translate_wmt.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1237 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/uniref50.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2060 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/uniref50.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1318 2024-05-10 09:35:44.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/cifar100.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1306 2024-05-10 09:35:44.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/imagenet.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1324 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/lm1b.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1354 2024-05-10 09:35:44.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/translate_wmt.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1346 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/uniref50.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.097407 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        0 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.097407 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      167 2024-02-01 12:57:22.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      161 2023-01-16 15:42:15.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5224 2024-02-01 12:57:22.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/__pycache__/columns.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4542 2023-01-17 16:48:50.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/__pycache__/columns.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    12836 2024-02-01 12:57:22.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/__pycache__/process_script.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     8996 2023-01-17 17:23:34.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/__pycache__/process_script.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     6635 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/columns.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    13226 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/process_script.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.100741 mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        0 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.100741 mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      160 2023-01-17 17:54:08.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5014 2023-01-17 17:54:08.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/__pycache__/training.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1038 2023-01-17 17:54:24.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/__pycache__/xgboost_space.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3243 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/train_xgboost.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     6767 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/training.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1853 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/xgboost_space.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.067407 mf_prior_bench-1.9.0/src/mfpbench/pd1_tabular/
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.100741 mf_prior_bench-1.9.0/src/mfpbench/pd1_tabular/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      423 2024-01-19 10:32:58.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1_tabular/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4446 2024-02-01 15:35:02.000000 mf_prior_bench-1.9.0/src/mfpbench/pd1_tabular/__pycache__/benchmark.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5580 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/priors.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3380 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/result.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4590 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/resultframe.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    12570 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/setup_benchmark.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2389 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/stats.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.104074 mf_prior_bench-1.9.0/src/mfpbench/synthetic/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      963 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.104074 mf_prior_bench-1.9.0/src/mfpbench/synthetic/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      820 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      944 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.104074 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1028 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.107407 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      891 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1111 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     8241 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/benchmark.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    10827 2023-02-21 11:37:19.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/benchmark.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1652 2023-09-06 11:27:34.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1574 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5251 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/generators.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5468 2023-01-16 15:30:59.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/generators.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1834 2023-08-24 14:40:54.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/result.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1805 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/result.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     7935 2024-05-10 09:35:44.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/benchmark.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5882 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/generators.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    18429 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/tabular.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.070741 mf_prior_bench-1.9.0/src/mfpbench/taskset_tabular/
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.107407 mf_prior_bench-1.9.0/src/mfpbench/taskset_tabular/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      360 2024-01-24 12:49:55.000000 mf_prior_bench-1.9.0/src/mfpbench/taskset_tabular/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    23736 2024-02-01 16:05:53.000000 mf_prior_bench-1.9.0/src/mfpbench/taskset_tabular/__pycache__/benchmark.cpython-310.pyc
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.070741 mf_prior_bench-1.9.0/src/mfpbench/taskset_tabular/processing/
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.107407 mf_prior_bench-1.9.0/src/mfpbench/taskset_tabular/processing/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      179 2024-01-19 10:32:58.000000 mf_prior_bench-1.9.0/src/mfpbench/taskset_tabular/processing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     9764 2024-01-19 18:32:33.000000 mf_prior_bench-1.9.0/src/mfpbench/taskset_tabular/processing/__pycache__/process.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     8553 2023-11-13 07:28:25.000000 mf_prior_bench-1.9.0/src/mfpbench/util.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.110741 mf_prior_bench-1.9.0/src/mfpbench/yahpo/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      829 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.110741 mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      761 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      809 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    10149 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/benchmark.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     7604 2023-02-21 11:37:19.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/benchmark.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      572 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      564 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      646 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/result.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      638 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/result.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)    12688 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmark.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.110741 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      967 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.114074 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      903 2023-09-11 05:17:40.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      955 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2460 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/lcbench.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3857 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/lcbench.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4160 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/nb301.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     5936 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/nb301.cpython-38.pyc
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.114074 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      938 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.117407 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      937 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1156 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2963 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3478 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      937 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_glmnet.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1461 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_glmnet.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1245 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_ranger.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2003 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_ranger.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      983 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_rpart.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1572 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_rpart.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2283 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_super.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4643 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_super.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1499 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_xgboost.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2700 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_xgboost.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2698 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      513 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml_glmnet.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      769 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml_ranger.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      547 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml_rpart.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1968 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml_super.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1071 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml_xgboost.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2821 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/lcbench.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3927 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/nb301.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.120741 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1227 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__init__.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.124074 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1168 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1470 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3016 2024-05-10 09:36:03.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3446 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1822 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_aknn.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2977 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_aknn.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1722 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_glmnet.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2764 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_glmnet.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2009 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_ranger.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3301 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_ranger.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1782 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_rpart.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2897 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_rpart.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3364 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_super.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     6806 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_super.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     1856 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_svm.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3124 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_svm.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2287 2023-12-19 13:38:01.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_xgboost.cpython-310.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4009 2023-01-11 23:02:12.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_xgboost.cpython-38.pyc
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2544 2024-05-10 09:35:41.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2597 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_aknn.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2489 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_glmnet.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2777 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_ranger.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2563 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_rpart.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     4804 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_super.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     2720 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_svm.py
+-rw-r--r--   0 skantify  (1000) skantify  (1000)     3337 2023-12-05 15:34:32.000000 mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_xgboost.py
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.224074 mf_prior_bench-1.9.0/src/priors/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      127 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/cifar100-wide_resnet-2048-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      137 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/cifar100-wide_resnet-2048-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      129 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/cifar100-wide_resnet-2048-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       74 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/cifar100-wide_resnet-2048-gpt.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      129 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/cifar100-wide_resnet-2048-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       47 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/iaml_glmnet-1067-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       52 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/iaml_glmnet-1489-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       52 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/iaml_glmnet-40981-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       51 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/iaml_glmnet-41146-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       64 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/iaml_rpart-1067-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       65 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/iaml_rpart-1489-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       65 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/iaml_rpart-40981-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       67 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/iaml_rpart-41146-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/imagenet-resnet-512-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      134 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/imagenet-resnet-512-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      130 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/imagenet-resnet-512-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       77 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/imagenet-resnet-512-gpt.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      129 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/imagenet-resnet-512-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      191 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_CIFAR10-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      189 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_CIFAR10-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      191 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_CIFAR10-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      190 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_CIFAR10-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      194 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_ColorectalHistology-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      190 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_ColorectalHistology-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      192 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_ColorectalHistology-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      192 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_ColorectalHistology-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      192 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_FashionMNIST-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      191 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_FashionMNIST-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      191 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_FashionMNIST-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      192 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/jahs_FashionMNIST-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-126025-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-126026-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      180 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-126026-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-126026-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      117 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-126026-gpt.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-126026-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-126029-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      179 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-146212-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      175 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167104-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      175 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167149-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167152-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167161-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167168-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167181-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167184-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167185-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167190-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      180 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167190-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      173 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167190-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      117 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167190-gpt.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      174 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167190-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167200-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-167201-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168329-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168330-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      173 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168330-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168330-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      117 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168330-gpt.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168330-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168331-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168335-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168868-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168908-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168910-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      175 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168910-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168910-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      117 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168910-gpt.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-168910-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189354-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189862-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      175 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189865-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189866-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189873-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189905-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      176 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189906-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      182 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189906-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189906-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      117 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189906-gpt.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189906-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189908-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      178 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-189909-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-34539-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      177 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-3945-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      179 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lcbench-7593-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      134 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lm1b-transformer-2048-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      138 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lm1b-transformer-2048-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lm1b-transformer-2048-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       78 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lm1b-transformer-2048-gpt.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/lm1b-transformer-2048-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       71 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_bad-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       72 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_bad-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_bad-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_bad-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       71 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_good-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       72 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_good-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       42 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_good-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_good-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       71 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_moderate-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       72 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_moderate-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_moderate-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_moderate-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       71 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_terrible-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       72 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_terrible-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       42 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_terrible-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       73 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh3_terrible-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      143 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_bad-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      145 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_bad-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      147 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_bad-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      149 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_bad-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      143 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_good-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      145 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_good-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       81 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_good-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      146 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_good-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      143 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_moderate-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      145 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_moderate-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      147 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_moderate-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      149 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_moderate-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      143 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_terrible-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      145 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_terrible-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       81 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_terrible-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      146 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/mfh6_terrible-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1040-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1049-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1050-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1053-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1056-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1063-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1067-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1068-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-11-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1111-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-12-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1220-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-14-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1457-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1461-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1462-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1464-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1468-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1475-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1476-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1478-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1479-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1480-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1485-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1486-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1487-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1489-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1493-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1494-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1497-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-15-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1501-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-151-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1510-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1515-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-1590-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-16-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-18-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-181-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-182-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-188-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-22-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-23-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-23381-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-23512-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-23517-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-24-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-28-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-29-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-3-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-300-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-307-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-31-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-312-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-32-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-334-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-37-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-375-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-377-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-38-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40496-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40498-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40499-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40536-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40668-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40670-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40685-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40701-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40900-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40923-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40927-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40966-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40975-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40978-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40979-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40981-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40982-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40983-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40984-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40994-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-40996-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41027-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41138-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41142-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41143-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41146-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41150-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41156-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41157-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41159-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41161-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       96 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41162-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41163-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       90 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41164-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41165-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41166-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41168-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41169-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41212-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41216-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-41278-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-4134-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-4154-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-42-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-44-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-4534-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-4538-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       91 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-4541-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-458-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-46-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       90 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-469-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       95 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-470-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-50-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-54-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       93 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-554-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       92 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-6-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-60-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_aknn-6332-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1040-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1049-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1050-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1053-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1056-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1063-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1067-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1068-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-11-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1111-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-12-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1220-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-14-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1457-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1461-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1462-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1464-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1468-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1475-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1476-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1478-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1479-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1480-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       90 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1485-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1486-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1487-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1489-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1493-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1494-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1497-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-15-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1501-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-151-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1510-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1515-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-1590-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-16-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-18-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-181-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-182-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-188-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-22-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-23-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-23381-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-23512-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-23517-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-24-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-28-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-29-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-3-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-300-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-307-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-31-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-312-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-32-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       84 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-334-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-37-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-375-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-377-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-38-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40496-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       89 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40498-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40499-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40536-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40668-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40670-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40685-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40701-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40900-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40966-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40975-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40978-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40979-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40981-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40982-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40983-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40984-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-40994-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41027-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41138-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41142-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41143-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41146-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41150-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41156-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41157-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41159-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41161-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41162-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41163-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41164-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41166-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41168-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41169-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41212-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41216-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-41278-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-4134-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-4135-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-4154-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       86 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-42-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-44-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-4534-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-4538-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-4541-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-458-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-46-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-469-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-470-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-50-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-54-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-554-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-6-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       87 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-60-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       88 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_glmnet-6332-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1040-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1049-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1050-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1053-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       99 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1056-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1063-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1067-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1068-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-11-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1111-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-12-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1220-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-14-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1457-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1461-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1462-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1464-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1468-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1475-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1476-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1478-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1479-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1480-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1485-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1486-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1487-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1489-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1493-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1494-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1497-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       99 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-15-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1501-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-151-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1510-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1515-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-1590-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-16-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-18-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-181-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-182-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-188-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-22-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-23-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-23381-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-23512-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-23517-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-24-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-28-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-29-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-3-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-300-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-307-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-31-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-312-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-32-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-334-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-37-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-375-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-377-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-38-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40496-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40498-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40499-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40536-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40668-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40670-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40685-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40701-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40900-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40923-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40927-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40966-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40975-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40978-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40979-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40981-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40982-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      100 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40983-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40984-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40994-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-40996-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41027-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41138-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41142-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41143-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41146-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41150-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41156-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41157-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41159-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41161-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41162-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41163-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41164-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41165-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41166-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41168-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41169-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-41212-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       99 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-4134-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-4135-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       99 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-4154-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      101 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-42-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-44-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      100 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-4534-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-4538-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-4541-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-458-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-46-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-469-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-470-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      102 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-50-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-54-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-554-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-6-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      104 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-60-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      103 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/rbv2_rpart-6332-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      128 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/translate_wmt-xformer_translate-64-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      136 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/translate_wmt-xformer_translate-64-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      130 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/translate_wmt-xformer_translate-64-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)       81 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/translate_wmt-xformer_translate-64-gpt.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/translate_wmt-xformer_translate-64-medium.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      129 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/uniref50-transformer-128-at25.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      131 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/uniref50-transformer-128-bad.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      132 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/uniref50-transformer-128-good.yaml
+-rw-r--r--   0 skantify  (1000) skantify  (1000)      125 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/priors/uniref50-transformer-128-medium.yaml
+drwxr-xr-x   0 skantify  (1000) skantify  (1000)        0 2024-05-10 09:39:47.224074 mf_prior_bench-1.9.0/src/requirements/
+-rw-r--r--   0 skantify  (1000) skantify  (1000)        5 2023-09-11 05:16:51.000000 mf_prior_bench-1.9.0/src/requirements/yahpo.txt
```

### Comparing `mf-prior-bench-1.8.1/LICENSE.txt` & `mf_prior_bench-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/PKG-INFO` & `mf_prior_bench-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mf-prior-bench
-Version: 1.8.1
+Version: 1.9.0
 Summary: A wrapper for multi-fidelity benchmarks with priors
 Author-email: Eddie Bergman <eddiebergmanhs@gmail.com>
 License:                               Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mf-prior-bench-1.8.1/pyproject.toml` & `mf_prior_bench-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   "pyyaml",
   "numpy",
   "configspace<=0.7",
   "pandas",
   "more_itertools",
   "pyarrow"
 ]
-version = "1.8.1"
+version = "1.9.0"
 description = "A wrapper for multi-fidelity benchmarks with priors"
 authors = [{name = "Eddie Bergman", email="eddiebergmanhs@gmail.com"}]
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.8"
 classifiers = [
   'Intended Audience :: Science/Research',
```

### Comparing `mf-prior-bench-1.8.1/src/mf_prior_bench.egg-info/PKG-INFO` & `mf_prior_bench-1.9.0/src/mf_prior_bench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mf-prior-bench
-Version: 1.8.1
+Version: 1.9.0
 Summary: A wrapper for multi-fidelity benchmarks with priors
 Author-email: Eddie Bergman <eddiebergmanhs@gmail.com>
 License:                               Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mf-prior-bench-1.8.1/src/mf_prior_bench.egg-info/SOURCES.txt` & `mf_prior_bench-1.9.0/src/mf_prior_bench.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 src/mfpbench/jahs/__pycache__/result.cpython-38.pyc
 src/mfpbench/jahs/__pycache__/spaces.cpython-310.pyc
 src/mfpbench/jahs/__pycache__/spaces.cpython-38.pyc
 src/mfpbench/lcbench_tabular/__init__.py
 src/mfpbench/lcbench_tabular/benchmark.py
 src/mfpbench/lcbench_tabular/__pycache__/__init__.cpython-310.pyc
 src/mfpbench/lcbench_tabular/__pycache__/benchmark.cpython-310.pyc
+src/mfpbench/nb201_tabular/__pycache__/__init__.cpython-310.pyc
+src/mfpbench/nb201_tabular/__pycache__/benchmark.cpython-310.pyc
 src/mfpbench/pd1/__init__.py
 src/mfpbench/pd1/benchmark.py
 src/mfpbench/pd1/__pycache__/__init__.cpython-310.pyc
 src/mfpbench/pd1/__pycache__/__init__.cpython-38.pyc
 src/mfpbench/pd1/__pycache__/benchmark.cpython-310.pyc
 src/mfpbench/pd1/__pycache__/benchmark.cpython-38.pyc
 src/mfpbench/pd1/__pycache__/config.cpython-310.pyc
@@ -89,24 +91,29 @@
 src/mfpbench/pd1/benchmarks/__pycache__/translate_wmt.cpython-310.pyc
 src/mfpbench/pd1/benchmarks/__pycache__/translate_wmt.cpython-38.pyc
 src/mfpbench/pd1/benchmarks/__pycache__/uniref50.cpython-310.pyc
 src/mfpbench/pd1/benchmarks/__pycache__/uniref50.cpython-38.pyc
 src/mfpbench/pd1/processing/__init__.py
 src/mfpbench/pd1/processing/columns.py
 src/mfpbench/pd1/processing/process_script.py
+src/mfpbench/pd1/processing/__pycache__/__init__.cpython-310.pyc
 src/mfpbench/pd1/processing/__pycache__/__init__.cpython-38.pyc
+src/mfpbench/pd1/processing/__pycache__/columns.cpython-310.pyc
 src/mfpbench/pd1/processing/__pycache__/columns.cpython-38.pyc
+src/mfpbench/pd1/processing/__pycache__/process_script.cpython-310.pyc
 src/mfpbench/pd1/processing/__pycache__/process_script.cpython-38.pyc
 src/mfpbench/pd1/surrogate/__init__.py
 src/mfpbench/pd1/surrogate/train_xgboost.py
 src/mfpbench/pd1/surrogate/training.py
 src/mfpbench/pd1/surrogate/xgboost_space.py
 src/mfpbench/pd1/surrogate/__pycache__/__init__.cpython-38.pyc
 src/mfpbench/pd1/surrogate/__pycache__/training.cpython-38.pyc
 src/mfpbench/pd1/surrogate/__pycache__/xgboost_space.cpython-38.pyc
+src/mfpbench/pd1_tabular/__pycache__/__init__.cpython-310.pyc
+src/mfpbench/pd1_tabular/__pycache__/benchmark.cpython-310.pyc
 src/mfpbench/synthetic/__init__.py
 src/mfpbench/synthetic/__pycache__/__init__.cpython-310.pyc
 src/mfpbench/synthetic/__pycache__/__init__.cpython-38.pyc
 src/mfpbench/synthetic/hartmann/__init__.py
 src/mfpbench/synthetic/hartmann/benchmark.py
 src/mfpbench/synthetic/hartmann/generators.py
 src/mfpbench/synthetic/hartmann/__pycache__/__init__.cpython-310.pyc
@@ -115,14 +122,18 @@
 src/mfpbench/synthetic/hartmann/__pycache__/benchmark.cpython-38.pyc
 src/mfpbench/synthetic/hartmann/__pycache__/config.cpython-310.pyc
 src/mfpbench/synthetic/hartmann/__pycache__/config.cpython-38.pyc
 src/mfpbench/synthetic/hartmann/__pycache__/generators.cpython-310.pyc
 src/mfpbench/synthetic/hartmann/__pycache__/generators.cpython-38.pyc
 src/mfpbench/synthetic/hartmann/__pycache__/result.cpython-310.pyc
 src/mfpbench/synthetic/hartmann/__pycache__/result.cpython-38.pyc
+src/mfpbench/taskset_tabular/__pycache__/__init__.cpython-310.pyc
+src/mfpbench/taskset_tabular/__pycache__/benchmark.cpython-310.pyc
+src/mfpbench/taskset_tabular/processing/__pycache__/__init__.cpython-310.pyc
+src/mfpbench/taskset_tabular/processing/__pycache__/process.cpython-310.pyc
 src/mfpbench/yahpo/__init__.py
 src/mfpbench/yahpo/benchmark.py
 src/mfpbench/yahpo/__pycache__/__init__.cpython-310.pyc
 src/mfpbench/yahpo/__pycache__/__init__.cpython-38.pyc
 src/mfpbench/yahpo/__pycache__/benchmark.cpython-310.pyc
 src/mfpbench/yahpo/__pycache__/benchmark.cpython-38.pyc
 src/mfpbench/yahpo/__pycache__/config.cpython-310.pyc
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__init__.py` & `mf_prior_bench-1.9.0/src/mfpbench/__init__.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__main__.py` & `mf_prior_bench-1.9.0/src/mfpbench/__main__.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/__init__.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/__init__.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/__main__.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/__main__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Sep 11 05:16:51 2023 UTC, .py size: 10274 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c3a2 fe64 2228 0000  o..........d"(..
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 2228 0000  o.......m.=f"(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 e200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a03 6401 6403 6c04 5a04 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6401  d.l.m.Z.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6401 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -328,20 +328,20 @@
 00001470: 7279 6406 6b01 7382 6e01 0100 7402 640b  ryd.k.s.n...t.d.
 00001480: 7c01 9b00 6408 9d03 8301 8201 5700 6e18  |...d.......W.n.
 00001490: 0400 7402 799b 0100 7d07 0100 7a0c 7404  ..t.y...}...z.t.
 000014a0: 640c 7c05 9b00 640d 7c01 9b00 6408 9d05  d.|...d.|...d...
 000014b0: 8301 7c07 8202 6403 7d07 7e07 7701 7700  ..|...d.}.~.w.w.
 000014c0: 7c02 7c06 7c08 7c09 6604 5300 290e 7a15  |.|.|.|.f.S.).z.
 000014d0: 5061 7273 6520 6120 7072 696f 7220 7374  Parse a prior st
-000014e0: 7269 6e67 2efa 013a 7a0e 496e 7661 6c69  ring...:z.Invali
+000014e0: 7269 6e67 2eda 013a 7a0e 496e 7661 6c69  ring...:z.Invali
 000014f0: 6420 696e 6465 7820 4e29 0472 0f00 0000  d index N).r....
 00001500: da01 307a 0330 2e30 7a04 302e 3030 7201  ..0z.0.0z.0.00r.
 00001510: 0000 00e9 0100 0000 7a1c 6e6f 6973 6520  ........z.noise 
 00001520: 6d75 7374 2062 6520 696e 205b 302c 2031  must be in [0, 1
-00001530: 5d20 696e 2028 fa01 297a 0e43 616e 2774  ] in (..)z.Can't
+00001530: 5d20 696e 2028 da01 297a 0e43 616e 2774  ] in (..)z.Can't
 00001540: 2063 6f6e 7665 7274 207a 0e20 746f 2066   convert z. to f
 00001550: 6c6f 6174 2069 6e20 287a 2e63 6174 6567  loat in (z.categ
 00001560: 6f72 6963 616c 5f73 7761 705f 6368 616e  orical_swap_chan
 00001570: 6365 206d 7573 7420 6265 2069 6e20 5b30  ce must be in [0
 00001580: 2c20 315d 2069 6e20 287a 2743 616e 2774  , 1] in (z'Can't
 00001590: 2063 6f6e 7665 7274 2063 6174 6567 6f72   convert categor
 000015a0: 6963 616c 5f73 7761 705f 6368 616e 6365  ical_swap_chance
@@ -488,15 +488,15 @@
 00001e70: 0000 5300 0001 7314 0000 0069 007c 005d  ..S...s....i.|.]
 00001e80: 067d 017c 016a 007c 0193 0271 0253 0072  .}.|.j.|...q.S.r
 00001e90: 1100 0000 723f 0000 0029 0272 4100 0000  ....r?...).rA...
 00001ea0: da07 6861 6e64 6c65 7272 1100 0000 7211  ..handlerr....r.
 00001eb0: 0000 0072 1400 0000 da0a 3c64 6963 7463  ...r......<dictc
 00001ec0: 6f6d 703e 3c01 0000 7302 0000 0014 007a  omp><...s......z
 00001ed0: 186d 6169 6e2e 3c6c 6f63 616c 733e 2e3c  .main.<locals>.<
-00001ee0: 6469 6374 636f 6d70 3efa 012d da01 0afa  dictcomp>..-....
+00001ee0: 6469 6374 636f 6d70 3efa 012d da01 0ada  dictcomp>..-....
 00001ef0: 0120 7a09 202d 2d68 656c 700a 0a29 0172  . z. --help..).r
 00001f00: 0b00 0000 4e72 6000 0000 7201 0000 0029  ....Nr`...r....)
 00001f10: 0fda 0861 7267 7061 7273 65da 0e41 7267  ...argparse..Arg
 00001f20: 756d 656e 7450 6172 7365 72da 1452 6177  umentParser..Raw
 00001f30: 5465 7874 4865 6c70 466f 726d 6174 7465  TextHelpFormatte
 00001f40: 72da 0e61 6464 5f73 7562 7061 7273 6572  r..add_subparser
 00001f50: 7372 0900 0000 721d 0000 00da 0569 7465  sr....r......ite
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/__main__.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/__main__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/benchmark.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/tabular.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 15923 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,831 +1,930 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 333e 0000  o........Coe3>..
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 fd47 0000  o.......m.=f.G..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0173 fc00 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0173 9601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
-00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
-00000080: 6d10 5a10 6d11 5a11 0100 6400 6402 6c12  m.Z.m.Z...d.d.l.
-00000090: 5a13 6400 6406 6c14 6d15 5a15 0100 6400  Z.d.d.l.m.Z...d.
-000000a0: 6407 6c16 6d17 5a17 0100 6400 6408 6c18  d.l.m.Z...d.d.l.
-000000b0: 6d19 5a19 0100 6509 7252 6400 6409 6c1a  m.Z...e.rRd.d.l.
-000000c0: 6d1b 5a1b 0100 6400 640a 6c1c 6d1d 5a1d  m.Z...d.d.l.m.Z.
-000000d0: 0100 6507 651e 8301 6a1f 6a1f 5a20 6520  ..e.e...j.j.Z e 
-000000e0: 640b 1b00 5a21 6510 640c 6515 640d 8d02  d...Z!e.d.e.d...
-000000f0: 5a22 6510 640e 6517 640d 8d02 5a23 6510  Z"e.d.e.d...Z#e.
-00000100: 640f 6524 6525 8303 5a26 4700 6410 6411  d.e$e%..Z&G.d.d.
-00000110: 8400 6411 650c 6522 6523 6526 6603 1900  ..d.e.e"e#e&f...
-00000120: 6504 8304 5a27 6402 5300 2912 e900 0000  e...Z'd.S.).....
-00000130: 0029 01da 0b61 6e6e 6f74 6174 696f 6e73  .)...annotations
-00000140: 4e29 02da 0341 4243 da0e 6162 7374 7261  N)...ABC..abstra
-00000150: 6374 6d65 7468 6f64 2901 da04 5061 7468  ctmethod)...Path
-00000160: 2909 da0d 5459 5045 5f43 4845 434b 494e  )...TYPE_CHECKIN
-00000170: 47da 0341 6e79 da08 436c 6173 7356 6172  G..Any..ClassVar
-00000180: da07 4765 6e65 7269 63da 0849 7465 7261  ..Generic..Itera
-00000190: 626c 65da 0849 7465 7261 746f 72da 074d  ble..Iterator..M
-000001a0: 6170 7069 6e67 da07 5479 7065 5661 72da  apping..TypeVar.
-000001b0: 086f 7665 726c 6f61 6429 01da 0643 6f6e  .overload)...Con
-000001c0: 6669 6729 01da 0652 6573 756c 7429 01da  fig)...Result)..
-000001d0: 0b52 6573 756c 7446 7261 6d65 2901 da12  .ResultFrame)...
-000001e0: 436f 6e66 6967 7572 6174 696f 6e53 7061  ConfigurationSpa
-000001f0: 6365 2901 da06 4d65 7472 6963 5a06 7072  ce)...MetricZ.pr
-00000200: 696f 7273 da01 4329 01da 0562 6f75 6e64  iors..C)...bound
-00000210: da01 52da 0146 6300 0000 0000 0000 0000  ..R..Fc.........
-00000220: 0000 0000 0000 0007 0000 0040 0000 0173  ...........@...s
-00000230: 4601 0000 6500 5a01 6400 5a02 5500 6401  F...e.Z.d.Z.U.d.
-00000240: 5a03 6504 5a05 6402 6506 6403 3c00 0900  Z.e.Z.d.e.d.<...
-00000250: 6404 5a07 6405 6506 6406 3c00 0900 6404  d.Z.d.e.d.<...d.
-00000260: 5a08 6405 6506 6407 3c00 0900 6408 6404  Z.d.e.d.<...d.d.
-00000270: 6404 6404 6404 6404 6409 9c06 645b 6420  d.d.d.d.d...d[d 
-00000280: 6421 8406 5a09 650a 645c 6424 6425 8404  d!..Z.e.d\d$d%..
-00000290: 8301 5a0b 650a 645d 6427 6428 8404 8301  ..Z.e.d]d'd(....
-000002a0: 5a0c 650a 645d 6429 642a 8404 8301 5a0d  Z.e.d]d)d*....Z.
-000002b0: 650a 645d 642b 642c 8404 8301 5a0e 0904  e.d]d+d,....Z...
-000002c0: 645e 645f 6430 6431 8405 5a0f 0904 0904  d^d_d0d1..Z.....
-000002d0: 0904 6460 6461 6437 6438 8405 5a10 6462  ..d`dad7d8..Z.db
-000002e0: 643a 643b 8404 5a11 6404 6404 6404 643c  d:d;..Z.d.d.d.d<
-000002f0: 9c03 6463 6441 6442 8406 5a12 6404 6404  ..dcdAdB..Z.d.d.
-00000300: 6404 6404 6404 6443 9c05 6464 6445 6446  d.d.d.dC..dddEdF
-00000310: 8406 5a13 6514 6465 6449 644a 8404 8301  ..Z.e.dedIdJ....
-00000320: 5a15 6466 644c 644d 8404 5a16 6517 0904  Z.dfdLdM..Z.e...
-00000330: 645e 6404 644e 9c01 6467 6451 6452 8407  d^d.dN..dgdQdR..
-00000340: 8301 5a18 6517 6404 644e 9c01 6468 6455  ..Z.e.d.dN..dhdU
-00000350: 6452 8406 8301 5a18 0904 645e 6404 644e  dR....Z...d^d.dN
-00000360: 9c01 6469 6457 6452 8407 5a18 646a 6459  ..didWdR..Z.djdY
-00000370: 645a 8404 5a19 6404 5300 296b da09 4265  dZ..Z.d.S.)k..Be
-00000380: 6e63 686d 6172 6b7a 1b42 6173 6520 636c  nchmarkz.Base cl
-00000390: 6173 7320 666f 7220 6120 4265 6e63 686d  ass for a Benchm
-000003a0: 6172 6b2e 7a0e 436c 6173 7356 6172 5b50  ark.z.ClassVar[P
-000003b0: 6174 685d da12 5f64 6566 6175 6c74 5f70  ath].._default_p
-000003c0: 7269 6f72 5f64 6972 4e7a 2243 6c61 7373  rior_dirNz"Class
-000003d0: 5661 725b 4d61 7070 696e 675b 7374 722c  Var[Mapping[str,
-000003e0: 2073 7472 5d20 7c20 4e6f 6e65 5dda 0f5f   str] | None].._
-000003f0: 7265 7375 6c74 5f72 656e 616d 6573 da0f  result_renames..
-00000400: 5f63 6f6e 6669 675f 7265 6e61 6d65 7346  _config_renamesF
-00000410: 2906 da10 6861 735f 636f 6e64 6974 696f  )...has_conditio
-00000420: 6e61 6c73 da04 7365 6564 da05 7072 696f  nals..seed..prio
-00000430: 72da 0d70 6572 7475 7262 5f70 7269 6f72  r..perturb_prior
-00000440: da0c 7661 6c75 655f 6d65 7472 6963 da0b  ..value_metric..
-00000450: 636f 7374 5f6d 6574 7269 63da 046e 616d  cost_metric..nam
-00000460: 65da 0373 7472 da05 7370 6163 6572 1200  e..str..spacer..
-00000470: 0000 da0b 636f 6e66 6967 5f74 7970 65fa  ....config_type.
-00000480: 0774 7970 655b 435d da0b 7265 7375 6c74  .type[C]..result
-00000490: 5f74 7970 65fa 0774 7970 655b 525d da0e  _type..type[R]..
-000004a0: 6669 6465 6c69 7479 5f72 616e 6765 fa0e  fidelity_range..
-000004b0: 7475 706c 655b 462c 2046 2c20 465d da0d  tuple[F, F, F]..
-000004c0: 6669 6465 6c69 7479 5f6e 616d 6572 1c00  fidelity_namer..
-000004d0: 0000 da04 626f 6f6c 721d 0000 00fa 0a69  ....boolr......i
-000004e0: 6e74 207c 204e 6f6e 6572 1e00 0000 fa29  nt | Noner.....)
-000004f0: 7374 7220 7c20 5061 7468 207c 2043 207c  str | Path | C |
-00000500: 204d 6170 7069 6e67 5b73 7472 2c20 416e   Mapping[str, An
-00000510: 795d 207c 204e 6f6e 6572 1f00 0000 fa0c  y] | Noner......
-00000520: 666c 6f61 7420 7c20 4e6f 6e65 7220 0000  float | Noner ..
-00000530: 00fa 0a73 7472 207c 204e 6f6e 6572 2100  ...str | Noner!.
-00000540: 0000 6307 0000 0000 0000 0006 0000 000d  ..c.............
-00000550: 0000 0006 0000 0043 0000 0173 4401 0000  .......C...sD...
-00000560: 7c0b 6401 7500 7207 7c04 6a00 7d0b 7c0c  |.d.u.r.|.j.}.|.
-00000570: 6401 7500 720e 7c04 6a01 7d0c 7c01 7c00  d.u.r.|.j.}.|.|.
-00000580: 5f02 7c08 7c00 5f03 7c02 7c00 5f04 7c0b  _.|.|._.|.|._.|.
-00000590: 7c00 5f05 7c0c 7c00 5f06 7c05 7c00 5f07  |._.|.|._.|.|._.
-000005a0: 7c06 7c00 5f08 7c07 7c00 5f09 7c03 7c00  |.|._.|.|._.|.|.
-000005b0: 5f0a 7c04 7c00 5f0b 6402 6403 8400 7c00  _.|.|._.d.d...|.
-000005c0: 6a0b 6a0c a00d a100 4400 8301 7c00 5f0e  j.j.....D...|._.
-000005d0: 7c0b 6401 7500 724b 740f 7c00 6a0b 6404  |.d.u.rKt.|.j.d.
-000005e0: 6401 8303 6401 7501 7347 4a00 8201 7c00  d...d.u.sGJ...|.
-000005f0: 6a0b 6a05 7d0b 7c09 7c00 5f10 7c0a 6401  j.j.}.|.|._.|.d.
-00000600: 7501 7264 6405 7c0a 0400 0300 6b01 725f  u.rdd.|.....k.r_
-00000610: 6406 6b01 7364 7411 6407 8301 8201 0100  d.k.sdt.d.......
-00000620: 7411 6407 8301 8201 7c0a 7c00 5f12 6401  t.d.....|.|._.d.
-00000630: 7c00 5f13 7c09 6401 7501 7278 7c00 6a14  |._.|.d.u.rx|.j.
-00000640: 7c09 7c00 6a02 6408 8d02 7c00 5f13 6e03  |.|.j.d...|._.n.
-00000650: 6401 7c00 5f13 7c00 6a13 6401 7501 7293  d.|._.|.j.d.u.r.
-00000660: 7c00 6a12 6401 7501 7293 7c00 6a13 6a15  |.j.d.u.r.|.j.j.
-00000670: 7c02 7c00 6a03 7c00 6a12 7c00 6a12 6409  |.|.j.|.j.|.j.d.
-00000680: 8d04 7c00 5f13 7c00 6a13 6401 7501 72a0  ..|._.|.j.d.u.r.
-00000690: 7c00 6a13 a016 7c02 a101 0100 6401 5300  |.j...|.....d.S.
-000006a0: 6401 5300 290a 61db 0500 0049 6e69 7469  d.S.).a....Initi
-000006b0: 616c 697a 6520 7468 6520 6265 6e63 686d  alize the benchm
-000006c0: 6172 6b2e 0a0a 2020 2020 2020 2020 4172  ark...        Ar
-000006d0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-000006e0: 6e61 6d65 3a20 5468 6520 6e61 6d65 206f  name: The name o
-000006f0: 6620 7468 6973 2062 656e 6368 6d61 726b  f this benchmark
-00000700: 0a20 2020 2020 2020 2020 2020 2073 7061  .            spa
-00000710: 6365 3a20 5468 6520 636f 6e66 6967 7572  ce: The configur
-00000720: 6174 696f 6e20 7370 6163 6520 746f 2075  ation space to u
-00000730: 7365 2066 6f72 2074 6865 2062 656e 6368  se for the bench
-00000740: 6d61 726b 2e0a 2020 2020 2020 2020 2020  mark..          
-00000750: 2020 636f 6e66 6967 5f74 7970 653a 2054    config_type: T
-00000760: 6865 2074 7970 6520 6f66 2063 6f6e 6669  he type of confi
-00000770: 6720 746f 2075 7365 2066 6f72 2074 6865  g to use for the
-00000780: 2062 656e 6368 6d61 726b 2e0a 2020 2020   benchmark..    
-00000790: 2020 2020 2020 2020 7265 7375 6c74 5f74          result_t
-000007a0: 7970 653a 2054 6865 2074 7970 6520 6f66  ype: The type of
-000007b0: 2072 6573 756c 7420 746f 2075 7365 2066   result to use f
-000007c0: 6f72 2074 6865 2062 656e 6368 6d61 726b  or the benchmark
-000007d0: 2e0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
-000007e0: 6465 6c69 7479 5f6e 616d 653a 2054 6865  delity_name: The
-000007f0: 206e 616d 6520 6f66 2074 6865 2066 6964   name of the fid
-00000800: 656c 6974 7920 746f 2075 7365 2066 6f72  elity to use for
-00000810: 2074 6865 2062 656e 6368 6d61 726b 2e0a   the benchmark..
-00000820: 2020 2020 2020 2020 2020 2020 6669 6465              fide
-00000830: 6c69 7479 5f72 616e 6765 3a20 5468 6520  lity_range: The 
-00000840: 7261 6e67 6520 6f66 2066 6964 656c 6974  range of fidelit
-00000850: 6965 7320 746f 2075 7365 2066 6f72 2074  ies to use for t
-00000860: 6865 2062 656e 6368 6d61 726b 2e0a 2020  he benchmark..  
-00000870: 2020 2020 2020 2020 2020 6861 735f 636f            has_co
-00000880: 6e64 6974 696f 6e61 6c73 3a20 5768 6574  nditionals: Whet
-00000890: 6865 7220 7468 6973 2062 656e 6368 6d61  her this benchma
-000008a0: 726b 2068 6173 2063 6f6e 6469 7469 6f6e  rk has condition
-000008b0: 616c 7320 696e 2069 7420 6f72 206e 6f74  als in it or not
-000008c0: 2e0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000008d0: 6564 3a20 5468 6520 7365 6564 2074 6f20  ed: The seed to 
-000008e0: 7573 652e 0a20 2020 2020 2020 2020 2020  use..           
-000008f0: 2070 7269 6f72 3a20 5468 6520 7072 696f   prior: The prio
-00000900: 7220 746f 2075 7365 2066 6f72 2074 6865  r to use for the
-00000910: 2062 656e 6368 6d61 726b 2e20 4966 204e   benchmark. If N
-00000920: 6f6e 652c 206e 6f20 7072 696f 7220 6973  one, no prior is
-00000930: 2075 7365 642e 0a20 2020 2020 2020 2020   used..         
-00000940: 2020 2020 2020 2049 6620 6120 7374 722c         If a str,
-00000950: 2077 696c 6c20 6368 6563 6b20 7468 6520   will check the 
-00000960: 6c6f 6361 6c20 6c6f 6361 7469 6f6e 2066  local location f
-00000970: 6972 7374 2066 6f72 2061 2070 7269 6f72  irst for a prior
-00000980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000990: 2073 7065 6369 6669 6320 666f 7220 7468   specific for th
-000009a0: 6973 2062 656e 6368 6d61 726b 2c20 6f74  is benchmark, ot
-000009b0: 6865 7277 6973 6520 6173 7375 6d65 7320  herwise assumes 
-000009c0: 6974 2074 6f20 6265 2061 2050 6174 682e  it to be a Path.
-000009d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009e0: 2049 6620 6120 5061 7468 2c20 7769 6c6c   If a Path, will
-000009f0: 206c 6f61 6420 7468 6520 7072 696f 7220   load the prior 
-00000a00: 6672 6f6d 2074 6865 2070 6174 682e 0a20  from the path.. 
-00000a10: 2020 2020 2020 2020 2020 2020 2020 2049                 I
-00000a20: 6620 6120 4d61 7070 696e 672c 2077 696c  f a Mapping, wil
-00000a30: 6c20 6265 2075 7365 6420 6469 7265 6374  l be used direct
-00000a40: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
-00000a50: 7065 7274 7572 625f 7072 696f 723a 2049  perturb_prior: I
-00000a60: 6620 6e6f 7420 4e6f 6e65 2c20 7769 6c6c  f not None, will
-00000a70: 2070 6572 7475 7262 2074 6865 2070 7269   perturb the pri
-00000a80: 6f72 2062 7920 7468 6973 2061 6d6f 756e  or by this amoun
-00000a90: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
-00000aa0: 2020 2046 6f72 206e 756d 6572 6963 616c     For numerical
-00000ab0: 732c 2074 6869 7320 6973 2069 6e74 6572  s, this is inter
-00000ac0: 7072 6574 6564 2061 7320 7468 6520 7374  preted as the st
-00000ad0: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-00000ae0: 206f 6620 610a 2020 2020 2020 2020 2020   of a.          
-00000af0: 2020 2020 2020 6e6f 726d 616c 2064 6973        normal dis
-00000b00: 7472 6962 7574 696f 6e20 7768 696c 6520  tribution while 
-00000b10: 666f 7220 6361 7465 676f 7269 6361 6c73  for categoricals
-00000b20: 2c20 7468 6973 2069 7320 696e 7465 7270  , this is interp
-00000b30: 7265 7465 640a 2020 2020 2020 2020 2020  reted.          
-00000b40: 2020 2020 2020 6173 2074 6865 2070 726f        as the pro
-00000b50: 6261 6269 6c69 7479 206f 6620 7377 6170  bability of swap
-00000b60: 7069 6e67 2074 6865 2076 616c 7565 2066  ping the value f
-00000b70: 6f72 2061 2072 616e 646f 6d20 6f6e 652e  or a random one.
-00000b80: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-00000b90: 7565 5f6d 6574 7269 633a 2054 6865 206d  ue_metric: The m
-00000ba0: 6574 7269 6320 746f 2075 7365 2066 6f72  etric to use for
-00000bb0: 2074 6869 7320 6265 6e63 686d 6172 6b2e   this benchmark.
-00000bc0: 2055 7365 730a 2020 2020 2020 2020 2020   Uses.          
-00000bd0: 2020 2020 2020 7468 6520 6465 6661 756c        the defaul
-00000be0: 7420 6d65 7472 6963 2066 726f 6d20 7468  t metric from th
-00000bf0: 6520 5265 7375 6c74 2069 6620 4e6f 6e65  e Result if None
-00000c00: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00000c10: 7374 5f6d 6574 7269 633a 2054 6865 2063  st_metric: The c
-00000c20: 6f73 7420 746f 2075 7365 2066 6f72 2074  ost to use for t
-00000c30: 6869 7320 6265 6e63 686d 6172 6b2e 2055  his benchmark. U
-00000c40: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
-00000c50: 2020 2020 7468 6520 6465 6661 756c 7420      the default 
-00000c60: 636f 7374 2066 726f 6d20 7468 6520 5265  cost from the Re
-00000c70: 7375 6c74 2069 6620 4e6f 6e65 2e0a 2020  sult if None..  
-00000c80: 2020 2020 2020 4e63 0100 0000 0000 0000        Nc........
-00000c90: 0000 0000 0300 0000 0400 0000 5300 0001  ............S...
-00000ca0: 7318 0000 0069 007c 005d 085c 027d 017d  s....i.|.].\.}.}
-00000cb0: 027c 017c 026a 0093 0271 0253 00a9 0029  .|.|.j...q.S...)
-00000cc0: 015a 0d6f 7074 696d 756d 5f76 616c 7565  .Z.optimum_value
-00000cd0: 2903 da02 2e30 5a0b 6d65 7472 6963 5f6e  )....0Z.metric_n
-00000ce0: 616d 655a 066d 6574 7269 6372 3100 0000  ameZ.metricr1...
-00000cf0: 7231 0000 00fa 3c2f 686f 6d65 2f73 6b61  r1....</home/ska
-00000d00: 6e74 6966 792f 636f 6465 2f6d 662d 7072  ntify/code/mf-pr
-00000d10: 696f 722d 6265 6e63 682f 7372 632f 6d66  ior-bench/src/mf
-00000d20: 7062 656e 6368 2f62 656e 6368 6d61 726b  pbench/benchmark
-00000d30: 2e70 79da 0a3c 6469 6374 636f 6d70 3e77  .py..<dictcomp>w
-00000d40: 0000 0073 0800 0000 0600 0602 06ff 06ff  ...s............
-00000d50: 7a26 4265 6e63 686d 6172 6b2e 5f5f 696e  z&Benchmark.__in
-00000d60: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c64  it__.<locals>.<d
-00000d70: 6963 7463 6f6d 703e 7220 0000 0072 0100  ictcomp>r ...r..
-00000d80: 0000 e901 0000 007a 3649 6620 7065 7274  .......z6If pert
-00000d90: 7572 6269 6e67 2070 7269 6f72 2c20 6070  urbing prior, `p
-00000da0: 6572 7475 7262 5f70 7269 6f72 6020 6d75  erturb_prior` mu
-00000db0: 7374 2062 6520 696e 205b 302c 2031 5d29  st be in [0, 1])
-00000dc0: 01da 0962 656e 6368 6e61 6d65 2903 721d  ...benchname).r.
-00000dd0: 0000 00da 0373 7464 5a17 6361 7465 676f  .....stdZ.catego
-00000de0: 7269 6361 6c5f 7377 6170 5f63 6861 6e63  rical_swap_chanc
-00000df0: 6529 175a 1464 6566 6175 6c74 5f76 616c  e).Z.default_val
-00000e00: 7565 5f6d 6574 7269 635a 1364 6566 6175  ue_metricZ.defau
-00000e10: 6c74 5f63 6f73 745f 6d65 7472 6963 7222  lt_cost_metricr"
-00000e20: 0000 0072 1d00 0000 7224 0000 0072 2000  ...r....r$...r .
-00000e30: 0000 7221 0000 0072 2900 0000 722b 0000  ..r!...r)...r+..
-00000e40: 0072 1c00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00000e50: da0b 6d65 7472 6963 5f64 6566 73da 0569  ..metric_defs..i
-00000e60: 7465 6d73 5a0f 6d65 7472 6963 5f6f 7074  temsZ.metric_opt
-00000e70: 696d 756d 73da 0767 6574 6174 7472 5a0a  imums..getattrZ.
-00000e80: 5f70 7269 6f72 5f61 7267 da13 4e6f 7449  _prior_arg..NotI
-00000e90: 6d70 6c65 6d65 6e74 6564 4572 726f 7272  mplementedErrorr
-00000ea0: 1f00 0000 721e 0000 00da 0b5f 6c6f 6164  ....r......_load
-00000eb0: 5f70 7269 6f72 5a07 7065 7274 7572 625a  _priorZ.perturbZ
-00000ec0: 1473 6574 5f61 735f 6465 6661 756c 745f  .set_as_default_
-00000ed0: 7072 696f 7229 0dda 0473 656c 6672 2200  prior)...selfr".
-00000ee0: 0000 7224 0000 0072 2500 0000 7227 0000  ..r$...r%...r'..
-00000ef0: 0072 2900 0000 722b 0000 0072 1c00 0000  .r)...r+...r....
-00000f00: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00000f10: 2000 0000 7221 0000 0072 3100 0000 7231   ...r!...r1...r1
-00000f20: 0000 0072 3300 0000 da08 5f5f 696e 6974  ...r3.....__init
-00000f30: 5f5f 3e00 0000 7358 0000 0008 2906 0108  __>...sX....)...
-00000f40: 0206 0106 0206 0106 0106 0106 0106 0106  ................
-00000f50: 0106 0106 0106 0106 010a 0208 fe08 0516  ................
-00000f60: 0108 0106 021a 0602 0102 0104 ff02 ff02  ................
-00000f70: 0102 0104 ff06 0406 0108 0214 0106 0214  ................
-00000f80: 0206 0102 0104 0104 0104 0108 fc0a 0710  ................
-00000f90: 0104 ff7a 1242 656e 6368 6d61 726b 2e5f  ...z.Benchmark._
-00000fa0: 5f69 6e69 745f 5fda 0672 6574 7572 6efa  _init__..return.
-00000fb0: 1164 6963 745b 7374 722c 204d 6574 7269  .dict[str, Metri
-00000fc0: 635d 6301 0000 0000 0000 0000 0000 0001  c]c.............
-00000fd0: 0000 0002 0000 0043 0000 0173 0c00 0000  .......C...s....
-00000fe0: 7400 7c00 6a01 6a02 8301 5300 2901 7a1f  t.|.j.j...S.).z.
-00000ff0: 5468 6520 6d65 7472 6963 7320 666f 7220  The metrics for 
-00001000: 7468 6973 2062 656e 6368 6d61 726b 2e29  this benchmark.)
-00001010: 03da 0464 6963 7472 1000 0000 7238 0000  ...dictr....r8..
-00001020: 00a9 0172 3d00 0000 7231 0000 0072 3100  ...r=...r1...r1.
-00001030: 0000 7233 0000 00da 076d 6574 7269 6373  ..r3.....metrics
-00001040: 9e00 0000 7302 0000 000c 037a 1142 656e  ....s......z.Ben
-00001050: 6368 6d61 726b 2e6d 6574 7269 6373 7217  chmark.metricsr.
-00001060: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001070: 0100 0000 0200 0000 4300 0001 f30a 0000  ........C.......
-00001080: 007c 006a 0064 0119 0053 0029 027a 2054  .|.j.d...S.).z T
-00001090: 6865 2073 7461 7274 206f 6620 7468 6520  he start of the 
-000010a0: 6669 6465 6c69 7479 2072 616e 6765 2e72  fidelity range.r
-000010b0: 0100 0000 a901 7229 0000 0072 4200 0000  ......r)...rB...
-000010c0: 7231 0000 0072 3100 0000 7233 0000 00da  r1...r1...r3....
-000010d0: 0573 7461 7274 a300 0000 f302 0000 000a  .start..........
-000010e0: 037a 0f42 656e 6368 6d61 726b 2e73 7461  .z.Benchmark.sta
-000010f0: 7274 6301 0000 0000 0000 0000 0000 0001  rtc.............
-00001100: 0000 0002 0000 0043 0000 0172 4400 0000  .......C...rD...
-00001110: 2902 7a1e 5468 6520 656e 6420 6f66 2074  ).z.The end of t
-00001120: 6865 2066 6964 656c 6974 7920 7261 6e67  he fidelity rang
-00001130: 652e 7235 0000 0072 4500 0000 7242 0000  e.r5...rE...rB..
-00001140: 0072 3100 0000 7231 0000 0072 3300 0000  .r1...r1...r3...
-00001150: da03 656e 64a8 0000 0072 4700 0000 7a0d  ..end....rG...z.
-00001160: 4265 6e63 686d 6172 6b2e 656e 6463 0100  Benchmark.endc..
-00001170: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00001180: 0000 4300 0001 7244 0000 0029 027a 1f54  ..C...rD...).z.T
-00001190: 6865 2073 7465 7020 6f66 2074 6865 2066  he step of the f
-000011a0: 6964 656c 6974 7920 7261 6e67 652e e902  idelity range...
-000011b0: 0000 0072 4500 0000 7242 0000 0072 3100  ...rE...rB...r1.
-000011c0: 0000 7231 0000 0072 3300 0000 da04 7374  ..r1...r3.....st
-000011d0: 6570 ad00 0000 7247 0000 007a 0e42 656e  ep....rG...z.Ben
-000011e0: 6368 6d61 726b 2e73 7465 70fa 2273 7472  chmark.step."str
-000011f0: 207c 2050 6174 6820 7c20 4d61 7070 696e   | Path | Mappin
-00001200: 675b 7374 722c 2041 6e79 5d20 7c20 4372  g[str, Any] | Cr
-00001210: 3600 0000 7214 0000 0063 0300 0000 0000  6...r....c......
-00001220: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
-00001230: 0001 739c 0000 007c 006a 007d 0374 017c  ..s....|.j.}.t.|
-00001240: 0174 0283 0272 277c 0264 0075 0172 207c  .t...r'|.d.u.r |
-00001250: 006a 037c 029b 0064 017c 019b 0064 029d  .j.|...d.|...d..
-00001260: 041b 007d 047c 04a0 04a1 0072 207c 03a0  ...}.|.....r |..
-00001270: 057c 04a1 0153 007c 03a0 0574 067c 0183  .|...S.|...t.|..
-00001280: 01a1 0153 0074 017c 0174 0683 0272 317c  ...S.t.|.t...r1|
-00001290: 03a0 057c 01a1 0153 0074 017c 017c 0383  ...|...S.t.|.|..
-000012a0: 0272 387c 0153 0074 017c 0174 0783 0272  .r8|.S.t.|.t...r
-000012b0: 457c 036a 087c 017c 006a 0964 038d 0253  E|.j.|.|.j.d...S
-000012c0: 0074 0a64 0474 0b7c 0183 019b 009d 0283  .t.d.t.|........
-000012d0: 0182 0129 054e fa01 2d7a 052e 7961 6d6c  ...).N..-z..yaml
-000012e0: a901 da07 7265 6e61 6d65 737a 1355 6e6b  ....renamesz.Unk
-000012f0: 6e6f 776e 2070 7269 6f72 2074 7970 6520  nown prior type 
-00001300: 290c 720f 0000 00da 0a69 7369 6e73 7461  ).r......isinsta
-00001310: 6e63 6572 2300 0000 7219 0000 00da 0665  ncer#...r......e
-00001320: 7869 7374 73da 0966 726f 6d5f 6669 6c65  xists..from_file
-00001330: 7205 0000 0072 0c00 0000 da09 6672 6f6d  r....r......from
-00001340: 5f64 6963 7472 1b00 0000 da0a 5661 6c75  _dictr......Valu
-00001350: 6545 7272 6f72 da04 7479 7065 2905 723d  eError..type).r=
-00001360: 0000 0072 1e00 0000 7236 0000 0072 0f00  ...r....r6...r..
-00001370: 0000 5a0c 6173 7375 6d65 645f 7061 7468  ..Z.assumed_path
-00001380: 7231 0000 0072 3100 0000 7233 0000 0072  r1...r1...r3...r
-00001390: 3c00 0000 b200 0000 731c 0000 0006 050a  <.......s.......
-000013a0: 0208 0216 0108 010a 010e 030a 020a 010a  ................
-000013b0: 0204 010a 0210 0112 027a 1542 656e 6368  .........z.Bench
-000013c0: 6d61 726b 2e5f 6c6f 6164 5f70 7269 6f72  mark._load_prior
-000013d0: da03 6672 6dfa 0846 207c 204e 6f6e 65da  ..frm..F | None.
-000013e0: 0274 6f72 4a00 0000 fa0b 4974 6572 6174  .torJ.....Iterat
-000013f0: 6f72 5b46 5d63 0400 0000 0000 0000 0000  or[F]c..........
-00001400: 0000 0600 0000 0700 0000 6300 0001 73be  ..........c...s.
-00001410: 0000 0081 007c 0164 0175 0172 077c 016e  .....|.d.u.r.|.n
-00001420: 027c 006a 007d 017c 0264 0175 0172 107c  .|.j.}.|.d.u.r.|
-00001430: 026e 027c 006a 017d 027c 0364 0175 0172  .n.|.j.}.|.d.u.r
-00001440: 197c 036e 027c 006a 027d 037c 006a 007c  .|.n.|.j.}.|.j.|
-00001450: 0104 0003 006b 0172 2e7c 0204 0003 006b  .....k.r.|.....k
-00001460: 0172 2e7c 006a 016b 0173 314a 0082 0101  .r.|.j.k.s1J....
-00001470: 004a 0082 0174 037c 0174 0483 0272 3874  .J...t.|.t...r8t
-00001480: 046e 0174 057d 0474 0674 076a 087c 017c  .n.t.}.t.t.j.|.|
-00001490: 027c 0317 007c 037c 0464 028d 0483 017d  .|...|.|.d.....}
-000014a0: 0574 037c 0374 0583 0272 587c 0564 0319  .t.|.t...rX|.d..
-000014b0: 007c 006a 016b 0572 587c 006a 017c 0564  .|.j.k.rX|.j.|.d
-000014c0: 033c 007c 0545 0064 0148 0001 0064 0153  .<.|.E.d.H...d.S
-000014d0: 0029 0461 6801 0000 4974 6572 6174 6520  .).ah...Iterate 
-000014e0: 7468 726f 7567 6820 7468 6520 6164 7665  through the adve
-000014f0: 7274 6973 6564 2066 6964 656c 6974 7920  rtised fidelity 
-00001500: 7370 6163 6520 6f66 2074 6865 2062 656e  space of the ben
-00001510: 6368 6d61 726b 2e0a 0a20 2020 2020 2020  chmark...       
-00001520: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00001530: 2020 2066 726d 3a20 5374 6172 7420 6f66     frm: Start of
-00001540: 2074 6865 2063 7572 7665 2c20 6465 6661   the curve, defa
-00001550: 756c 7473 2074 6f20 7468 6520 6d69 6e69  ults to the mini
-00001560: 6d75 6d20 6669 6465 6c69 7479 0a20 2020  mum fidelity.   
-00001570: 2020 2020 2020 2020 2074 6f3a 2045 6e64           to: End
-00001580: 206f 6620 7468 6520 6375 7276 652c 2064   of the curve, d
-00001590: 6566 6175 6c74 7320 746f 2074 6865 206d  efaults to the m
-000015a0: 6178 696d 756d 2066 6964 656c 6974 790a  aximum fidelity.
-000015b0: 2020 2020 2020 2020 2020 2020 7374 6570              step
-000015c0: 3a20 5374 6570 2073 697a 652c 2064 6566  : Step size, def
-000015d0: 6175 6c74 7320 746f 2062 656e 6368 6d61  aults to benchma
-000015e0: 726b 2073 7461 6e64 6172 6420 2831 2066  rk standard (1 f
-000015f0: 6f72 2065 706f 6368 290a 0a20 2020 2020  or epoch)..     
-00001600: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00001610: 2020 2020 2020 2020 416e 2069 7465 7261          An itera
-00001620: 746f 7220 6f76 6572 2074 6865 2066 6964  tor over the fid
-00001630: 656c 6974 6965 730a 2020 2020 2020 2020  elities.        
-00001640: 4e29 0472 4600 0000 da04 7374 6f70 724a  N).rF.....stoprJ
-00001650: 0000 00da 0564 7479 7065 e9ff ffff ff29  .....dtype.....)
-00001660: 0972 4600 0000 7248 0000 0072 4a00 0000  .rF...rH...rJ...
-00001670: 724f 0000 00da 0369 6e74 da05 666c 6f61  rO.....int..floa
-00001680: 74da 046c 6973 74da 026e 70da 0661 7261  t..list..np..ara
-00001690: 6e67 6529 0672 3d00 0000 7255 0000 0072  nge).r=...rU...r
-000016a0: 5700 0000 724a 0000 0072 5a00 0000 5a0a  W...rJ...rZ...Z.
-000016b0: 6669 6465 6c69 7469 6573 7231 0000 0072  fidelitiesr1...r
-000016c0: 3100 0000 7233 0000 00da 0f69 7465 725f  1...r3.....iter_
-000016d0: 6669 6465 6c69 7469 6573 ce00 0000 7318  fidelities....s.
-000016e0: 0000 0002 8012 1012 0112 012a 0112 0202  ...........*....
-000016f0: 0114 0104 ff18 0b0a 010e 027a 1942 656e  ...........z.Ben
-00001700: 6368 6d61 726b 2e69 7465 725f 6669 6465  chmark.iter_fide
-00001710: 6c69 7469 6573 da04 4e6f 6e65 6301 0000  lities..Nonec...
-00001720: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00001730: 0043 0000 01f3 0400 0000 6401 5300 2902  .C........d.S.).
-00001740: 7a38 4578 706c 6963 6974 6c79 206c 6f61  z8Explicitly loa
-00001750: 6420 7468 6520 6265 6e63 686d 6172 6b20  d the benchmark 
-00001760: 6265 666f 7265 2071 7565 7279 696e 672c  before querying,
-00001770: 206f 7074 696f 6e61 6c2e 4e72 3100 0000   optional.Nr1...
-00001780: 7242 0000 0072 3100 0000 7231 0000 0072  rB...r1...r1...r
-00001790: 3300 0000 da04 6c6f 6164 f400 0000 7302  3.....load....s.
-000017a0: 0000 0004 007a 0e42 656e 6368 6d61 726b  .....z.Benchmark
-000017b0: 2e6c 6f61 6429 03da 0261 7472 2000 0000  .load)...atr ...
-000017c0: 7221 0000 00da 0663 6f6e 6669 67fa 1543  r!.....config..C
-000017d0: 207c 204d 6170 7069 6e67 5b73 7472 2c20   | Mapping[str, 
-000017e0: 416e 795d 7265 0000 0072 1600 0000 6302  Any]re...r....c.
-000017f0: 0000 0000 0000 0003 0000 0007 0000 0008  ................
-00001800: 0000 0003 0000 0173 e200 0000 7c02 6401  .......s....|.d.
-00001810: 7501 7206 7c02 6e02 7c00 6a00 7d02 7c00  u.r.|.n.|.j.}.|.
-00001820: 6a01 7c02 0400 0300 6b01 7216 7c00 6a00  j.|.....k.r.|.j.
-00001830: 6b01 7319 4a00 8201 0100 4a00 8201 7402  k.s.J.....J...t.
-00001840: 7c01 7c00 6a03 8302 7329 7c00 6a03 6a04  |.|.j...s)|.j.j.
-00001850: 7c01 7c00 6a05 6402 8d02 7d05 6e02 7c01  |.|.j.d...}.n.|.
-00001860: 7d05 7406 7c05 8301 8900 7c00 6a05 6401  }.t.|.....|.j.d.
-00001870: 7501 7249 6403 6404 8400 7c00 6a05 a007  u.rId.d...|.j...
-00001880: a100 4400 8301 7d06 8700 6601 6405 6404  ..D...}...f.d.d.
-00001890: 8408 7c06 a007 a100 4400 8301 8900 7c03  ..|.....D.....|.
-000018a0: 6401 7501 724f 7c03 6e02 7c00 6a08 7d03  d.u.rO|.n.|.j.}.
-000018b0: 7c04 6401 7501 7258 7c04 6e02 7c00 6a09  |.d.u.rX|.n.|.j.
-000018c0: 7d04 7c00 6a0a 6a04 7c01 7c02 7c00 6a0b  }.|.j.j.|.|.|.j.
-000018d0: 8800 7c02 6406 8d02 740c 7c03 8301 740c  ..|.d...t.|...t.
-000018e0: 7c04 8301 7c00 6a0d 6407 8d06 5300 2908  |...|.j.d...S.).
-000018f0: 6199 0200 0053 7562 6d69 7420 6120 7175  a....Submit a qu
-00001900: 6572 7920 616e 6420 6765 7420 6120 7265  ery and get a re
-00001910: 7375 6c74 2e0a 0a20 2020 2020 2020 2041  sult...        A
-00001920: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00001930: 2063 6f6e 6669 673a 2054 6865 2071 7565   config: The que
-00001940: 7279 2074 6f20 7573 650a 2020 2020 2020  ry to use.      
-00001950: 2020 2020 2020 6174 3a20 5468 6520 6669        at: The fi
-00001960: 6465 6c69 7479 2061 7420 7768 6963 6820  delity at which 
-00001970: 746f 2071 7565 7279 2c20 6465 6661 756c  to query, defaul
-00001980: 7473 2074 6f20 4e6f 6e65 2077 6869 6368  ts to None which
-00001990: 206d 6561 6e73 202a 6d61 7869 6d75 6d2a   means *maximum*
-000019a0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
-000019b0: 7565 5f6d 6574 7269 633a 2054 6865 206d  ue_metric: The m
-000019c0: 6574 7269 6320 746f 2075 7365 2066 6f72  etric to use for
-000019d0: 2074 6869 7320 7265 7375 6c74 2e20 5573   this result. Us
-000019e0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-000019f0: 2020 2074 6865 2076 616c 7565 206d 6574     the value met
-00001a00: 7269 6320 7061 7373 6564 2069 6e20 746f  ric passed in to
-00001a10: 2074 6865 2063 6f6e 7374 7275 6374 6f72   the constructor
-00001a20: 2069 6620 6e6f 7420 7370 6563 6966 6965   if not specifie
-00001a30: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00001a40: 2020 206f 7468 6572 7769 7365 2074 6865     otherwise the
-00001a50: 2064 6566 6175 6c74 206d 6574 7269 6320   default metric 
-00001a60: 6672 6f6d 2074 6865 2052 6573 756c 7420  from the Result 
-00001a70: 6966 204e 6f6e 652e 0a20 2020 2020 2020  if None..       
-00001a80: 2020 2020 2063 6f73 745f 6d65 7472 6963       cost_metric
-00001a90: 3a20 5468 6520 6d65 7472 6963 2074 6f20  : The metric to 
-00001aa0: 7573 6520 666f 7220 7468 6973 2072 6573  use for this res
-00001ab0: 756c 742e 2055 7365 730a 2020 2020 2020  ult. Uses.      
-00001ac0: 2020 2020 2020 2020 2020 7468 6520 636f            the co
-00001ad0: 7374 206d 6574 7269 6320 7061 7373 6564  st metric passed
-00001ae0: 2069 6e20 746f 2074 6865 2063 6f6e 7374   in to the const
-00001af0: 7275 6374 6f72 2069 6620 6e6f 7420 7370  ructor if not sp
-00001b00: 6563 6966 6965 642c 0a20 2020 2020 2020  ecified,.       
-00001b10: 2020 2020 2020 2020 206f 7468 6572 7769           otherwi
-00001b20: 7365 2074 6865 2064 6566 6175 6c74 206d  se the default m
-00001b30: 6574 7269 6320 6672 6f6d 2074 6865 2052  etric from the R
-00001b40: 6573 756c 7420 6966 204e 6f6e 652e 0a0a  esult if None...
-00001b50: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00001b60: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-00001b70: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
-00001b80: 7175 6572 790a 2020 2020 2020 2020 4e72  query.        Nr
-00001b90: 4d00 0000 6301 0000 0000 0000 0000 0000  M...c...........
-00001ba0: 0003 0000 0004 0000 0053 0000 01f3 1600  .........S......
-00001bb0: 0000 6900 7c00 5d07 5c02 7d01 7d02 7c02  ..i.|.].\.}.}.|.
-00001bc0: 7c01 9302 7102 5300 7231 0000 0072 3100  |...q.S.r1...r1.
-00001bd0: 0000 a903 7232 0000 00da 016b da01 7672  ....r2.....k..vr
-00001be0: 3100 0000 7231 0000 0072 3300 0000 7234  1...r1...r3...r4
-00001bf0: 0000 0019 0100 00f3 0200 0000 1600 7a23  ..............z#
-00001c00: 4265 6e63 686d 6172 6b2e 7175 6572 792e  Benchmark.query.
-00001c10: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
-00001c20: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-00001c30: 0300 0000 0700 0000 1300 0001 f31e 0000  ................
-00001c40: 0069 007c 005d 0b5c 027d 017d 027c 0188  .i.|.].\.}.}.|..
-00001c50: 00a0 007c 027c 02a1 0293 0271 0253 0072  ...|.|.....q.S.r
-00001c60: 3100 0000 a901 da03 6765 7472 6900 0000  1.......getri...
-00001c70: a901 da12 5f42 656e 6368 6d61 726b 5f5f  ...._Benchmark__
-00001c80: 636f 6e66 6967 7231 0000 0072 3300 0000  configr1...r3...
-00001c90: 7234 0000 001a 0100 00f3 0200 0000 1e00  r4..............
-00001ca0: a901 7265 0000 00a9 0672 6600 0000 da08  ..re.....rf.....
-00001cb0: 6669 6465 6c69 7479 da06 7265 7375 6c74  fidelity..result
-00001cc0: 7220 0000 0072 2100 0000 724e 0000 0029  r ...r!...rN...)
-00001cd0: 0e72 4800 0000 7246 0000 0072 4f00 0000  .rH...rF...rO...
-00001ce0: 720f 0000 0072 5200 0000 721b 0000 0072  r....rR...r....r
-00001cf0: 4100 0000 7239 0000 0072 2000 0000 7221  A...r9...r ...r!
-00001d00: 0000 0072 1000 0000 da13 5f6f 626a 6563  ...r......_objec
-00001d10: 7469 7665 5f66 756e 6374 696f 6e72 2300  tive_functionr#.
-00001d20: 0000 721a 0000 0029 0772 3d00 0000 7266  ..r....).r=...rf
-00001d30: 0000 0072 6500 0000 7220 0000 0072 2100  ...re...r ...r!.
-00001d40: 0000 da07 5f63 6f6e 6669 67da 105f 7265  ...._config.._re
-00001d50: 7665 7273 655f 7265 6e61 6d65 7372 3100  verse_renamesr1.
-00001d60: 0000 7270 0000 0072 3300 0000 da05 7175  ..rp...r3.....qu
-00001d70: 6572 79f7 0000 0073 2600 0000 1218 2001  ery....s&..... .
-00001d80: 0c02 1401 0402 0802 0a01 1401 1601 1202  ................
-00001d90: 1201 0602 0201 0201 0c01 0601 0601 0401  ................
-00001da0: 06fa 7a0f 4265 6e63 686d 6172 6b2e 7175  ..z.Benchmark.qu
-00001db0: 6572 7929 0572 5500 0000 7257 0000 0072  ery).rU...rW...r
-00001dc0: 4a00 0000 7220 0000 0072 2100 0000 fa07  J...r ...r!.....
-00001dd0: 6c69 7374 5b52 5d63 0200 0000 0000 0000  list[R]c........
-00001de0: 0500 0000 0800 0000 0700 0000 0300 0001  ................
-00001df0: 73bc 0000 007c 0364 0175 0172 067c 036e  s....|.d.u.r.|.n
-00001e00: 0288 036a 007d 037c 0264 0175 0172 0f7c  ...j.}.|.d.u.r.|
-00001e10: 026e 0288 036a 017d 027c 0464 0175 0172  .n...j.}.|.d.u.r
-00001e20: 187c 046e 0288 036a 027d 0474 0388 0183  .|.n...j.}.t....
-00001e30: 0189 0088 036a 0464 0175 0172 3964 0264  .....j.d.u.r9d.d
-00001e40: 0384 0088 036a 04a0 05a1 0044 0083 017d  .....j.....D...}
-00001e50: 0787 0066 0164 0464 0384 087c 07a0 05a1  ...f.d.d...|....
-00001e60: 0044 0083 0189 0088 0464 0175 0172 3f88  .D.......d.u.r?.
-00001e70: 046e 0288 036a 0689 0488 0264 0175 0172  .n...j.....d.u.r
-00001e80: 4888 026e 0288 036a 0789 0287 0187 0287  H..n...j........
-00001e90: 0387 0466 0464 0564 0684 0888 036a 0888  ...f.d.d.....j..
-00001ea0: 007c 027c 037c 0464 078d 0444 0083 0153  .|.|.|.d...D...S
-00001eb0: 0029 0861 1a03 0000 4765 7420 7468 6520  .).a....Get the 
-00001ec0: 6675 6c6c 2074 7261 6a65 6374 6f72 7920  full trajectory 
-00001ed0: 6f66 2061 2063 6f6e 6669 6775 7261 7469  of a configurati
-00001ee0: 6f6e 2e0a 0a20 2020 2020 2020 2041 7267  on...        Arg
-00001ef0: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
-00001f00: 6f6e 6669 673a 2054 6865 2063 6f6e 6669  onfig: The confi
-00001f10: 6720 746f 2071 7565 7279 0a20 2020 2020  g to query.     
-00001f20: 2020 2020 2020 2066 726d 3a20 5374 6172         frm: Star
-00001f30: 7420 6f66 2074 6865 2063 7572 7665 2c20  t of the curve, 
-00001f40: 7368 6f75 6c64 2064 6566 6175 6c74 2074  should default t
-00001f50: 6f20 7468 6520 7374 6172 740a 2020 2020  o the start.    
-00001f60: 2020 2020 2020 2020 746f 3a20 456e 6420          to: End 
-00001f70: 6f66 2074 6865 2063 7572 7665 2c20 7368  of the curve, sh
-00001f80: 6f75 6c64 2064 6566 6175 6c74 2074 6f20  ould default to 
-00001f90: 7468 6520 746f 7461 6c0a 2020 2020 2020  the total.      
-00001fa0: 2020 2020 2020 7374 6570 3a20 5374 6570        step: Step
-00001fb0: 2073 697a 652c 2064 6566 6175 6c74 7320   size, defaults 
-00001fc0: 746f 2060 6063 6c73 2e64 6566 6175 6c74  to ``cls.default
-00001fd0: 5f73 7465 7060 600a 2020 2020 2020 2020  _step``.        
-00001fe0: 2020 2020 7661 6c75 655f 6d65 7472 6963      value_metric
-00001ff0: 3a20 5468 6520 6d65 7472 6963 2074 6f20  : The metric to 
-00002000: 7573 6520 666f 7220 7468 6973 2072 6573  use for this res
-00002010: 756c 742e 2055 7365 730a 2020 2020 2020  ult. Uses.      
-00002020: 2020 2020 2020 2020 2020 7468 6520 7661            the va
-00002030: 6c75 6520 6d65 7472 6963 2070 6173 7365  lue metric passe
-00002040: 6420 696e 2074 6f20 7468 6520 636f 6e73  d in to the cons
-00002050: 7472 7563 746f 7220 6966 206e 6f74 2073  tructor if not s
-00002060: 7065 6369 6669 6564 2c0a 2020 2020 2020  pecified,.      
-00002070: 2020 2020 2020 2020 2020 6f74 6865 7277            otherw
-00002080: 6973 6520 7468 6520 6465 6661 756c 7420  ise the default 
-00002090: 6d65 7472 6963 2066 726f 6d20 7468 6520  metric from the 
-000020a0: 5265 7375 6c74 2069 6620 4e6f 6e65 2e0a  Result if None..
-000020b0: 2020 2020 2020 2020 2020 2020 636f 7374              cost
-000020c0: 5f6d 6574 7269 633a 2054 6865 206d 6574  _metric: The met
-000020d0: 7269 6320 746f 2075 7365 2066 6f72 2074  ric to use for t
-000020e0: 6869 7320 7265 7375 6c74 2e20 5573 6573  his result. Uses
-000020f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002100: 2074 6865 2063 6f73 7420 6d65 7472 6963   the cost metric
-00002110: 2070 6173 7365 6420 696e 2074 6f20 7468   passed in to th
-00002120: 6520 636f 6e73 7472 7563 746f 7220 6966  e constructor if
-00002130: 206e 6f74 2073 7065 6369 6669 6564 2c0a   not specified,.
-00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002150: 6f74 6865 7277 6973 6520 7468 6520 6465  otherwise the de
-00002160: 6661 756c 7420 6d65 7472 6963 2066 726f  fault metric fro
-00002170: 6d20 7468 6520 5265 7375 6c74 2069 6620  m the Result if 
-00002180: 4e6f 6e65 2e0a 0a20 2020 2020 2020 2052  None...        R
-00002190: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000021a0: 2020 2020 4120 6c69 7374 206f 6620 7468      A list of th
-000021b0: 6520 7265 7375 6c74 7320 666f 7220 7468  e results for th
-000021c0: 6973 2063 6f6e 6669 670a 2020 2020 2020  is config.      
-000021d0: 2020 4e63 0100 0000 0000 0000 0000 0000    Nc............
-000021e0: 0300 0000 0400 0000 5300 0001 7268 0000  ........S...rh..
-000021f0: 0072 3100 0000 7231 0000 0072 6900 0000  .r1...r1...ri...
-00002200: 7231 0000 0072 3100 0000 7233 0000 0072  r1...r1...r3...r
-00002210: 3400 0000 4901 0000 726c 0000 007a 2842  4...I...rl...z(B
-00002220: 656e 6368 6d61 726b 2e74 7261 6a65 6374  enchmark.traject
-00002230: 6f72 792e 3c6c 6f63 616c 733e 2e3c 6469  ory.<locals>.<di
-00002240: 6374 636f 6d70 3e63 0100 0000 0000 0000  ctcomp>c........
-00002250: 0000 0000 0300 0000 0700 0000 1300 0001  ................
-00002260: 726d 0000 0072 3100 0000 726e 0000 0072  rm...r1...rn...r
-00002270: 6900 0000 7270 0000 0072 3100 0000 7233  i...rp...r1...r3
-00002280: 0000 0072 3400 0000 4a01 0000 7272 0000  ...r4...J...rr..
-00002290: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
-000022a0: 0000 0a00 0000 1300 0001 7332 0000 0067  ..........s2...g
-000022b0: 007c 005d 155c 027d 017d 0288 026a 006a  .|.].\.}.}...j.j
-000022c0: 0188 007c 017c 0274 0288 0383 0174 0288  ...|.|.t.....t..
-000022d0: 0183 0188 026a 0364 008d 0691 0271 0253  .....j.d.....q.S
-000022e0: 0029 0172 7400 0000 2904 7210 0000 0072  .).rt...).r....r
-000022f0: 5200 0000 7223 0000 0072 1a00 0000 2903  R...r#...r....).
-00002300: 7232 0000 0072 7500 0000 7276 0000 0029  r2...ru...rv...)
-00002310: 0472 6600 0000 7221 0000 0072 3d00 0000  .rf...r!...r=...
-00002320: 7220 0000 0072 3100 0000 7233 0000 00da  r ...r1...r3....
-00002330: 0a3c 6c69 7374 636f 6d70 3e4f 0100 0073  .<listcomp>O...s
-00002340: 1600 0000 0600 0609 06f8 0201 0201 0201  ................
-00002350: 0601 0601 0401 04fa 06ff 7a28 4265 6e63  ..........z(Benc
-00002360: 686d 6172 6b2e 7472 616a 6563 746f 7279  hmark.trajectory
-00002370: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00002380: 6f6d 703e a903 7255 0000 0072 5700 0000  omp>..rU...rW...
-00002390: 724a 0000 0029 0972 4800 0000 7246 0000  rJ...).rH...rF..
-000023a0: 0072 4a00 0000 7241 0000 0072 1b00 0000  .rJ...rA...r....
-000023b0: 7239 0000 0072 2000 0000 7221 0000 00da  r9...r ...r!....
-000023c0: 0b5f 7472 616a 6563 746f 7279 2908 723d  ._trajectory).r=
-000023d0: 0000 0072 6600 0000 7255 0000 0072 5700  ...rf...rU...rW.
-000023e0: 0000 724a 0000 0072 2000 0000 7221 0000  ..rJ...r ...r!..
-000023f0: 0072 7900 0000 7231 0000 0029 0572 7100  .ry...r1...).rq.
-00002400: 0000 7266 0000 0072 2100 0000 723d 0000  ..rf...r!...r=..
-00002410: 0072 2000 0000 7233 0000 00da 0a74 7261  .r ...r3.....tra
-00002420: 6a65 6374 6f72 7928 0100 0073 2200 0000  jectory(...s"...
-00002430: 121b 1201 1201 0802 0a01 1401 1601 1202  ................
-00002440: 1201 1002 0409 0201 0201 0201 0201 04fc  ................
-00002450: 06f7 7a14 4265 6e63 686d 6172 6b2e 7472  ..z.Benchmark.tr
-00002460: 616a 6563 746f 7279 fa11 4d61 7070 696e  ajectory..Mappin
-00002470: 675b 7374 722c 2041 6e79 5dfa 134d 6170  g[str, Any]..Map
-00002480: 7069 6e67 5b73 7472 2c20 666c 6f61 745d  ping[str, float]
-00002490: 6302 0000 0000 0000 0001 0000 0003 0000  c...............
-000024a0: 0001 0000 0043 0000 0172 6300 0000 2902  .....C...rc...).
-000024b0: 7af6 4765 7420 7468 6520 7661 6c75 6520  z.Get the value 
-000024c0: 6f66 2074 6865 2062 656e 6368 6d61 726b  of the benchmark
-000024d0: 2066 6f72 2061 2063 6f6e 6669 6720 6174   for a config at
-000024e0: 2061 2066 6964 656c 6974 792e 0a0a 2020   a fidelity...  
-000024f0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00002500: 2020 2020 2020 2020 636f 6e66 6967 3a20          config: 
-00002510: 5468 6520 636f 6e66 6967 2074 6f20 7175  The config to qu
-00002520: 6572 790a 2020 2020 2020 2020 2020 2020  ery.            
-00002530: 6174 3a20 5468 6520 6669 6465 6c69 7479  at: The fidelity
-00002540: 2074 6f20 6765 7420 7468 6520 7265 7375   to get the resu
-00002550: 6c74 2061 740a 0a20 2020 2020 2020 2052  lt at..        R
-00002560: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00002570: 2020 2020 5468 6520 7265 7375 6c74 206f      The result o
-00002580: 6620 7468 6520 636f 6e66 6967 2061 7320  f the config as 
-00002590: 6b65 7920 7661 6c75 6520 7061 6972 730a  key value pairs.
-000025a0: 2020 2020 2020 2020 4e72 3100 0000 2903          Nr1...).
-000025b0: 723d 0000 0072 6600 0000 7265 0000 0072  r=...rf...re...r
-000025c0: 3100 0000 7231 0000 0072 3300 0000 7277  1...r1...r3...rw
-000025d0: 0000 0060 0100 0073 0200 0000 0410 7a1d  ...`...s......z.
-000025e0: 4265 6e63 686d 6172 6b2e 5f6f 626a 6563  Benchmark._objec
-000025f0: 7469 7665 5f66 756e 6374 696f 6efa 2749  tive_function.'I
-00002600: 7465 7261 626c 655b 7475 706c 655b 462c  terable[tuple[F,
-00002610: 204d 6170 7069 6e67 5b73 7472 2c20 666c   Mapping[str, fl
-00002620: 6f61 745d 5d5d 6302 0000 0000 0000 0003  oat]]]c.........
-00002630: 0000 0005 0000 0006 0000 0003 0000 0173  ...............s
-00002640: 2000 0000 8700 8701 6602 6401 6402 8408   .......f.d.d...
-00002650: 8801 6a00 7c02 7c03 7c04 6403 8d03 4400  ..j.|.|.|.d...D.
-00002660: 8301 5300 2904 61d6 0100 0047 6574 2074  ..S.).a....Get t
-00002670: 6865 2074 7261 6a65 6374 6f72 7920 6f66  he trajectory of
-00002680: 2061 2063 6f6e 6669 672e 0a0a 2020 2020   a config...    
-00002690: 2020 2020 4279 2064 6566 6175 6c74 2074      By default t
-000026a0: 6869 7320 7769 6c6c 206a 7573 7420 6361  his will just ca
-000026b0: 6c6c 2074 6865 0a20 2020 2020 2020 205b  ll the.        [
-000026c0: 605f 6f62 6a65 6374 6976 655f 6675 6e63  `_objective_func
-000026d0: 7469 6f6e 2829 605d 5b6d 6670 6265 6e63  tion()`][mfpbenc
-000026e0: 682e 4265 6e63 686d 6172 6b2e 5f6f 626a  h.Benchmark._obj
-000026f0: 6563 7469 7665 5f66 756e 6374 696f 6e5d  ective_function]
-00002700: 2066 6f72 0a20 2020 2020 2020 2065 6163   for.        eac
-00002710: 6820 6669 6465 6c69 7479 2062 7574 2074  h fidelity but t
-00002720: 6869 7320 6361 6e20 6265 206f 7665 7277  his can be overw
-00002730: 7269 7474 656e 2069 6620 7468 6973 2063  ritten if this c
-00002740: 616e 2062 6520 646f 6e65 206d 6f72 6520  an be done more 
-00002750: 6f70 7469 6d61 6c79 2e0a 0a20 2020 2020  optimaly...     
-00002760: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00002770: 2020 2020 2063 6f6e 6669 673a 2054 6865       config: The
-00002780: 2063 6f6e 6669 6720 746f 2071 7565 7279   config to query
-00002790: 0a20 2020 2020 2020 2020 2020 2066 726d  .            frm
-000027a0: 3a20 5374 6172 7420 6f66 2074 6865 2063  : Start of the c
-000027b0: 7572 7665 2e0a 2020 2020 2020 2020 2020  urve..          
-000027c0: 2020 746f 3a20 456e 6420 6f66 2074 6865    to: End of the
-000027d0: 2063 7572 7665 2e0a 2020 2020 2020 2020   curve..        
-000027e0: 2020 2020 7374 6570 3a20 5374 6570 2073      step: Step s
-000027f0: 697a 652e 0a0a 2020 2020 2020 2020 5265  ize...        Re
-00002800: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00002810: 2020 2041 206c 6973 7420 6f66 2074 6865     A list of the
-00002820: 2072 6573 756c 7473 2066 6f72 2074 6869   results for thi
-00002830: 7320 636f 6e66 6967 0a20 2020 2020 2020  s config.       
-00002840: 2063 0100 0000 0000 0000 0000 0000 0200   c..............
-00002850: 0000 0700 0000 1300 0001 731e 0000 0067  ..........s....g
-00002860: 007c 005d 0b7d 017c 0188 016a 0088 007c  .|.].}.|...j...|
-00002870: 0164 008d 0266 0291 0271 0253 0029 0172  .d...f...q.S.).r
-00002880: 7300 0000 2901 7277 0000 0029 0272 3200  s...).rw...).r2.
-00002890: 0000 7275 0000 00a9 0272 6600 0000 723d  ..ru.....rf...r=
-000028a0: 0000 0072 3100 0000 7233 0000 0072 7c00  ...r1...r3...r|.
-000028b0: 0000 8901 0000 f308 0000 0006 0002 0210  ................
-000028c0: ff06 ff7a 2942 656e 6368 6d61 726b 2e5f  ...z)Benchmark._
-000028d0: 7472 616a 6563 746f 7279 2e3c 6c6f 6361  trajectory.<loca
-000028e0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 727d  ls>.<listcomp>r}
-000028f0: 0000 0029 0172 6100 0000 2905 723d 0000  ...).ra...).r=..
-00002900: 0072 6600 0000 7255 0000 0072 5700 0000  .rf...rU...rW...
-00002910: 724a 0000 0072 3100 0000 7283 0000 0072  rJ...r1...r....r
-00002920: 3300 0000 727e 0000 0072 0100 0073 0600  3...r~...r...s..
-00002930: 0000 0c17 0e02 06fe 7a15 4265 6e63 686d  ........z.Benchm
-00002940: 6172 6b2e 5f74 7261 6a65 6374 6f72 7929  ark._trajectory)
-00002950: 0172 1d00 0000 da01 6efa 2269 6e74 207c  .r......n."int |
-00002960: 206e 702e 7261 6e64 6f6d 2e52 616e 646f   np.random.Rando
-00002970: 6d53 7461 7465 207c 204e 6f6e 6563 0200  mState | Nonec..
-00002980: 0000 0000 0000 0100 0000 0300 0000 0100  ................
-00002990: 0000 4300 0001 f304 0000 0064 0053 00a9  ..C........d.S..
-000029a0: 014e 7231 0000 00a9 0372 3d00 0000 7285  .Nr1.....r=...r.
-000029b0: 0000 0072 1d00 0000 7231 0000 0072 3100  ...r....r1...r1.
-000029c0: 0000 7233 0000 00da 0673 616d 706c 658f  ..r3.....sample.
-000029d0: 0100 00f3 0200 0000 0407 7a10 4265 6e63  ..........z.Benc
-000029e0: 686d 6172 6b2e 7361 6d70 6c65 725c 0000  hmark.sampler\..
-000029f0: 00fa 076c 6973 745b 435d 6302 0000 0000  ...list[C]c.....
-00002a00: 0000 0001 0000 0003 0000 0001 0000 0043  ...............C
-00002a10: 0000 0172 8700 0000 7288 0000 0072 3100  ...r....r....r1.
-00002a20: 0000 7289 0000 0072 3100 0000 7231 0000  ..r....r1...r1..
-00002a30: 0072 3300 0000 728a 0000 0099 0100 0072  .r3...r........r
-00002a40: 8b00 0000 fa0b 4320 7c20 6c69 7374 5b43  ......C | list[C
-00002a50: 5d63 0200 0000 0000 0000 0100 0000 0500  ]c..............
-00002a60: 0000 0400 0000 0300 0001 73a6 0000 0074  ..........s....t
-00002a70: 00a0 0188 006a 02a1 017d 0374 037c 0274  .....j...}.t.|.t
-00002a80: 046a 056a 0683 0272 147c 02a0 0764 0164  .j.j...r.|...d.d
-00002a90: 02a1 027d 046e 0f7c 0264 0375 0172 1a7c  ...}.n.|.d.u.r.|
-00002aa0: 026e 0874 046a 05a0 08a1 00a0 0964 0164  .n.t.j.......d.d
-00002ab0: 02a1 027d 047c 03a0 0a7c 04a1 0101 007c  ...}.|...|.....|
-00002ac0: 0164 0375 0072 3788 006a 0b6a 0c7c 03a0  .d.u.r7..j.j.|..
-00002ad0: 0da1 0088 006a 0e64 048d 0253 007c 0164  .....j.d...S.|.d
-00002ae0: 056b 0272 4788 006a 0b6a 0c7c 03a0 0da1  .k.rG..j.j.|....
-00002af0: 0088 006a 0e64 048d 0267 0153 0087 0066  ...j.d...g.S...f
-00002b00: 0164 0664 0784 087c 03a0 0d7c 01a1 0144  .d.d...|...|...D
-00002b10: 0083 0153 0029 0861 9601 0000 5361 6d70  ...S.).a....Samp
-00002b20: 6c65 2061 2072 616e 646f 6d20 706f 7373  le a random poss
-00002b30: 6962 6c65 2063 6f6e 6669 672e 0a0a 2020  ible config...  
-00002b40: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00002b50: 2020 2020 2020 2020 6e3a 2048 6f77 206d          n: How m
-00002b60: 616e 7920 7361 6d70 6c65 7320 746f 2074  any samples to t
-00002b70: 616b 652c 204e 6f6e 6520 6d65 616e 7320  ake, None means 
-00002b80: 6a73 7574 2061 2073 696e 676c 6520 6f6e  jsut a single on
-00002b90: 652c 206e 6f74 2069 6e20 6120 6c69 7374  e, not in a list
-00002ba0: 0a20 2020 2020 2020 2020 2020 2073 6565  .            see
-00002bb0: 643a 2054 6865 2073 6565 6420 746f 2075  d: The seed to u
-00002bc0: 7365 2066 6f72 2073 616d 706c 696e 670a  se for sampling.
-00002bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002be0: 2021 2121 206e 6f74 6520 2253 6565 6469   !!! note "Seedi
-00002bf0: 6e67 220a 0a20 2020 2020 2020 2020 2020  ng"..           
-00002c00: 2020 2020 2020 2020 2054 6869 7320 6973           This is
-00002c10: 2064 6966 6665 7265 6e74 2074 6861 6e20   different than 
-00002c20: 616e 7920 7365 6564 2070 6173 7365 6420  any seed passed 
-00002c30: 746f 2074 6865 2063 6f6e 7374 7275 6374  to the construct
-00002c40: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00002c50: 2020 2020 2020 2020 6f66 2074 6865 2062          of the b
-00002c60: 656e 6368 6d61 726b 2e0a 0a20 2020 2020  enchmark...     
-00002c70: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00002c80: 2020 2020 2020 2020 4765 7420 6261 636b          Get back
-00002c90: 2061 2070 6f73 7369 626c 6520 436f 6e66   a possible Conf
-00002ca0: 6967 2074 6f20 7573 650a 2020 2020 2020  ig to use.      
-00002cb0: 2020 7201 0000 0069 ffff ff7f 4e72 4d00    r....i....NrM.
-00002cc0: 0000 7235 0000 0063 0100 0000 0000 0000  ..r5...c........
-00002cd0: 0000 0000 0200 0000 0600 0000 1300 0001  ................
-00002ce0: 731e 0000 0067 007c 005d 0b7d 0188 006a  s....g.|.].}...j
-00002cf0: 006a 017c 0188 006a 0264 008d 0291 0271  .j.|...j.d.....q
-00002d00: 0253 0029 0172 4d00 0000 2903 720f 0000  .S.).rM...).r...
-00002d10: 0072 5200 0000 721b 0000 0029 0272 3200  .rR...r....).r2.
-00002d20: 0000 da01 6372 4200 0000 7231 0000 0072  ....crB...r1...r
-00002d30: 3300 0000 727c 0000 00d0 0100 0072 8400  3...r|.......r..
-00002d40: 0000 7a24 4265 6e63 686d 6172 6b2e 7361  ..z$Benchmark.sa
-00002d50: 6d70 6c65 2e3c 6c6f 6361 6c73 3e2e 3c6c  mple.<locals>.<l
-00002d60: 6973 7463 6f6d 703e 290f da04 636f 7079  istcomp>)...copy
-00002d70: da08 6465 6570 636f 7079 7224 0000 0072  ..deepcopyr$...r
-00002d80: 4f00 0000 725f 0000 00da 0672 616e 646f  O...r_.....rando
-00002d90: 6d5a 0b52 616e 646f 6d53 7461 7465 da07  mZ.RandomState..
-00002da0: 7261 6e64 696e 745a 0b64 6566 6175 6c74  randintZ.default
-00002db0: 5f72 6e67 da08 696e 7465 6765 7273 721d  _rng..integersr.
-00002dc0: 0000 0072 0f00 0000 7252 0000 005a 1473  ...r....rR...Z.s
-00002dd0: 616d 706c 655f 636f 6e66 6967 7572 6174  ample_configurat
-00002de0: 696f 6e72 1b00 0000 2905 723d 0000 0072  ionr....).r=...r
-00002df0: 8500 0000 721d 0000 0072 2400 0000 da03  ....r....r$.....
-00002e00: 726e 6772 3100 0000 7242 0000 0072 3300  rngr1...rB...r3.
-00002e10: 0000 728a 0000 00a2 0100 0073 2c00 0000  ..r........s,...
-00002e20: 0c14 0e01 0e01 0804 04ff 1002 02fd 0a06  ................
-00002e30: 0801 0601 0601 0401 06fe 0806 0602 0601  ................
-00002e40: 0401 04fe 04ff 0a07 0802 06fe fa14 5265  ..............Re
-00002e50: 7375 6c74 4672 616d 655b 432c 2046 2c20  sultFrame[C, F, 
-00002e60: 525d 6301 0000 0000 0000 0000 0000 0001  R]c.............
-00002e70: 0000 0004 0000 0043 0000 0173 1000 0000  .......C...s....
-00002e80: 7400 7401 7402 7403 6603 1900 8300 5300  t.t.t.t.f.....S.
-00002e90: 2901 7a22 4765 7420 616e 2065 6d70 7479  ).z"Get an empty
-00002ea0: 2066 7261 6d65 2074 6f20 7265 636f 7264   frame to record
-00002eb0: 2077 6974 682e 2904 7211 0000 0072 1400   with.).r....r..
-00002ec0: 0000 7217 0000 0072 1600 0000 7242 0000  ..r....r....rB..
-00002ed0: 0072 3100 0000 7231 0000 0072 3300 0000  .r1...r1...r3...
-00002ee0: da05 6672 616d 65d5 0100 0073 0200 0000  ..frame....s....
-00002ef0: 1002 7a0f 4265 6e63 686d 6172 6b2e 6672  ..z.Benchmark.fr
-00002f00: 616d 6529 1872 2200 0000 7223 0000 0072  ame).r"...r#...r
-00002f10: 2400 0000 7212 0000 0072 2500 0000 7226  $...r....r%...r&
-00002f20: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
-00002f30: 0000 722a 0000 0072 2b00 0000 7223 0000  ..r*...r+...r#..
-00002f40: 0072 1c00 0000 722c 0000 0072 1d00 0000  .r....r,...r....
-00002f50: 722d 0000 0072 1e00 0000 722e 0000 0072  r-...r....r....r
-00002f60: 1f00 0000 722f 0000 0072 2000 0000 7230  ....r/...r ...r0
-00002f70: 0000 0072 2100 0000 7230 0000 0029 0272  ...r!...r0...).r
-00002f80: 3f00 0000 7240 0000 0029 0272 3f00 0000  ?...r@...).r?...
-00002f90: 7217 0000 0072 8800 0000 2906 721e 0000  r....r....).r...
-00002fa0: 0072 4b00 0000 7236 0000 0072 3000 0000  .rK...r6...r0...
-00002fb0: 723f 0000 0072 1400 0000 2903 4e4e 4e29  r?...r....).NNN)
-00002fc0: 0872 5500 0000 7256 0000 0072 5700 0000  .rU...rV...rW...
-00002fd0: 7256 0000 0072 4a00 0000 7256 0000 0072  rV...rJ...rV...r
-00002fe0: 3f00 0000 7258 0000 0029 0272 3f00 0000  ?...rX...).r?...
-00002ff0: 7262 0000 0029 0a72 6600 0000 7267 0000  rb...).rf...rg..
-00003000: 0072 6500 0000 7256 0000 0072 2000 0000  .re...rV...r ...
-00003010: 7230 0000 0072 2100 0000 7230 0000 0072  r0...r!...r0...r
-00003020: 3f00 0000 7216 0000 0029 0e72 6600 0000  ?...r....).rf...
-00003030: 7267 0000 0072 5500 0000 7256 0000 0072  rg...rU...rV...r
-00003040: 5700 0000 7256 0000 0072 4a00 0000 7256  W...rV...rJ...rV
-00003050: 0000 0072 2000 0000 7230 0000 0072 2100  ...r ...r0...r!.
-00003060: 0000 7230 0000 0072 3f00 0000 727b 0000  ..r0...r?...r{..
-00003070: 0029 0672 6600 0000 7280 0000 0072 6500  .).rf...r....re.
-00003080: 0000 7217 0000 0072 3f00 0000 7281 0000  ..r....r?...r...
-00003090: 0029 0a72 6600 0000 7280 0000 0072 5500  .).rf...r....rU.
-000030a0: 0000 7217 0000 0072 5700 0000 7217 0000  ..r....rW...r...
-000030b0: 0072 4a00 0000 7217 0000 0072 3f00 0000  .rJ...r....r?...
-000030c0: 7282 0000 0029 0672 8500 0000 7262 0000  r....).r....rb..
-000030d0: 0072 1d00 0000 7286 0000 0072 3f00 0000  .r....r....r?...
-000030e0: 7214 0000 0029 0672 8500 0000 725c 0000  r....).r....r\..
-000030f0: 0072 1d00 0000 7286 0000 0072 3f00 0000  .r....r....r?...
-00003100: 728c 0000 0029 0672 8500 0000 722d 0000  r....).r....r-..
-00003110: 0072 1d00 0000 7286 0000 0072 3f00 0000  .r....r....r?...
-00003120: 728d 0000 0029 0272 3f00 0000 7295 0000  r....).r?...r...
-00003130: 0029 1ada 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
-00003140: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-00003150: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
-00003160: da09 5052 494f 525f 4449 5272 1900 0000  ..PRIOR_DIRr....
-00003170: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-00003180: 5f72 1a00 0000 721b 0000 0072 3e00 0000  _r....r....r>...
-00003190: da08 7072 6f70 6572 7479 7243 0000 0072  ..propertyrC...r
-000031a0: 4600 0000 7248 0000 0072 4a00 0000 723c  F...rH...rJ...r<
-000031b0: 0000 0072 6100 0000 7264 0000 0072 7a00  ...ra...rd...rz.
-000031c0: 0000 727f 0000 0072 0400 0000 7277 0000  ..r....r....rw..
-000031d0: 0072 7e00 0000 720e 0000 0072 8a00 0000  .r~...r....r....
-000031e0: 7296 0000 0072 3100 0000 7231 0000 0072  r....r1...r1...r
-000031f0: 3100 0000 7233 0000 0072 1800 0000 2a00  1...r3...r....*.
-00003200: 0000 7370 0000 000a 0004 010c 0202 010c  ..sp............
-00003210: 0202 010c 0602 0102 0f02 0102 0102 0102  ................
-00003220: 0102 010e f202 600c 0102 040c 0102 040c  ......`.........
-00003230: 0102 040c 0102 070c fd02 1e02 0102 010c  ................
-00003240: fc0a 2602 0702 0102 010e fa02 3502 0102  ..&.........5...
-00003250: 0102 0102 010e f802 380c 010a 1102 1d02  ........8.......
-00003260: 0302 fe02 0410 fc02 0902 0510 fc02 0a02  ................
-00003270: fe02 040e fc0e 3372 1800 0000 2928 da0a  ......3r....)(..
-00003280: 5f5f 6675 7475 7265 5f5f 7202 0000 0072  __future__r....r
-00003290: 8f00 0000 da03 6162 6372 0300 0000 7204  ......abcr....r.
-000032a0: 0000 00da 0770 6174 686c 6962 7205 0000  .....pathlibr...
-000032b0: 00da 0674 7970 696e 6772 0600 0000 7207  ...typingr....r.
-000032c0: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-000032d0: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-000032e0: 0072 0e00 0000 da05 6e75 6d70 7972 5f00  .r......numpyr_.
-000032f0: 0000 da0f 6d66 7062 656e 6368 2e63 6f6e  ....mfpbench.con
-00003300: 6669 6772 0f00 0000 da0f 6d66 7062 656e  figr......mfpben
-00003310: 6368 2e72 6573 756c 7472 1000 0000 5a14  ch.resultr....Z.
-00003320: 6d66 7062 656e 6368 2e72 6573 756c 7466  mfpbench.resultf
-00003330: 7261 6d65 7211 0000 005a 0b43 6f6e 6669  ramer....Z.Confi
-00003340: 6753 7061 6365 7212 0000 00da 0f6d 6670  gSpacer......mfp
-00003350: 6265 6e63 682e 6d65 7472 6963 7213 0000  bench.metricr...
-00003360: 00da 085f 5f66 696c 655f 5fda 0670 6172  ...__file__..par
-00003370: 656e 745a 0448 4552 4572 9b00 0000 7214  entZ.HEREr....r.
-00003380: 0000 0072 1600 0000 725c 0000 0072 5d00  ...r....r\...r].
-00003390: 0000 7217 0000 0072 1800 0000 7231 0000  ..r....r....r1..
-000033a0: 0072 3100 0000 7231 0000 0072 3300 0000  .r1...r1...r3...
-000033b0: da08 3c6d 6f64 756c 653e 0100 0000 7324  ..<module>....s$
-000033c0: 0000 000c 0008 0210 010c 012c 0108 0c0c  ...........,....
-000033d0: 020c 010c 0104 020c 010c 020c 0208 010c  ................
-000033e0: 030c 030c 0320 03                        ..... .
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
+00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6405 6c0d 5a0e 6400 6405 6c0f  ..d.d.l.Z.d.d.l.
+00000080: 5a10 6400 6406 6c11 6d12 5a12 0100 6400  Z.d.d.l.m.Z...d.
+00000090: 6407 6c13 6d14 5a14 0100 6400 6408 6c15  d.l.m.Z...d.d.l.
+000000a0: 6d16 5a16 0100 6400 6409 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
+000000b0: 0100 6400 640a 6c19 6d1a 5a1a 0100 6505  ..d.d.l.m.Z...e.
+000000c0: 7250 6400 640b 6c1b 6d1c 5a1c 0100 6509  rPd.d.l.m.Z...e.
+000000d0: 640c 6518 640d 8d02 5a1d 6509 640e 651a  d.e.d...Z.e.d.e.
+000000e0: 640d 8d02 5a1e 6509 640f 651f 6520 8303  d...Z.e.d.e.e ..
+000000f0: 5a21 4700 6410 6411 8400 6411 6516 651d  Z!G.d.d...d.e.e.
+00000100: 651e 6521 6603 1900 8303 5a22 6523 6412  e.e!f.....Z"e#d.
+00000110: 6b02 72c9 6503 6524 8301 6a25 5a26 6526  k.r.e.e$..j%Z&e&
+00000120: 6a25 6a25 6413 1b00 6414 1b00 6415 1b00  j%j%d...d...d...
+00000130: 5a27 6510 a028 6527 a101 5a29 6400 6416  Z'e..(e'..Z)d.d.
+00000140: 6c2a 6d2b 5a2b 6d2c 5a2c 0100 6522 6417  l*m+Z+m,Z,..e"d.
+00000150: 6529 6418 6419 652c 652b 641a 8d06 5a2d  e)d.d.e,e+d...Z-
+00000160: 652d 6a2e 5a2f 6530 652f a031 a100 8301  e-j.Z/e0e/.1....
+00000170: 5a32 6530 652f a033 a100 8301 5a2e 652d  Z2e0e/.3....Z.e-
+00000180: 6a34 641b 641c 8d01 5a35 6535 6a36 5a37  j4d.d...Z5e5j6Z7
+00000190: 652d 6a38 6535 641b 641d 8d02 5a39 652d  e-j8e5d.d...Z9e-
+000001a0: 6a38 6535 641e 641d 8d02 5a3a 652d 6a3b  j8e5d.d...Z:e-j;
+000001b0: 6535 641b 641f 6420 8d03 5a3b 6405 5300  e5d.d.d ..Z;d.S.
+000001c0: 6405 5300 2921 e900 0000 0029 01da 0b61  d.S.)!.....)...a
+000001d0: 6e6e 6f74 6174 696f 6e73 2901 da04 5061  nnotations)...Pa
+000001e0: 7468 2906 da0d 5459 5045 5f43 4845 434b  th)...TYPE_CHECK
+000001f0: 494e 47da 0341 6e79 da08 4974 6572 6162  ING..Any..Iterab
+00000200: 6c65 da07 4d61 7070 696e 67da 0754 7970  le..Mapping..Typ
+00000210: 6556 6172 da08 6f76 6572 6c6f 6164 2901  eVar..overload).
+00000220: da08 6f76 6572 7269 6465 4e29 01da 1243  ..overrideN)...C
+00000230: 6f6e 6669 6775 7261 7469 6f6e 5370 6163  onfigurationSpac
+00000240: 6529 01da 0a66 6972 7374 5f74 7275 6529  e)...first_true)
+00000250: 01da 0942 656e 6368 6d61 726b 2901 da0d  ...Benchmark)...
+00000260: 5461 6275 6c61 7243 6f6e 6669 6729 01da  TabularConfig)..
+00000270: 0652 6573 756c 7429 01da 064d 6574 7269  .Result)...Metri
+00000280: 63da 0843 5461 6275 6c61 7229 01da 0562  c..CTabular)...b
+00000290: 6f75 6e64 da01 52da 0146 6300 0000 0000  ound..R..Fc.....
+000002a0: 0000 0000 0000 0000 0000 0007 0000 0000  ................
+000002b0: 0000 0173 c800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+000002c0: 6401 6401 6401 6401 6401 6401 6402 9c06  d.d.d.d.d.d.d...
+000002d0: 6442 8700 6601 6418 6419 840e 5a03 6401  dB..f.d.d...Z.d.
+000002e0: 6401 6401 641a 9c03 6443 6421 6422 8406  d.d.d...dCd!d"..
+000002f0: 5a04 6505 6401 6401 6401 6401 6401 6423  Z.e.d.d.d.d.d.d#
+00000300: 9c05 6444 6428 6429 8406 8301 5a06 6445  ..dDd(d)....Z.dE
+00000310: 642c 642d 8404 5a07 6505 6446 6431 6432  d,d-..Z.e.dFd1d2
+00000320: 8404 8301 5a08 6505 6447 6434 6435 8404  ....Z.e.dGd4d5..
+00000330: 8301 5a09 650a 0901 6448 6436 6437 9c01  ..Z.e...dHd6d7..
+00000340: 6449 643b 643c 8407 8301 5a0b 650a 6436  dId;d<....Z.e.d6
+00000350: 6437 9c01 644a 643f 643c 8406 8301 5a0b  d7..dJd?d<....Z.
+00000360: 6505 0901 6448 6401 6437 9c01 644b 6441  e...dHd.d7..dKdA
+00000370: 643c 8407 8301 5a0b 8700 0400 5a0c 5300  d<....Z.....Z.S.
+00000380: 294c da10 5461 6275 6c61 7242 656e 6368  )L..TabularBench
+00000390: 6d61 726b 4e29 06da 0c76 616c 7565 5f6d  markN)...value_m
+000003a0: 6574 7269 63da 0b63 6f73 745f 6d65 7472  etric..cost_metr
+000003b0: 6963 da05 7370 6163 65da 0473 6565 64da  ic..space..seed.
+000003c0: 0570 7269 6f72 da0d 7065 7274 7572 625f  .prior..perturb_
+000003d0: 7072 696f 72da 046e 616d 65da 0373 7472  prior..name..str
+000003e0: da05 7461 626c 65fa 0c70 642e 4461 7461  ..table..pd.Data
+000003f0: 4672 616d 65da 0669 645f 6b65 79da 0c66  Frame..id_key..f
+00000400: 6964 656c 6974 795f 6b65 79da 0b72 6573  idelity_key..res
+00000410: 756c 745f 7479 7065 fa07 7479 7065 5b52  ult_type..type[R
+00000420: 5dda 0b63 6f6e 6669 675f 7479 7065 fa0e  ]..config_type..
+00000430: 7479 7065 5b43 5461 6275 6c61 725d 7216  type[CTabular]r.
+00000440: 0000 00fa 0a73 7472 207c 204e 6f6e 6572  .....str | Noner
+00000450: 1700 0000 7218 0000 00fa 1943 6f6e 6669  ....r......Confi
+00000460: 6775 7261 7469 6f6e 5370 6163 6520 7c20  gurationSpace | 
+00000470: 4e6f 6e65 7219 0000 00fa 0a69 6e74 207c  Noner......int |
+00000480: 204e 6f6e 6572 1a00 0000 fa30 7374 7220   Noner.....0str 
+00000490: 7c20 5061 7468 207c 2043 5461 6275 6c61  | Path | CTabula
+000004a0: 7220 7c20 4d61 7070 696e 675b 7374 722c  r | Mapping[str,
+000004b0: 2041 6e79 5d20 7c20 4e6f 6e65 721b 0000   Any] | Noner...
+000004c0: 00fa 0c66 6c6f 6174 207c 204e 6f6e 6563  ...float | Nonec
+000004d0: 0300 0000 0000 0000 0a00 0000 1900 0000  ................
+000004e0: 0d00 0000 0300 0001 738c 0200 0088 02a0  ........s.......
+000004f0: 00a1 0089 027c 0388 026a 0176 0172 1474  .....|...j.v.r.t
+00000500: 0264 017c 039b 0264 0288 026a 019b 009d  .d.|...d...j....
+00000510: 0483 0182 017c 0488 026a 0176 0172 2474  .....|...j.v.r$t
+00000520: 0264 037c 049b 0264 0288 026a 019b 009d  .d.|...d...j....
+00000530: 0483 0182 0174 037c 056a 04a0 05a1 0083  .....t.|.j......
+00000540: 017d 0d74 0687 0266 0164 0464 0584 087c  .}.t...f.d.d...|
+00000550: 0d44 0083 0183 0173 4174 0264 067c 0d9b  .D.....sAt.d.|..
+00000560: 0264 0788 026a 019b 009d 0483 0182 0188  .d...j..........
+00000570: 01a0 07a1 0089 0074 0687 0266 0164 0864  .......t...f.d.d
+00000580: 0584 0888 0044 0083 0183 0173 5b74 0264  .....D.....s[t.d
+00000590: 0988 009b 0264 0788 026a 019b 009d 0483  .....d...j......
+000005a0: 0182 0164 0a88 026a 0176 0072 6c7c 0364  ...d...j.v.rl|.d
+000005b0: 0a6b 0372 6c74 0264 0b7c 039b 0264 0c9d  .k.rlt.d.|...d..
+000005c0: 0383 0182 0188 026a 087c 0364 0a69 0164  .......j.|.d.i.d
+000005d0: 0d8d 0189 0264 0a7c 0467 027d 0e67 007c  .....d.|.g.}.g.|
+000005e0: 0ea2 017c 0da2 0188 00a2 017d 0f88 027c  ...|.......}...|
+000005f0: 0f19 0089 0288 02a0 097c 0ea1 01a0 0aa1  .........|......
+00000600: 0089 0288 026a 0ba0 0c7c 04a1 017d 107c  .....j...|...}.|
+00000610: 10a0 0da1 007d 117c 117c 116a 0e64 0e19  .....}.|.|.j.d..
+00000620: 006b 02a0 06a1 0073 a874 0264 0f7c 049b  .k.....s.t.d.|..
+00000630: 0264 107c 119b 009d 0483 0182 0174 0f7c  .d.|.........t.|
+00000640: 10a0 10a1 0083 017d 127c 1264 0e19 007d  .......}.|.d...}
+00000650: 137c 1264 1119 007d 147c 1264 1219 007c  .|.d...}.|.d...|
+00000660: 1264 0e19 0018 007d 1588 026a 1164 0a64  .d.....}...j.d.d
+00000670: 138d 01a0 1264 14a1 017d 1687 0087 0166  .....d...}.....f
+00000680: 0264 1564 1684 087c 16a0 13a1 0044 0083  .d.d...|.....D..
+00000690: 017d 177c 0964 1775 0072 dd74 147c 017c  .}.|.d.u.r.t.|.|
+000006a0: 0a64 188d 027d 0988 027c 005f 157c 177c  .d...}...|._.|.|
+000006b0: 005f 167c 037c 005f 177c 047c 005f 1874  ._.|.|._.|.|._.t
+000006c0: 0f88 0083 017c 005f 1974 0f7c 0d83 017c  .....|._.t.|...|
+000006d0: 005f 1a74 1b83 006a 1c7c 017c 0a88 017c  ._.t...j.|.|...|
+000006e0: 057c 047c 137c 147c 1566 037c 097c 0b7c  .|.|.|.|.f.|.|.|
+000006f0: 0c7c 077c 0864 198d 0b01 0087 0266 0164  .|.|.d.......f.d
+00000700: 1a64 1684 087c 006a 1d6a 04a0 1ea1 0044  .d...|.j.j.....D
+00000710: 0083 017d 1864 1b64 1684 007c 18a0 1ea1  ...}.d.d...|....
+00000720: 0044 0083 017c 005f 1f7c 006a 207c 006a  .D...|._.|.j |.j
+00000730: 1a76 0190 0172 3174 0264 1c7c 006a 209b  .v...r1t.d.|.j .
+00000740: 0264 1d7c 006a 1a9b 009d 0483 0182 017c  .d.|.j.........|
+00000750: 006a 217c 006a 1a76 0190 0172 4474 0264  .j!|.j.v...rDt.d
+00000760: 1e7c 006a 219b 0264 1d7c 006a 1a9b 009d  .|.j!..d.|.j....
+00000770: 0483 0182 0164 1753 0029 1f61 a605 0000  .....d.S.).a....
+00000780: 496e 6974 6961 6c69 7a65 2074 6865 2062  Initialize the b
+00000790: 656e 6368 6d61 726b 2e0a 0a20 2020 2020  enchmark...     
+000007a0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+000007b0: 2020 2020 206e 616d 653a 2054 6865 206e       name: The n
+000007c0: 616d 6520 6f66 2074 6869 7320 6265 6e63  ame of this benc
+000007d0: 686d 6172 6b2e 0a20 2020 2020 2020 2020  hmark..         
+000007e0: 2020 2074 6162 6c65 3a20 5468 6520 7461     table: The ta
+000007f0: 626c 6520 746f 2075 7365 2066 6f72 2074  ble to use for t
+00000800: 6865 2062 656e 6368 6d61 726b 2e0a 2020  he benchmark..  
+00000810: 2020 2020 2020 2020 2020 6964 5f6b 6579            id_key
+00000820: 3a20 5468 6520 636f 6c75 6d6e 2069 6e20  : The column in 
+00000830: 7468 6520 7461 626c 6520 7468 6174 2063  the table that c
+00000840: 6f6e 7461 696e 7320 7468 6520 636f 6e66  ontains the conf
+00000850: 6967 2069 640a 2020 2020 2020 2020 2020  ig id.          
+00000860: 2020 6669 6465 6c69 7479 5f6b 6579 3a20    fidelity_key: 
+00000870: 5468 6520 636f 6c75 6d6e 2069 6e20 7468  The column in th
+00000880: 6520 7461 626c 6520 7468 6174 2063 6f6e  e table that con
+00000890: 7461 696e 7320 7468 6520 6669 6465 6c69  tains the fideli
+000008a0: 7479 0a20 2020 2020 2020 2020 2020 2072  ty.            r
+000008b0: 6573 756c 745f 7479 7065 3a20 5468 6520  esult_type: The 
+000008c0: 7265 7375 6c74 2074 7970 6520 666f 7220  result type for 
+000008d0: 7468 6973 2062 656e 6368 6d61 726b 2e0a  this benchmark..
+000008e0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+000008f0: 6967 5f74 7970 653a 2054 6865 2063 6f6e  ig_type: The con
+00000900: 6669 6720 7479 7065 2066 6f72 2074 6869  fig type for thi
+00000910: 7320 6265 6e63 686d 6172 6b2e 0a20 2020  s benchmark..   
+00000920: 2020 2020 2020 2020 2076 616c 7565 5f6d           value_m
+00000930: 6574 7269 633a 2054 6865 206d 6574 7269  etric: The metri
+00000940: 6320 746f 2075 7365 2066 6f72 2074 6869  c to use for thi
+00000950: 7320 6265 6e63 686d 6172 6b2e 2055 7365  s benchmark. Use
+00000960: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00000970: 2020 7468 6520 6465 6661 756c 7420 6d65    the default me
+00000980: 7472 6963 2066 726f 6d20 7468 6520 5265  tric from the Re
+00000990: 7375 6c74 2069 6620 4e6f 6e65 2e0a 2020  sult if None..  
+000009a0: 2020 2020 2020 2020 2020 636f 7374 5f6d            cost_m
+000009b0: 6574 7269 633a 2054 6865 2063 6f73 7420  etric: The cost 
+000009c0: 746f 2075 7365 2066 6f72 2074 6869 7320  to use for this 
+000009d0: 6265 6e63 686d 6172 6b2e 2055 7365 730a  benchmark. Uses.
+000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000009f0: 7468 6520 6465 6661 756c 7420 636f 7374  the default cost
+00000a00: 2066 726f 6d20 7468 6520 5265 7375 6c74   from the Result
+00000a10: 2069 6620 4e6f 6e65 2e0a 2020 2020 2020   if None..      
+00000a20: 2020 2020 2020 7370 6163 653a 2054 6865        space: The
+00000a30: 2063 6f6e 6669 6775 7261 7469 6f6e 2073   configuration s
+00000a40: 7061 6365 2074 6f20 7573 6520 666f 7220  pace to use for 
+00000a50: 7468 6520 6265 6e63 686d 6172 6b2e 2049  the benchmark. I
+00000a60: 6620 4e6f 6e65 2c20 7769 6c6c 0a20 2020  f None, will.   
+00000a70: 2020 2020 2020 2020 2020 2020 206a 7573               jus
+00000a80: 7420 6265 2061 6e20 656d 7074 7920 7370  t be an empty sp
+00000a90: 6163 652e 0a20 2020 2020 2020 2020 2020  ace..           
+00000aa0: 2070 7269 6f72 3a20 5468 6520 7072 696f   prior: The prio
+00000ab0: 7220 746f 2075 7365 2066 6f72 2074 6865  r to use for the
+00000ac0: 2062 656e 6368 6d61 726b 2e20 4966 204e   benchmark. If N
+00000ad0: 6f6e 652c 206e 6f20 7072 696f 7220 6973  one, no prior is
+00000ae0: 2075 7365 642e 0a20 2020 2020 2020 2020   used..         
+00000af0: 2020 2020 2020 2049 6620 6120 7374 7269         If a stri
+00000b00: 6e67 2c20 7769 6c6c 2062 6520 7472 6561  ng, will be trea
+00000b10: 7465 6420 6173 2061 2070 7269 6f72 2073  ted as a prior s
+00000b20: 7065 6369 6669 6320 666f 7220 7468 6973  pecific for this
+00000b30: 2062 656e 6368 6d61 726b 0a20 2020 2020   benchmark.     
+00000b40: 2020 2020 2020 2020 2020 2069 6620 6974             if it
+00000b50: 2063 616e 2062 6520 666f 756e 642c 206f   can be found, o
+00000b60: 7468 6572 7769 7365 2061 7373 756d 6573  therwise assumes
+00000b70: 2069 7420 746f 2062 6520 6120 5061 7468   it to be a Path
+00000b80: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000b90: 2020 4966 2061 2050 6174 682c 2077 696c    If a Path, wil
+00000ba0: 6c20 6c6f 6164 2074 6865 2070 7269 6f72  l load the prior
+00000bb0: 2066 726f 6d20 7468 6520 7061 7468 2e0a   from the path..
+00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bd0: 4966 2061 2064 6963 7420 6f72 2043 6f6e  If a dict or Con
+00000be0: 6669 6775 7261 7469 6f6e 2c20 7769 6c6c  figuration, will
+00000bf0: 2062 6520 7573 6564 2064 6972 6563 746c   be used directl
+00000c00: 792e 0a20 2020 2020 2020 2020 2020 2070  y..            p
+00000c10: 6572 7475 7262 5f70 7269 6f72 3a20 4966  erturb_prior: If
+00000c20: 206e 6f74 204e 6f6e 652c 2077 696c 6c20   not None, will 
+00000c30: 7065 7274 7572 6220 7468 6520 7072 696f  perturb the prio
+00000c40: 7220 6279 2074 6869 7320 616d 6f75 6e74  r by this amount
+00000c50: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000c60: 2020 466f 7220 6e75 6d65 7269 6361 6c73    For numericals
+00000c70: 2c20 7768 696c 6520 666f 7220 6361 7465  , while for cate
+00000c80: 676f 7269 6361 6c73 2c20 7468 6973 2069  goricals, this i
+00000c90: 7320 696e 7465 7270 7265 7465 6420 6173  s interpreted as
+00000ca0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00000cb0: 2020 2020 2070 726f 6261 6269 6c69 7479       probability
+00000cc0: 206f 6620 7377 6170 7069 6e67 2074 6865   of swapping the
+00000cd0: 2076 616c 7565 2066 6f72 2061 2072 616e   value for a ran
+00000ce0: 646f 6d20 6f6e 652e 0a20 2020 2020 2020  dom one..       
+00000cf0: 2020 2020 2073 6565 643a 2054 6865 2073       seed: The s
+00000d00: 6565 6420 746f 2075 7365 2066 6f72 2074  eed to use for t
+00000d10: 6865 2062 656e 6368 6d61 726b 2e0a 2020  he benchmark..  
+00000d20: 2020 2020 2020 7a08 2769 645f 6b65 793d        z.'id_key=
+00000d30: 7a11 2720 6e6f 7420 696e 2063 6f6c 756d  z.' not in colum
+00000d40: 6e73 207a 0e27 6669 6465 6c69 7479 5f6b  ns z.'fidelity_k
+00000d50: 6579 3d63 0100 0000 0000 0000 0000 0000  ey=c............
+00000d60: 0200 0000 0300 0000 3300 0001 f31a 0000  ........3.......
+00000d70: 0081 007c 005d 087d 017c 0188 006a 0076  ...|.].}.|...j.v
+00000d80: 0056 0001 0071 0264 0053 00a9 014e a901  .V...q.d.S...N..
+00000d90: da07 636f 6c75 6d6e 73a9 02da 022e 30da  ..columns.....0.
+00000da0: 036b 6579 a901 721e 0000 00a9 00fa 3a2f  .key..r.......:/
+00000db0: 686f 6d65 2f73 6b61 6e74 6966 792f 636f  home/skantify/co
+00000dc0: 6465 2f6d 662d 7072 696f 722d 6265 6e63  de/mf-prior-benc
+00000dd0: 682f 7372 632f 6d66 7062 656e 6368 2f74  h/src/mfpbench/t
+00000de0: 6162 756c 6172 2e70 79da 093c 6765 6e65  abular.py..<gene
+00000df0: 7870 723e 5300 0000 f304 0000 0002 8018  xpr>S...........
+00000e00: 007a 2c54 6162 756c 6172 4265 6e63 686d  .z,TabularBenchm
+00000e10: 6172 6b2e 5f5f 696e 6974 5f5f 2e3c 6c6f  ark.__init__.<lo
+00000e20: 6361 6c73 3e2e 3c67 656e 6578 7072 3e7a  cals>.<genexpr>z
+00000e30: 144e 6f74 2061 6c6c 2072 6573 756c 745f  .Not all result_
+00000e40: 6b65 7973 3d7a 1020 6e6f 7420 696e 2063  keys=z. not in c
+00000e50: 6f6c 756d 6e73 2063 0100 0000 0000 0000  olumns c........
+00000e60: 0000 0000 0200 0000 0300 0000 3300 0001  ............3...
+00000e70: 722b 0000 0072 2c00 0000 722d 0000 0072  r+...r,...r-...r
+00000e80: 2f00 0000 7232 0000 0072 3300 0000 7234  /...r2...r3...r4
+00000e90: 0000 0072 3500 0000 5900 0000 7236 0000  ...r5...Y...r6..
+00000ea0: 007a 0c63 6f6e 6669 675f 6b65 7973 3dda  .z.config_keys=.
+00000eb0: 0269 647a 3643 616e 2774 2068 6176 6520  .idz6Can't have 
+00000ec0: 6069 6460 2069 6e20 7468 6520 636f 6c75  `id` in the colu
+00000ed0: 6d6e 7320 6966 2069 7427 7320 6e6f 7420  mns if it's not 
+00000ee0: 7468 6520 6964 5f6b 6579 3d7a 1e2e 2050  the id_key=z.. P
+00000ef0: 6c65 6173 6520 6472 6f70 2069 7420 6f72  lease drop it or
+00000f00: 2072 656e 616d 6520 6974 2e72 2d00 0000   rename it.r-...
+00000f10: 7201 0000 007a 0d66 6964 656c 6974 795f  r....z.fidelity_
+00000f20: 6b65 793d 7a0f 206e 6f74 2075 6e69 666f  key=z. not unifo
+00000f30: 726d 2e20 0ae9 ffff ffff e901 0000 0029  rm. ...........)
+00000f40: 01da 056c 6576 656c da05 6669 7273 7463  ...level..firstc
+00000f50: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00000f60: 0900 0000 1300 0001 7338 0000 0069 007c  ........s8...i.|
+00000f70: 005d 185c 027d 017d 0274 007c 0183 0188  .].\.}.}.t.|....
+00000f80: 01a0 0169 007c 0288 0019 00a0 02a1 00a5  ...i.|..........
+00000f90: 0164 0074 007c 0183 0169 01a5 01a1 0193  .d.t.|...i......
+00000fa0: 0271 0253 0029 0172 3700 0000 2903 721d  .q.S.).r7...).r.
+00000fb0: 0000 00da 0966 726f 6d5f 6469 6374 da07  .....from_dict..
+00000fc0: 746f 5f64 6963 7429 0372 3000 0000 da09  to_dict).r0.....
+00000fd0: 636f 6e66 6967 5f69 64da 0372 6f77 2902  config_id..row).
+00000fe0: da0b 636f 6e66 6967 5f6b 6579 7372 2400  ..config_keysr$.
+00000ff0: 0000 7233 0000 0072 3400 0000 da0a 3c64  ..r3...r4.....<d
+00001000: 6963 7463 6f6d 703e 8e00 0000 7314 0000  ictcomp>....s...
+00001010: 0006 0006 070a fa02 010a 0102 ff08 0204  ................
+00001020: fe02 ff06 ff7a 2d54 6162 756c 6172 4265  .....z-TabularBe
+00001030: 6e63 686d 6172 6b2e 5f5f 696e 6974 5f5f  nchmark.__init__
+00001040: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00001050: 6f6d 703e 4ea9 0172 1900 0000 290b 721c  omp>N..r....).r.
+00001060: 0000 0072 1900 0000 7224 0000 0072 2200  ...r....r$...r".
+00001070: 0000 da0d 6669 6465 6c69 7479 5f6e 616d  ....fidelity_nam
+00001080: 65da 0e66 6964 656c 6974 795f 7261 6e67  e..fidelity_rang
+00001090: 6572 1800 0000 721a 0000 0072 1b00 0000  er....r....r....
+000010a0: 7216 0000 0072 1700 0000 6301 0000 0000  r....r....c.....
+000010b0: 0000 0000 0000 0003 0000 0006 0000 0013  ................
+000010c0: 0000 0173 3c00 0000 6900 7c00 5d1a 5c02  ...s<...i.|.].\.
+000010d0: 7d01 7d02 7c01 7c02 6602 7c02 6a00 7214  }.}.|.|.f.|.j.r.
+000010e0: 7401 8800 7c01 1900 a002 a100 8301 6e07  t...|.........n.
+000010f0: 7401 8800 7c01 1900 a003 a100 8301 9302  t...|...........
+00001100: 7102 5300 7233 0000 0029 04da 086d 696e  q.S.r3...)...min
+00001110: 696d 697a 65da 0566 6c6f 6174 da03 6d69  imize..float..mi
+00001120: 6eda 036d 6178 2903 7230 0000 00da 016b  n..max).r0.....k
+00001130: da06 6d65 7472 6963 7232 0000 0072 3300  ..metricr2...r3.
+00001140: 0000 7234 0000 0072 4100 0000 b100 0000  ..r4...rA.......
+00001150: 730a 0000 0006 0006 0406 fd24 0106 fe63  s..........$...c
+00001160: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+00001170: 0600 0000 5300 0001 7320 0000 0069 007c  ....S...s ...i.|
+00001180: 005d 0c5c 025c 027d 017d 027d 037c 017c  .].\.\.}.}.}.|.|
+00001190: 02a0 007c 03a1 0193 0271 0253 0072 3300  ...|.....q.S.r3.
+000011a0: 0000 2901 da08 6173 5f76 616c 7565 2904  ..)...as_value).
+000011b0: 7230 0000 0072 4900 0000 724a 0000 00da  r0...rI...rJ....
+000011c0: 0176 7233 0000 0072 3300 0000 7234 0000  .vr3...r3...r4..
+000011d0: 0072 4100 0000 b700 0000 7306 0000 0006  .rA.......s.....
+000011e0: 0014 0106 ff7a 1273 656c 662e 7661 6c75  .....z.self.valu
+000011f0: 655f 6d65 7472 6963 3dfa 0820 6e6f 7420  e_metric=.. not 
+00001200: 696e 207a 1173 656c 662e 636f 7374 5f6d  in z.self.cost_m
+00001210: 6574 7269 633d 2922 da0b 7265 7365 745f  etric=)"..reset_
+00001220: 696e 6465 7872 2e00 0000 da0a 5661 6c75  indexr......Valu
+00001230: 6545 7272 6f72 da04 6c69 7374 da0b 6d65  eError..list..me
+00001240: 7472 6963 5f64 6566 73da 046b 6579 73da  tric_defs..keys.
+00001250: 0361 6c6c da05 6e61 6d65 73da 0672 656e  .all..names..ren
+00001260: 616d 65da 0973 6574 5f69 6e64 6578 da0a  ame..set_index..
+00001270: 736f 7274 5f69 6e64 6578 da05 696e 6465  sort_index..inde
+00001280: 78da 1067 6574 5f6c 6576 656c 5f76 616c  x..get_level_val
+00001290: 7565 73da 0c76 616c 7565 5f63 6f75 6e74  ues..value_count
+000012a0: 73da 0469 6c6f 63da 0673 6f72 7465 64da  s..iloc..sorted.
+000012b0: 0675 6e69 7175 65da 0767 726f 7570 6279  .unique..groupby
+000012c0: da03 6167 67da 0869 7465 7272 6f77 7372  ..agg..iterrowsr
+000012d0: 0b00 0000 721e 0000 00da 0763 6f6e 6669  ....r......confi
+000012e0: 6773 7220 0000 0072 2100 0000 7240 0000  gsr ...r!...r@..
+000012f0: 00da 0b72 6573 756c 745f 6b65 7973 da05  ...result_keys..
+00001300: 7375 7065 72da 085f 5f69 6e69 745f 5f72  super..__init__r
+00001310: 0f00 0000 da05 6974 656d 735a 0e74 6162  ......itemsZ.tab
+00001320: 6c65 5f6f 7074 696d 756d 7372 1600 0000  le_optimumsr....
+00001330: 7217 0000 0029 19da 0473 656c 6672 1c00  r....)...selfr..
+00001340: 0000 721e 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
+00001350: 0072 2200 0000 7224 0000 0072 1600 0000  .r"...r$...r....
+00001360: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00001370: 1a00 0000 721b 0000 0072 6200 0000 da0a  ....r....rb.....
+00001380: 696e 6465 785f 636f 6c73 5a0d 7265 6c65  index_colsZ.rele
+00001390: 7661 6e74 5f63 6f6c 735a 0f66 6964 656c  vant_colsZ.fidel
+000013a0: 6974 795f 7661 6c75 6573 5a0f 6669 6465  ity_valuesZ.fide
+000013b0: 6c69 7479 5f63 6f75 6e74 735a 0b73 6f72  lity_countsZ.sor
+000013c0: 7465 645f 6669 6473 da05 7374 6172 74da  ted_fids..start.
+000013d0: 0365 6e64 da04 7374 6570 5a08 6964 5f74  .end..stepZ.id_t
+000013e0: 6162 6c65 7261 0000 005a 0d5f 7261 775f  ablera...Z._raw_
+000013f0: 6f70 7469 6d75 6d73 a901 da09 5f5f 636c  optimums....__cl
+00001400: 6173 735f 5f29 0372 4000 0000 7224 0000  ass__).r@...r$..
+00001410: 0072 1e00 0000 7234 0000 0072 6400 0000  .r....r4...rd...
+00001420: 1f00 0000 7390 0000 0008 2a0a 0316 010a  ....s.....*.....
+00001430: 0216 010e 0216 0102 0110 0104 ff08 0416  ................
+00001440: 0116 0112 0302 010a 0104 ff10 0608 0302  ................
+00001450: 0302 0102 ff02 0202 fe02 0304 fd08 050e  ................
+00001460: 010c 0e08 0112 0114 010c 0208 0108 0110  ................
+00001470: 0112 070c 0106 0706 f908 0b0c 0106 0206  ................
+00001480: 0106 0106 010a 010a 0106 0202 0102 0102  ................
+00001490: 0102 0102 0108 0102 0102 0102 0102 0102  ................
+000014a0: 0106 f50a 0e0a 0406 fc06 0606 0108 ff0e  ................
+000014b0: 0418 010e 0218 0104 ff7a 1954 6162 756c  .........z.Tabul
+000014c0: 6172 4265 6e63 686d 6172 6b2e 5f5f 696e  arBenchmark.__in
+000014d0: 6974 5f5f 2903 da02 6174 7216 0000 0072  it__)...atr....r
+000014e0: 1700 0000 da06 636f 6e66 6967 fa22 4354  ......config."CT
+000014f0: 6162 756c 6172 207c 204d 6170 7069 6e67  abular | Mapping
+00001500: 5b73 7472 2c20 416e 795d 207c 2073 7472  [str, Any] | str
+00001510: 726d 0000 00fa 0846 207c 204e 6f6e 65da  rm.....F | None.
+00001520: 0672 6574 7572 6e72 1300 0000 6302 0000  .returnr....c...
+00001530: 0000 0000 0003 0000 0007 0000 0008 0000  ................
+00001540: 0003 0000 0173 cc00 0000 7c00 a000 7c01  .....s....|...|.
+00001550: a101 7d05 7c02 6401 7501 720b 7c02 6e02  ..}.|.d.u.r.|.n.
+00001560: 7c00 6a01 7d02 7c00 6a02 7c02 0400 0300  |.j.}.|.j.|.....
+00001570: 6b01 721b 7c00 6a01 6b01 731e 4a00 8201  k.r.|.j.k.s.J...
+00001580: 0100 4a00 8201 7c05 6a03 6402 6403 8d01  ..J...|.j.d.d...
+00001590: 8900 7c00 6a04 6401 7501 723e 6404 6405  ..|.j.d.u.r>d.d.
+000015a0: 8400 7c00 6a04 a005 a100 4400 8301 7d06  ..|.j.....D...}.
+000015b0: 8700 6601 6406 6405 8408 7c06 a005 a100  ..f.d.d...|.....
+000015c0: 4400 8301 8900 7c03 6401 7501 7244 7c03  D.....|.d.u.rD|.
+000015d0: 6e02 7c00 6a06 7d03 7c04 6401 7501 724d  n.|.j.}.|.d.u.rM
+000015e0: 7c04 6e02 7c00 6a07 7d04 7c00 6a08 6a09  |.n.|.j.}.|.j.j.
+000015f0: 7c01 7c02 7c00 6a0a 8800 7c02 6407 8d02  |.|.|.j...|.d...
+00001600: 740b 7c03 8301 740b 7c04 8301 7c00 6a0c  t.|...t.|...|.j.
+00001610: 6408 8d06 5300 2909 61f9 0400 0053 7562  d...S.).a....Sub
+00001620: 6d69 7420 6120 7175 6572 7920 616e 6420  mit a query and 
+00001630: 6765 7420 6120 7265 7375 6c74 2e0a 0a20  get a result... 
+00001640: 2020 2020 2020 2021 2121 2077 6172 6e69         !!! warni
+00001650: 6e67 2022 5061 7373 696e 6720 6120 7261  ng "Passing a ra
+00001660: 7720 636f 6e66 6967 220a 0a20 2020 2020  w config"..     
+00001670: 2020 2020 2020 2049 6620 6120 6d61 7070         If a mapp
+00001680: 696e 6720 6973 2070 6173 7365 6420 2861  ing is passed (a
+00001690: 6e64 202a 2a6e 6f74 2a2a 2061 205b 6043  nd **not** a [`C
+000016a0: 6f6e 6669 6760 5d5b 6d66 7062 656e 6368  onfig`][mfpbench
+000016b0: 2e43 6f6e 6669 675d 206f 626a 6563 7429  .Config] object)
+000016c0: 2c0a 2020 2020 2020 2020 2020 2020 7765  ,.            we
+000016d0: 2077 696c 6c20 6174 7465 6d70 7420 746f   will attempt to
+000016e0: 206c 6f6f 6b20 666f 7220 6069 6460 2069   look for `id` i
+000016f0: 6e20 7468 6520 6d61 7070 696e 672c 2074  n the mapping, t
+00001700: 6f20 6b6e 6f77 2077 6869 6368 2063 6f6e  o know which con
+00001710: 6669 6720 746f 0a20 2020 2020 2020 2020  fig to.         
+00001720: 2020 206c 6f6f 6b75 702e 0a0a 2020 2020     lookup...    
+00001730: 2020 2020 2020 2020 4966 2074 6869 7320          If this 
+00001740: 6661 696c 732c 2077 6520 7769 6c6c 2074  fails, we will t
+00001750: 7279 206d 6174 6368 2074 6865 2063 6f6e  ry match the con
+00001760: 6669 6720 746f 206f 6e65 206f 6620 7468  fig to one of th
+00001770: 6520 636f 6e66 6967 7320 696e 0a20 2020  e configs in.   
+00001780: 2020 2020 2020 2020 2074 6865 2062 656e           the ben
+00001790: 6368 6d61 726b 2e0a 0a20 2020 2020 2020  chmark...       
+000017a0: 2020 2020 2050 7265 6665 7220 746f 2070       Prefer to p
+000017b0: 6173 7320 7468 6520 5b60 436f 6e66 6967  ass the [`Config
+000017c0: 605d 5b6d 6670 6265 6e63 682e 436f 6e66  `][mfpbench.Conf
+000017d0: 6967 5d20 6f62 6a65 6374 2064 6972 6563  ig] object direc
+000017e0: 746c 7920 6966 2070 6f73 7369 626c 652e  tly if possible.
+000017f0: 0a0a 2020 2020 2020 2020 3f3f 3f20 6e6f  ..        ??? no
+00001800: 7465 2022 4f76 6572 7269 6465 220a 0a20  te "Override".. 
+00001810: 2020 2020 2020 2020 2020 2054 6869 7320             This 
+00001820: 6675 6e63 7469 6f6e 206f 7665 7272 6964  function overrid
+00001830: 6573 2074 6865 2064 6566 6175 6c74 0a20  es the default. 
+00001840: 2020 2020 2020 2020 2020 205b 6071 7565             [`que
+00001850: 7279 2829 605d 5b6d 6670 6265 6e63 682e  ry()`][mfpbench.
+00001860: 4265 6e63 686d 6172 6b2e 7175 6572 795d  Benchmark.query]
+00001870: 2074 6f20 616c 6c6f 7720 666f 7220 7468   to allow for th
+00001880: 6973 0a20 2020 2020 2020 2020 2020 2063  is.            c
+00001890: 6f6e 6669 6720 6d61 7463 6869 6e67 0a0a  onfig matching..
+000018a0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+000018b0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+000018c0: 3a20 5468 6520 7175 6572 7920 746f 2075  : The query to u
+000018d0: 7365 0a20 2020 2020 2020 2020 2020 2061  se.            a
+000018e0: 743a 2054 6865 2066 6964 656c 6974 7920  t: The fidelity 
+000018f0: 6174 2077 6869 6368 2074 6f20 7175 6572  at which to quer
+00001900: 792c 2064 6566 6175 6c74 7320 746f 204e  y, defaults to N
+00001910: 6f6e 6520 7768 6963 6820 6d65 616e 7320  one which means 
+00001920: 2a6d 6178 696d 756d 2a0a 2020 2020 2020  *maximum*.      
+00001930: 2020 2020 2020 7661 6c75 655f 6d65 7472        value_metr
+00001940: 6963 3a20 5468 6520 6d65 7472 6963 2074  ic: The metric t
+00001950: 6f20 7573 6520 666f 7220 7468 6973 2072  o use for this r
+00001960: 6573 756c 742e 2055 7365 730a 2020 2020  esult. Uses.    
+00001970: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00001980: 7661 6c75 6520 6d65 7472 6963 2070 6173  value metric pas
+00001990: 7365 6420 696e 2074 6f20 7468 6520 636f  sed in to the co
+000019a0: 6e73 7472 7563 746f 7220 6966 206e 6f74  nstructor if not
+000019b0: 2073 7065 6369 6669 6564 2c0a 2020 2020   specified,.    
+000019c0: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
+000019d0: 7277 6973 6520 7468 6520 6465 6661 756c  rwise the defaul
+000019e0: 7420 6d65 7472 6963 2066 726f 6d20 7468  t metric from th
+000019f0: 6520 5265 7375 6c74 2069 6620 4e6f 6e65  e Result if None
+00001a00: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00001a10: 7374 5f6d 6574 7269 633a 2054 6865 206d  st_metric: The m
+00001a20: 6574 7269 6320 746f 2075 7365 2066 6f72  etric to use for
+00001a30: 2074 6869 7320 7265 7375 6c74 2e20 5573   this result. Us
+00001a40: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00001a50: 2020 2074 6865 2063 6f73 7420 6d65 7472     the cost metr
+00001a60: 6963 2070 6173 7365 6420 696e 2074 6f20  ic passed in to 
+00001a70: 7468 6520 636f 6e73 7472 7563 746f 7220  the constructor 
+00001a80: 6966 206e 6f74 2073 7065 6369 6669 6564  if not specified
+00001a90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001aa0: 2020 6f74 6865 7277 6973 6520 7468 6520    otherwise the 
+00001ab0: 6465 6661 756c 7420 6d65 7472 6963 2066  default metric f
+00001ac0: 726f 6d20 7468 6520 5265 7375 6c74 2069  rom the Result i
+00001ad0: 6620 4e6f 6e65 2e0a 0a20 2020 2020 2020  f None...       
+00001ae0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00001af0: 2020 2020 2020 5468 6520 7265 7375 6c74        The result
+00001b00: 206f 6620 7468 6520 7175 6572 790a 2020   of the query.  
+00001b10: 2020 2020 2020 4e54 a901 da07 7769 7468        NT....with
+00001b20: 5f69 6463 0100 0000 0000 0000 0000 0000  _idc............
+00001b30: 0300 0000 0400 0000 5300 0001 f316 0000  ........S.......
+00001b40: 0069 007c 005d 075c 027d 017d 027c 027c  .i.|.].\.}.}.|.|
+00001b50: 0193 0271 0253 0072 3300 0000 7233 0000  ...q.S.r3...r3..
+00001b60: 00a9 0372 3000 0000 7249 0000 0072 4c00  ...r0...rI...rL.
+00001b70: 0000 7233 0000 0072 3300 0000 7234 0000  ..r3...r3...r4..
+00001b80: 0072 4100 0000 f000 0000 f302 0000 0016  .rA.............
+00001b90: 007a 2a54 6162 756c 6172 4265 6e63 686d  .z*TabularBenchm
+00001ba0: 6172 6b2e 7175 6572 792e 3c6c 6f63 616c  ark.query.<local
+00001bb0: 733e 2e3c 6469 6374 636f 6d70 3e63 0100  s>.<dictcomp>c..
+00001bc0: 0000 0000 0000 0000 0000 0300 0000 0700  ................
+00001bd0: 0000 1300 0001 f31e 0000 0069 007c 005d  ...........i.|.]
+00001be0: 0b5c 027d 017d 027c 0188 00a0 007c 027c  .\.}.}.|.....|.|
+00001bf0: 02a1 0293 0271 0253 0072 3300 0000 a901  .....q.S.r3.....
+00001c00: da03 6765 7472 7500 0000 a901 da19 5f54  ..getru......._T
+00001c10: 6162 756c 6172 4265 6e63 686d 6172 6b5f  abularBenchmark_
+00001c20: 5f63 6f6e 6669 6772 3300 0000 7234 0000  _configr3...r4..
+00001c30: 0072 4100 0000 f100 0000 f302 0000 001e  .rA.............
+00001c40: 00a9 0172 6d00 0000 a906 726e 0000 00da  ...rm.....rn....
+00001c50: 0866 6964 656c 6974 79da 0672 6573 756c  .fidelity..resul
+00001c60: 7472 1600 0000 7217 0000 00da 0772 656e  tr....r......ren
+00001c70: 616d 6573 290d da0c 5f66 696e 645f 636f  ames)..._find_co
+00001c80: 6e66 6967 7269 0000 0072 6800 0000 da07  nfigri...rh.....
+00001c90: 6173 5f64 6963 74da 0f5f 636f 6e66 6967  as_dict.._config
+00001ca0: 5f72 656e 616d 6573 7265 0000 0072 1600  _renamesre...r..
+00001cb0: 0000 7217 0000 0072 0f00 0000 723c 0000  ..r....r....r<..
+00001cc0: 00da 135f 6f62 6a65 6374 6976 655f 6675  ..._objective_fu
+00001cd0: 6e63 7469 6f6e 721d 0000 00da 0f5f 7265  nctionr......_re
+00001ce0: 7375 6c74 5f72 656e 616d 6573 2907 7266  sult_renames).rf
+00001cf0: 0000 0072 6e00 0000 726d 0000 0072 1600  ...rn...rm...r..
+00001d00: 0000 7217 0000 00da 075f 636f 6e66 6967  ..r......_config
+00001d10: da10 5f72 6576 6572 7365 5f72 656e 616d  .._reverse_renam
+00001d20: 6573 7233 0000 0072 7a00 0000 7234 0000  esr3...rz...r4..
+00001d30: 00da 0571 7565 7279 c100 0000 7322 0000  ...query....s"..
+00001d40: 000a 2812 0220 010c 020a 0114 0116 0112  ..(.. ..........
+00001d50: 0212 0106 0202 0102 010c 0106 0106 0104  ................
+00001d60: 0106 fa7a 1654 6162 756c 6172 4265 6e63  ...z.TabularBenc
+00001d70: 686d 6172 6b2e 7175 6572 7929 05da 0366  hmark.query)...f
+00001d80: 726d da02 746f 726a 0000 0072 1600 0000  rm..torj...r....
+00001d90: 7217 0000 0072 8a00 0000 728b 0000 0072  r....r....r....r
+00001da0: 6a00 0000 fa07 6c69 7374 5b52 5d63 0200  j.....list[R]c..
+00001db0: 0000 0000 0000 0500 0000 0900 0000 0700  ................
+00001dc0: 0000 0300 0001 73ca 0000 0088 03a0 0088  ......s.........
+00001dd0: 01a1 017d 077c 0364 0175 0172 0b7c 036e  ...}.|.d.u.r.|.n
+00001de0: 0288 036a 017d 037c 0264 0175 0172 147c  ...j.}.|.d.u.r.|
+00001df0: 026e 0288 036a 027d 027c 0464 0175 0172  .n...j.}.|.d.u.r
+00001e00: 1d7c 046e 0288 036a 037d 047c 076a 0464  .|.n...j.}.|.j.d
+00001e10: 0264 038d 0189 0088 036a 0564 0175 0172  .d.......j.d.u.r
+00001e20: 4064 0464 0584 0088 036a 05a0 06a1 0044  @d.d.....j.....D
+00001e30: 0083 017d 0887 0066 0164 0664 0584 087c  ...}...f.d.d...|
+00001e40: 08a0 06a1 0044 0083 0189 0088 0464 0175  .....D.......d.u
+00001e50: 0172 4688 046e 0288 036a 0789 0488 0264  .rF..n...j.....d
+00001e60: 0175 0172 4f88 026e 0288 036a 0889 0287  .u.rO..n...j....
+00001e70: 0187 0287 0387 0466 0464 0764 0884 0888  .......f.d.d....
+00001e80: 036a 0988 007c 027c 037c 0464 098d 0444  .j...|.|.|.d...D
+00001e90: 0083 0153 0029 0a61 6905 0000 5375 626d  ...S.).ai...Subm
+00001ea0: 6974 2061 2071 7565 7279 2061 6e64 2067  it a query and g
+00001eb0: 6574 2061 2072 6573 756c 742e 0a0a 2020  et a result...  
+00001ec0: 2020 2020 2020 2121 2120 7761 726e 696e        !!! warnin
+00001ed0: 6720 2250 6173 7369 6e67 2061 2072 6177  g "Passing a raw
+00001ee0: 2063 6f6e 6669 6722 0a0a 2020 2020 2020   config"..      
+00001ef0: 2020 2020 2020 4966 2061 206d 6170 7069        If a mappi
+00001f00: 6e67 2069 7320 7061 7373 6564 2028 616e  ng is passed (an
+00001f10: 6420 2a2a 6e6f 742a 2a20 6120 5b60 436f  d **not** a [`Co
+00001f20: 6e66 6967 605d 5b6d 6670 6265 6e63 682e  nfig`][mfpbench.
+00001f30: 436f 6e66 6967 5d20 6f62 6a65 6374 292c  Config] object),
+00001f40: 0a20 2020 2020 2020 2020 2020 2077 6520  .            we 
+00001f50: 7769 6c6c 2061 7474 656d 7074 2074 6f20  will attempt to 
+00001f60: 6c6f 6f6b 2066 6f72 2060 6964 6020 696e  look for `id` in
+00001f70: 2074 6865 206d 6170 7069 6e67 2c20 746f   the mapping, to
+00001f80: 206b 6e6f 7720 7768 6963 6820 636f 6e66   know which conf
+00001f90: 6967 2074 6f0a 2020 2020 2020 2020 2020  ig to.          
+00001fa0: 2020 6c6f 6f6b 7570 2e0a 0a20 2020 2020    lookup...     
+00001fb0: 2020 2020 2020 2049 6620 7468 6973 2066         If this f
+00001fc0: 6169 6c73 2c20 7765 2077 696c 6c20 7472  ails, we will tr
+00001fd0: 7920 6d61 7463 6820 7468 6520 636f 6e66  y match the conf
+00001fe0: 6967 2074 6f20 6f6e 6520 6f66 2074 6865  ig to one of the
+00001ff0: 2063 6f6e 6669 6773 2069 6e0a 2020 2020   configs in.    
+00002000: 2020 2020 2020 2020 7468 6520 6265 6e63          the benc
+00002010: 686d 6172 6b2e 0a0a 2020 2020 2020 2020  hmark...        
+00002020: 2020 2020 5072 6566 6572 2074 6f20 7061      Prefer to pa
+00002030: 7373 2074 6865 205b 6043 6f6e 6669 6760  ss the [`Config`
+00002040: 5d5b 6d66 7062 656e 6368 2e43 6f6e 6669  ][mfpbench.Confi
+00002050: 675d 206f 626a 6563 7420 6469 7265 6374  g] object direct
+00002060: 6c79 2069 6620 706f 7373 6962 6c65 2e0a  ly if possible..
+00002070: 0a20 2020 2020 2020 203f 3f3f 206e 6f74  .        ??? not
+00002080: 6520 224f 7665 7272 6964 6522 0a0a 2020  e "Override"..  
+00002090: 2020 2020 2020 2020 2020 5468 6973 2066            This f
+000020a0: 756e 6374 696f 6e20 6f76 6572 7269 6465  unction override
+000020b0: 7320 7468 6520 6465 6661 756c 740a 2020  s the default.  
+000020c0: 2020 2020 2020 2020 2020 5b60 7472 616a            [`traj
+000020d0: 6563 746f 7279 2829 605d 5b6d 6670 6265  ectory()`][mfpbe
+000020e0: 6e63 682e 4265 6e63 686d 6172 6b2e 7472  nch.Benchmark.tr
+000020f0: 616a 6563 746f 7279 5d20 746f 2061 6c6c  ajectory] to all
+00002100: 6f77 2066 6f72 2074 6869 730a 2020 2020  ow for this.    
+00002110: 2020 2020 2020 2020 636f 6e66 6967 206d          config m
+00002120: 6174 6368 696e 670a 0a20 2020 2020 2020  atching..       
+00002130: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00002140: 2020 2063 6f6e 6669 673a 2054 6865 2071     config: The q
+00002150: 7565 7279 2074 6f20 7573 650a 2020 2020  uery to use.    
+00002160: 2020 2020 2020 2020 6672 6d3a 2053 7461          frm: Sta
+00002170: 7274 206f 6620 7468 6520 6375 7276 652c  rt of the curve,
+00002180: 2073 686f 756c 6420 6465 6661 756c 7420   should default 
+00002190: 746f 2074 6865 2073 7461 7274 0a20 2020  to the start.   
+000021a0: 2020 2020 2020 2020 2074 6f3a 2045 6e64           to: End
+000021b0: 206f 6620 7468 6520 6375 7276 652c 2073   of the curve, s
+000021c0: 686f 756c 6420 6465 6661 756c 7420 746f  hould default to
+000021d0: 2074 6865 2074 6f74 616c 0a20 2020 2020   the total.     
+000021e0: 2020 2020 2020 2073 7465 703a 2053 7465         step: Ste
+000021f0: 7020 7369 7a65 2c20 6465 6661 756c 7473  p size, defaults
+00002200: 2074 6f20 6060 636c 732e 6465 6661 756c   to ``cls.defaul
+00002210: 745f 7374 6570 6060 0a20 2020 2020 2020  t_step``.       
+00002220: 2020 2020 2076 616c 7565 5f6d 6574 7269       value_metri
+00002230: 633a 2054 6865 206d 6574 7269 6320 746f  c: The metric to
+00002240: 2075 7365 2066 6f72 2074 6869 7320 7265   use for this re
+00002250: 7375 6c74 2e20 5573 6573 0a20 2020 2020  sult. Uses.     
+00002260: 2020 2020 2020 2020 2020 2074 6865 2076             the v
+00002270: 616c 7565 206d 6574 7269 6320 7061 7373  alue metric pass
+00002280: 6564 2069 6e20 746f 2074 6865 2063 6f6e  ed in to the con
+00002290: 7374 7275 6374 6f72 2069 6620 6e6f 7420  structor if not 
+000022a0: 7370 6563 6966 6965 642c 0a20 2020 2020  specified,.     
+000022b0: 2020 2020 2020 2020 2020 206f 7468 6572             other
+000022c0: 7769 7365 2074 6865 2064 6566 6175 6c74  wise the default
+000022d0: 206d 6574 7269 6320 6672 6f6d 2074 6865   metric from the
+000022e0: 2052 6573 756c 7420 6966 204e 6f6e 652e   Result if None.
+000022f0: 0a20 2020 2020 2020 2020 2020 2063 6f73  .            cos
+00002300: 745f 6d65 7472 6963 3a20 5468 6520 6d65  t_metric: The me
+00002310: 7472 6963 2074 6f20 7573 6520 666f 7220  tric to use for 
+00002320: 7468 6973 2072 6573 756c 742e 2055 7365  this result. Use
+00002330: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00002340: 2020 7468 6520 636f 7374 206d 6574 7269    the cost metri
+00002350: 6320 7061 7373 6564 2069 6e20 746f 2074  c passed in to t
+00002360: 6865 2063 6f6e 7374 7275 6374 6f72 2069  he constructor i
+00002370: 6620 6e6f 7420 7370 6563 6966 6965 642c  f not specified,
+00002380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002390: 206f 7468 6572 7769 7365 2074 6865 2064   otherwise the d
+000023a0: 6566 6175 6c74 206d 6574 7269 6320 6672  efault metric fr
+000023b0: 6f6d 2074 6865 2052 6573 756c 7420 6966  om the Result if
+000023c0: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
+000023d0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+000023e0: 2020 2020 2054 6865 2072 6573 756c 7420       The result 
+000023f0: 6f66 2074 6865 2071 7565 7279 0a20 2020  of the query.   
+00002400: 2020 2020 204e 5472 7200 0000 6301 0000       NTrr...c...
+00002410: 0000 0000 0000 0000 0003 0000 0004 0000  ................
+00002420: 0053 0000 0172 7400 0000 7233 0000 0072  .S...rt...r3...r
+00002430: 3300 0000 7275 0000 0072 3300 0000 7233  3...ru...r3...r3
+00002440: 0000 0072 3400 0000 7241 0000 0034 0100  ...r4...rA...4..
+00002450: 0072 7600 0000 7a2f 5461 6275 6c61 7242  .rv...z/TabularB
+00002460: 656e 6368 6d61 726b 2e74 7261 6a65 6374  enchmark.traject
+00002470: 6f72 792e 3c6c 6f63 616c 733e 2e3c 6469  ory.<locals>.<di
+00002480: 6374 636f 6d70 3e63 0100 0000 0000 0000  ctcomp>c........
+00002490: 0000 0000 0300 0000 0700 0000 1300 0001  ................
+000024a0: 7277 0000 0072 3300 0000 7278 0000 0072  rw...r3...rx...r
+000024b0: 7500 0000 727a 0000 0072 3300 0000 7234  u...rz...r3...r4
+000024c0: 0000 0072 4100 0000 3501 0000 727c 0000  ...rA...5...r|..
+000024d0: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+000024e0: 0000 0a00 0000 1300 0001 7332 0000 0067  ..........s2...g
+000024f0: 007c 005d 155c 027d 017d 0288 026a 006a  .|.].\.}.}...j.j
+00002500: 0188 007c 017c 0274 0288 0383 0174 0288  ...|.|.t.....t..
+00002510: 0183 0188 026a 0364 008d 0691 0271 0253  .....j.d.....q.S
+00002520: 0029 0172 7e00 0000 2904 720f 0000 0072  .).r~...).r....r
+00002530: 3c00 0000 721d 0000 0072 8600 0000 2903  <...r....r....).
+00002540: 7230 0000 0072 7f00 0000 7280 0000 0029  r0...r....r....)
+00002550: 0472 6e00 0000 7217 0000 0072 6600 0000  .rn...r....rf...
+00002560: 7216 0000 0072 3300 0000 7234 0000 00da  r....r3...r4....
+00002570: 0a3c 6c69 7374 636f 6d70 3e3a 0100 0073  .<listcomp>:...s
+00002580: 1600 0000 0600 0609 06f8 0201 0201 0201  ................
+00002590: 0601 0601 0401 04fa 06ff 7a2f 5461 6275  ..........z/Tabu
+000025a0: 6c61 7242 656e 6368 6d61 726b 2e74 7261  larBenchmark.tra
+000025b0: 6a65 6374 6f72 792e 3c6c 6f63 616c 733e  jectory.<locals>
+000025c0: 2e3c 6c69 7374 636f 6d70 3e29 0372 8a00  .<listcomp>).r..
+000025d0: 0000 728b 0000 0072 6a00 0000 290a 7282  ..r....rj...).r.
+000025e0: 0000 0072 6900 0000 7268 0000 0072 6a00  ...ri...rh...rj.
+000025f0: 0000 7283 0000 0072 8400 0000 7265 0000  ..r....r....re..
+00002600: 0072 1600 0000 7217 0000 00da 0b5f 7472  .r....r......_tr
+00002610: 616a 6563 746f 7279 2909 7266 0000 0072  ajectory).rf...r
+00002620: 6e00 0000 728a 0000 0072 8b00 0000 726a  n...r....r....rj
+00002630: 0000 0072 1600 0000 7217 0000 0072 8700  ...r....r....r..
+00002640: 0000 7288 0000 0072 3300 0000 2905 727b  ..r....r3...).r{
+00002650: 0000 0072 6e00 0000 7217 0000 0072 6600  ...rn...r....rf.
+00002660: 0000 7216 0000 0072 3400 0000 da0a 7472  ..r....r4.....tr
+00002670: 616a 6563 746f 7279 ff00 0000 7324 0000  ajectory....s$..
+00002680: 000a 2d12 0212 0112 010c 020a 0114 0116  ..-.............
+00002690: 0112 0212 0110 0204 0902 0102 0102 0102  ................
+000026a0: 0104 fc06 f77a 1b54 6162 756c 6172 4265  .....z.TabularBe
+000026b0: 6e63 686d 6172 6b2e 7472 616a 6563 746f  nchmark.trajecto
+000026c0: 7279 fa28 4354 6162 756c 6172 207c 204d  ry.(CTabular | M
+000026d0: 6170 7069 6e67 5b73 7472 2c20 416e 795d  apping[str, Any]
+000026e0: 207c 2073 7472 207c 2069 6e74 7211 0000   | str | intr...
+000026f0: 0063 0200 0000 0000 0000 0000 0000 0500  .c..............
+00002700: 0000 0600 0000 0300 0001 73e8 0000 0074  ..........s....t
+00002710: 0088 0074 0183 0272 0974 0288 0083 0189  ...t...r.t......
+00002720: 0074 0088 0074 0283 0272 137c 006a 0388  .t...t...r.|.j..
+00002730: 0019 0053 0074 0088 007c 006a 0483 0272  ...S.t...|.j...r
+00002740: 2f88 006a 057c 006a 0376 0172 2d74 0664  /..j.|.j.v.r-t.d
+00002750: 0188 006a 059b 0064 027c 006a 03a0 07a1  ...j...d.|.j....
+00002760: 009b 009d 0483 0182 0188 0053 0074 0088  ...........S.t..
+00002770: 0074 0883 0273 364a 0082 017c 006a 0988  .t...s6J...|.j..
+00002780: 0076 0072 4774 0288 007c 006a 0919 0083  .v.rGt...|.j....
+00002790: 017d 027c 006a 037c 0219 0053 0064 0388  .}.|.j.|...S.d..
+000027a0: 0076 0072 5488 0064 0319 007d 037c 006a  .v.rT..d...}.|.j
+000027b0: 037c 0319 0053 0074 0a7c 006a 03a0 0ba1  .|...S.t.|.j....
+000027c0: 0087 0066 0164 0464 0584 0864 0064 068d  ...f.d.d...d.d..
+000027d0: 037d 047c 0464 0075 0072 7274 0664 0788  .}.|.d.u.rrt.d..
+000027e0: 009b 0064 0874 0c88 0083 019b 009d 0483  ...d.t..........
+000027f0: 0182 017c 0453 0029 094e 7a07 436f 6e66  ...|.S.).Nz.Conf
+00002800: 6967 2072 4d00 0000 7237 0000 0063 0100  ig rM...r7...c..
+00002810: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00002820: 0000 1300 0001 7310 0000 007c 006a 0064  ......s....|.j.d
+00002830: 0164 028d 0188 006b 0253 0029 034e 4672  .d.....k.S.).NFr
+00002840: 7200 0000 2901 7283 0000 0029 01da 0163  r...).r....)...c
+00002850: a901 726e 0000 0072 3300 0000 7234 0000  ..rn...r3...r4..
+00002860: 00da 083c 6c61 6d62 6461 3e72 0100 0073  ...<lambda>r...s
+00002870: 0200 0000 1000 7a2f 5461 6275 6c61 7242  ......z/TabularB
+00002880: 656e 6368 6d61 726b 2e5f 6669 6e64 5f63  enchmark._find_c
+00002890: 6f6e 6669 672e 3c6c 6f63 616c 733e 2e3c  onfig.<locals>.<
+000028a0: 6c61 6d62 6461 3e29 02da 0470 7265 64da  lambda>)...pred.
+000028b0: 0764 6566 6175 6c74 7a1f 436f 756c 6420  .defaultz.Could 
+000028c0: 6e6f 7420 6669 6e64 2063 6f6e 6669 6720  not find config 
+000028d0: 6d61 7463 6869 6e67 207a 3d2e 2050 6c65  matching z=. Ple
+000028e0: 6173 6520 7061 7373 2074 6865 2060 436f  ase pass the `Co
+000028f0: 6e66 6967 6020 6f62 6a65 6374 206f 7220  nfig` object or 
+00002900: 7370 6563 6966 7920 7468 6520 6069 6460  specify the `id`
+00002910: 2069 6e20 7468 6520 290d da0a 6973 696e   in the )...isin
+00002920: 7374 616e 6365 da03 696e 7472 1d00 0000  stance..intr....
+00002930: 7261 0000 00da 0643 6f6e 6669 6772 3700  ra.....Configr7.
+00002940: 0000 724f 0000 0072 5200 0000 7207 0000  ..rO...rR...r...
+00002950: 0072 2000 0000 720c 0000 00da 0676 616c  .r ...r......val
+00002960: 7565 73da 0474 7970 6529 0572 6600 0000  ues..type).rf...
+00002970: 726e 0000 005a 0f5f 7265 616c 5f63 6f6e  rn...Z._real_con
+00002980: 6669 675f 6964 da03 5f69 64da 056d 6174  fig_id.._id..mat
+00002990: 6368 7233 0000 0072 9200 0000 7234 0000  chr3...r....r4..
+000029a0: 0072 8200 0000 4b01 0000 733a 0000 000a  .r....K...s:....
+000029b0: 0608 010a 030a 010c 030c 0102 0116 0104  ................
+000029c0: ff04 030e 030a 030e 010a 0108 0308 010a  ................
+000029d0: 0102 0508 010a 0102 0106 fd08 0502 0108  ................
+000029e0: 0106 0104 ff04 ff04 047a 1d54 6162 756c  .........z.Tabul
+000029f0: 6172 4265 6e63 686d 6172 6b2e 5f66 696e  arBenchmark._fin
+00002a00: 645f 636f 6e66 6967 fa11 4d61 7070 696e  d_config..Mappin
+00002a10: 675b 7374 722c 2041 6e79 5d72 1400 0000  g[str, Any]r....
+00002a20: fa13 4d61 7070 696e 675b 7374 722c 2066  ..Mapping[str, f
+00002a30: 6c6f 6174 5d63 0200 0000 0000 0000 0100  loat]c..........
+00002a40: 0000 0600 0000 0700 0000 4300 0001 7366  ..........C...sf
+00002a50: 0000 0074 007c 0183 017d 017c 01a0 0164  ...t.|...}.|...d
+00002a60: 01a1 017d 037c 006a 026a 037c 037c 0266  ...}.|.j.j.|.|.f
+00002a70: 0219 007d 047c 037c 045f 0474 007c 047c  ...}.|.|._.t.|.|
+00002a80: 006a 0519 0083 017d 057c 017c 056b 0372  .j.....}.|.|.k.r
+00002a90: 2c74 0664 027c 039b 0264 037c 019b 0264  ,t.d.|...d.|...d
+00002aa0: 047c 059b 029d 0683 0182 0174 007c 047c  .|.........t.|.|
+00002ab0: 006a 0719 0083 0153 0029 057a c253 7562  .j.....S.).z.Sub
+00002ac0: 6d69 7420 6120 7175 6572 7920 616e 6420  mit a query and 
+00002ad0: 6765 7420 6120 7265 7375 6c74 2e0a 0a20  get a result... 
+00002ae0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00002af0: 2020 2020 2020 2020 2063 6f6e 6669 673a           config:
+00002b00: 2054 6865 2071 7565 7279 2074 6f20 7573   The query to us
+00002b10: 650a 2020 2020 2020 2020 2020 2020 6174  e.            at
+00002b20: 3a20 5468 6520 6669 6465 6c69 7479 2061  : The fidelity a
+00002b30: 7420 7768 6963 6820 746f 2071 7565 7279  t which to query
+00002b40: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00002b50: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
+00002b60: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
+00002b70: 2071 7565 7279 0a20 2020 2020 2020 2072   query.        r
+00002b80: 3700 0000 fa42 436f 6e66 6967 2071 7565  7....BConfig que
+00002b90: 7269 6564 2077 6974 6820 6973 206e 6f74  ried with is not
+00002ba0: 2065 7175 616c 2074 6f20 7468 6520 6f6e   equal to the on
+00002bb0: 6520 696e 2074 6865 2074 6162 6c65 2077  e in the table w
+00002bc0: 6974 6820 5f69 643d fa19 2e0a 636f 6e66  ith _id=....conf
+00002bd0: 6967 2070 726f 7669 6465 6420 636f 6e66  ig provided conf
+00002be0: 6967 3d7a 190a 636f 6e66 6967 2069 6e20  ig=z..config in 
+00002bf0: 7461 626c 6520 5f63 6f6e 6669 673d 2908  table _config=).
+00002c00: da04 6469 6374 da03 706f 7072 1e00 0000  ..dict..popr....
+00002c10: da03 6c6f 6372 1c00 0000 7240 0000 0072  ..locr....r@...r
+00002c20: 4f00 0000 7262 0000 0029 0672 6600 0000  O...rb...).rf...
+00002c30: 726e 0000 0072 6d00 0000 729b 0000 0072  rn...rm...r....r
+00002c40: 3f00 0000 7287 0000 0072 3300 0000 7233  ?...r....r3...r3
+00002c50: 0000 0072 3400 0000 7285 0000 007c 0100  ...r4...r....|..
+00002c60: 0073 1c00 0000 0810 0a01 1001 0602 0e01  .s..............
+00002c70: 0801 0201 0801 0201 04ff 0202 04fe 04ff  ................
+00002c80: 0e06 7a24 5461 6275 6c61 7242 656e 6368  ..z$TabularBench
+00002c90: 6d61 726b 2e5f 6f62 6a65 6374 6976 655f  mark._objective_
+00002ca0: 6675 6e63 7469 6f6e fa27 4974 6572 6162  function.'Iterab
+00002cb0: 6c65 5b74 7570 6c65 5b46 2c20 4d61 7070  le[tuple[F, Mapp
+00002cc0: 696e 675b 7374 722c 2066 6c6f 6174 5d5d  ing[str, float]]
+00002cd0: 5d63 0200 0000 0000 0000 0300 0000 0800  ]c..............
+00002ce0: 0000 0700 0000 0300 0001 7378 0000 0074  ..........sx...t
+00002cf0: 007c 0183 017d 017c 01a0 0164 01a1 017d  .|...}.|...d...}
+00002d00: 0588 006a 026a 037c 057c 0266 027c 057c  ...j.j.|.|.f.|.|
+00002d10: 0366 027c 0485 0319 007d 0674 007c 066a  .f.|.....}.t.|.j
+00002d20: 0464 0219 0088 006a 0519 0083 017d 077c  .d.....j.....}.|
+00002d30: 017c 076b 0372 3174 0664 037c 059b 0264  .|.k.r1t.d.|...d
+00002d40: 047c 019b 0264 057c 079b 029d 0683 0182  .|...d.|........
+00002d50: 0187 0066 0164 0664 0784 087c 06a0 07a1  ...f.d.d...|....
+00002d60: 0044 0083 0153 0029 084e 7237 0000 0072  .D...S.).Nr7...r
+00002d70: 0100 0000 729f 0000 0072 a000 0000 7a1e  ....r....r....z.
+00002d80: 0a63 6f6e 6669 6720 696e 2074 6162 6c65  .config in table
+00002d90: 2066 6972 7374 5f63 6f6e 6669 673d 6301   first_config=c.
+00002da0: 0000 0000 0000 0000 0000 0004 0000 0006  ................
+00002db0: 0000 0013 0000 0173 2600 0000 6700 7c00  .......s&...g.|.
+00002dc0: 5d0f 5c02 5c02 7d01 7d02 7d03 7c02 7400  ].\.\.}.}.}.|.t.
+00002dd0: 7c03 8800 6a01 1900 8301 6602 9102 7102  |...j.....f...q.
+00002de0: 5300 7233 0000 0029 0272 a100 0000 7262  S.r3...).r....rb
+00002df0: 0000 0029 0472 3000 0000 da01 5f72 7f00  ...).r0....._r..
+00002e00: 0000 723f 0000 00a9 0172 6600 0000 7233  ..r?.....rf...r3
+00002e10: 0000 0072 3400 0000 728d 0000 00b0 0100  ...r4...r.......
+00002e20: 0073 0800 0000 0600 0a02 10ff 06ff 7a30  .s............z0
+00002e30: 5461 6275 6c61 7242 656e 6368 6d61 726b  TabularBenchmark
+00002e40: 2e5f 7472 616a 6563 746f 7279 2e3c 6c6f  ._trajectory.<lo
+00002e50: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00002e60: 2908 72a1 0000 0072 a200 0000 721e 0000  ).r....r....r...
+00002e70: 0072 a300 0000 725b 0000 0072 4000 0000  .r....r[...r@...
+00002e80: 724f 0000 0072 6000 0000 2908 7266 0000  rO...r`...).rf..
+00002e90: 0072 6e00 0000 728a 0000 0072 8b00 0000  .rn...r....r....
+00002ea0: 726a 0000 0072 9b00 0000 da04 726f 7773  rj...r......rows
+00002eb0: 5a0c 6669 7273 745f 636f 6e66 6967 7233  Z.first_configr3
+00002ec0: 0000 0072 a600 0000 7234 0000 0072 8e00  ...r....r4...r..
+00002ed0: 0000 9b01 0000 731e 0000 0008 090a 011a  ......s.........
+00002ee0: 0114 0108 0202 0108 0102 0104 ff02 0204  ................
+00002ef0: fe04 ff0a 0606 0206 fe7a 1c54 6162 756c  .........z.Tabul
+00002f00: 6172 4265 6e63 686d 6172 6b2e 5f74 7261  arBenchmark._tra
+00002f10: 6a65 6374 6f72 792e 7242 0000 00da 016e  jectory.rB.....n
+00002f20: da04 4e6f 6e65 fa22 696e 7420 7c20 6e70  ..None."int | np
+00002f30: 2e72 616e 646f 6d2e 5261 6e64 6f6d 5374  .random.RandomSt
+00002f40: 6174 6520 7c20 4e6f 6e65 6302 0000 0000  ate | Nonec.....
+00002f50: 0000 0001 0000 0003 0000 0001 0000 0043  ...............C
+00002f60: 0000 01f3 0400 0000 6400 5300 722c 0000  ........d.S.r,..
+00002f70: 0072 3300 0000 a903 7266 0000 0072 a800  .r3.....rf...r..
+00002f80: 0000 7219 0000 0072 3300 0000 7233 0000  ..r....r3...r3..
+00002f90: 0072 3400 0000 da06 7361 6d70 6c65 b601  .r4.....sample..
+00002fa0: 0000 f302 0000 0004 077a 1754 6162 756c  .........z.Tabul
+00002fb0: 6172 4265 6e63 686d 6172 6b2e 7361 6d70  arBenchmark.samp
+00002fc0: 6c65 7297 0000 00fa 0e6c 6973 745b 4354  ler......list[CT
+00002fd0: 6162 756c 6172 5d63 0200 0000 0000 0000  abular]c........
+00002fe0: 0100 0000 0300 0000 0100 0000 4300 0001  ............C...
+00002ff0: 72ab 0000 0072 2c00 0000 7233 0000 0072  r....r,...r3...r
+00003000: ac00 0000 7233 0000 0072 3300 0000 7234  ....r3...r3...r4
+00003010: 0000 0072 ad00 0000 c001 0000 72ae 0000  ...r........r...
+00003020: 00fa 1943 5461 6275 6c61 7220 7c20 6c69  ...CTabular | li
+00003030: 7374 5b43 5461 6275 6c61 725d 6302 0000  st[CTabular]c...
+00003040: 0000 0000 0001 0000 0009 0000 0006 0000  ................
+00003050: 0003 0000 0173 ac00 0000 7400 7c02 7401  .....s....t.|.t.
+00003060: 6a02 6a03 8302 720e 7c02 a004 6401 6402  j.j...r.|...d.d.
+00003070: a102 7d03 6e02 7c02 7d03 7401 6a02 6a05  ..}.n.|.}.t.j.j.
+00003080: 7c03 6403 8d01 7d04 7406 7c00 6a07 a008  |.d...}.t.|.j...
+00003090: a100 8301 8900 7409 8800 8301 7d05 7c01  ......t.....}.|.
+000030a0: 6404 7501 7228 7c01 6e01 6405 7d06 7c06  d.u.r(|.n.d.}.|.
+000030b0: 7c05 6b04 7239 740a 6406 7c06 9b00 6407  |.k.r9t.d.|...d.
+000030c0: 7c05 9b00 6408 9d05 8301 8201 7c04 6a0b  |...d.......|.j.
+000030d0: 7c05 7c06 6409 640a 8d03 7d07 7c01 6404  |.|.d.d...}.|.d.
+000030e0: 7500 724d 7c07 6401 1900 7d08 8800 7c08  u.rM|.d...}...|.
+000030f0: 1900 5300 8700 6601 640b 640c 8408 7c07  ..S...f.d.d...|.
+00003100: 4400 8301 5300 290d 619b 0100 0053 616d  D...S.).a....Sam
+00003110: 706c 6520 6120 7261 6e64 6f6d 2070 6f73  ple a random pos
+00003120: 7369 626c 6520 636f 6e66 6967 2e0a 0a20  sible config... 
+00003130: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00003140: 2020 2020 2020 2020 206e 3a20 486f 7720           n: How 
+00003150: 6d61 6e79 2073 616d 706c 6573 2074 6f20  many samples to 
+00003160: 7461 6b65 2c20 4e6f 6e65 206d 6561 6e73  take, None means
+00003170: 206a 7375 7420 6120 7369 6e67 6c65 206f   jsut a single o
+00003180: 6e65 2c20 6e6f 7420 696e 2061 206c 6973  ne, not in a lis
+00003190: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
+000031a0: 6564 3a20 5468 6520 7365 6564 2074 6f20  ed: The seed to 
+000031b0: 7573 6520 666f 7220 7468 6520 7361 6d70  use for the samp
+000031c0: 6c69 6e67 2e0a 0a20 2020 2020 2020 2020  ling...         
+000031d0: 2020 2020 2020 2021 2121 206e 6f74 6520         !!! note 
+000031e0: 2253 6565 6469 6e67 220a 0a20 2020 2020  "Seeding"..     
+000031f0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00003200: 6869 7320 6973 2064 6966 6665 7265 6e74  his is different
+00003210: 2074 6861 6e20 616e 7920 7365 6564 2070   than any seed p
+00003220: 6173 7365 6420 746f 2074 6865 2063 6f6e  assed to the con
+00003230: 7374 7275 6374 696f 6e0a 2020 2020 2020  struction.      
+00003240: 2020 2020 2020 2020 2020 2020 2020 6f66                of
+00003250: 2074 6865 2062 656e 6368 6d61 726b 2e0a   the benchmark..
+00003260: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00003270: 3a0a 2020 2020 2020 2020 2020 2020 4765  :.            Ge
+00003280: 7420 6261 636b 2061 2070 6f73 7369 626c  t back a possibl
+00003290: 6520 436f 6e66 6967 2074 6f20 7573 650a  e Config to use.
+000032a0: 2020 2020 2020 2020 7201 0000 0069 ffff          r....i..
+000032b0: ff7f 7242 0000 004e 7239 0000 007a 0d43  ..rB...Nr9...z.C
+000032c0: 616e 2774 2073 616d 706c 6520 7a0e 2063  an't sample z. c
+000032d0: 6f6e 6669 6773 2066 726f 6d20 7a08 2063  onfigs from z. c
+000032e0: 6f6e 6669 6773 4629 02da 0473 697a 65da  onfigsF)...size.
+000032f0: 0772 6570 6c61 6365 6301 0000 0000 0000  .replacec.......
+00003300: 0000 0000 0002 0000 0004 0000 0013 0000  ................
+00003310: 0173 1400 0000 6700 7c00 5d06 7d01 8800  .s....g.|.].}...
+00003320: 7c01 1900 9102 7102 5300 7233 0000 0072  |.....q.S.r3...r
+00003330: 3300 0000 2902 7230 0000 00da 0169 a901  3...).r0.....i..
+00003340: 5a0c 636f 6e66 6967 5f69 7465 6d73 7233  Z.config_itemsr3
+00003350: 0000 0072 3400 0000 728d 0000 00f4 0100  ...r4...r.......
+00003360: 0073 0200 0000 1400 7a2b 5461 6275 6c61  .s......z+Tabula
+00003370: 7242 656e 6368 6d61 726b 2e73 616d 706c  rBenchmark.sampl
+00003380: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
+00003390: 636f 6d70 3e29 0c72 9600 0000 da02 6e70  comp>).r......np
+000033a0: da06 7261 6e64 6f6d da0b 5261 6e64 6f6d  ..random..Random
+000033b0: 5374 6174 65da 0f72 616e 646f 6d5f 696e  State..random_in
+000033c0: 7465 6765 7273 da0b 6465 6661 756c 745f  tegers..default_
+000033d0: 726e 6772 5000 0000 7261 0000 0072 9900  rngrP...ra...r..
+000033e0: 0000 da03 6c65 6e72 4f00 0000 da06 6368  ....lenrO.....ch
+000033f0: 6f69 6365 2909 7266 0000 0072 a800 0000  oice).rf...r....
+00003400: 7219 0000 005a 055f 7365 6564 da03 726e  r....Z._seed..rn
+00003410: 675a 096e 5f63 6f6e 6669 6773 5a0d 7361  gZ.n_configsZ.sa
+00003420: 6d70 6c65 5f61 6d6f 756e 74da 0769 6e64  mple_amount..ind
+00003430: 6963 6573 da0b 6669 7273 745f 696e 6465  ices..first_inde
+00003440: 7872 3300 0000 72b4 0000 0072 3400 0000  xr3...r....r4...
+00003450: 72ad 0000 00c9 0100 0073 2000 0000 0e16  r........s .....
+00003460: 0e01 0402 0e02 0e02 0801 1001 0802 0201  ................
+00003470: 1001 04ff 1004 0801 0801 0801 1202 2918  ..............).
+00003480: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00003490: 1f00 0000 7220 0000 0072 1d00 0000 7221  ....r ...r....r!
+000034a0: 0000 0072 1d00 0000 7222 0000 0072 2300  ...r....r"...r#.
+000034b0: 0000 7224 0000 0072 2500 0000 7216 0000  ..r$...r%...r...
+000034c0: 0072 2600 0000 7217 0000 0072 2600 0000  .r&...r....r&...
+000034d0: 7218 0000 0072 2700 0000 7219 0000 0072  r....r'...r....r
+000034e0: 2800 0000 721a 0000 0072 2900 0000 721b  (...r....r)...r.
+000034f0: 0000 0072 2a00 0000 290a 726e 0000 0072  ...r*...).rn...r
+00003500: 6f00 0000 726d 0000 0072 7000 0000 7216  o...rm...rp...r.
+00003510: 0000 0072 2600 0000 7217 0000 0072 2600  ...r&...r....r&.
+00003520: 0000 7271 0000 0072 1300 0000 290e 726e  ..rq...r....).rn
+00003530: 0000 0072 6f00 0000 728a 0000 0072 7000  ...ro...r....rp.
+00003540: 0000 728b 0000 0072 7000 0000 726a 0000  ..r....rp...rj..
+00003550: 0072 7000 0000 7216 0000 0072 2600 0000  .rp...r....r&...
+00003560: 7217 0000 0072 2600 0000 7271 0000 0072  r....r&...rq...r
+00003570: 8c00 0000 2904 726e 0000 0072 9000 0000  ....).rn...r....
+00003580: 7271 0000 0072 1100 0000 2906 726e 0000  rq...r....).rn..
+00003590: 0072 9d00 0000 726d 0000 0072 1400 0000  .r....rm...r....
+000035a0: 7271 0000 0072 9e00 0000 290a 726e 0000  rq...r....).rn..
+000035b0: 0072 9d00 0000 728a 0000 0072 1400 0000  .r....r....r....
+000035c0: 728b 0000 0072 1400 0000 726a 0000 0072  r....r....rj...r
+000035d0: 1400 0000 7271 0000 0072 a400 0000 722c  ....rq...r....r,
+000035e0: 0000 0029 0672 a800 0000 72a9 0000 0072  ...).r....r....r
+000035f0: 1900 0000 72aa 0000 0072 7100 0000 7211  ....r....rq...r.
+00003600: 0000 0029 0672 a800 0000 7297 0000 0072  ...).r....r....r
+00003610: 1900 0000 72aa 0000 0072 7100 0000 72af  ....r....rq...r.
+00003620: 0000 0029 0672 a800 0000 7228 0000 0072  ...).r....r(...r
+00003630: 1900 0000 72aa 0000 0072 7100 0000 72b0  ....r....rq...r.
+00003640: 0000 0029 0dda 085f 5f6e 616d 655f 5fda  ...)...__name__.
+00003650: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00003660: 7561 6c6e 616d 655f 5f72 6400 0000 7289  ualname__rd...r.
+00003670: 0000 0072 0a00 0000 728f 0000 0072 8200  ...r....r....r..
+00003680: 0000 7285 0000 0072 8e00 0000 7209 0000  ..r....r....r...
+00003690: 0072 ad00 0000 da0d 5f5f 636c 6173 7363  .r......__classc
+000036a0: 656c 6c5f 5f72 3300 0000 7233 0000 0072  ell__r3...r3...r
+000036b0: 6b00 0000 7234 0000 0072 1500 0000 1e00  k...r4...r......
+000036c0: 0000 734c 0000 0008 0002 0a02 0102 0102  ..sL............
+000036d0: 0102 0102 0112 f200 7f02 2702 0102 010e  ..........'.....
+000036e0: fa02 3e02 0502 0102 0102 0102 0110 f80a  ..>.............
+000036f0: 4b02 310c 0102 1e0c 0102 1a02 0302 fe02  K.1.............
+00003700: 0410 fc02 0902 0510 fc02 0802 0302 fe02  ................
+00003710: 0418 fc72 1500 0000 da08 5f5f 6d61 696e  ...r......__main
+00003720: 5f5f da04 6461 7461 7a0f 6c63 6265 6e63  __..dataz.lcbenc
+00003730: 682d 7461 6275 6c61 727a 0d61 6475 6c74  h-tabularz.adult
+00003740: 2e70 6172 7175 6574 2902 da14 4c43 4265  .parquet)...LCBe
+00003750: 6e63 6854 6162 756c 6172 436f 6e66 6967  nchTabularConfig
+00003760: da14 4c43 4265 6e63 6854 6162 756c 6172  ..LCBenchTabular
+00003770: 5265 7375 6c74 5a03 746f 7972 3700 0000  ResultZ.toyr7...
+00003780: da05 6570 6f63 6829 0472 2000 0000 7221  ..epoch).r ...r!
+00003790: 0000 0072 2200 0000 7224 0000 0072 3900  ...r"...r$...r9.
+000037a0: 0000 7242 0000 0072 7d00 0000 e92a 0000  ..rB...r}....*..
+000037b0: 00e9 0a00 0000 2902 728a 0000 0072 8b00  ......).r....r..
+000037c0: 0000 293c da0a 5f5f 6675 7475 7265 5f5f  ..)<..__future__
+000037d0: 7202 0000 00da 0770 6174 686c 6962 7203  r......pathlibr.
+000037e0: 0000 00da 0674 7970 696e 6772 0400 0000  .....typingr....
+000037f0: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
+00003800: 0800 0000 7209 0000 00da 1174 7970 696e  ....r......typin
+00003810: 675f 6578 7465 6e73 696f 6e73 720a 0000  g_extensionsr...
+00003820: 00da 056e 756d 7079 72b5 0000 00da 0670  ...numpyr......p
+00003830: 616e 6461 73da 0270 64da 0b43 6f6e 6669  andas..pd..Confi
+00003840: 6753 7061 6365 720b 0000 00da 0e6d 6f72  gSpacer......mor
+00003850: 655f 6974 6572 746f 6f6c 7372 0c00 0000  e_itertoolsr....
+00003860: da12 6d66 7062 656e 6368 2e62 656e 6368  ..mfpbench.bench
+00003870: 6d61 726b 720d 0000 00da 0f6d 6670 6265  markr......mfpbe
+00003880: 6e63 682e 636f 6e66 6967 720e 0000 00da  nch.configr.....
+00003890: 0f6d 6670 6265 6e63 682e 7265 7375 6c74  .mfpbench.result
+000038a0: 720f 0000 00da 0f6d 6670 6265 6e63 682e  r......mfpbench.
+000038b0: 6d65 7472 6963 7210 0000 0072 1100 0000  metricr....r....
+000038c0: 7213 0000 0072 9700 0000 7246 0000 0072  r....r....rF...r
+000038d0: 1400 0000 7215 0000 0072 bf00 0000 da08  ....r....r......
+000038e0: 5f5f 6669 6c65 5f5f da06 7061 7265 6e74  __file__..parent
+000038f0: da04 4845 5245 da04 7061 7468 da0c 7265  ..HERE..path..re
+00003900: 6164 5f70 6172 7175 6574 721e 0000 00da  ad_parquetr.....
+00003910: 186d 6670 6265 6e63 682e 6c63 6265 6e63  .mfpbench.lcbenc
+00003920: 685f 7461 6275 6c61 7272 c500 0000 72c6  h_tabularr....r.
+00003930: 0000 00da 0962 656e 6368 6d61 726b 7261  .....benchmarkra
+00003940: 0000 005a 0b61 6c6c 5f63 6f6e 6669 6773  ...Z.all_configs
+00003950: 7250 0000 0072 5200 0000 5a0a 636f 6e66  rP...rR...Z.conf
+00003960: 6967 5f69 6473 7299 0000 0072 ad00 0000  ig_idsr....r....
+00003970: 726e 0000 0072 3700 0000 723e 0000 0072  rn...r7...r>...r
+00003980: 8900 0000 7280 0000 005a 0c61 7267 6d69  ....r....Z.argmi
+00003990: 6e5f 7363 6f72 6572 8f00 0000 7233 0000  n_scorer....r3..
+000039a0: 0072 3300 0000 7233 0000 0072 3400 0000  .r3...r3...r4...
+000039b0: da08 3c6d 6f64 756c 653e 0100 0000 7354  ..<module>....sT
+000039c0: 0000 000c 000c 0220 010c 0108 0208 010c  ....... ........
+000039d0: 010c 010c 020c 010c 0104 020c 010c 040c  ................
+000039e0: 030c 031a 0300 7f00 7f00 7f08 5c0a 0114  ............\...
+000039f0: 010a 0110 0102 0202 0102 0102 0102 0102  ................
+00003a00: 0102 0106 fa06 090c 010c 010c 0206 010e  ................
+00003a10: 020e 0114 0204 e7                        .......
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/benchmark.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/benchmark.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/config.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/config.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/download.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/download.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/download.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/download.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/get.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/get.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 6066 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 b217 0000  o........Coe....
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 b217 0000  o.......m.=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0010 0000 0040 0000 0173 9e01 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 6d01 5a01 0100 6400 6402  d.d.l.m.Z...d.d.
 00000040: 6c02 6d03 5a03 0100 6400 6403 6c04 6d05  l.m.Z...d.d.l.m.
 00000050: 5a05 6d06 5a06 0100 6400 6404 6c07 6d08  Z.m.Z...d.d.l.m.
 00000060: 5a08 0100 6400 6405 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
 00000070: 6400 6406 6c0b 6d0c 5a0c 6d0d 5a0d 6d0e  d.d.l.m.Z.m.Z.m.
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/metric.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/metric.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 5098 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 ea13 0000  o........Coe....
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 ea13 0000  o.......m.=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a06 4700 6404 6405 8400 6405 6507 8303  Z.G.d.d...d.e...
 00000060: 5a08 6503 6406 6407 8d01 4700 6408 6409  Z.e.d.d...G.d.d.
 00000070: 8400 6409 8302 8301 5a09 6403 5300 290a  ..d.....Z.d.S.).
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/priors.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/priors.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/priors.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/priors.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/result.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/result.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 3380 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 340d 0000  o........Coe4...
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 340d 0000  o.......m.=f4...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0173 ac00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/result.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/result.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/resultframe.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/resultframe.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/resultframe.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/resultframe.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/setup_benchmark.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/setup_benchmark.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 12570 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 1a31 0000  o........Coe.1..
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 1a31 0000  o.......m.=f.1..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 a601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6402 6c05 5a05 6400 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 5a06 6400 6402 6c07 5a07 6400 6402 6c08  Z.d.d.l.Z.d.d.l.
 00000070: 5a09 6400 6402 6c0a 5a0a 6400 6403 6c0b  Z.d.d.l.Z.d.d.l.
@@ -379,15 +379,15 @@
 000017a0: 6f61 6469 6e67 2066 726f 6d20 290e da05  oading from )...
 000017b0: 6d6b 6469 7272 5a00 0000 725b 0000 0072  mkdirrZ...r[...r
 000017c0: 2300 0000 724d 0000 0072 4e00 0000 724f  #...rM...rN...rO
 000017d0: 0000 0072 5000 0000 7251 0000 0072 5200  ...rP...rQ...rR.
 000017e0: 0000 7253 0000 00da 077a 6970 6669 6c65  ..rS.....zipfile
 000017f0: da07 5a69 7046 696c 6572 5500 0000 2908  ..ZipFilerU...).
 00001800: 7214 0000 0072 0f00 0000 5a0d 7375 7272  r....r....Z.surr
-00001810: 6f67 6174 655f 6469 72da 087a 6970 5f70  ogate_dir..zip_p
+00001810: 6f67 6174 655f 6469 725a 087a 6970 5f70  ogate_dirZ.zip_p
 00001820: 6174 6872 4c00 0000 7257 0000 0072 5800  athrL...rW...rX.
 00001830: 0000 da03 7a69 7072 1200 0000 7212 0000  ....zipr....r...
 00001840: 0072 1500 0000 725c 0000 009c 0000 0073  .r....r\.......s
 00001850: 2400 0000 0802 0e01 0801 1403 0e01 0802  $...............
 00001860: 1201 0201 04ff 0202 0e01 1cfd 0280 1c00  ................
 00001870: 0e05 0c01 1cff 1203 7a1e 5044 3153 6f75  ........z.PD1Sou
 00001880: 7263 652e 5f64 6f77 6e6c 6f61 645f 7375  rce._download_su
@@ -433,15 +433,15 @@
 00001b00: 7262 0000 0072 4a00 0000 724b 0000 007a  rb...rJ...rK...z
 00001b10: 0b44 6f77 6e6c 6f61 6465 6420 290e 724d  .Downloaded ).rM
 00001b20: 0000 0072 4e00 0000 724f 0000 0072 5000  ...rN...rO...rP.
 00001b30: 0000 7223 0000 0072 4c00 0000 7251 0000  ..r#...rL...rQ..
 00001b40: 0072 5200 0000 7253 0000 0072 6400 0000  .rR...rS...rd...
 00001b50: 7265 0000 0072 5500 0000 720e 0000 00da  re...rU...r.....
 00001b60: 085f 7072 6f63 6573 7329 0772 1400 0000  ._process).r....
-00001b70: 720f 0000 00da 077a 6970 7061 7468 5a08  r......zippathZ.
+00001b70: 720f 0000 005a 077a 6970 7061 7468 5a08  r....Z.zippathZ.
 00001b80: 5f75 726c 6f70 656e 7257 0000 0072 5800  _urlopenrW...rX.
 00001b90: 0000 5a07 7a69 705f 7265 6672 1200 0000  ..Z.zip_refr....
 00001ba0: 7212 0000 0072 1500 0000 7216 0000 00b7  r....r....r.....
 00001bb0: 0000 0073 1c00 0000 0803 0801 0801 1001  ...s............
 00001bc0: 1801 0e01 1cff 0280 1c00 0e03 0c01 1cff  ................
 00001bd0: 1003 0e01 7a1d 4c43 4265 6e63 6854 6162  ....z.LCBenchTab
 00001be0: 756c 6172 536f 7572 6365 2e64 6f77 6e6c  ularSource.downl
@@ -480,87 +480,87 @@
 00001df0: 7a1b 5472 6169 6e2f 7661 6c5f 6261 6c61  z.Train/val_bala
 00001e00: 6e63 6564 5f61 6363 7572 6163 797a 1854  nced_accuracyz.T
 00001e10: 7261 696e 2f74 6573 745f 6372 6f73 735f  rain/test_cross_
 00001e20: 656e 7472 6f70 797a 1c54 7261 696e 2f74  entropyz.Train/t
 00001e30: 6573 745f 6261 6c61 6e63 6564 5f61 6363  est_balanced_acc
 00001e40: 7572 6163 797a 1154 7261 696e 2f74 6573  uracyz.Train/tes
 00001e50: 745f 7265 7375 6c74 da04 7469 6d65 da05  t_result..time..
-00001e60: 6570 6f63 6829 0972 6d00 0000 726e 0000  epoch).rm...rn..
+00001e60: 6570 6f63 6829 0972 6b00 0000 726c 0000  epoch).rk...rl..
 00001e70: 00da 046c 6f73 735a 0c76 616c 5f61 6363  ...lossZ.val_acc
 00001e80: 7572 6163 795a 1176 616c 5f63 726f 7373  uracyZ.val_cross
 00001e90: 5f65 6e74 726f 7079 5a15 7661 6c5f 6261  _entropyZ.val_ba
 00001ea0: 6c61 6e63 6564 5f61 6363 7572 6163 795a  lanced_accuracyZ
 00001eb0: 0d74 6573 745f 6163 6375 7261 6379 5a12  .test_accuracyZ.
 00001ec0: 7465 7374 5f63 726f 7373 5f65 6e74 726f  test_cross_entro
 00001ed0: 7079 5a16 7465 7374 5f62 616c 616e 6365  pyZ.test_balance
 00001ee0: 645f 6163 6375 7261 6379 da02 6964 5429  d_accuracy..idT)
 00001ef0: 015a 0c69 676e 6f72 655f 696e 6465 787a  .Z.ignore_indexz
 00001f00: 082e 7061 7271 7565 747a 0a50 726f 6365  ..parquetz.Proce
 00001f10: 7373 6564 207a 0420 746f 2072 1200 0000  ssed z. to r....
 00001f20: 2911 7223 0000 0072 0e00 0000 7251 0000  ).r#...r....rQ..
 00001f30: 00da 046a 736f 6eda 046c 6f61 64da 0569  ...json..load..i
 00001f40: 7465 6d73 da06 6c6f 6767 6572 da04 696e  tems..logger..in
-00001f50: 666f da02 7064 da09 4461 7461 4672 616d  fo..pd..DataFram
+00001f50: 666f da02 7064 5a09 4461 7461 4672 616d  fo..pdZ.DataFram
 00001f60: 655a 0661 7373 6967 6eda 0661 7070 656e  eZ.assign..appen
 00001f70: 64da 0663 6f6e 6361 745a 0e63 6f6e 7665  d..concatZ.conve
 00001f80: 7274 5f64 7479 7065 735a 0973 6574 5f69  rt_dtypesZ.set_i
 00001f90: 6e64 6578 5a0a 736f 7274 5f69 6e64 6578  ndexZ.sort_index
 00001fa0: 5a0a 746f 5f70 6172 7175 6574 2918 7214  Z.to_parquet).r.
 00001fb0: 0000 0072 0f00 0000 da08 6669 6c65 7061  ...r......filepa
 00001fc0: 7468 7258 0000 005a 0861 6c6c 5f64 6174  thrX...Z.all_dat
 00001fd0: 615a 0c64 6174 6173 6574 5f6e 616d 6572  aZ.dataset_namer
 00001fe0: 0a00 0000 5a19 636f 6e66 6967 5f66 7261  ....Z.config_fra
 00001ff0: 6d65 735f 666f 725f 6461 7461 7365 74da  mes_for_dataset.
 00002000: 0963 6f6e 6669 675f 6964 5a0b 636f 6e66  .config_idZ.conf
-00002010: 6967 5f64 6174 6172 6b00 0000 5a08 6c6f  ig_datark...Z.lo
-00002020: 675f 6461 7461 726f 0000 005a 0676 616c  g_dataro...Z.val
+00002010: 6967 5f64 6174 6172 6900 0000 5a08 6c6f  ig_datari...Z.lo
+00002020: 675f 6461 7461 726d 0000 005a 0676 616c  g_datarm...Z.val
 00002030: 5f63 655a 0776 616c 5f61 6363 5a0b 7661  _ceZ.val_accZ.va
 00002040: 6c5f 6261 6c5f 6163 635a 0774 6573 745f  l_bal_accZ.test_
 00002050: 6365 5a0c 7465 7374 5f62 616c 5f61 6363  ceZ.test_bal_acc
-00002060: da08 7465 7374 5f61 6363 726d 0000 0072  ..test_accrm...r
-00002070: 6e00 0000 da02 6466 5a0e 6466 5f66 6f72  n.....dfZ.df_for
+00002060: da08 7465 7374 5f61 6363 726b 0000 0072  ..test_accrk...r
+00002070: 6c00 0000 da02 6466 5a0e 6466 5f66 6f72  l.....dfZ.df_for
 00002080: 5f64 6174 6173 6574 5a0a 7461 626c 655f  _datasetZ.table_
 00002090: 7061 7468 7212 0000 0072 1200 0000 7215  pathr....r....r.
-000020a0: 0000 0072 6900 0000 c700 0000 7356 0000  ...ri.......sV..
+000020a0: 0000 0072 6800 0000 c700 0000 7356 0000  ...rh.......sV..
 000020b0: 0008 0212 010c 010c 011c ff10 0310 0104  ................
 000020c0: 0110 0108 0108 0208 0108 0108 0108 0108  ................
 000020d0: 0208 0108 0408 0208 0104 0202 0202 0102  ................
 000020e0: 0102 0102 0102 0102 0102 0102 0104 f704  ................
 000020f0: ff18 0f0c 020c 0504 010a 0104 0102 fc0e  ................
 00002100: 060a 0118 0104 cd7a 1d4c 4342 656e 6368  .......z.LCBench
 00002110: 5461 6275 6c61 7253 6f75 7263 652e 5f70  TabularSource._p
 00002120: 726f 6365 7373 4e72 3d00 0000 290a 723e  rocessNr=...).r>
 00002130: 0000 0072 3f00 0000 7240 0000 0072 4c00  ...r?...r@...rL.
 00002140: 0000 7241 0000 0072 0e00 0000 7208 0000  ..rA...r....r...
-00002150: 0072 4200 0000 7216 0000 0072 6900 0000  .rB...r....ri...
+00002150: 0072 4200 0000 7216 0000 0072 6800 0000  .rB...r....rh...
 00002160: 7212 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00002170: 1500 0000 7268 0000 00b2 0000 0073 1000  ....rh.......s..
+00002170: 1500 0000 7267 0000 00b2 0000 0073 1000  ....rg.......s..
 00002180: 0000 0a00 0c02 0401 0202 0201 0e01 020e  ................
-00002190: 1001 7268 0000 0072 3a00 0000 721e 0000  ..rh...r:...r...
+00002190: 1001 7267 0000 0072 3a00 0000 721e 0000  ..rg...r:...r...
 000021a0: 00da 0764 6174 6164 6972 fa0b 5061 7468  ...datadir..Path
 000021b0: 207c 204e 6f6e 6572 1000 0000 da04 626f   | Noner......bo
 000021c0: 6f6c 6302 0000 0000 0000 0000 0000 0004  olc.............
 000021d0: 0000 0004 0000 0043 0000 0173 3e00 0000  .......C...s>...
 000021e0: 7c01 6401 7501 7206 7c01 6e01 7400 7d01  |.d.u.r.|.n.t.}.
 000021f0: 7401 a002 7c00 a101 7d02 7c01 7c02 6a03  t...|...}.|.|.j.
 00002200: 1b00 7d03 7c03 a004 a100 6f1e 7405 7406  ..}.|.....o.t.t.
 00002210: 7c03 a007 a100 6402 8302 8301 5300 2903  |.....d.....S.).
 00002220: 7a35 4368 6563 6b20 7768 6574 6865 7220  z5Check whether 
 00002230: 7468 6520 6461 7461 2069 7320 646f 776e  the data is down
 00002240: 6c6f 6164 6564 2066 6f72 2073 6f6d 6520  loaded for some 
 00002250: 736f 7572 6365 2e4e 4629 0872 1800 0000  source.NF).r....
 00002260: 720d 0000 0072 3a00 0000 720e 0000 0072  r....r:...r....r
-00002270: 4d00 0000 7280 0000 00da 046e 6578 74da  M...r......next.
+00002270: 4d00 0000 727d 0000 00da 046e 6578 74da  M...r}.....next.
 00002280: 0769 7465 7264 6972 2904 723a 0000 0072  .iterdir).r:...r
-00002290: 7e00 0000 da07 5f73 6f75 7263 65da 0b73  ~....._source..s
+00002290: 7b00 0000 da07 5f73 6f75 7263 65da 0b73  {....._source..s
 000022a0: 6f75 7263 655f 7061 7468 7212 0000 0072  ource_pathr....r
 000022b0: 1200 0000 7215 0000 00da 0f64 6f77 6e6c  ....r......downl
 000022c0: 6f61 645f 7374 6174 7573 0401 0000 730c  oad_status....s.
 000022d0: 0000 0010 020a 010a 010a 010c 0104 ff72  ...............r
-000022e0: 8500 0000 723c 0000 00fa 106c 6973 745b  ....r<.....list[
+000022e0: 8200 0000 723c 0000 00fa 106c 6973 745b  ....r<.....list[
 000022f0: 7374 725d 207c 204e 6f6e 6572 1100 0000  str] | Noner....
 00002300: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
 00002310: 0006 0000 0043 0000 0173 a600 0000 7c01  .....C...s....|.
 00002320: 6401 7501 7206 7c01 6e01 7400 7d01 6402  d.u.r.|.n.t.}.d.
 00002330: 7c01 a001 a100 9b00 9d02 7d02 7402 7c02  |.........}.t.|.
 00002340: 8301 0100 7402 6403 7403 7c02 8301 1400  ....t.d.t.|.....
 00002350: 8301 0100 7c00 6401 7501 7223 6404 7c00  ....|.d.u.r#d.|.
@@ -585,28 +585,28 @@
 00002480: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
 00002490: 0003 0000 0053 0000 0172 3000 0000 7212  .....S...r0...r.
 000024a0: 0000 0072 2b00 0000 a902 7231 0000 0072  ...r+.....r1...r
 000024b0: 3a00 0000 7212 0000 0072 1200 0000 7215  :...r....r....r.
 000024c0: 0000 0072 3300 0000 1e01 0000 7234 0000  ...r3.......r4..
 000024d0: 007a 2970 7269 6e74 5f64 6f77 6e6c 6f61  .z)print_downloa
 000024e0: 645f 7374 6174 7573 2e3c 6c6f 6361 6c73  d_status.<locals
-000024f0: 3e2e 3c6c 6973 7463 6f6d 703e 2901 727e  >.<listcomp>).r~
+000024f0: 3e2e 3c6c 6973 7463 6f6d 703e 2901 727b  >.<listcomp>).r{
 00002500: 0000 0075 0600 0000 5be2 9c93 5d20 7a04  ...u....[...] z.
 00002510: 5b78 5d20 7a04 203c 3230 7a29 2070 7974  [x] z. <20z) pyt
 00002520: 686f 6e20 2d6d 206d 6670 6265 6e63 6820  hon -m mfpbench 
 00002530: 646f 776e 6c6f 6164 202d 2d62 656e 6368  download --bench
 00002540: 6d61 726b 2029 0772 1800 0000 721f 0000  mark ).r....r...
 00002550: 0072 2300 0000 da03 6c65 6e72 0d00 0000  .r#.....lenr....
-00002560: 723c 0000 0072 8500 0000 2905 723c 0000  r<...r....).r<..
-00002570: 0072 7e00 0000 da01 7372 3900 0000 720e  .r~.....sr9...r.
+00002560: 723c 0000 0072 8200 0000 2905 723c 0000  r<...r....).r<..
+00002570: 0072 7b00 0000 da01 7372 3900 0000 720e  .r{.....sr9...r.
 00002580: 0000 0072 1200 0000 7212 0000 0072 1500  ...r....r....r..
 00002590: 0000 da15 7072 696e 745f 646f 776e 6c6f  ....print_downlo
 000025a0: 6164 5f73 7461 7475 730e 0100 0073 1800  ad_status....s..
 000025b0: 0000 100a 0e01 0801 1001 1802 1401 0402  ................
-000025c0: 0802 0c01 1001 1802 04fc 728c 0000 00da  ..........r.....
+000025c0: 0802 0c01 1001 1802 04fc 7289 0000 00da  ..........r.....
 000025d0: 0a62 656e 6368 6d61 726b 73fa 096c 6973  .benchmarks..lis
 000025e0: 745b 7374 725d 6301 0000 0000 0000 0000  t[str]c.........
 000025f0: 0000 000b 0000 0009 0000 0003 0000 0173  ...............s
 00002600: 3601 0000 7400 a001 a100 7d01 8800 6401  6...t.....}...d.
 00002610: 7501 7215 6402 8800 7601 7215 8700 6601  u.r.d...v.r...f.
 00002620: 6403 6404 8408 7c01 4400 8301 7d01 7c01  d.d...|.D...}.|.
 00002630: 4400 5d81 7d02 7402 6405 7403 7c02 6a04  D.].}.t.d.t.|.j.
@@ -629,47 +629,47 @@
 00002740: 696e 7420 7468 6520 7374 6174 7573 206f  int the status o
 00002750: 6620 7468 6520 6461 7461 2e0a 0a20 2020  f the data...   
 00002760: 2041 7267 733a 0a20 2020 2020 2020 2062   Args:.        b
 00002770: 656e 6368 6d61 726b 733a 2054 6865 2062  enchmarks: The b
 00002780: 656e 6368 6d61 726b 7320 746f 2063 6865  enchmarks to che
 00002790: 636b 2074 6865 2073 7461 7475 7320 6f66  ck the status of
 000027a0: 2e20 604e 6f6e 6560 2066 6f72 2061 6c6c  . `None` for all
-000027b0: 2e0a 2020 2020 4e72 8800 0000 6301 0000  ..    Nr....c...
+000027b0: 2e0a 2020 2020 4e72 8500 0000 6301 0000  ..    Nr....c...
 000027c0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
 000027d0: 0013 0000 0173 1a00 0000 6700 7c00 5d09  .....s....g.|.].
 000027e0: 7d01 7c01 6a00 8800 7600 7202 7c01 9102  }.|.j...v.r.|...
-000027f0: 7102 5300 7212 0000 0072 2b00 0000 7289  q.S.r....r+...r.
-00002800: 0000 00a9 0172 8d00 0000 7212 0000 0072  .....r....r....r
+000027f0: 7102 5300 7212 0000 0072 2b00 0000 7286  q.S.r....r+...r.
+00002800: 0000 00a9 0172 8a00 0000 7212 0000 0072  .....r....r....r
 00002810: 1500 0000 7233 0000 0031 0100 0073 0200  ....r3...1...s..
 00002820: 0000 1a00 7a26 7072 696e 745f 7265 7175  ....z&print_requ
 00002830: 6972 656d 656e 7473 2e3c 6c6f 6361 6c73  irements.<locals
 00002840: 3e2e 3c6c 6973 7463 6f6d 703e da01 3d7a  >.<listcomp>..=z
 00002850: 0670 6174 683a 207a 0563 6d64 3a20 7a06  .path: z.cmd: z.
-00002860: 6578 6563 3a20 7287 0000 007a 0a4e 6f74  exec: r....z.Not
+00002860: 6578 6563 3a20 7284 0000 007a 0a4e 6f74  exec: r....z.Not
 00002870: 2066 6f75 6e64 217a 0223 2072 4b00 0000   found!z.# rK...
 00002880: 290d 720d 0000 0072 3c00 0000 7223 0000  ).r....r<...r#..
-00002890: 0072 8a00 0000 720e 0000 0072 1c00 0000  .r....r....r....
+00002890: 0072 8700 0000 720e 0000 0072 1c00 0000  .r....r....r....
 000028a0: 7220 0000 00da 0373 7973 da0a 6578 6563  r .....sys..exec
 000028b0: 7574 6162 6c65 da03 6d61 7872 4d00 0000  utable..maxrM...
-000028c0: 7251 0000 00da 0472 6561 6429 0b72 8d00  rQ.....read).r..
+000028c0: 7251 0000 00da 0472 6561 6429 0b72 8a00  rQ.....read).r..
 000028d0: 0000 723c 0000 0072 3a00 0000 720f 0000  ..r<...r:...r...
 000028e0: 005a 0770 6174 6873 7472 7226 0000 005a  .Z.pathstrr&...Z
 000028f0: 0663 6d64 7374 725a 0865 7865 6370 6174  .cmdstrZ.execpat
 00002900: 685a 0765 7865 6373 7472 da01 6e72 5800  hZ.execstr..nrX.
-00002910: 0000 7212 0000 0072 8f00 0000 7215 0000  ..r....r....r...
+00002910: 0000 7212 0000 0072 8c00 0000 7215 0000  ..r....r....r...
 00002920: 00da 1270 7269 6e74 5f72 6571 7569 7265  ...print_require
 00002930: 6d65 6e74 7329 0100 0073 3400 0000 0806  ments)...s4.....
 00002940: 1001 1201 0802 1201 0c01 1201 0802 0a01  ................
 00002950: 0a01 0a01 0601 0a01 1801 0802 0801 0801  ................
 00002960: 0c01 0801 0a01 0e02 0c01 0e01 1cff 0802  ................
-00002970: 04e9 7296 0000 0046 2904 727e 0000 0072  ..r....F).r~...r
+00002970: 04e9 7293 0000 0046 2904 727b 0000 0072  ..r....F).r{...r
 00002980: 1600 0000 7227 0000 00da 0566 6f72 6365  ....r'.....force
 00002990: da09 6265 6e63 686d 6172 6b72 1600 0000  ..benchmarkr....
 000029a0: 7227 0000 00fa 0a73 7472 207c 2062 6f6f  r'.....str | boo
-000029b0: 6c72 9700 0000 6301 0000 0000 0000 0004  lr....c.........
+000029b0: 6c72 9400 0000 6301 0000 0000 0000 0004  lr....c.........
 000029c0: 0000 0008 0000 0004 0000 0043 0000 0173  ...........C...s
 000029d0: 0201 0000 7c01 6401 7501 7206 7c01 6e01  ....|.d.u.r.|.n.
 000029e0: 7400 7d01 7401 a002 7c00 a101 7d05 7c01  t.}.t...|...}.|.
 000029f0: 7c05 6a03 1b00 7d06 7c02 7255 7c06 a004  |.j...}.|.rU|...
 00002a00: a100 7226 7c04 7226 7405 6402 7c06 9b00  ..r&|.r&t.d.|...
 00002a10: 9d02 8301 0100 7406 a007 7c06 a101 0100  ......t...|.....
 00002a20: 7c06 a004 a100 7233 7408 7c06 a009 a100  |.....r3t.|.....
@@ -719,57 +719,57 @@
 00002ce0: 6d65 7468 696e 6720 6174 2046 7a1f 436f  mething at Fz.Co
 00002cf0: 756c 6420 6e6f 7420 6669 6e64 2072 6571  uld not find req
 00002d00: 7569 7265 6d65 6e74 7320 6174 207a 1b49  uirements at z.I
 00002d10: 6e73 7461 6c6c 696e 6720 7265 7175 6972  nstalling requir
 00002d20: 656d 656e 7473 2061 7420 2910 7218 0000  ements at ).r...
 00002d30: 0072 0d00 0000 723a 0000 0072 0e00 0000  .r....r:...r....
 00002d40: 724d 0000 0072 2300 0000 7252 0000 00da  rM...r#...rR....
-00002d50: 0672 6d74 7265 6572 8100 0000 7282 0000  .rmtreer....r...
+00002d50: 0672 6d74 7265 6572 7e00 0000 727f 0000  .rmtreer~...r...
 00002d60: 0072 6300 0000 7216 0000 0072 1c00 0000  .rc...r....r....
 00002d70: 7206 0000 00da 1146 696c 654e 6f74 466f  r......FileNotFo
 00002d80: 756e 6445 7272 6f72 7227 0000 0029 0872  undErrorr'...).r
-00002d90: 9800 0000 727e 0000 0072 1600 0000 7227  ....r~...r....r'
-00002da0: 0000 0072 9700 0000 723a 0000 0072 8400  ...r....r:...r..
+00002d90: 9500 0000 727b 0000 0072 1600 0000 7227  ....r{...r....r'
+00002da0: 0000 0072 9400 0000 723a 0000 0072 8100  ...r....r:...r..
 00002db0: 0000 5a08 7265 715f 7061 7468 7212 0000  ..Z.req_pathr...
 00002dc0: 0072 1200 0000 7215 0000 00da 0573 6574  .r....r......set
 00002dd0: 7570 4d01 0000 732c 0000 0010 130a 020a  upM...s,........
 00002de0: 0104 020c 010e 010a 011a 020e 010e 010a  ................
 00002df0: 0110 010e 0208 0208 010a 0108 0208 010e  ................
-00002e00: 010e 020e 0104 f772 9c00 0000 da08 5f5f  .......r......__
+00002e00: 010e 020e 0104 f772 9900 0000 da08 5f5f  .......r......__
 00002e10: 6d61 696e 5f5f 7a14 6461 7461 2f6c 6362  main__z.data/lcb
 00002e20: 656e 6368 2d74 6162 756c 6172 722a 0000  ench-tabularr*..
-00002e30: 0029 0672 3a00 0000 721e 0000 0072 7e00  .).r:...r....r~.
-00002e40: 0000 727f 0000 0072 1000 0000 7280 0000  ..r....r....r...
-00002e50: 0029 024e 4e29 0672 3c00 0000 7286 0000  .).NN).r<...r...
-00002e60: 0072 7e00 0000 727f 0000 0072 1000 0000  .r~...r....r....
-00002e70: 7211 0000 0029 0472 8d00 0000 728e 0000  r....).r....r...
-00002e80: 0072 1000 0000 7211 0000 0029 0c72 9800  .r....r....).r..
-00002e90: 0000 721e 0000 0072 7e00 0000 727f 0000  ..r....r~...r...
-00002ea0: 0072 1600 0000 7280 0000 0072 2700 0000  .r....r....r'...
-00002eb0: 7299 0000 0072 9700 0000 7280 0000 0072  r....r....r....r
+00002e30: 0029 0672 3a00 0000 721e 0000 0072 7b00  .).r:...r....r{.
+00002e40: 0000 727c 0000 0072 1000 0000 727d 0000  ..r|...r....r}..
+00002e50: 0029 024e 4e29 0672 3c00 0000 7283 0000  .).NN).r<...r...
+00002e60: 0072 7b00 0000 727c 0000 0072 1000 0000  .r{...r|...r....
+00002e70: 7211 0000 0029 0472 8a00 0000 728b 0000  r....).r....r...
+00002e80: 0072 1000 0000 7211 0000 0029 0c72 9500  .r....r....).r..
+00002e90: 0000 721e 0000 0072 7b00 0000 727c 0000  ..r....r{...r|..
+00002ea0: 0072 1600 0000 727d 0000 0072 2700 0000  .r....r}...r'...
+00002eb0: 7296 0000 0072 9400 0000 727d 0000 0072  r....r....r}...r
 00002ec0: 1000 0000 7211 0000 0029 2dda 0a5f 5f66  ....r....)-..__f
-00002ed0: 7574 7572 655f 5f72 0200 0000 7271 0000  uture__r....rq..
+00002ed0: 7574 7572 655f 5f72 0200 0000 726f 0000  uture__r....ro..
 00002ee0: 00da 076c 6f67 6769 6e67 7252 0000 0072  ...loggingrR...r
-00002ef0: 2400 0000 7291 0000 0072 5400 0000 da0e  $...r....rT.....
+00002ef0: 2400 0000 728e 0000 0072 5400 0000 da0e  $...r....rT.....
 00002f00: 7572 6c6c 6962 2e72 6571 7565 7374 724e  urllib.requestrN
 00002f10: 0000 0072 6400 0000 da03 6162 6372 0300  ...rd.....abcr..
 00002f20: 0000 7204 0000 00da 0b64 6174 6163 6c61  ..r......datacla
 00002f30: 7373 6573 7205 0000 00da 0770 6174 686c  ssesr......pathl
 00002f40: 6962 7206 0000 00da 0674 7970 696e 6772  ibr......typingr
 00002f50: 0700 0000 da11 7479 7069 6e67 5f65 7874  ......typing_ext
-00002f60: 656e 7369 6f6e 7372 0800 0000 da06 7061  ensionsr......pa
-00002f70: 6e64 6173 7276 0000 005a 0e6d 6f72 655f  ndasrv...Z.more_
+00002f60: 656e 7369 6f6e 7372 0800 0000 5a06 7061  ensionsr....Z.pa
+00002f70: 6e64 6173 7274 0000 005a 0e6d 6f72 655f  ndasrt...Z.more_
 00002f80: 6974 6572 746f 6f6c 7372 0900 0000 da09  itertoolsr......
-00002f90: 6765 744c 6f67 6765 7272 3e00 0000 7274  getLoggerr>...rt
+00002f90: 6765 744c 6f67 6765 7272 3e00 0000 7272  getLoggerr>...rr
 00002fa0: 0000 0072 1800 0000 da08 5f5f 6669 6c65  ...r......__file
 00002fb0: 5f5f da06 7061 7265 6e74 721f 0000 00da  __..parentr.....
 00002fc0: 0448 4552 4572 1b00 0000 720d 0000 0072  .HEREr....r....r
-00002fd0: 4300 0000 7248 0000 0072 5900 0000 7268  C...rH...rY...rh
-00002fe0: 0000 0072 8500 0000 728c 0000 0072 9600  ...r....r....r..
-00002ff0: 0000 729c 0000 0072 6900 0000 7212 0000  ..r....ri...r...
+00002fd0: 4300 0000 7248 0000 0072 5900 0000 7267  C...rH...rY...rg
+00002fe0: 0000 0072 8200 0000 7289 0000 0072 9300  ...r....r....r..
+00002ff0: 0000 7299 0000 0072 6800 0000 7212 0000  ..r....rh...r...
 00003000: 0072 1200 0000 7212 0000 0072 1500 0000  .r....r....r....
 00003010: da08 3c6d 6f64 756c 653e 0100 0000 7356  ..<module>....sV
 00003020: 0000 000c 0008 0208 0108 0108 0108 0108  ................
 00003030: 0108 0108 0110 010c 010c 010c 010c 0108  ................
 00003040: 020c 010a 0208 020e 010a 0108 0312 0108  ................
 00003050: 4012 0108 0c12 0108 1512 0108 3212 010c  @...........2...
 00003060: 5102 0b02 010c fe0a 1b02 2702 0102 0102  Q.........'.....
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/stats.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/stats.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/stats.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/tabular.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/benchmark.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 18429 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,930 +1,831 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 fd47 0000  o........Coe.G..
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 333e 0000  o.......m.=f3>..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0173 9601 0000 6400  .....@...s....d.
+00000020: 0007 0000 0040 0000 0173 fc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
-00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
-00000070: 0100 6400 6405 6c0d 5a0e 6400 6405 6c0f  ..d.d.l.Z.d.d.l.
-00000080: 5a10 6400 6406 6c11 6d12 5a12 0100 6400  Z.d.d.l.m.Z...d.
-00000090: 6407 6c13 6d14 5a14 0100 6400 6408 6c15  d.l.m.Z...d.d.l.
-000000a0: 6d16 5a16 0100 6400 6409 6c17 6d18 5a18  m.Z...d.d.l.m.Z.
-000000b0: 0100 6400 640a 6c19 6d1a 5a1a 0100 6505  ..d.d.l.m.Z...e.
-000000c0: 7250 6400 640b 6c1b 6d1c 5a1c 0100 6509  rPd.d.l.m.Z...e.
-000000d0: 640c 6518 640d 8d02 5a1d 6509 640e 651a  d.e.d...Z.e.d.e.
-000000e0: 640d 8d02 5a1e 6509 640f 651f 6520 8303  d...Z.e.d.e.e ..
-000000f0: 5a21 4700 6410 6411 8400 6411 6516 651d  Z!G.d.d...d.e.e.
-00000100: 651e 6521 6603 1900 8303 5a22 6523 6412  e.e!f.....Z"e#d.
-00000110: 6b02 72c9 6503 6524 8301 6a25 5a26 6526  k.r.e.e$..j%Z&e&
-00000120: 6a25 6a25 6413 1b00 6414 1b00 6415 1b00  j%j%d...d...d...
-00000130: 5a27 6510 a028 6527 a101 5a29 6400 6416  Z'e..(e'..Z)d.d.
-00000140: 6c2a 6d2b 5a2b 6d2c 5a2c 0100 6522 6417  l*m+Z+m,Z,..e"d.
-00000150: 6529 6418 6419 652c 652b 641a 8d06 5a2d  e)d.d.e,e+d...Z-
-00000160: 652d 6a2e 5a2f 6530 652f a031 a100 8301  e-j.Z/e0e/.1....
-00000170: 5a32 6530 652f a033 a100 8301 5a2e 652d  Z2e0e/.3....Z.e-
-00000180: 6a34 641b 641c 8d01 5a35 6535 6a36 5a37  j4d.d...Z5e5j6Z7
-00000190: 652d 6a38 6535 641b 641d 8d02 5a39 652d  e-j8e5d.d...Z9e-
-000001a0: 6a38 6535 641e 641d 8d02 5a3a 652d 6a3b  j8e5d.d...Z:e-j;
-000001b0: 6535 641b 641f 6420 8d03 5a3b 6405 5300  e5d.d.d ..Z;d.S.
-000001c0: 6405 5300 2921 e900 0000 0029 01da 0b61  d.S.)!.....)...a
-000001d0: 6e6e 6f74 6174 696f 6e73 2901 da04 5061  nnotations)...Pa
-000001e0: 7468 2906 da0d 5459 5045 5f43 4845 434b  th)...TYPE_CHECK
-000001f0: 494e 47da 0341 6e79 da08 4974 6572 6162  ING..Any..Iterab
-00000200: 6c65 da07 4d61 7070 696e 67da 0754 7970  le..Mapping..Typ
-00000210: 6556 6172 da08 6f76 6572 6c6f 6164 2901  eVar..overload).
-00000220: da08 6f76 6572 7269 6465 4e29 01da 1243  ..overrideN)...C
-00000230: 6f6e 6669 6775 7261 7469 6f6e 5370 6163  onfigurationSpac
-00000240: 6529 01da 0a66 6972 7374 5f74 7275 6529  e)...first_true)
-00000250: 01da 0942 656e 6368 6d61 726b 2901 da0d  ...Benchmark)...
-00000260: 5461 6275 6c61 7243 6f6e 6669 6729 01da  TabularConfig)..
-00000270: 0652 6573 756c 7429 01da 064d 6574 7269  .Result)...Metri
-00000280: 63da 0843 5461 6275 6c61 7229 01da 0562  c..CTabular)...b
-00000290: 6f75 6e64 da01 52da 0146 6300 0000 0000  ound..R..Fc.....
-000002a0: 0000 0000 0000 0000 0000 0007 0000 0000  ................
-000002b0: 0000 0173 c800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-000002c0: 6401 6401 6401 6401 6401 6401 6402 9c06  d.d.d.d.d.d.d...
-000002d0: 6442 8700 6601 6418 6419 840e 5a03 6401  dB..f.d.d...Z.d.
-000002e0: 6401 6401 641a 9c03 6443 6421 6422 8406  d.d.d...dCd!d"..
-000002f0: 5a04 6505 6401 6401 6401 6401 6401 6423  Z.e.d.d.d.d.d.d#
-00000300: 9c05 6444 6428 6429 8406 8301 5a06 6445  ..dDd(d)....Z.dE
-00000310: 642c 642d 8404 5a07 6505 6446 6431 6432  d,d-..Z.e.dFd1d2
-00000320: 8404 8301 5a08 6505 6447 6434 6435 8404  ....Z.e.dGd4d5..
-00000330: 8301 5a09 650a 0901 6448 6436 6437 9c01  ..Z.e...dHd6d7..
-00000340: 6449 643b 643c 8407 8301 5a0b 650a 6436  dId;d<....Z.e.d6
-00000350: 6437 9c01 644a 643f 643c 8406 8301 5a0b  d7..dJd?d<....Z.
-00000360: 6505 0901 6448 6401 6437 9c01 644b 6441  e...dHd.d7..dKdA
-00000370: 643c 8407 8301 5a0b 8700 0400 5a0c 5300  d<....Z.....Z.S.
-00000380: 294c da10 5461 6275 6c61 7242 656e 6368  )L..TabularBench
-00000390: 6d61 726b 4e29 06da 0c76 616c 7565 5f6d  markN)...value_m
-000003a0: 6574 7269 63da 0b63 6f73 745f 6d65 7472  etric..cost_metr
-000003b0: 6963 da05 7370 6163 65da 0473 6565 64da  ic..space..seed.
-000003c0: 0570 7269 6f72 da0d 7065 7274 7572 625f  .prior..perturb_
-000003d0: 7072 696f 72da 046e 616d 65da 0373 7472  prior..name..str
-000003e0: da05 7461 626c 65fa 0c70 642e 4461 7461  ..table..pd.Data
-000003f0: 4672 616d 65da 0669 645f 6b65 79da 0c66  Frame..id_key..f
-00000400: 6964 656c 6974 795f 6b65 79da 0b72 6573  idelity_key..res
-00000410: 756c 745f 7479 7065 fa07 7479 7065 5b52  ult_type..type[R
-00000420: 5dda 0b63 6f6e 6669 675f 7479 7065 fa0e  ]..config_type..
-00000430: 7479 7065 5b43 5461 6275 6c61 725d 7216  type[CTabular]r.
-00000440: 0000 00fa 0a73 7472 207c 204e 6f6e 6572  .....str | Noner
-00000450: 1700 0000 7218 0000 00fa 1943 6f6e 6669  ....r......Confi
-00000460: 6775 7261 7469 6f6e 5370 6163 6520 7c20  gurationSpace | 
-00000470: 4e6f 6e65 7219 0000 00fa 0a69 6e74 207c  Noner......int |
-00000480: 204e 6f6e 6572 1a00 0000 fa30 7374 7220   Noner.....0str 
-00000490: 7c20 5061 7468 207c 2043 5461 6275 6c61  | Path | CTabula
-000004a0: 7220 7c20 4d61 7070 696e 675b 7374 722c  r | Mapping[str,
-000004b0: 2041 6e79 5d20 7c20 4e6f 6e65 721b 0000   Any] | Noner...
-000004c0: 00fa 0c66 6c6f 6174 207c 204e 6f6e 6563  ...float | Nonec
-000004d0: 0300 0000 0000 0000 0a00 0000 1900 0000  ................
-000004e0: 0d00 0000 0300 0001 738c 0200 0088 02a0  ........s.......
-000004f0: 00a1 0089 027c 0388 026a 0176 0172 1474  .....|...j.v.r.t
-00000500: 0264 017c 039b 0264 0288 026a 019b 009d  .d.|...d...j....
-00000510: 0483 0182 017c 0488 026a 0176 0172 2474  .....|...j.v.r$t
-00000520: 0264 037c 049b 0264 0288 026a 019b 009d  .d.|...d...j....
-00000530: 0483 0182 0174 037c 056a 04a0 05a1 0083  .....t.|.j......
-00000540: 017d 0d74 0687 0266 0164 0464 0584 087c  .}.t...f.d.d...|
-00000550: 0d44 0083 0183 0173 4174 0264 067c 0d9b  .D.....sAt.d.|..
-00000560: 0264 0788 026a 019b 009d 0483 0182 0188  .d...j..........
-00000570: 01a0 07a1 0089 0074 0687 0266 0164 0864  .......t...f.d.d
-00000580: 0584 0888 0044 0083 0183 0173 5b74 0264  .....D.....s[t.d
-00000590: 0988 009b 0264 0788 026a 019b 009d 0483  .....d...j......
-000005a0: 0182 0164 0a88 026a 0176 0072 6c7c 0364  ...d...j.v.rl|.d
-000005b0: 0a6b 0372 6c74 0264 0b7c 039b 0264 0c9d  .k.rlt.d.|...d..
-000005c0: 0383 0182 0188 026a 087c 0364 0a69 0164  .......j.|.d.i.d
-000005d0: 0d8d 0189 0264 0a7c 0467 027d 0e67 007c  .....d.|.g.}.g.|
-000005e0: 0ea2 017c 0da2 0188 00a2 017d 0f88 027c  ...|.......}...|
-000005f0: 0f19 0089 0288 02a0 097c 0ea1 01a0 0aa1  .........|......
-00000600: 0089 0288 026a 0ba0 0c7c 04a1 017d 107c  .....j...|...}.|
-00000610: 10a0 0da1 007d 117c 117c 116a 0e64 0e19  .....}.|.|.j.d..
-00000620: 006b 02a0 06a1 0073 a874 0264 0f7c 049b  .k.....s.t.d.|..
-00000630: 0264 107c 119b 009d 0483 0182 0174 0f7c  .d.|.........t.|
-00000640: 10a0 10a1 0083 017d 127c 1264 0e19 007d  .......}.|.d...}
-00000650: 137c 1264 1119 007d 147c 1264 1219 007c  .|.d...}.|.d...|
-00000660: 1264 0e19 0018 007d 1588 026a 1164 0a64  .d.....}...j.d.d
-00000670: 138d 01a0 1264 14a1 017d 1687 0087 0166  .....d...}.....f
-00000680: 0264 1564 1684 087c 16a0 13a1 0044 0083  .d.d...|.....D..
-00000690: 017d 177c 0964 1775 0072 dd74 147c 017c  .}.|.d.u.r.t.|.|
-000006a0: 0a64 188d 027d 0988 027c 005f 157c 177c  .d...}...|._.|.|
-000006b0: 005f 167c 037c 005f 177c 047c 005f 1874  ._.|.|._.|.|._.t
-000006c0: 0f88 0083 017c 005f 1974 0f7c 0d83 017c  .....|._.t.|...|
-000006d0: 005f 1a74 1b83 006a 1c7c 017c 0a88 017c  ._.t...j.|.|...|
-000006e0: 057c 047c 137c 147c 1566 037c 097c 0b7c  .|.|.|.|.f.|.|.|
-000006f0: 0c7c 077c 0864 198d 0b01 0087 0266 0164  .|.|.d.......f.d
-00000700: 1a64 1684 087c 006a 1d6a 04a0 1ea1 0044  .d...|.j.j.....D
-00000710: 0083 017d 1864 1b64 1684 007c 18a0 1ea1  ...}.d.d...|....
-00000720: 0044 0083 017c 005f 1f7c 006a 207c 006a  .D...|._.|.j |.j
-00000730: 1a76 0190 0172 3174 0264 1c7c 006a 209b  .v...r1t.d.|.j .
-00000740: 0264 1d7c 006a 1a9b 009d 0483 0182 017c  .d.|.j.........|
-00000750: 006a 217c 006a 1a76 0190 0172 4474 0264  .j!|.j.v...rDt.d
-00000760: 1e7c 006a 219b 0264 1d7c 006a 1a9b 009d  .|.j!..d.|.j....
-00000770: 0483 0182 0164 1753 0029 1f61 a605 0000  .....d.S.).a....
-00000780: 496e 6974 6961 6c69 7a65 2074 6865 2062  Initialize the b
-00000790: 656e 6368 6d61 726b 2e0a 0a20 2020 2020  enchmark...     
-000007a0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-000007b0: 2020 2020 206e 616d 653a 2054 6865 206e       name: The n
-000007c0: 616d 6520 6f66 2074 6869 7320 6265 6e63  ame of this benc
-000007d0: 686d 6172 6b2e 0a20 2020 2020 2020 2020  hmark..         
-000007e0: 2020 2074 6162 6c65 3a20 5468 6520 7461     table: The ta
-000007f0: 626c 6520 746f 2075 7365 2066 6f72 2074  ble to use for t
-00000800: 6865 2062 656e 6368 6d61 726b 2e0a 2020  he benchmark..  
-00000810: 2020 2020 2020 2020 2020 6964 5f6b 6579            id_key
-00000820: 3a20 5468 6520 636f 6c75 6d6e 2069 6e20  : The column in 
-00000830: 7468 6520 7461 626c 6520 7468 6174 2063  the table that c
-00000840: 6f6e 7461 696e 7320 7468 6520 636f 6e66  ontains the conf
-00000850: 6967 2069 640a 2020 2020 2020 2020 2020  ig id.          
-00000860: 2020 6669 6465 6c69 7479 5f6b 6579 3a20    fidelity_key: 
-00000870: 5468 6520 636f 6c75 6d6e 2069 6e20 7468  The column in th
-00000880: 6520 7461 626c 6520 7468 6174 2063 6f6e  e table that con
-00000890: 7461 696e 7320 7468 6520 6669 6465 6c69  tains the fideli
-000008a0: 7479 0a20 2020 2020 2020 2020 2020 2072  ty.            r
-000008b0: 6573 756c 745f 7479 7065 3a20 5468 6520  esult_type: The 
-000008c0: 7265 7375 6c74 2074 7970 6520 666f 7220  result type for 
-000008d0: 7468 6973 2062 656e 6368 6d61 726b 2e0a  this benchmark..
-000008e0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-000008f0: 6967 5f74 7970 653a 2054 6865 2063 6f6e  ig_type: The con
-00000900: 6669 6720 7479 7065 2066 6f72 2074 6869  fig type for thi
-00000910: 7320 6265 6e63 686d 6172 6b2e 0a20 2020  s benchmark..   
-00000920: 2020 2020 2020 2020 2076 616c 7565 5f6d           value_m
-00000930: 6574 7269 633a 2054 6865 206d 6574 7269  etric: The metri
-00000940: 6320 746f 2075 7365 2066 6f72 2074 6869  c to use for thi
-00000950: 7320 6265 6e63 686d 6172 6b2e 2055 7365  s benchmark. Use
-00000960: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00000970: 2020 7468 6520 6465 6661 756c 7420 6d65    the default me
-00000980: 7472 6963 2066 726f 6d20 7468 6520 5265  tric from the Re
-00000990: 7375 6c74 2069 6620 4e6f 6e65 2e0a 2020  sult if None..  
-000009a0: 2020 2020 2020 2020 2020 636f 7374 5f6d            cost_m
-000009b0: 6574 7269 633a 2054 6865 2063 6f73 7420  etric: The cost 
-000009c0: 746f 2075 7365 2066 6f72 2074 6869 7320  to use for this 
-000009d0: 6265 6e63 686d 6172 6b2e 2055 7365 730a  benchmark. Uses.
-000009e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009f0: 7468 6520 6465 6661 756c 7420 636f 7374  the default cost
-00000a00: 2066 726f 6d20 7468 6520 5265 7375 6c74   from the Result
-00000a10: 2069 6620 4e6f 6e65 2e0a 2020 2020 2020   if None..      
-00000a20: 2020 2020 2020 7370 6163 653a 2054 6865        space: The
-00000a30: 2063 6f6e 6669 6775 7261 7469 6f6e 2073   configuration s
-00000a40: 7061 6365 2074 6f20 7573 6520 666f 7220  pace to use for 
-00000a50: 7468 6520 6265 6e63 686d 6172 6b2e 2049  the benchmark. I
-00000a60: 6620 4e6f 6e65 2c20 7769 6c6c 0a20 2020  f None, will.   
-00000a70: 2020 2020 2020 2020 2020 2020 206a 7573               jus
-00000a80: 7420 6265 2061 6e20 656d 7074 7920 7370  t be an empty sp
-00000a90: 6163 652e 0a20 2020 2020 2020 2020 2020  ace..           
-00000aa0: 2070 7269 6f72 3a20 5468 6520 7072 696f   prior: The prio
-00000ab0: 7220 746f 2075 7365 2066 6f72 2074 6865  r to use for the
-00000ac0: 2062 656e 6368 6d61 726b 2e20 4966 204e   benchmark. If N
-00000ad0: 6f6e 652c 206e 6f20 7072 696f 7220 6973  one, no prior is
-00000ae0: 2075 7365 642e 0a20 2020 2020 2020 2020   used..         
-00000af0: 2020 2020 2020 2049 6620 6120 7374 7269         If a stri
-00000b00: 6e67 2c20 7769 6c6c 2062 6520 7472 6561  ng, will be trea
-00000b10: 7465 6420 6173 2061 2070 7269 6f72 2073  ted as a prior s
-00000b20: 7065 6369 6669 6320 666f 7220 7468 6973  pecific for this
-00000b30: 2062 656e 6368 6d61 726b 0a20 2020 2020   benchmark.     
-00000b40: 2020 2020 2020 2020 2020 2069 6620 6974             if it
-00000b50: 2063 616e 2062 6520 666f 756e 642c 206f   can be found, o
-00000b60: 7468 6572 7769 7365 2061 7373 756d 6573  therwise assumes
-00000b70: 2069 7420 746f 2062 6520 6120 5061 7468   it to be a Path
-00000b80: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000b90: 2020 4966 2061 2050 6174 682c 2077 696c    If a Path, wil
-00000ba0: 6c20 6c6f 6164 2074 6865 2070 7269 6f72  l load the prior
-00000bb0: 2066 726f 6d20 7468 6520 7061 7468 2e0a   from the path..
-00000bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bd0: 4966 2061 2064 6963 7420 6f72 2043 6f6e  If a dict or Con
-00000be0: 6669 6775 7261 7469 6f6e 2c20 7769 6c6c  figuration, will
-00000bf0: 2062 6520 7573 6564 2064 6972 6563 746c   be used directl
-00000c00: 792e 0a20 2020 2020 2020 2020 2020 2070  y..            p
-00000c10: 6572 7475 7262 5f70 7269 6f72 3a20 4966  erturb_prior: If
-00000c20: 206e 6f74 204e 6f6e 652c 2077 696c 6c20   not None, will 
-00000c30: 7065 7274 7572 6220 7468 6520 7072 696f  perturb the prio
-00000c40: 7220 6279 2074 6869 7320 616d 6f75 6e74  r by this amount
-00000c50: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000c60: 2020 466f 7220 6e75 6d65 7269 6361 6c73    For numericals
-00000c70: 2c20 7768 696c 6520 666f 7220 6361 7465  , while for cate
-00000c80: 676f 7269 6361 6c73 2c20 7468 6973 2069  goricals, this i
-00000c90: 7320 696e 7465 7270 7265 7465 6420 6173  s interpreted as
-00000ca0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-00000cb0: 2020 2020 2070 726f 6261 6269 6c69 7479       probability
-00000cc0: 206f 6620 7377 6170 7069 6e67 2074 6865   of swapping the
-00000cd0: 2076 616c 7565 2066 6f72 2061 2072 616e   value for a ran
-00000ce0: 646f 6d20 6f6e 652e 0a20 2020 2020 2020  dom one..       
-00000cf0: 2020 2020 2073 6565 643a 2054 6865 2073       seed: The s
-00000d00: 6565 6420 746f 2075 7365 2066 6f72 2074  eed to use for t
-00000d10: 6865 2062 656e 6368 6d61 726b 2e0a 2020  he benchmark..  
-00000d20: 2020 2020 2020 7a08 2769 645f 6b65 793d        z.'id_key=
-00000d30: 7a11 2720 6e6f 7420 696e 2063 6f6c 756d  z.' not in colum
-00000d40: 6e73 207a 0e27 6669 6465 6c69 7479 5f6b  ns z.'fidelity_k
-00000d50: 6579 3d63 0100 0000 0000 0000 0000 0000  ey=c............
-00000d60: 0200 0000 0300 0000 3300 0001 f31a 0000  ........3.......
-00000d70: 0081 007c 005d 087d 017c 0188 006a 0076  ...|.].}.|...j.v
-00000d80: 0056 0001 0071 0264 0053 00a9 014e a901  .V...q.d.S...N..
-00000d90: da07 636f 6c75 6d6e 73a9 02da 022e 30da  ..columns.....0.
-00000da0: 036b 6579 a901 721e 0000 00a9 00fa 3a2f  .key..r.......:/
-00000db0: 686f 6d65 2f73 6b61 6e74 6966 792f 636f  home/skantify/co
-00000dc0: 6465 2f6d 662d 7072 696f 722d 6265 6e63  de/mf-prior-benc
-00000dd0: 682f 7372 632f 6d66 7062 656e 6368 2f74  h/src/mfpbench/t
-00000de0: 6162 756c 6172 2e70 79da 093c 6765 6e65  abular.py..<gene
-00000df0: 7870 723e 5300 0000 f304 0000 0002 8018  xpr>S...........
-00000e00: 007a 2c54 6162 756c 6172 4265 6e63 686d  .z,TabularBenchm
-00000e10: 6172 6b2e 5f5f 696e 6974 5f5f 2e3c 6c6f  ark.__init__.<lo
-00000e20: 6361 6c73 3e2e 3c67 656e 6578 7072 3e7a  cals>.<genexpr>z
-00000e30: 144e 6f74 2061 6c6c 2072 6573 756c 745f  .Not all result_
-00000e40: 6b65 7973 3d7a 1020 6e6f 7420 696e 2063  keys=z. not in c
-00000e50: 6f6c 756d 6e73 2063 0100 0000 0000 0000  olumns c........
-00000e60: 0000 0000 0200 0000 0300 0000 3300 0001  ............3...
-00000e70: 722b 0000 0072 2c00 0000 722d 0000 0072  r+...r,...r-...r
-00000e80: 2f00 0000 7232 0000 0072 3300 0000 7234  /...r2...r3...r4
-00000e90: 0000 0072 3500 0000 5900 0000 7236 0000  ...r5...Y...r6..
-00000ea0: 007a 0c63 6f6e 6669 675f 6b65 7973 3dda  .z.config_keys=.
-00000eb0: 0269 647a 3643 616e 2774 2068 6176 6520  .idz6Can't have 
-00000ec0: 6069 6460 2069 6e20 7468 6520 636f 6c75  `id` in the colu
-00000ed0: 6d6e 7320 6966 2069 7427 7320 6e6f 7420  mns if it's not 
-00000ee0: 7468 6520 6964 5f6b 6579 3d7a 1e2e 2050  the id_key=z.. P
-00000ef0: 6c65 6173 6520 6472 6f70 2069 7420 6f72  lease drop it or
-00000f00: 2072 656e 616d 6520 6974 2e72 2d00 0000   rename it.r-...
-00000f10: 7201 0000 007a 0d66 6964 656c 6974 795f  r....z.fidelity_
-00000f20: 6b65 793d 7a0f 206e 6f74 2075 6e69 666f  key=z. not unifo
-00000f30: 726d 2e20 0ae9 ffff ffff e901 0000 0029  rm. ...........)
-00000f40: 01da 056c 6576 656c da05 6669 7273 7463  ...level..firstc
-00000f50: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00000f60: 0900 0000 1300 0001 7338 0000 0069 007c  ........s8...i.|
-00000f70: 005d 185c 027d 017d 0274 007c 0183 0188  .].\.}.}.t.|....
-00000f80: 01a0 0169 007c 0288 0019 00a0 02a1 00a5  ...i.|..........
-00000f90: 0164 0074 007c 0183 0169 01a5 01a1 0193  .d.t.|...i......
-00000fa0: 0271 0253 0029 0172 3700 0000 2903 721d  .q.S.).r7...).r.
-00000fb0: 0000 00da 0966 726f 6d5f 6469 6374 da07  .....from_dict..
-00000fc0: 746f 5f64 6963 7429 0372 3000 0000 da09  to_dict).r0.....
-00000fd0: 636f 6e66 6967 5f69 64da 0372 6f77 2902  config_id..row).
-00000fe0: da0b 636f 6e66 6967 5f6b 6579 7372 2400  ..config_keysr$.
-00000ff0: 0000 7233 0000 0072 3400 0000 da0a 3c64  ..r3...r4.....<d
-00001000: 6963 7463 6f6d 703e 8e00 0000 7314 0000  ictcomp>....s...
-00001010: 0006 0006 070a fa02 010a 0102 ff08 0204  ................
-00001020: fe02 ff06 ff7a 2d54 6162 756c 6172 4265  .....z-TabularBe
-00001030: 6e63 686d 6172 6b2e 5f5f 696e 6974 5f5f  nchmark.__init__
-00001040: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00001050: 6f6d 703e 4ea9 0172 1900 0000 290b 721c  omp>N..r....).r.
-00001060: 0000 0072 1900 0000 7224 0000 0072 2200  ...r....r$...r".
-00001070: 0000 da0d 6669 6465 6c69 7479 5f6e 616d  ....fidelity_nam
-00001080: 65da 0e66 6964 656c 6974 795f 7261 6e67  e..fidelity_rang
-00001090: 6572 1800 0000 721a 0000 0072 1b00 0000  er....r....r....
-000010a0: 7216 0000 0072 1700 0000 6301 0000 0000  r....r....c.....
-000010b0: 0000 0000 0000 0003 0000 0006 0000 0013  ................
-000010c0: 0000 0173 3c00 0000 6900 7c00 5d1a 5c02  ...s<...i.|.].\.
-000010d0: 7d01 7d02 7c01 7c02 6602 7c02 6a00 7214  }.}.|.|.f.|.j.r.
-000010e0: 7401 8800 7c01 1900 a002 a100 8301 6e07  t...|.........n.
-000010f0: 7401 8800 7c01 1900 a003 a100 8301 9302  t...|...........
-00001100: 7102 5300 7233 0000 0029 04da 086d 696e  q.S.r3...)...min
-00001110: 696d 697a 65da 0566 6c6f 6174 da03 6d69  imize..float..mi
-00001120: 6eda 036d 6178 2903 7230 0000 00da 016b  n..max).r0.....k
-00001130: da06 6d65 7472 6963 7232 0000 0072 3300  ..metricr2...r3.
-00001140: 0000 7234 0000 0072 4100 0000 b100 0000  ..r4...rA.......
-00001150: 730a 0000 0006 0006 0406 fd24 0106 fe63  s..........$...c
-00001160: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-00001170: 0600 0000 5300 0001 7320 0000 0069 007c  ....S...s ...i.|
-00001180: 005d 0c5c 025c 027d 017d 027d 037c 017c  .].\.\.}.}.}.|.|
-00001190: 02a0 007c 03a1 0193 0271 0253 0072 3300  ...|.....q.S.r3.
-000011a0: 0000 2901 da08 6173 5f76 616c 7565 2904  ..)...as_value).
-000011b0: 7230 0000 0072 4900 0000 724a 0000 00da  r0...rI...rJ....
-000011c0: 0176 7233 0000 0072 3300 0000 7234 0000  .vr3...r3...r4..
-000011d0: 0072 4100 0000 b700 0000 7306 0000 0006  .rA.......s.....
-000011e0: 0014 0106 ff7a 1273 656c 662e 7661 6c75  .....z.self.valu
-000011f0: 655f 6d65 7472 6963 3dfa 0820 6e6f 7420  e_metric=.. not 
-00001200: 696e 207a 1173 656c 662e 636f 7374 5f6d  in z.self.cost_m
-00001210: 6574 7269 633d 2922 da0b 7265 7365 745f  etric=)"..reset_
-00001220: 696e 6465 7872 2e00 0000 da0a 5661 6c75  indexr......Valu
-00001230: 6545 7272 6f72 da04 6c69 7374 da0b 6d65  eError..list..me
-00001240: 7472 6963 5f64 6566 73da 046b 6579 73da  tric_defs..keys.
-00001250: 0361 6c6c da05 6e61 6d65 73da 0672 656e  .all..names..ren
-00001260: 616d 65da 0973 6574 5f69 6e64 6578 da0a  ame..set_index..
-00001270: 736f 7274 5f69 6e64 6578 da05 696e 6465  sort_index..inde
-00001280: 78da 1067 6574 5f6c 6576 656c 5f76 616c  x..get_level_val
-00001290: 7565 73da 0c76 616c 7565 5f63 6f75 6e74  ues..value_count
-000012a0: 73da 0469 6c6f 63da 0673 6f72 7465 64da  s..iloc..sorted.
-000012b0: 0675 6e69 7175 65da 0767 726f 7570 6279  .unique..groupby
-000012c0: da03 6167 67da 0869 7465 7272 6f77 7372  ..agg..iterrowsr
-000012d0: 0b00 0000 721e 0000 00da 0763 6f6e 6669  ....r......confi
-000012e0: 6773 7220 0000 0072 2100 0000 7240 0000  gsr ...r!...r@..
-000012f0: 00da 0b72 6573 756c 745f 6b65 7973 da05  ...result_keys..
-00001300: 7375 7065 72da 085f 5f69 6e69 745f 5f72  super..__init__r
-00001310: 0f00 0000 da05 6974 656d 735a 0e74 6162  ......itemsZ.tab
-00001320: 6c65 5f6f 7074 696d 756d 7372 1600 0000  le_optimumsr....
-00001330: 7217 0000 0029 19da 0473 656c 6672 1c00  r....)...selfr..
-00001340: 0000 721e 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-00001350: 0072 2200 0000 7224 0000 0072 1600 0000  .r"...r$...r....
-00001360: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00001370: 1a00 0000 721b 0000 0072 6200 0000 da0a  ....r....rb.....
-00001380: 696e 6465 785f 636f 6c73 5a0d 7265 6c65  index_colsZ.rele
-00001390: 7661 6e74 5f63 6f6c 735a 0f66 6964 656c  vant_colsZ.fidel
-000013a0: 6974 795f 7661 6c75 6573 5a0f 6669 6465  ity_valuesZ.fide
-000013b0: 6c69 7479 5f63 6f75 6e74 735a 0b73 6f72  lity_countsZ.sor
-000013c0: 7465 645f 6669 6473 da05 7374 6172 74da  ted_fids..start.
-000013d0: 0365 6e64 da04 7374 6570 5a08 6964 5f74  .end..stepZ.id_t
-000013e0: 6162 6c65 7261 0000 005a 0d5f 7261 775f  ablera...Z._raw_
-000013f0: 6f70 7469 6d75 6d73 a901 da09 5f5f 636c  optimums....__cl
-00001400: 6173 735f 5f29 0372 4000 0000 7224 0000  ass__).r@...r$..
-00001410: 0072 1e00 0000 7234 0000 0072 6400 0000  .r....r4...rd...
-00001420: 1f00 0000 7390 0000 0008 2a0a 0316 010a  ....s.....*.....
-00001430: 0216 010e 0216 0102 0110 0104 ff08 0416  ................
-00001440: 0116 0112 0302 010a 0104 ff10 0608 0302  ................
-00001450: 0302 0102 ff02 0202 fe02 0304 fd08 050e  ................
-00001460: 010c 0e08 0112 0114 010c 0208 0108 0110  ................
-00001470: 0112 070c 0106 0706 f908 0b0c 0106 0206  ................
-00001480: 0106 0106 010a 010a 0106 0202 0102 0102  ................
-00001490: 0102 0102 0108 0102 0102 0102 0102 0102  ................
-000014a0: 0106 f50a 0e0a 0406 fc06 0606 0108 ff0e  ................
-000014b0: 0418 010e 0218 0104 ff7a 1954 6162 756c  .........z.Tabul
-000014c0: 6172 4265 6e63 686d 6172 6b2e 5f5f 696e  arBenchmark.__in
-000014d0: 6974 5f5f 2903 da02 6174 7216 0000 0072  it__)...atr....r
-000014e0: 1700 0000 da06 636f 6e66 6967 fa22 4354  ......config."CT
-000014f0: 6162 756c 6172 207c 204d 6170 7069 6e67  abular | Mapping
-00001500: 5b73 7472 2c20 416e 795d 207c 2073 7472  [str, Any] | str
-00001510: 726d 0000 00fa 0846 207c 204e 6f6e 65da  rm.....F | None.
-00001520: 0672 6574 7572 6e72 1300 0000 6302 0000  .returnr....c...
-00001530: 0000 0000 0003 0000 0007 0000 0008 0000  ................
-00001540: 0003 0000 0173 cc00 0000 7c00 a000 7c01  .....s....|...|.
-00001550: a101 7d05 7c02 6401 7501 720b 7c02 6e02  ..}.|.d.u.r.|.n.
-00001560: 7c00 6a01 7d02 7c00 6a02 7c02 0400 0300  |.j.}.|.j.|.....
-00001570: 6b01 721b 7c00 6a01 6b01 731e 4a00 8201  k.r.|.j.k.s.J...
-00001580: 0100 4a00 8201 7c05 6a03 6402 6403 8d01  ..J...|.j.d.d...
-00001590: 8900 7c00 6a04 6401 7501 723e 6404 6405  ..|.j.d.u.r>d.d.
-000015a0: 8400 7c00 6a04 a005 a100 4400 8301 7d06  ..|.j.....D...}.
-000015b0: 8700 6601 6406 6405 8408 7c06 a005 a100  ..f.d.d...|.....
-000015c0: 4400 8301 8900 7c03 6401 7501 7244 7c03  D.....|.d.u.rD|.
-000015d0: 6e02 7c00 6a06 7d03 7c04 6401 7501 724d  n.|.j.}.|.d.u.rM
-000015e0: 7c04 6e02 7c00 6a07 7d04 7c00 6a08 6a09  |.n.|.j.}.|.j.j.
-000015f0: 7c01 7c02 7c00 6a0a 8800 7c02 6407 8d02  |.|.|.j...|.d...
-00001600: 740b 7c03 8301 740b 7c04 8301 7c00 6a0c  t.|...t.|...|.j.
-00001610: 6408 8d06 5300 2909 61f9 0400 0053 7562  d...S.).a....Sub
-00001620: 6d69 7420 6120 7175 6572 7920 616e 6420  mit a query and 
-00001630: 6765 7420 6120 7265 7375 6c74 2e0a 0a20  get a result... 
-00001640: 2020 2020 2020 2021 2121 2077 6172 6e69         !!! warni
-00001650: 6e67 2022 5061 7373 696e 6720 6120 7261  ng "Passing a ra
-00001660: 7720 636f 6e66 6967 220a 0a20 2020 2020  w config"..     
-00001670: 2020 2020 2020 2049 6620 6120 6d61 7070         If a mapp
-00001680: 696e 6720 6973 2070 6173 7365 6420 2861  ing is passed (a
-00001690: 6e64 202a 2a6e 6f74 2a2a 2061 205b 6043  nd **not** a [`C
-000016a0: 6f6e 6669 6760 5d5b 6d66 7062 656e 6368  onfig`][mfpbench
-000016b0: 2e43 6f6e 6669 675d 206f 626a 6563 7429  .Config] object)
-000016c0: 2c0a 2020 2020 2020 2020 2020 2020 7765  ,.            we
-000016d0: 2077 696c 6c20 6174 7465 6d70 7420 746f   will attempt to
-000016e0: 206c 6f6f 6b20 666f 7220 6069 6460 2069   look for `id` i
-000016f0: 6e20 7468 6520 6d61 7070 696e 672c 2074  n the mapping, t
-00001700: 6f20 6b6e 6f77 2077 6869 6368 2063 6f6e  o know which con
-00001710: 6669 6720 746f 0a20 2020 2020 2020 2020  fig to.         
-00001720: 2020 206c 6f6f 6b75 702e 0a0a 2020 2020     lookup...    
-00001730: 2020 2020 2020 2020 4966 2074 6869 7320          If this 
-00001740: 6661 696c 732c 2077 6520 7769 6c6c 2074  fails, we will t
-00001750: 7279 206d 6174 6368 2074 6865 2063 6f6e  ry match the con
-00001760: 6669 6720 746f 206f 6e65 206f 6620 7468  fig to one of th
-00001770: 6520 636f 6e66 6967 7320 696e 0a20 2020  e configs in.   
-00001780: 2020 2020 2020 2020 2074 6865 2062 656e           the ben
-00001790: 6368 6d61 726b 2e0a 0a20 2020 2020 2020  chmark...       
-000017a0: 2020 2020 2050 7265 6665 7220 746f 2070       Prefer to p
-000017b0: 6173 7320 7468 6520 5b60 436f 6e66 6967  ass the [`Config
-000017c0: 605d 5b6d 6670 6265 6e63 682e 436f 6e66  `][mfpbench.Conf
-000017d0: 6967 5d20 6f62 6a65 6374 2064 6972 6563  ig] object direc
-000017e0: 746c 7920 6966 2070 6f73 7369 626c 652e  tly if possible.
-000017f0: 0a0a 2020 2020 2020 2020 3f3f 3f20 6e6f  ..        ??? no
-00001800: 7465 2022 4f76 6572 7269 6465 220a 0a20  te "Override".. 
-00001810: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00001820: 6675 6e63 7469 6f6e 206f 7665 7272 6964  function overrid
-00001830: 6573 2074 6865 2064 6566 6175 6c74 0a20  es the default. 
-00001840: 2020 2020 2020 2020 2020 205b 6071 7565             [`que
-00001850: 7279 2829 605d 5b6d 6670 6265 6e63 682e  ry()`][mfpbench.
-00001860: 4265 6e63 686d 6172 6b2e 7175 6572 795d  Benchmark.query]
-00001870: 2074 6f20 616c 6c6f 7720 666f 7220 7468   to allow for th
-00001880: 6973 0a20 2020 2020 2020 2020 2020 2063  is.            c
-00001890: 6f6e 6669 6720 6d61 7463 6869 6e67 0a0a  onfig matching..
-000018a0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-000018b0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-000018c0: 3a20 5468 6520 7175 6572 7920 746f 2075  : The query to u
-000018d0: 7365 0a20 2020 2020 2020 2020 2020 2061  se.            a
-000018e0: 743a 2054 6865 2066 6964 656c 6974 7920  t: The fidelity 
-000018f0: 6174 2077 6869 6368 2074 6f20 7175 6572  at which to quer
-00001900: 792c 2064 6566 6175 6c74 7320 746f 204e  y, defaults to N
-00001910: 6f6e 6520 7768 6963 6820 6d65 616e 7320  one which means 
-00001920: 2a6d 6178 696d 756d 2a0a 2020 2020 2020  *maximum*.      
-00001930: 2020 2020 2020 7661 6c75 655f 6d65 7472        value_metr
-00001940: 6963 3a20 5468 6520 6d65 7472 6963 2074  ic: The metric t
-00001950: 6f20 7573 6520 666f 7220 7468 6973 2072  o use for this r
-00001960: 6573 756c 742e 2055 7365 730a 2020 2020  esult. Uses.    
-00001970: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00001980: 7661 6c75 6520 6d65 7472 6963 2070 6173  value metric pas
-00001990: 7365 6420 696e 2074 6f20 7468 6520 636f  sed in to the co
-000019a0: 6e73 7472 7563 746f 7220 6966 206e 6f74  nstructor if not
-000019b0: 2073 7065 6369 6669 6564 2c0a 2020 2020   specified,.    
-000019c0: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-000019d0: 7277 6973 6520 7468 6520 6465 6661 756c  rwise the defaul
-000019e0: 7420 6d65 7472 6963 2066 726f 6d20 7468  t metric from th
-000019f0: 6520 5265 7375 6c74 2069 6620 4e6f 6e65  e Result if None
-00001a00: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00001a10: 7374 5f6d 6574 7269 633a 2054 6865 206d  st_metric: The m
-00001a20: 6574 7269 6320 746f 2075 7365 2066 6f72  etric to use for
-00001a30: 2074 6869 7320 7265 7375 6c74 2e20 5573   this result. Us
-00001a40: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-00001a50: 2020 2074 6865 2063 6f73 7420 6d65 7472     the cost metr
-00001a60: 6963 2070 6173 7365 6420 696e 2074 6f20  ic passed in to 
-00001a70: 7468 6520 636f 6e73 7472 7563 746f 7220  the constructor 
-00001a80: 6966 206e 6f74 2073 7065 6369 6669 6564  if not specified
-00001a90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001aa0: 2020 6f74 6865 7277 6973 6520 7468 6520    otherwise the 
-00001ab0: 6465 6661 756c 7420 6d65 7472 6963 2066  default metric f
-00001ac0: 726f 6d20 7468 6520 5265 7375 6c74 2069  rom the Result i
-00001ad0: 6620 4e6f 6e65 2e0a 0a20 2020 2020 2020  f None...       
-00001ae0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00001af0: 2020 2020 2020 5468 6520 7265 7375 6c74        The result
-00001b00: 206f 6620 7468 6520 7175 6572 790a 2020   of the query.  
-00001b10: 2020 2020 2020 4e54 a901 da07 7769 7468        NT....with
-00001b20: 5f69 6463 0100 0000 0000 0000 0000 0000  _idc............
-00001b30: 0300 0000 0400 0000 5300 0001 f316 0000  ........S.......
-00001b40: 0069 007c 005d 075c 027d 017d 027c 027c  .i.|.].\.}.}.|.|
-00001b50: 0193 0271 0253 0072 3300 0000 7233 0000  ...q.S.r3...r3..
-00001b60: 00a9 0372 3000 0000 7249 0000 0072 4c00  ...r0...rI...rL.
-00001b70: 0000 7233 0000 0072 3300 0000 7234 0000  ..r3...r3...r4..
-00001b80: 0072 4100 0000 f000 0000 f302 0000 0016  .rA.............
-00001b90: 007a 2a54 6162 756c 6172 4265 6e63 686d  .z*TabularBenchm
-00001ba0: 6172 6b2e 7175 6572 792e 3c6c 6f63 616c  ark.query.<local
-00001bb0: 733e 2e3c 6469 6374 636f 6d70 3e63 0100  s>.<dictcomp>c..
-00001bc0: 0000 0000 0000 0000 0000 0300 0000 0700  ................
-00001bd0: 0000 1300 0001 f31e 0000 0069 007c 005d  ...........i.|.]
-00001be0: 0b5c 027d 017d 027c 0188 00a0 007c 027c  .\.}.}.|.....|.|
-00001bf0: 02a1 0293 0271 0253 0072 3300 0000 a901  .....q.S.r3.....
-00001c00: da03 6765 7472 7500 0000 a901 da19 5f54  ..getru......._T
-00001c10: 6162 756c 6172 4265 6e63 686d 6172 6b5f  abularBenchmark_
-00001c20: 5f63 6f6e 6669 6772 3300 0000 7234 0000  _configr3...r4..
-00001c30: 0072 4100 0000 f100 0000 f302 0000 001e  .rA.............
-00001c40: 00a9 0172 6d00 0000 a906 726e 0000 00da  ...rm.....rn....
-00001c50: 0866 6964 656c 6974 79da 0672 6573 756c  .fidelity..resul
-00001c60: 7472 1600 0000 7217 0000 00da 0772 656e  tr....r......ren
-00001c70: 616d 6573 290d da0c 5f66 696e 645f 636f  ames)..._find_co
-00001c80: 6e66 6967 7269 0000 0072 6800 0000 da07  nfigri...rh.....
-00001c90: 6173 5f64 6963 74da 0f5f 636f 6e66 6967  as_dict.._config
-00001ca0: 5f72 656e 616d 6573 7265 0000 0072 1600  _renamesre...r..
-00001cb0: 0000 7217 0000 0072 0f00 0000 723c 0000  ..r....r....r<..
-00001cc0: 00da 135f 6f62 6a65 6374 6976 655f 6675  ..._objective_fu
-00001cd0: 6e63 7469 6f6e 721d 0000 00da 0f5f 7265  nctionr......_re
-00001ce0: 7375 6c74 5f72 656e 616d 6573 2907 7266  sult_renames).rf
-00001cf0: 0000 0072 6e00 0000 726d 0000 0072 1600  ...rn...rm...r..
-00001d00: 0000 7217 0000 00da 075f 636f 6e66 6967  ..r......_config
-00001d10: da10 5f72 6576 6572 7365 5f72 656e 616d  .._reverse_renam
-00001d20: 6573 7233 0000 0072 7a00 0000 7234 0000  esr3...rz...r4..
-00001d30: 00da 0571 7565 7279 c100 0000 7322 0000  ...query....s"..
-00001d40: 000a 2812 0220 010c 020a 0114 0116 0112  ..(.. ..........
-00001d50: 0212 0106 0202 0102 010c 0106 0106 0104  ................
-00001d60: 0106 fa7a 1654 6162 756c 6172 4265 6e63  ...z.TabularBenc
-00001d70: 686d 6172 6b2e 7175 6572 7929 05da 0366  hmark.query)...f
-00001d80: 726d da02 746f 726a 0000 0072 1600 0000  rm..torj...r....
-00001d90: 7217 0000 0072 8a00 0000 728b 0000 0072  r....r....r....r
-00001da0: 6a00 0000 fa07 6c69 7374 5b52 5d63 0200  j.....list[R]c..
-00001db0: 0000 0000 0000 0500 0000 0900 0000 0700  ................
-00001dc0: 0000 0300 0001 73ca 0000 0088 03a0 0088  ......s.........
-00001dd0: 01a1 017d 077c 0364 0175 0172 0b7c 036e  ...}.|.d.u.r.|.n
-00001de0: 0288 036a 017d 037c 0264 0175 0172 147c  ...j.}.|.d.u.r.|
-00001df0: 026e 0288 036a 027d 027c 0464 0175 0172  .n...j.}.|.d.u.r
-00001e00: 1d7c 046e 0288 036a 037d 047c 076a 0464  .|.n...j.}.|.j.d
-00001e10: 0264 038d 0189 0088 036a 0564 0175 0172  .d.......j.d.u.r
-00001e20: 4064 0464 0584 0088 036a 05a0 06a1 0044  @d.d.....j.....D
-00001e30: 0083 017d 0887 0066 0164 0664 0584 087c  ...}...f.d.d...|
-00001e40: 08a0 06a1 0044 0083 0189 0088 0464 0175  .....D.......d.u
-00001e50: 0172 4688 046e 0288 036a 0789 0488 0264  .rF..n...j.....d
-00001e60: 0175 0172 4f88 026e 0288 036a 0889 0287  .u.rO..n...j....
-00001e70: 0187 0287 0387 0466 0464 0764 0884 0888  .......f.d.d....
-00001e80: 036a 0988 007c 027c 037c 0464 098d 0444  .j...|.|.|.d...D
-00001e90: 0083 0153 0029 0a61 6905 0000 5375 626d  ...S.).ai...Subm
-00001ea0: 6974 2061 2071 7565 7279 2061 6e64 2067  it a query and g
-00001eb0: 6574 2061 2072 6573 756c 742e 0a0a 2020  et a result...  
-00001ec0: 2020 2020 2020 2121 2120 7761 726e 696e        !!! warnin
-00001ed0: 6720 2250 6173 7369 6e67 2061 2072 6177  g "Passing a raw
-00001ee0: 2063 6f6e 6669 6722 0a0a 2020 2020 2020   config"..      
-00001ef0: 2020 2020 2020 4966 2061 206d 6170 7069        If a mappi
-00001f00: 6e67 2069 7320 7061 7373 6564 2028 616e  ng is passed (an
-00001f10: 6420 2a2a 6e6f 742a 2a20 6120 5b60 436f  d **not** a [`Co
-00001f20: 6e66 6967 605d 5b6d 6670 6265 6e63 682e  nfig`][mfpbench.
-00001f30: 436f 6e66 6967 5d20 6f62 6a65 6374 292c  Config] object),
-00001f40: 0a20 2020 2020 2020 2020 2020 2077 6520  .            we 
-00001f50: 7769 6c6c 2061 7474 656d 7074 2074 6f20  will attempt to 
-00001f60: 6c6f 6f6b 2066 6f72 2060 6964 6020 696e  look for `id` in
-00001f70: 2074 6865 206d 6170 7069 6e67 2c20 746f   the mapping, to
-00001f80: 206b 6e6f 7720 7768 6963 6820 636f 6e66   know which conf
-00001f90: 6967 2074 6f0a 2020 2020 2020 2020 2020  ig to.          
-00001fa0: 2020 6c6f 6f6b 7570 2e0a 0a20 2020 2020    lookup...     
-00001fb0: 2020 2020 2020 2049 6620 7468 6973 2066         If this f
-00001fc0: 6169 6c73 2c20 7765 2077 696c 6c20 7472  ails, we will tr
-00001fd0: 7920 6d61 7463 6820 7468 6520 636f 6e66  y match the conf
-00001fe0: 6967 2074 6f20 6f6e 6520 6f66 2074 6865  ig to one of the
-00001ff0: 2063 6f6e 6669 6773 2069 6e0a 2020 2020   configs in.    
-00002000: 2020 2020 2020 2020 7468 6520 6265 6e63          the benc
-00002010: 686d 6172 6b2e 0a0a 2020 2020 2020 2020  hmark...        
-00002020: 2020 2020 5072 6566 6572 2074 6f20 7061      Prefer to pa
-00002030: 7373 2074 6865 205b 6043 6f6e 6669 6760  ss the [`Config`
-00002040: 5d5b 6d66 7062 656e 6368 2e43 6f6e 6669  ][mfpbench.Confi
-00002050: 675d 206f 626a 6563 7420 6469 7265 6374  g] object direct
-00002060: 6c79 2069 6620 706f 7373 6962 6c65 2e0a  ly if possible..
-00002070: 0a20 2020 2020 2020 203f 3f3f 206e 6f74  .        ??? not
-00002080: 6520 224f 7665 7272 6964 6522 0a0a 2020  e "Override"..  
-00002090: 2020 2020 2020 2020 2020 5468 6973 2066            This f
-000020a0: 756e 6374 696f 6e20 6f76 6572 7269 6465  unction override
-000020b0: 7320 7468 6520 6465 6661 756c 740a 2020  s the default.  
-000020c0: 2020 2020 2020 2020 2020 5b60 7472 616a            [`traj
-000020d0: 6563 746f 7279 2829 605d 5b6d 6670 6265  ectory()`][mfpbe
-000020e0: 6e63 682e 4265 6e63 686d 6172 6b2e 7472  nch.Benchmark.tr
-000020f0: 616a 6563 746f 7279 5d20 746f 2061 6c6c  ajectory] to all
-00002100: 6f77 2066 6f72 2074 6869 730a 2020 2020  ow for this.    
-00002110: 2020 2020 2020 2020 636f 6e66 6967 206d          config m
-00002120: 6174 6368 696e 670a 0a20 2020 2020 2020  atching..       
-00002130: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00002140: 2020 2063 6f6e 6669 673a 2054 6865 2071     config: The q
-00002150: 7565 7279 2074 6f20 7573 650a 2020 2020  uery to use.    
-00002160: 2020 2020 2020 2020 6672 6d3a 2053 7461          frm: Sta
-00002170: 7274 206f 6620 7468 6520 6375 7276 652c  rt of the curve,
-00002180: 2073 686f 756c 6420 6465 6661 756c 7420   should default 
-00002190: 746f 2074 6865 2073 7461 7274 0a20 2020  to the start.   
-000021a0: 2020 2020 2020 2020 2074 6f3a 2045 6e64           to: End
-000021b0: 206f 6620 7468 6520 6375 7276 652c 2073   of the curve, s
-000021c0: 686f 756c 6420 6465 6661 756c 7420 746f  hould default to
-000021d0: 2074 6865 2074 6f74 616c 0a20 2020 2020   the total.     
-000021e0: 2020 2020 2020 2073 7465 703a 2053 7465         step: Ste
-000021f0: 7020 7369 7a65 2c20 6465 6661 756c 7473  p size, defaults
-00002200: 2074 6f20 6060 636c 732e 6465 6661 756c   to ``cls.defaul
-00002210: 745f 7374 6570 6060 0a20 2020 2020 2020  t_step``.       
-00002220: 2020 2020 2076 616c 7565 5f6d 6574 7269       value_metri
-00002230: 633a 2054 6865 206d 6574 7269 6320 746f  c: The metric to
-00002240: 2075 7365 2066 6f72 2074 6869 7320 7265   use for this re
-00002250: 7375 6c74 2e20 5573 6573 0a20 2020 2020  sult. Uses.     
-00002260: 2020 2020 2020 2020 2020 2074 6865 2076             the v
-00002270: 616c 7565 206d 6574 7269 6320 7061 7373  alue metric pass
-00002280: 6564 2069 6e20 746f 2074 6865 2063 6f6e  ed in to the con
-00002290: 7374 7275 6374 6f72 2069 6620 6e6f 7420  structor if not 
-000022a0: 7370 6563 6966 6965 642c 0a20 2020 2020  specified,.     
-000022b0: 2020 2020 2020 2020 2020 206f 7468 6572             other
-000022c0: 7769 7365 2074 6865 2064 6566 6175 6c74  wise the default
-000022d0: 206d 6574 7269 6320 6672 6f6d 2074 6865   metric from the
-000022e0: 2052 6573 756c 7420 6966 204e 6f6e 652e   Result if None.
-000022f0: 0a20 2020 2020 2020 2020 2020 2063 6f73  .            cos
-00002300: 745f 6d65 7472 6963 3a20 5468 6520 6d65  t_metric: The me
-00002310: 7472 6963 2074 6f20 7573 6520 666f 7220  tric to use for 
-00002320: 7468 6973 2072 6573 756c 742e 2055 7365  this result. Use
-00002330: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00002340: 2020 7468 6520 636f 7374 206d 6574 7269    the cost metri
-00002350: 6320 7061 7373 6564 2069 6e20 746f 2074  c passed in to t
-00002360: 6865 2063 6f6e 7374 7275 6374 6f72 2069  he constructor i
-00002370: 6620 6e6f 7420 7370 6563 6966 6965 642c  f not specified,
-00002380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002390: 206f 7468 6572 7769 7365 2074 6865 2064   otherwise the d
-000023a0: 6566 6175 6c74 206d 6574 7269 6320 6672  efault metric fr
-000023b0: 6f6d 2074 6865 2052 6573 756c 7420 6966  om the Result if
-000023c0: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
-000023d0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-000023e0: 2020 2020 2054 6865 2072 6573 756c 7420       The result 
-000023f0: 6f66 2074 6865 2071 7565 7279 0a20 2020  of the query.   
-00002400: 2020 2020 204e 5472 7200 0000 6301 0000       NTrr...c...
-00002410: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00002420: 0053 0000 0172 7400 0000 7233 0000 0072  .S...rt...r3...r
-00002430: 3300 0000 7275 0000 0072 3300 0000 7233  3...ru...r3...r3
-00002440: 0000 0072 3400 0000 7241 0000 0034 0100  ...r4...rA...4..
-00002450: 0072 7600 0000 7a2f 5461 6275 6c61 7242  .rv...z/TabularB
-00002460: 656e 6368 6d61 726b 2e74 7261 6a65 6374  enchmark.traject
-00002470: 6f72 792e 3c6c 6f63 616c 733e 2e3c 6469  ory.<locals>.<di
-00002480: 6374 636f 6d70 3e63 0100 0000 0000 0000  ctcomp>c........
-00002490: 0000 0000 0300 0000 0700 0000 1300 0001  ................
-000024a0: 7277 0000 0072 3300 0000 7278 0000 0072  rw...r3...rx...r
-000024b0: 7500 0000 727a 0000 0072 3300 0000 7234  u...rz...r3...r4
-000024c0: 0000 0072 4100 0000 3501 0000 727c 0000  ...rA...5...r|..
-000024d0: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
-000024e0: 0000 0a00 0000 1300 0001 7332 0000 0067  ..........s2...g
-000024f0: 007c 005d 155c 027d 017d 0288 026a 006a  .|.].\.}.}...j.j
-00002500: 0188 007c 017c 0274 0288 0383 0174 0288  ...|.|.t.....t..
-00002510: 0183 0188 026a 0364 008d 0691 0271 0253  .....j.d.....q.S
-00002520: 0029 0172 7e00 0000 2904 720f 0000 0072  .).r~...).r....r
-00002530: 3c00 0000 721d 0000 0072 8600 0000 2903  <...r....r....).
-00002540: 7230 0000 0072 7f00 0000 7280 0000 0029  r0...r....r....)
-00002550: 0472 6e00 0000 7217 0000 0072 6600 0000  .rn...r....rf...
-00002560: 7216 0000 0072 3300 0000 7234 0000 00da  r....r3...r4....
-00002570: 0a3c 6c69 7374 636f 6d70 3e3a 0100 0073  .<listcomp>:...s
-00002580: 1600 0000 0600 0609 06f8 0201 0201 0201  ................
-00002590: 0601 0601 0401 04fa 06ff 7a2f 5461 6275  ..........z/Tabu
-000025a0: 6c61 7242 656e 6368 6d61 726b 2e74 7261  larBenchmark.tra
-000025b0: 6a65 6374 6f72 792e 3c6c 6f63 616c 733e  jectory.<locals>
-000025c0: 2e3c 6c69 7374 636f 6d70 3e29 0372 8a00  .<listcomp>).r..
-000025d0: 0000 728b 0000 0072 6a00 0000 290a 7282  ..r....rj...).r.
-000025e0: 0000 0072 6900 0000 7268 0000 0072 6a00  ...ri...rh...rj.
-000025f0: 0000 7283 0000 0072 8400 0000 7265 0000  ..r....r....re..
-00002600: 0072 1600 0000 7217 0000 00da 0b5f 7472  .r....r......_tr
-00002610: 616a 6563 746f 7279 2909 7266 0000 0072  ajectory).rf...r
-00002620: 6e00 0000 728a 0000 0072 8b00 0000 726a  n...r....r....rj
-00002630: 0000 0072 1600 0000 7217 0000 0072 8700  ...r....r....r..
-00002640: 0000 7288 0000 0072 3300 0000 2905 727b  ..r....r3...).r{
-00002650: 0000 0072 6e00 0000 7217 0000 0072 6600  ...rn...r....rf.
-00002660: 0000 7216 0000 0072 3400 0000 da0a 7472  ..r....r4.....tr
-00002670: 616a 6563 746f 7279 ff00 0000 7324 0000  ajectory....s$..
-00002680: 000a 2d12 0212 0112 010c 020a 0114 0116  ..-.............
-00002690: 0112 0212 0110 0204 0902 0102 0102 0102  ................
-000026a0: 0104 fc06 f77a 1b54 6162 756c 6172 4265  .....z.TabularBe
-000026b0: 6e63 686d 6172 6b2e 7472 616a 6563 746f  nchmark.trajecto
-000026c0: 7279 fa28 4354 6162 756c 6172 207c 204d  ry.(CTabular | M
-000026d0: 6170 7069 6e67 5b73 7472 2c20 416e 795d  apping[str, Any]
-000026e0: 207c 2073 7472 207c 2069 6e74 7211 0000   | str | intr...
-000026f0: 0063 0200 0000 0000 0000 0000 0000 0500  .c..............
-00002700: 0000 0600 0000 0300 0001 73e8 0000 0074  ..........s....t
-00002710: 0088 0074 0183 0272 0974 0288 0083 0189  ...t...r.t......
-00002720: 0074 0088 0074 0283 0272 137c 006a 0388  .t...t...r.|.j..
-00002730: 0019 0053 0074 0088 007c 006a 0483 0272  ...S.t...|.j...r
-00002740: 2f88 006a 057c 006a 0376 0172 2d74 0664  /..j.|.j.v.r-t.d
-00002750: 0188 006a 059b 0064 027c 006a 03a0 07a1  ...j...d.|.j....
-00002760: 009b 009d 0483 0182 0188 0053 0074 0088  ...........S.t..
-00002770: 0074 0883 0273 364a 0082 017c 006a 0988  .t...s6J...|.j..
-00002780: 0076 0072 4774 0288 007c 006a 0919 0083  .v.rGt...|.j....
-00002790: 017d 027c 006a 037c 0219 0053 0064 0388  .}.|.j.|...S.d..
-000027a0: 0076 0072 5488 0064 0319 007d 037c 006a  .v.rT..d...}.|.j
-000027b0: 037c 0319 0053 0074 0a7c 006a 03a0 0ba1  .|...S.t.|.j....
-000027c0: 0087 0066 0164 0464 0584 0864 0064 068d  ...f.d.d...d.d..
-000027d0: 037d 047c 0464 0075 0072 7274 0664 0788  .}.|.d.u.rrt.d..
-000027e0: 009b 0064 0874 0c88 0083 019b 009d 0483  ...d.t..........
-000027f0: 0182 017c 0453 0029 094e 7a07 436f 6e66  ...|.S.).Nz.Conf
-00002800: 6967 2072 4d00 0000 7237 0000 0063 0100  ig rM...r7...c..
-00002810: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00002820: 0000 1300 0001 7310 0000 007c 006a 0064  ......s....|.j.d
-00002830: 0164 028d 0188 006b 0253 0029 034e 4672  .d.....k.S.).NFr
-00002840: 7200 0000 2901 7283 0000 0029 01da 0163  r...).r....)...c
-00002850: a901 726e 0000 0072 3300 0000 7234 0000  ..rn...r3...r4..
-00002860: 00da 083c 6c61 6d62 6461 3e72 0100 0073  ...<lambda>r...s
-00002870: 0200 0000 1000 7a2f 5461 6275 6c61 7242  ......z/TabularB
-00002880: 656e 6368 6d61 726b 2e5f 6669 6e64 5f63  enchmark._find_c
-00002890: 6f6e 6669 672e 3c6c 6f63 616c 733e 2e3c  onfig.<locals>.<
-000028a0: 6c61 6d62 6461 3e29 02da 0470 7265 64da  lambda>)...pred.
-000028b0: 0764 6566 6175 6c74 7a1f 436f 756c 6420  .defaultz.Could 
-000028c0: 6e6f 7420 6669 6e64 2063 6f6e 6669 6720  not find config 
-000028d0: 6d61 7463 6869 6e67 207a 3d2e 2050 6c65  matching z=. Ple
-000028e0: 6173 6520 7061 7373 2074 6865 2060 436f  ase pass the `Co
-000028f0: 6e66 6967 6020 6f62 6a65 6374 206f 7220  nfig` object or 
-00002900: 7370 6563 6966 7920 7468 6520 6069 6460  specify the `id`
-00002910: 2069 6e20 7468 6520 290d da0a 6973 696e   in the )...isin
-00002920: 7374 616e 6365 da03 696e 7472 1d00 0000  stance..intr....
-00002930: 7261 0000 00da 0643 6f6e 6669 6772 3700  ra.....Configr7.
-00002940: 0000 724f 0000 0072 5200 0000 7207 0000  ..rO...rR...r...
-00002950: 0072 2000 0000 720c 0000 00da 0676 616c  .r ...r......val
-00002960: 7565 73da 0474 7970 6529 0572 6600 0000  ues..type).rf...
-00002970: 726e 0000 005a 0f5f 7265 616c 5f63 6f6e  rn...Z._real_con
-00002980: 6669 675f 6964 da03 5f69 64da 056d 6174  fig_id.._id..mat
-00002990: 6368 7233 0000 0072 9200 0000 7234 0000  chr3...r....r4..
-000029a0: 0072 8200 0000 4b01 0000 733a 0000 000a  .r....K...s:....
-000029b0: 0608 010a 030a 010c 030c 0102 0116 0104  ................
-000029c0: ff04 030e 030a 030e 010a 0108 0308 010a  ................
-000029d0: 0102 0508 010a 0102 0106 fd08 0502 0108  ................
-000029e0: 0106 0104 ff04 ff04 047a 1d54 6162 756c  .........z.Tabul
-000029f0: 6172 4265 6e63 686d 6172 6b2e 5f66 696e  arBenchmark._fin
-00002a00: 645f 636f 6e66 6967 fa11 4d61 7070 696e  d_config..Mappin
-00002a10: 675b 7374 722c 2041 6e79 5d72 1400 0000  g[str, Any]r....
-00002a20: fa13 4d61 7070 696e 675b 7374 722c 2066  ..Mapping[str, f
-00002a30: 6c6f 6174 5d63 0200 0000 0000 0000 0100  loat]c..........
-00002a40: 0000 0600 0000 0700 0000 4300 0001 7366  ..........C...sf
-00002a50: 0000 0074 007c 0183 017d 017c 01a0 0164  ...t.|...}.|...d
-00002a60: 01a1 017d 037c 006a 026a 037c 037c 0266  ...}.|.j.j.|.|.f
-00002a70: 0219 007d 047c 037c 045f 0474 007c 047c  ...}.|.|._.t.|.|
-00002a80: 006a 0519 0083 017d 057c 017c 056b 0372  .j.....}.|.|.k.r
-00002a90: 2c74 0664 027c 039b 0264 037c 019b 0264  ,t.d.|...d.|...d
-00002aa0: 047c 059b 029d 0683 0182 0174 007c 047c  .|.........t.|.|
-00002ab0: 006a 0719 0083 0153 0029 057a c253 7562  .j.....S.).z.Sub
-00002ac0: 6d69 7420 6120 7175 6572 7920 616e 6420  mit a query and 
-00002ad0: 6765 7420 6120 7265 7375 6c74 2e0a 0a20  get a result... 
-00002ae0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00002af0: 2020 2020 2020 2020 2063 6f6e 6669 673a           config:
-00002b00: 2054 6865 2071 7565 7279 2074 6f20 7573   The query to us
-00002b10: 650a 2020 2020 2020 2020 2020 2020 6174  e.            at
-00002b20: 3a20 5468 6520 6669 6465 6c69 7479 2061  : The fidelity a
-00002b30: 7420 7768 6963 6820 746f 2071 7565 7279  t which to query
-00002b40: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00002b50: 733a 0a20 2020 2020 2020 2020 2020 2054  s:.            T
-00002b60: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
-00002b70: 2071 7565 7279 0a20 2020 2020 2020 2072   query.        r
-00002b80: 3700 0000 fa42 436f 6e66 6967 2071 7565  7....BConfig que
-00002b90: 7269 6564 2077 6974 6820 6973 206e 6f74  ried with is not
-00002ba0: 2065 7175 616c 2074 6f20 7468 6520 6f6e   equal to the on
-00002bb0: 6520 696e 2074 6865 2074 6162 6c65 2077  e in the table w
-00002bc0: 6974 6820 5f69 643d fa19 2e0a 636f 6e66  ith _id=....conf
-00002bd0: 6967 2070 726f 7669 6465 6420 636f 6e66  ig provided conf
-00002be0: 6967 3d7a 190a 636f 6e66 6967 2069 6e20  ig=z..config in 
-00002bf0: 7461 626c 6520 5f63 6f6e 6669 673d 2908  table _config=).
-00002c00: da04 6469 6374 da03 706f 7072 1e00 0000  ..dict..popr....
-00002c10: da03 6c6f 6372 1c00 0000 7240 0000 0072  ..locr....r@...r
-00002c20: 4f00 0000 7262 0000 0029 0672 6600 0000  O...rb...).rf...
-00002c30: 726e 0000 0072 6d00 0000 729b 0000 0072  rn...rm...r....r
-00002c40: 3f00 0000 7287 0000 0072 3300 0000 7233  ?...r....r3...r3
-00002c50: 0000 0072 3400 0000 7285 0000 007c 0100  ...r4...r....|..
-00002c60: 0073 1c00 0000 0810 0a01 1001 0602 0e01  .s..............
-00002c70: 0801 0201 0801 0201 04ff 0202 04fe 04ff  ................
-00002c80: 0e06 7a24 5461 6275 6c61 7242 656e 6368  ..z$TabularBench
-00002c90: 6d61 726b 2e5f 6f62 6a65 6374 6976 655f  mark._objective_
-00002ca0: 6675 6e63 7469 6f6e fa27 4974 6572 6162  function.'Iterab
-00002cb0: 6c65 5b74 7570 6c65 5b46 2c20 4d61 7070  le[tuple[F, Mapp
-00002cc0: 696e 675b 7374 722c 2066 6c6f 6174 5d5d  ing[str, float]]
-00002cd0: 5d63 0200 0000 0000 0000 0300 0000 0800  ]c..............
-00002ce0: 0000 0700 0000 0300 0001 7378 0000 0074  ..........sx...t
-00002cf0: 007c 0183 017d 017c 01a0 0164 01a1 017d  .|...}.|...d...}
-00002d00: 0588 006a 026a 037c 057c 0266 027c 057c  ...j.j.|.|.f.|.|
-00002d10: 0366 027c 0485 0319 007d 0674 007c 066a  .f.|.....}.t.|.j
-00002d20: 0464 0219 0088 006a 0519 0083 017d 077c  .d.....j.....}.|
-00002d30: 017c 076b 0372 3174 0664 037c 059b 0264  .|.k.r1t.d.|...d
-00002d40: 047c 019b 0264 057c 079b 029d 0683 0182  .|...d.|........
-00002d50: 0187 0066 0164 0664 0784 087c 06a0 07a1  ...f.d.d...|....
-00002d60: 0044 0083 0153 0029 084e 7237 0000 0072  .D...S.).Nr7...r
-00002d70: 0100 0000 729f 0000 0072 a000 0000 7a1e  ....r....r....z.
-00002d80: 0a63 6f6e 6669 6720 696e 2074 6162 6c65  .config in table
-00002d90: 2066 6972 7374 5f63 6f6e 6669 673d 6301   first_config=c.
-00002da0: 0000 0000 0000 0000 0000 0004 0000 0006  ................
-00002db0: 0000 0013 0000 0173 2600 0000 6700 7c00  .......s&...g.|.
-00002dc0: 5d0f 5c02 5c02 7d01 7d02 7d03 7c02 7400  ].\.\.}.}.}.|.t.
-00002dd0: 7c03 8800 6a01 1900 8301 6602 9102 7102  |...j.....f...q.
-00002de0: 5300 7233 0000 0029 0272 a100 0000 7262  S.r3...).r....rb
-00002df0: 0000 0029 0472 3000 0000 da01 5f72 7f00  ...).r0....._r..
-00002e00: 0000 723f 0000 00a9 0172 6600 0000 7233  ..r?.....rf...r3
-00002e10: 0000 0072 3400 0000 728d 0000 00b0 0100  ...r4...r.......
-00002e20: 0073 0800 0000 0600 0a02 10ff 06ff 7a30  .s............z0
-00002e30: 5461 6275 6c61 7242 656e 6368 6d61 726b  TabularBenchmark
-00002e40: 2e5f 7472 616a 6563 746f 7279 2e3c 6c6f  ._trajectory.<lo
-00002e50: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00002e60: 2908 72a1 0000 0072 a200 0000 721e 0000  ).r....r....r...
-00002e70: 0072 a300 0000 725b 0000 0072 4000 0000  .r....r[...r@...
-00002e80: 724f 0000 0072 6000 0000 2908 7266 0000  rO...r`...).rf..
-00002e90: 0072 6e00 0000 728a 0000 0072 8b00 0000  .rn...r....r....
-00002ea0: 726a 0000 0072 9b00 0000 da04 726f 7773  rj...r......rows
-00002eb0: 5a0c 6669 7273 745f 636f 6e66 6967 7233  Z.first_configr3
-00002ec0: 0000 0072 a600 0000 7234 0000 0072 8e00  ...r....r4...r..
-00002ed0: 0000 9b01 0000 731e 0000 0008 090a 011a  ......s.........
-00002ee0: 0114 0108 0202 0108 0102 0104 ff02 0204  ................
-00002ef0: fe04 ff0a 0606 0206 fe7a 1c54 6162 756c  .........z.Tabul
-00002f00: 6172 4265 6e63 686d 6172 6b2e 5f74 7261  arBenchmark._tra
-00002f10: 6a65 6374 6f72 792e 7242 0000 00da 016e  jectory.rB.....n
-00002f20: da04 4e6f 6e65 fa22 696e 7420 7c20 6e70  ..None."int | np
-00002f30: 2e72 616e 646f 6d2e 5261 6e64 6f6d 5374  .random.RandomSt
-00002f40: 6174 6520 7c20 4e6f 6e65 6302 0000 0000  ate | Nonec.....
-00002f50: 0000 0001 0000 0003 0000 0001 0000 0043  ...............C
-00002f60: 0000 01f3 0400 0000 6400 5300 722c 0000  ........d.S.r,..
-00002f70: 0072 3300 0000 a903 7266 0000 0072 a800  .r3.....rf...r..
-00002f80: 0000 7219 0000 0072 3300 0000 7233 0000  ..r....r3...r3..
-00002f90: 0072 3400 0000 da06 7361 6d70 6c65 b601  .r4.....sample..
-00002fa0: 0000 f302 0000 0004 077a 1754 6162 756c  .........z.Tabul
-00002fb0: 6172 4265 6e63 686d 6172 6b2e 7361 6d70  arBenchmark.samp
-00002fc0: 6c65 7297 0000 00fa 0e6c 6973 745b 4354  ler......list[CT
-00002fd0: 6162 756c 6172 5d63 0200 0000 0000 0000  abular]c........
-00002fe0: 0100 0000 0300 0000 0100 0000 4300 0001  ............C...
-00002ff0: 72ab 0000 0072 2c00 0000 7233 0000 0072  r....r,...r3...r
-00003000: ac00 0000 7233 0000 0072 3300 0000 7234  ....r3...r3...r4
-00003010: 0000 0072 ad00 0000 c001 0000 72ae 0000  ...r........r...
-00003020: 00fa 1943 5461 6275 6c61 7220 7c20 6c69  ...CTabular | li
-00003030: 7374 5b43 5461 6275 6c61 725d 6302 0000  st[CTabular]c...
-00003040: 0000 0000 0001 0000 0009 0000 0006 0000  ................
-00003050: 0003 0000 0173 ac00 0000 7400 7c02 7401  .....s....t.|.t.
-00003060: 6a02 6a03 8302 720e 7c02 a004 6401 6402  j.j...r.|...d.d.
-00003070: a102 7d03 6e02 7c02 7d03 7401 6a02 6a05  ..}.n.|.}.t.j.j.
-00003080: 7c03 6403 8d01 7d04 7406 7c00 6a07 a008  |.d...}.t.|.j...
-00003090: a100 8301 8900 7409 8800 8301 7d05 7c01  ......t.....}.|.
-000030a0: 6404 7501 7228 7c01 6e01 6405 7d06 7c06  d.u.r(|.n.d.}.|.
-000030b0: 7c05 6b04 7239 740a 6406 7c06 9b00 6407  |.k.r9t.d.|...d.
-000030c0: 7c05 9b00 6408 9d05 8301 8201 7c04 6a0b  |...d.......|.j.
-000030d0: 7c05 7c06 6409 640a 8d03 7d07 7c01 6404  |.|.d.d...}.|.d.
-000030e0: 7500 724d 7c07 6401 1900 7d08 8800 7c08  u.rM|.d...}...|.
-000030f0: 1900 5300 8700 6601 640b 640c 8408 7c07  ..S...f.d.d...|.
-00003100: 4400 8301 5300 290d 619b 0100 0053 616d  D...S.).a....Sam
-00003110: 706c 6520 6120 7261 6e64 6f6d 2070 6f73  ple a random pos
-00003120: 7369 626c 6520 636f 6e66 6967 2e0a 0a20  sible config... 
-00003130: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00003140: 2020 2020 2020 2020 206e 3a20 486f 7720           n: How 
-00003150: 6d61 6e79 2073 616d 706c 6573 2074 6f20  many samples to 
-00003160: 7461 6b65 2c20 4e6f 6e65 206d 6561 6e73  take, None means
-00003170: 206a 7375 7420 6120 7369 6e67 6c65 206f   jsut a single o
-00003180: 6e65 2c20 6e6f 7420 696e 2061 206c 6973  ne, not in a lis
-00003190: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
-000031a0: 6564 3a20 5468 6520 7365 6564 2074 6f20  ed: The seed to 
-000031b0: 7573 6520 666f 7220 7468 6520 7361 6d70  use for the samp
-000031c0: 6c69 6e67 2e0a 0a20 2020 2020 2020 2020  ling...         
-000031d0: 2020 2020 2020 2021 2121 206e 6f74 6520         !!! note 
-000031e0: 2253 6565 6469 6e67 220a 0a20 2020 2020  "Seeding"..     
-000031f0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-00003200: 6869 7320 6973 2064 6966 6665 7265 6e74  his is different
-00003210: 2074 6861 6e20 616e 7920 7365 6564 2070   than any seed p
-00003220: 6173 7365 6420 746f 2074 6865 2063 6f6e  assed to the con
-00003230: 7374 7275 6374 696f 6e0a 2020 2020 2020  struction.      
-00003240: 2020 2020 2020 2020 2020 2020 2020 6f66                of
-00003250: 2074 6865 2062 656e 6368 6d61 726b 2e0a   the benchmark..
-00003260: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00003270: 3a0a 2020 2020 2020 2020 2020 2020 4765  :.            Ge
-00003280: 7420 6261 636b 2061 2070 6f73 7369 626c  t back a possibl
-00003290: 6520 436f 6e66 6967 2074 6f20 7573 650a  e Config to use.
-000032a0: 2020 2020 2020 2020 7201 0000 0069 ffff          r....i..
-000032b0: ff7f 7242 0000 004e 7239 0000 007a 0d43  ..rB...Nr9...z.C
-000032c0: 616e 2774 2073 616d 706c 6520 7a0e 2063  an't sample z. c
-000032d0: 6f6e 6669 6773 2066 726f 6d20 7a08 2063  onfigs from z. c
-000032e0: 6f6e 6669 6773 4629 02da 0473 697a 65da  onfigsF)...size.
-000032f0: 0772 6570 6c61 6365 6301 0000 0000 0000  .replacec.......
-00003300: 0000 0000 0002 0000 0004 0000 0013 0000  ................
-00003310: 0173 1400 0000 6700 7c00 5d06 7d01 8800  .s....g.|.].}...
-00003320: 7c01 1900 9102 7102 5300 7233 0000 0072  |.....q.S.r3...r
-00003330: 3300 0000 2902 7230 0000 00da 0169 a901  3...).r0.....i..
-00003340: 5a0c 636f 6e66 6967 5f69 7465 6d73 7233  Z.config_itemsr3
-00003350: 0000 0072 3400 0000 728d 0000 00f4 0100  ...r4...r.......
-00003360: 0073 0200 0000 1400 7a2b 5461 6275 6c61  .s......z+Tabula
-00003370: 7242 656e 6368 6d61 726b 2e73 616d 706c  rBenchmark.sampl
-00003380: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
-00003390: 636f 6d70 3e29 0c72 9600 0000 da02 6e70  comp>).r......np
-000033a0: da06 7261 6e64 6f6d da0b 5261 6e64 6f6d  ..random..Random
-000033b0: 5374 6174 65da 0f72 616e 646f 6d5f 696e  State..random_in
-000033c0: 7465 6765 7273 da0b 6465 6661 756c 745f  tegers..default_
-000033d0: 726e 6772 5000 0000 7261 0000 0072 9900  rngrP...ra...r..
-000033e0: 0000 da03 6c65 6e72 4f00 0000 da06 6368  ....lenrO.....ch
-000033f0: 6f69 6365 2909 7266 0000 0072 a800 0000  oice).rf...r....
-00003400: 7219 0000 005a 055f 7365 6564 da03 726e  r....Z._seed..rn
-00003410: 675a 096e 5f63 6f6e 6669 6773 5a0d 7361  gZ.n_configsZ.sa
-00003420: 6d70 6c65 5f61 6d6f 756e 74da 0769 6e64  mple_amount..ind
-00003430: 6963 6573 da0b 6669 7273 745f 696e 6465  ices..first_inde
-00003440: 7872 3300 0000 72b4 0000 0072 3400 0000  xr3...r....r4...
-00003450: 72ad 0000 00c9 0100 0073 2000 0000 0e16  r........s .....
-00003460: 0e01 0402 0e02 0e02 0801 1001 0802 0201  ................
-00003470: 1001 04ff 1004 0801 0801 0801 1202 2918  ..............).
-00003480: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00003490: 1f00 0000 7220 0000 0072 1d00 0000 7221  ....r ...r....r!
-000034a0: 0000 0072 1d00 0000 7222 0000 0072 2300  ...r....r"...r#.
-000034b0: 0000 7224 0000 0072 2500 0000 7216 0000  ..r$...r%...r...
-000034c0: 0072 2600 0000 7217 0000 0072 2600 0000  .r&...r....r&...
-000034d0: 7218 0000 0072 2700 0000 7219 0000 0072  r....r'...r....r
-000034e0: 2800 0000 721a 0000 0072 2900 0000 721b  (...r....r)...r.
-000034f0: 0000 0072 2a00 0000 290a 726e 0000 0072  ...r*...).rn...r
-00003500: 6f00 0000 726d 0000 0072 7000 0000 7216  o...rm...rp...r.
-00003510: 0000 0072 2600 0000 7217 0000 0072 2600  ...r&...r....r&.
-00003520: 0000 7271 0000 0072 1300 0000 290e 726e  ..rq...r....).rn
-00003530: 0000 0072 6f00 0000 728a 0000 0072 7000  ...ro...r....rp.
-00003540: 0000 728b 0000 0072 7000 0000 726a 0000  ..r....rp...rj..
-00003550: 0072 7000 0000 7216 0000 0072 2600 0000  .rp...r....r&...
-00003560: 7217 0000 0072 2600 0000 7271 0000 0072  r....r&...rq...r
-00003570: 8c00 0000 2904 726e 0000 0072 9000 0000  ....).rn...r....
-00003580: 7271 0000 0072 1100 0000 2906 726e 0000  rq...r....).rn..
-00003590: 0072 9d00 0000 726d 0000 0072 1400 0000  .r....rm...r....
-000035a0: 7271 0000 0072 9e00 0000 290a 726e 0000  rq...r....).rn..
-000035b0: 0072 9d00 0000 728a 0000 0072 1400 0000  .r....r....r....
-000035c0: 728b 0000 0072 1400 0000 726a 0000 0072  r....r....rj...r
-000035d0: 1400 0000 7271 0000 0072 a400 0000 722c  ....rq...r....r,
-000035e0: 0000 0029 0672 a800 0000 72a9 0000 0072  ...).r....r....r
-000035f0: 1900 0000 72aa 0000 0072 7100 0000 7211  ....r....rq...r.
-00003600: 0000 0029 0672 a800 0000 7297 0000 0072  ...).r....r....r
-00003610: 1900 0000 72aa 0000 0072 7100 0000 72af  ....r....rq...r.
-00003620: 0000 0029 0672 a800 0000 7228 0000 0072  ...).r....r(...r
-00003630: 1900 0000 72aa 0000 0072 7100 0000 72b0  ....r....rq...r.
-00003640: 0000 0029 0dda 085f 5f6e 616d 655f 5fda  ...)...__name__.
-00003650: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00003660: 7561 6c6e 616d 655f 5f72 6400 0000 7289  ualname__rd...r.
-00003670: 0000 0072 0a00 0000 728f 0000 0072 8200  ...r....r....r..
-00003680: 0000 7285 0000 0072 8e00 0000 7209 0000  ..r....r....r...
-00003690: 0072 ad00 0000 da0d 5f5f 636c 6173 7363  .r......__classc
-000036a0: 656c 6c5f 5f72 3300 0000 7233 0000 0072  ell__r3...r3...r
-000036b0: 6b00 0000 7234 0000 0072 1500 0000 1e00  k...r4...r......
-000036c0: 0000 734c 0000 0008 0002 0a02 0102 0102  ..sL............
-000036d0: 0102 0102 0112 f200 7f02 2702 0102 010e  ..........'.....
-000036e0: fa02 3e02 0502 0102 0102 0102 0110 f80a  ..>.............
-000036f0: 4b02 310c 0102 1e0c 0102 1a02 0302 fe02  K.1.............
-00003700: 0410 fc02 0902 0510 fc02 0802 0302 fe02  ................
-00003710: 0418 fc72 1500 0000 da08 5f5f 6d61 696e  ...r......__main
-00003720: 5f5f da04 6461 7461 7a0f 6c63 6265 6e63  __..dataz.lcbenc
-00003730: 682d 7461 6275 6c61 727a 0d61 6475 6c74  h-tabularz.adult
-00003740: 2e70 6172 7175 6574 2902 da14 4c43 4265  .parquet)...LCBe
-00003750: 6e63 6854 6162 756c 6172 436f 6e66 6967  nchTabularConfig
-00003760: da14 4c43 4265 6e63 6854 6162 756c 6172  ..LCBenchTabular
-00003770: 5265 7375 6c74 5a03 746f 7972 3700 0000  ResultZ.toyr7...
-00003780: da05 6570 6f63 6829 0472 2000 0000 7221  ..epoch).r ...r!
-00003790: 0000 0072 2200 0000 7224 0000 0072 3900  ...r"...r$...r9.
-000037a0: 0000 7242 0000 0072 7d00 0000 e92a 0000  ..rB...r}....*..
-000037b0: 00e9 0a00 0000 2902 728a 0000 0072 8b00  ......).r....r..
-000037c0: 0000 293c da0a 5f5f 6675 7475 7265 5f5f  ..)<..__future__
-000037d0: 7202 0000 00da 0770 6174 686c 6962 7203  r......pathlibr.
-000037e0: 0000 00da 0674 7970 696e 6772 0400 0000  .....typingr....
-000037f0: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
-00003800: 0800 0000 7209 0000 00da 1174 7970 696e  ....r......typin
-00003810: 675f 6578 7465 6e73 696f 6e73 720a 0000  g_extensionsr...
-00003820: 00da 056e 756d 7079 72b5 0000 00da 0670  ...numpyr......p
-00003830: 616e 6461 73da 0270 64da 0b43 6f6e 6669  andas..pd..Confi
-00003840: 6753 7061 6365 720b 0000 00da 0e6d 6f72  gSpacer......mor
-00003850: 655f 6974 6572 746f 6f6c 7372 0c00 0000  e_itertoolsr....
-00003860: da12 6d66 7062 656e 6368 2e62 656e 6368  ..mfpbench.bench
-00003870: 6d61 726b 720d 0000 00da 0f6d 6670 6265  markr......mfpbe
-00003880: 6e63 682e 636f 6e66 6967 720e 0000 00da  nch.configr.....
-00003890: 0f6d 6670 6265 6e63 682e 7265 7375 6c74  .mfpbench.result
-000038a0: 720f 0000 00da 0f6d 6670 6265 6e63 682e  r......mfpbench.
-000038b0: 6d65 7472 6963 7210 0000 0072 1100 0000  metricr....r....
-000038c0: 7213 0000 0072 9700 0000 7246 0000 0072  r....r....rF...r
-000038d0: 1400 0000 7215 0000 0072 bf00 0000 da08  ....r....r......
-000038e0: 5f5f 6669 6c65 5f5f da06 7061 7265 6e74  __file__..parent
-000038f0: da04 4845 5245 da04 7061 7468 da0c 7265  ..HERE..path..re
-00003900: 6164 5f70 6172 7175 6574 721e 0000 00da  ad_parquetr.....
-00003910: 186d 6670 6265 6e63 682e 6c63 6265 6e63  .mfpbench.lcbenc
-00003920: 685f 7461 6275 6c61 7272 c500 0000 72c6  h_tabularr....r.
-00003930: 0000 00da 0962 656e 6368 6d61 726b 7261  .....benchmarkra
-00003940: 0000 005a 0b61 6c6c 5f63 6f6e 6669 6773  ...Z.all_configs
-00003950: 7250 0000 0072 5200 0000 5a0a 636f 6e66  rP...rR...Z.conf
-00003960: 6967 5f69 6473 7299 0000 0072 ad00 0000  ig_idsr....r....
-00003970: 726e 0000 0072 3700 0000 723e 0000 0072  rn...r7...r>...r
-00003980: 8900 0000 7280 0000 005a 0c61 7267 6d69  ....r....Z.argmi
-00003990: 6e5f 7363 6f72 6572 8f00 0000 7233 0000  n_scorer....r3..
-000039a0: 0072 3300 0000 7233 0000 0072 3400 0000  .r3...r3...r4...
-000039b0: da08 3c6d 6f64 756c 653e 0100 0000 7354  ..<module>....sT
-000039c0: 0000 000c 000c 0220 010c 0108 0208 010c  ....... ........
-000039d0: 010c 010c 020c 010c 0104 020c 010c 040c  ................
-000039e0: 030c 031a 0300 7f00 7f00 7f08 5c0a 0114  ............\...
-000039f0: 010a 0110 0102 0202 0102 0102 0102 0102  ................
-00003a00: 0102 0106 fa06 090c 010c 010c 0206 010e  ................
-00003a10: 020e 0114 0204 e7                        .......
+00000040: 5a02 6400 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
+00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
+00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
+00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f  m.Z.m.Z.m.Z.m.Z.
+00000080: 6d10 5a10 6d11 5a11 0100 6400 6402 6c12  m.Z.m.Z...d.d.l.
+00000090: 5a13 6400 6406 6c14 6d15 5a15 0100 6400  Z.d.d.l.m.Z...d.
+000000a0: 6407 6c16 6d17 5a17 0100 6400 6408 6c18  d.l.m.Z...d.d.l.
+000000b0: 6d19 5a19 0100 6509 7252 6400 6409 6c1a  m.Z...e.rRd.d.l.
+000000c0: 6d1b 5a1b 0100 6400 640a 6c1c 6d1d 5a1d  m.Z...d.d.l.m.Z.
+000000d0: 0100 6507 651e 8301 6a1f 6a1f 5a20 6520  ..e.e...j.j.Z e 
+000000e0: 640b 1b00 5a21 6510 640c 6515 640d 8d02  d...Z!e.d.e.d...
+000000f0: 5a22 6510 640e 6517 640d 8d02 5a23 6510  Z"e.d.e.d...Z#e.
+00000100: 640f 6524 6525 8303 5a26 4700 6410 6411  d.e$e%..Z&G.d.d.
+00000110: 8400 6411 650c 6522 6523 6526 6603 1900  ..d.e.e"e#e&f...
+00000120: 6504 8304 5a27 6402 5300 2912 e900 0000  e...Z'd.S.).....
+00000130: 0029 01da 0b61 6e6e 6f74 6174 696f 6e73  .)...annotations
+00000140: 4e29 02da 0341 4243 da0e 6162 7374 7261  N)...ABC..abstra
+00000150: 6374 6d65 7468 6f64 2901 da04 5061 7468  ctmethod)...Path
+00000160: 2909 da0d 5459 5045 5f43 4845 434b 494e  )...TYPE_CHECKIN
+00000170: 47da 0341 6e79 da08 436c 6173 7356 6172  G..Any..ClassVar
+00000180: da07 4765 6e65 7269 63da 0849 7465 7261  ..Generic..Itera
+00000190: 626c 65da 0849 7465 7261 746f 72da 074d  ble..Iterator..M
+000001a0: 6170 7069 6e67 da07 5479 7065 5661 72da  apping..TypeVar.
+000001b0: 086f 7665 726c 6f61 6429 01da 0643 6f6e  .overload)...Con
+000001c0: 6669 6729 01da 0652 6573 756c 7429 01da  fig)...Result)..
+000001d0: 0b52 6573 756c 7446 7261 6d65 2901 da12  .ResultFrame)...
+000001e0: 436f 6e66 6967 7572 6174 696f 6e53 7061  ConfigurationSpa
+000001f0: 6365 2901 da06 4d65 7472 6963 5a06 7072  ce)...MetricZ.pr
+00000200: 696f 7273 da01 4329 015a 0562 6f75 6e64  iors..C).Z.bound
+00000210: da01 52da 0146 6300 0000 0000 0000 0000  ..R..Fc.........
+00000220: 0000 0000 0000 0007 0000 0040 0000 0173  ...........@...s
+00000230: 4601 0000 6500 5a01 6400 5a02 5500 6401  F...e.Z.d.Z.U.d.
+00000240: 5a03 6504 5a05 6402 6506 6403 3c00 0900  Z.e.Z.d.e.d.<...
+00000250: 6404 5a07 6405 6506 6406 3c00 0900 6404  d.Z.d.e.d.<...d.
+00000260: 5a08 6405 6506 6407 3c00 0900 6408 6404  Z.d.e.d.<...d.d.
+00000270: 6404 6404 6404 6404 6409 9c06 645b 6420  d.d.d.d.d...d[d 
+00000280: 6421 8406 5a09 650a 645c 6424 6425 8404  d!..Z.e.d\d$d%..
+00000290: 8301 5a0b 650a 645d 6427 6428 8404 8301  ..Z.e.d]d'd(....
+000002a0: 5a0c 650a 645d 6429 642a 8404 8301 5a0d  Z.e.d]d)d*....Z.
+000002b0: 650a 645d 642b 642c 8404 8301 5a0e 0904  e.d]d+d,....Z...
+000002c0: 645e 645f 6430 6431 8405 5a0f 0904 0904  d^d_d0d1..Z.....
+000002d0: 0904 6460 6461 6437 6438 8405 5a10 6462  ..d`dad7d8..Z.db
+000002e0: 643a 643b 8404 5a11 6404 6404 6404 643c  d:d;..Z.d.d.d.d<
+000002f0: 9c03 6463 6441 6442 8406 5a12 6404 6404  ..dcdAdB..Z.d.d.
+00000300: 6404 6404 6404 6443 9c05 6464 6445 6446  d.d.d.dC..dddEdF
+00000310: 8406 5a13 6514 6465 6449 644a 8404 8301  ..Z.e.dedIdJ....
+00000320: 5a15 6466 644c 644d 8404 5a16 6517 0904  Z.dfdLdM..Z.e...
+00000330: 645e 6404 644e 9c01 6467 6451 6452 8407  d^d.dN..dgdQdR..
+00000340: 8301 5a18 6517 6404 644e 9c01 6468 6455  ..Z.e.d.dN..dhdU
+00000350: 6452 8406 8301 5a18 0904 645e 6404 644e  dR....Z...d^d.dN
+00000360: 9c01 6469 6457 6452 8407 5a18 646a 6459  ..didWdR..Z.djdY
+00000370: 645a 8404 5a19 6404 5300 296b da09 4265  dZ..Z.d.S.)k..Be
+00000380: 6e63 686d 6172 6b7a 1b42 6173 6520 636c  nchmarkz.Base cl
+00000390: 6173 7320 666f 7220 6120 4265 6e63 686d  ass for a Benchm
+000003a0: 6172 6b2e 7a0e 436c 6173 7356 6172 5b50  ark.z.ClassVar[P
+000003b0: 6174 685d da12 5f64 6566 6175 6c74 5f70  ath].._default_p
+000003c0: 7269 6f72 5f64 6972 4e7a 2243 6c61 7373  rior_dirNz"Class
+000003d0: 5661 725b 4d61 7070 696e 675b 7374 722c  Var[Mapping[str,
+000003e0: 2073 7472 5d20 7c20 4e6f 6e65 5dda 0f5f   str] | None].._
+000003f0: 7265 7375 6c74 5f72 656e 616d 6573 da0f  result_renames..
+00000400: 5f63 6f6e 6669 675f 7265 6e61 6d65 7346  _config_renamesF
+00000410: 2906 da10 6861 735f 636f 6e64 6974 696f  )...has_conditio
+00000420: 6e61 6c73 da04 7365 6564 da05 7072 696f  nals..seed..prio
+00000430: 72da 0d70 6572 7475 7262 5f70 7269 6f72  r..perturb_prior
+00000440: da0c 7661 6c75 655f 6d65 7472 6963 da0b  ..value_metric..
+00000450: 636f 7374 5f6d 6574 7269 63da 046e 616d  cost_metric..nam
+00000460: 65da 0373 7472 da05 7370 6163 6572 1200  e..str..spacer..
+00000470: 0000 da0b 636f 6e66 6967 5f74 7970 65fa  ....config_type.
+00000480: 0774 7970 655b 435d da0b 7265 7375 6c74  .type[C]..result
+00000490: 5f74 7970 65fa 0774 7970 655b 525d da0e  _type..type[R]..
+000004a0: 6669 6465 6c69 7479 5f72 616e 6765 fa0e  fidelity_range..
+000004b0: 7475 706c 655b 462c 2046 2c20 465d da0d  tuple[F, F, F]..
+000004c0: 6669 6465 6c69 7479 5f6e 616d 6572 1b00  fidelity_namer..
+000004d0: 0000 da04 626f 6f6c 721c 0000 00fa 0a69  ....boolr......i
+000004e0: 6e74 207c 204e 6f6e 6572 1d00 0000 fa29  nt | Noner.....)
+000004f0: 7374 7220 7c20 5061 7468 207c 2043 207c  str | Path | C |
+00000500: 204d 6170 7069 6e67 5b73 7472 2c20 416e   Mapping[str, An
+00000510: 795d 207c 204e 6f6e 6572 1e00 0000 fa0c  y] | Noner......
+00000520: 666c 6f61 7420 7c20 4e6f 6e65 721f 0000  float | Noner...
+00000530: 00fa 0a73 7472 207c 204e 6f6e 6572 2000  ...str | Noner .
+00000540: 0000 6307 0000 0000 0000 0006 0000 000d  ..c.............
+00000550: 0000 0006 0000 0043 0000 0173 4401 0000  .......C...sD...
+00000560: 7c0b 6401 7500 7207 7c04 6a00 7d0b 7c0c  |.d.u.r.|.j.}.|.
+00000570: 6401 7500 720e 7c04 6a01 7d0c 7c01 7c00  d.u.r.|.j.}.|.|.
+00000580: 5f02 7c08 7c00 5f03 7c02 7c00 5f04 7c0b  _.|.|._.|.|._.|.
+00000590: 7c00 5f05 7c0c 7c00 5f06 7c05 7c00 5f07  |._.|.|._.|.|._.
+000005a0: 7c06 7c00 5f08 7c07 7c00 5f09 7c03 7c00  |.|._.|.|._.|.|.
+000005b0: 5f0a 7c04 7c00 5f0b 6402 6403 8400 7c00  _.|.|._.d.d...|.
+000005c0: 6a0b 6a0c a00d a100 4400 8301 7c00 5f0e  j.j.....D...|._.
+000005d0: 7c0b 6401 7500 724b 740f 7c00 6a0b 6404  |.d.u.rKt.|.j.d.
+000005e0: 6401 8303 6401 7501 7347 4a00 8201 7c00  d...d.u.sGJ...|.
+000005f0: 6a0b 6a05 7d0b 7c09 7c00 5f10 7c0a 6401  j.j.}.|.|._.|.d.
+00000600: 7501 7264 6405 7c0a 0400 0300 6b01 725f  u.rdd.|.....k.r_
+00000610: 6406 6b01 7364 7411 6407 8301 8201 0100  d.k.sdt.d.......
+00000620: 7411 6407 8301 8201 7c0a 7c00 5f12 6401  t.d.....|.|._.d.
+00000630: 7c00 5f13 7c09 6401 7501 7278 7c00 6a14  |._.|.d.u.rx|.j.
+00000640: 7c09 7c00 6a02 6408 8d02 7c00 5f13 6e03  |.|.j.d...|._.n.
+00000650: 6401 7c00 5f13 7c00 6a13 6401 7501 7293  d.|._.|.j.d.u.r.
+00000660: 7c00 6a12 6401 7501 7293 7c00 6a13 6a15  |.j.d.u.r.|.j.j.
+00000670: 7c02 7c00 6a03 7c00 6a12 7c00 6a12 6409  |.|.j.|.j.|.j.d.
+00000680: 8d04 7c00 5f13 7c00 6a13 6401 7501 72a0  ..|._.|.j.d.u.r.
+00000690: 7c00 6a13 a016 7c02 a101 0100 6401 5300  |.j...|.....d.S.
+000006a0: 6401 5300 290a 61db 0500 0049 6e69 7469  d.S.).a....Initi
+000006b0: 616c 697a 6520 7468 6520 6265 6e63 686d  alize the benchm
+000006c0: 6172 6b2e 0a0a 2020 2020 2020 2020 4172  ark...        Ar
+000006d0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+000006e0: 6e61 6d65 3a20 5468 6520 6e61 6d65 206f  name: The name o
+000006f0: 6620 7468 6973 2062 656e 6368 6d61 726b  f this benchmark
+00000700: 0a20 2020 2020 2020 2020 2020 2073 7061  .            spa
+00000710: 6365 3a20 5468 6520 636f 6e66 6967 7572  ce: The configur
+00000720: 6174 696f 6e20 7370 6163 6520 746f 2075  ation space to u
+00000730: 7365 2066 6f72 2074 6865 2062 656e 6368  se for the bench
+00000740: 6d61 726b 2e0a 2020 2020 2020 2020 2020  mark..          
+00000750: 2020 636f 6e66 6967 5f74 7970 653a 2054    config_type: T
+00000760: 6865 2074 7970 6520 6f66 2063 6f6e 6669  he type of confi
+00000770: 6720 746f 2075 7365 2066 6f72 2074 6865  g to use for the
+00000780: 2062 656e 6368 6d61 726b 2e0a 2020 2020   benchmark..    
+00000790: 2020 2020 2020 2020 7265 7375 6c74 5f74          result_t
+000007a0: 7970 653a 2054 6865 2074 7970 6520 6f66  ype: The type of
+000007b0: 2072 6573 756c 7420 746f 2075 7365 2066   result to use f
+000007c0: 6f72 2074 6865 2062 656e 6368 6d61 726b  or the benchmark
+000007d0: 2e0a 2020 2020 2020 2020 2020 2020 6669  ..            fi
+000007e0: 6465 6c69 7479 5f6e 616d 653a 2054 6865  delity_name: The
+000007f0: 206e 616d 6520 6f66 2074 6865 2066 6964   name of the fid
+00000800: 656c 6974 7920 746f 2075 7365 2066 6f72  elity to use for
+00000810: 2074 6865 2062 656e 6368 6d61 726b 2e0a   the benchmark..
+00000820: 2020 2020 2020 2020 2020 2020 6669 6465              fide
+00000830: 6c69 7479 5f72 616e 6765 3a20 5468 6520  lity_range: The 
+00000840: 7261 6e67 6520 6f66 2066 6964 656c 6974  range of fidelit
+00000850: 6965 7320 746f 2075 7365 2066 6f72 2074  ies to use for t
+00000860: 6865 2062 656e 6368 6d61 726b 2e0a 2020  he benchmark..  
+00000870: 2020 2020 2020 2020 2020 6861 735f 636f            has_co
+00000880: 6e64 6974 696f 6e61 6c73 3a20 5768 6574  nditionals: Whet
+00000890: 6865 7220 7468 6973 2062 656e 6368 6d61  her this benchma
+000008a0: 726b 2068 6173 2063 6f6e 6469 7469 6f6e  rk has condition
+000008b0: 616c 7320 696e 2069 7420 6f72 206e 6f74  als in it or not
+000008c0: 2e0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+000008d0: 6564 3a20 5468 6520 7365 6564 2074 6f20  ed: The seed to 
+000008e0: 7573 652e 0a20 2020 2020 2020 2020 2020  use..           
+000008f0: 2070 7269 6f72 3a20 5468 6520 7072 696f   prior: The prio
+00000900: 7220 746f 2075 7365 2066 6f72 2074 6865  r to use for the
+00000910: 2062 656e 6368 6d61 726b 2e20 4966 204e   benchmark. If N
+00000920: 6f6e 652c 206e 6f20 7072 696f 7220 6973  one, no prior is
+00000930: 2075 7365 642e 0a20 2020 2020 2020 2020   used..         
+00000940: 2020 2020 2020 2049 6620 6120 7374 722c         If a str,
+00000950: 2077 696c 6c20 6368 6563 6b20 7468 6520   will check the 
+00000960: 6c6f 6361 6c20 6c6f 6361 7469 6f6e 2066  local location f
+00000970: 6972 7374 2066 6f72 2061 2070 7269 6f72  irst for a prior
+00000980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000990: 2073 7065 6369 6669 6320 666f 7220 7468   specific for th
+000009a0: 6973 2062 656e 6368 6d61 726b 2c20 6f74  is benchmark, ot
+000009b0: 6865 7277 6973 6520 6173 7375 6d65 7320  herwise assumes 
+000009c0: 6974 2074 6f20 6265 2061 2050 6174 682e  it to be a Path.
+000009d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000009e0: 2049 6620 6120 5061 7468 2c20 7769 6c6c   If a Path, will
+000009f0: 206c 6f61 6420 7468 6520 7072 696f 7220   load the prior 
+00000a00: 6672 6f6d 2074 6865 2070 6174 682e 0a20  from the path.. 
+00000a10: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+00000a20: 6620 6120 4d61 7070 696e 672c 2077 696c  f a Mapping, wil
+00000a30: 6c20 6265 2075 7365 6420 6469 7265 6374  l be used direct
+00000a40: 6c79 2e0a 2020 2020 2020 2020 2020 2020  ly..            
+00000a50: 7065 7274 7572 625f 7072 696f 723a 2049  perturb_prior: I
+00000a60: 6620 6e6f 7420 4e6f 6e65 2c20 7769 6c6c  f not None, will
+00000a70: 2070 6572 7475 7262 2074 6865 2070 7269   perturb the pri
+00000a80: 6f72 2062 7920 7468 6973 2061 6d6f 756e  or by this amoun
+00000a90: 742e 0a20 2020 2020 2020 2020 2020 2020  t..             
+00000aa0: 2020 2046 6f72 206e 756d 6572 6963 616c     For numerical
+00000ab0: 732c 2074 6869 7320 6973 2069 6e74 6572  s, this is inter
+00000ac0: 7072 6574 6564 2061 7320 7468 6520 7374  preted as the st
+00000ad0: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
+00000ae0: 206f 6620 610a 2020 2020 2020 2020 2020   of a.          
+00000af0: 2020 2020 2020 6e6f 726d 616c 2064 6973        normal dis
+00000b00: 7472 6962 7574 696f 6e20 7768 696c 6520  tribution while 
+00000b10: 666f 7220 6361 7465 676f 7269 6361 6c73  for categoricals
+00000b20: 2c20 7468 6973 2069 7320 696e 7465 7270  , this is interp
+00000b30: 7265 7465 640a 2020 2020 2020 2020 2020  reted.          
+00000b40: 2020 2020 2020 6173 2074 6865 2070 726f        as the pro
+00000b50: 6261 6269 6c69 7479 206f 6620 7377 6170  bability of swap
+00000b60: 7069 6e67 2074 6865 2076 616c 7565 2066  ping the value f
+00000b70: 6f72 2061 2072 616e 646f 6d20 6f6e 652e  or a random one.
+00000b80: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00000b90: 7565 5f6d 6574 7269 633a 2054 6865 206d  ue_metric: The m
+00000ba0: 6574 7269 6320 746f 2075 7365 2066 6f72  etric to use for
+00000bb0: 2074 6869 7320 6265 6e63 686d 6172 6b2e   this benchmark.
+00000bc0: 2055 7365 730a 2020 2020 2020 2020 2020   Uses.          
+00000bd0: 2020 2020 2020 7468 6520 6465 6661 756c        the defaul
+00000be0: 7420 6d65 7472 6963 2066 726f 6d20 7468  t metric from th
+00000bf0: 6520 5265 7375 6c74 2069 6620 4e6f 6e65  e Result if None
+00000c00: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00000c10: 7374 5f6d 6574 7269 633a 2054 6865 2063  st_metric: The c
+00000c20: 6f73 7420 746f 2075 7365 2066 6f72 2074  ost to use for t
+00000c30: 6869 7320 6265 6e63 686d 6172 6b2e 2055  his benchmark. U
+00000c40: 7365 730a 2020 2020 2020 2020 2020 2020  ses.            
+00000c50: 2020 2020 7468 6520 6465 6661 756c 7420      the default 
+00000c60: 636f 7374 2066 726f 6d20 7468 6520 5265  cost from the Re
+00000c70: 7375 6c74 2069 6620 4e6f 6e65 2e0a 2020  sult if None..  
+00000c80: 2020 2020 2020 4e63 0100 0000 0000 0000        Nc........
+00000c90: 0000 0000 0300 0000 0400 0000 5300 0001  ............S...
+00000ca0: 7318 0000 0069 007c 005d 085c 027d 017d  s....i.|.].\.}.}
+00000cb0: 027c 017c 026a 0093 0271 0253 00a9 0029  .|.|.j...q.S...)
+00000cc0: 015a 0d6f 7074 696d 756d 5f76 616c 7565  .Z.optimum_value
+00000cd0: 2903 da02 2e30 5a0b 6d65 7472 6963 5f6e  )....0Z.metric_n
+00000ce0: 616d 655a 066d 6574 7269 6372 3000 0000  ameZ.metricr0...
+00000cf0: 7230 0000 00fa 3c2f 686f 6d65 2f73 6b61  r0....</home/ska
+00000d00: 6e74 6966 792f 636f 6465 2f6d 662d 7072  ntify/code/mf-pr
+00000d10: 696f 722d 6265 6e63 682f 7372 632f 6d66  ior-bench/src/mf
+00000d20: 7062 656e 6368 2f62 656e 6368 6d61 726b  pbench/benchmark
+00000d30: 2e70 79da 0a3c 6469 6374 636f 6d70 3e77  .py..<dictcomp>w
+00000d40: 0000 0073 0800 0000 0600 0602 06ff 06ff  ...s............
+00000d50: 7a26 4265 6e63 686d 6172 6b2e 5f5f 696e  z&Benchmark.__in
+00000d60: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c64  it__.<locals>.<d
+00000d70: 6963 7463 6f6d 703e 721f 0000 0072 0100  ictcomp>r....r..
+00000d80: 0000 e901 0000 007a 3649 6620 7065 7274  .......z6If pert
+00000d90: 7572 6269 6e67 2070 7269 6f72 2c20 6070  urbing prior, `p
+00000da0: 6572 7475 7262 5f70 7269 6f72 6020 6d75  erturb_prior` mu
+00000db0: 7374 2062 6520 696e 205b 302c 2031 5d29  st be in [0, 1])
+00000dc0: 01da 0962 656e 6368 6e61 6d65 2903 721c  ...benchname).r.
+00000dd0: 0000 005a 0373 7464 5a17 6361 7465 676f  ...Z.stdZ.catego
+00000de0: 7269 6361 6c5f 7377 6170 5f63 6861 6e63  rical_swap_chanc
+00000df0: 6529 175a 1464 6566 6175 6c74 5f76 616c  e).Z.default_val
+00000e00: 7565 5f6d 6574 7269 635a 1364 6566 6175  ue_metricZ.defau
+00000e10: 6c74 5f63 6f73 745f 6d65 7472 6963 7221  lt_cost_metricr!
+00000e20: 0000 0072 1c00 0000 7223 0000 0072 1f00  ...r....r#...r..
+00000e30: 0000 7220 0000 0072 2800 0000 722a 0000  ..r ...r(...r*..
+00000e40: 0072 1b00 0000 720f 0000 0072 1000 0000  .r....r....r....
+00000e50: da0b 6d65 7472 6963 5f64 6566 73da 0569  ..metric_defs..i
+00000e60: 7465 6d73 5a0f 6d65 7472 6963 5f6f 7074  temsZ.metric_opt
+00000e70: 696d 756d 73da 0767 6574 6174 7472 5a0a  imums..getattrZ.
+00000e80: 5f70 7269 6f72 5f61 7267 da13 4e6f 7449  _prior_arg..NotI
+00000e90: 6d70 6c65 6d65 6e74 6564 4572 726f 7272  mplementedErrorr
+00000ea0: 1e00 0000 721d 0000 00da 0b5f 6c6f 6164  ....r......_load
+00000eb0: 5f70 7269 6f72 5a07 7065 7274 7572 625a  _priorZ.perturbZ
+00000ec0: 1473 6574 5f61 735f 6465 6661 756c 745f  .set_as_default_
+00000ed0: 7072 696f 7229 0dda 0473 656c 6672 2100  prior)...selfr!.
+00000ee0: 0000 7223 0000 0072 2400 0000 7226 0000  ..r#...r$...r&..
+00000ef0: 0072 2800 0000 722a 0000 0072 1b00 0000  .r(...r*...r....
+00000f00: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
+00000f10: 1f00 0000 7220 0000 0072 3000 0000 7230  ....r ...r0...r0
+00000f20: 0000 0072 3200 0000 da08 5f5f 696e 6974  ...r2.....__init
+00000f30: 5f5f 3e00 0000 7358 0000 0008 2906 0108  __>...sX....)...
+00000f40: 0206 0106 0206 0106 0106 0106 0106 0106  ................
+00000f50: 0106 0106 0106 0106 010a 0208 fe08 0516  ................
+00000f60: 0108 0106 021a 0602 0102 0104 ff02 ff02  ................
+00000f70: 0102 0104 ff06 0406 0108 0214 0106 0214  ................
+00000f80: 0206 0102 0104 0104 0104 0108 fc0a 0710  ................
+00000f90: 0104 ff7a 1242 656e 6368 6d61 726b 2e5f  ...z.Benchmark._
+00000fa0: 5f69 6e69 745f 5fda 0672 6574 7572 6efa  _init__..return.
+00000fb0: 1164 6963 745b 7374 722c 204d 6574 7269  .dict[str, Metri
+00000fc0: 635d 6301 0000 0000 0000 0000 0000 0001  c]c.............
+00000fd0: 0000 0002 0000 0043 0000 0173 0c00 0000  .......C...s....
+00000fe0: 7400 7c00 6a01 6a02 8301 5300 2901 7a1f  t.|.j.j...S.).z.
+00000ff0: 5468 6520 6d65 7472 6963 7320 666f 7220  The metrics for 
+00001000: 7468 6973 2062 656e 6368 6d61 726b 2e29  this benchmark.)
+00001010: 03da 0464 6963 7472 1000 0000 7236 0000  ...dictr....r6..
+00001020: 00a9 0172 3b00 0000 7230 0000 0072 3000  ...r;...r0...r0.
+00001030: 0000 7232 0000 00da 076d 6574 7269 6373  ..r2.....metrics
+00001040: 9e00 0000 7302 0000 000c 037a 1142 656e  ....s......z.Ben
+00001050: 6368 6d61 726b 2e6d 6574 7269 6373 7216  chmark.metricsr.
+00001060: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001070: 0100 0000 0200 0000 4300 0001 f30a 0000  ........C.......
+00001080: 007c 006a 0064 0119 0053 0029 027a 2054  .|.j.d...S.).z T
+00001090: 6865 2073 7461 7274 206f 6620 7468 6520  he start of the 
+000010a0: 6669 6465 6c69 7479 2072 616e 6765 2e72  fidelity range.r
+000010b0: 0100 0000 a901 7228 0000 0072 4000 0000  ......r(...r@...
+000010c0: 7230 0000 0072 3000 0000 7232 0000 00da  r0...r0...r2....
+000010d0: 0573 7461 7274 a300 0000 f302 0000 000a  .start..........
+000010e0: 037a 0f42 656e 6368 6d61 726b 2e73 7461  .z.Benchmark.sta
+000010f0: 7274 6301 0000 0000 0000 0000 0000 0001  rtc.............
+00001100: 0000 0002 0000 0043 0000 0172 4200 0000  .......C...rB...
+00001110: 2902 7a1e 5468 6520 656e 6420 6f66 2074  ).z.The end of t
+00001120: 6865 2066 6964 656c 6974 7920 7261 6e67  he fidelity rang
+00001130: 652e 7234 0000 0072 4300 0000 7240 0000  e.r4...rC...r@..
+00001140: 0072 3000 0000 7230 0000 0072 3200 0000  .r0...r0...r2...
+00001150: da03 656e 64a8 0000 0072 4500 0000 7a0d  ..end....rE...z.
+00001160: 4265 6e63 686d 6172 6b2e 656e 6463 0100  Benchmark.endc..
+00001170: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00001180: 0000 4300 0001 7242 0000 0029 027a 1f54  ..C...rB...).z.T
+00001190: 6865 2073 7465 7020 6f66 2074 6865 2066  he step of the f
+000011a0: 6964 656c 6974 7920 7261 6e67 652e e902  idelity range...
+000011b0: 0000 0072 4300 0000 7240 0000 0072 3000  ...rC...r@...r0.
+000011c0: 0000 7230 0000 0072 3200 0000 da04 7374  ..r0...r2.....st
+000011d0: 6570 ad00 0000 7245 0000 007a 0e42 656e  ep....rE...z.Ben
+000011e0: 6368 6d61 726b 2e73 7465 70fa 2273 7472  chmark.step."str
+000011f0: 207c 2050 6174 6820 7c20 4d61 7070 696e   | Path | Mappin
+00001200: 675b 7374 722c 2041 6e79 5d20 7c20 4372  g[str, Any] | Cr
+00001210: 3500 0000 7214 0000 0063 0300 0000 0000  5...r....c......
+00001220: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
+00001230: 0001 739c 0000 007c 006a 007d 0374 017c  ..s....|.j.}.t.|
+00001240: 0174 0283 0272 277c 0264 0075 0172 207c  .t...r'|.d.u.r |
+00001250: 006a 037c 029b 0064 017c 019b 0064 029d  .j.|...d.|...d..
+00001260: 041b 007d 047c 04a0 04a1 0072 207c 03a0  ...}.|.....r |..
+00001270: 057c 04a1 0153 007c 03a0 0574 067c 0183  .|...S.|...t.|..
+00001280: 01a1 0153 0074 017c 0174 0683 0272 317c  ...S.t.|.t...r1|
+00001290: 03a0 057c 01a1 0153 0074 017c 017c 0383  ...|...S.t.|.|..
+000012a0: 0272 387c 0153 0074 017c 0174 0783 0272  .r8|.S.t.|.t...r
+000012b0: 457c 036a 087c 017c 006a 0964 038d 0253  E|.j.|.|.j.d...S
+000012c0: 0074 0a64 0474 0b7c 0183 019b 009d 0283  .t.d.t.|........
+000012d0: 0182 0129 054e fa01 2d7a 052e 7961 6d6c  ...).N..-z..yaml
+000012e0: a901 da07 7265 6e61 6d65 737a 1355 6e6b  ....renamesz.Unk
+000012f0: 6e6f 776e 2070 7269 6f72 2074 7970 6520  nown prior type 
+00001300: 290c 720f 0000 00da 0a69 7369 6e73 7461  ).r......isinsta
+00001310: 6e63 6572 2200 0000 7218 0000 00da 0665  ncer"...r......e
+00001320: 7869 7374 735a 0966 726f 6d5f 6669 6c65  xistsZ.from_file
+00001330: 7205 0000 0072 0c00 0000 da09 6672 6f6d  r....r......from
+00001340: 5f64 6963 7472 1a00 0000 da0a 5661 6c75  _dictr......Valu
+00001350: 6545 7272 6f72 da04 7479 7065 2905 723b  eError..type).r;
+00001360: 0000 0072 1d00 0000 7235 0000 0072 0f00  ...r....r5...r..
+00001370: 0000 5a0c 6173 7375 6d65 645f 7061 7468  ..Z.assumed_path
+00001380: 7230 0000 0072 3000 0000 7232 0000 0072  r0...r0...r2...r
+00001390: 3a00 0000 b200 0000 731c 0000 0006 050a  :.......s.......
+000013a0: 0208 0216 0108 010a 010e 030a 020a 010a  ................
+000013b0: 0204 010a 0210 0112 027a 1542 656e 6368  .........z.Bench
+000013c0: 6d61 726b 2e5f 6c6f 6164 5f70 7269 6f72  mark._load_prior
+000013d0: da03 6672 6dfa 0846 207c 204e 6f6e 65da  ..frm..F | None.
+000013e0: 0274 6f72 4800 0000 fa0b 4974 6572 6174  .torH.....Iterat
+000013f0: 6f72 5b46 5d63 0400 0000 0000 0000 0000  or[F]c..........
+00001400: 0000 0600 0000 0700 0000 6300 0001 73be  ..........c...s.
+00001410: 0000 0081 007c 0164 0175 0172 077c 016e  .....|.d.u.r.|.n
+00001420: 027c 006a 007d 017c 0264 0175 0172 107c  .|.j.}.|.d.u.r.|
+00001430: 026e 027c 006a 017d 027c 0364 0175 0172  .n.|.j.}.|.d.u.r
+00001440: 197c 036e 027c 006a 027d 037c 006a 007c  .|.n.|.j.}.|.j.|
+00001450: 0104 0003 006b 0172 2e7c 0204 0003 006b  .....k.r.|.....k
+00001460: 0172 2e7c 006a 016b 0173 314a 0082 0101  .r.|.j.k.s1J....
+00001470: 004a 0082 0174 037c 0174 0483 0272 3874  .J...t.|.t...r8t
+00001480: 046e 0174 057d 0474 0674 076a 087c 017c  .n.t.}.t.t.j.|.|
+00001490: 027c 0317 007c 037c 0464 028d 0483 017d  .|...|.|.d.....}
+000014a0: 0574 037c 0374 0583 0272 587c 0564 0319  .t.|.t...rX|.d..
+000014b0: 007c 006a 016b 0572 587c 006a 017c 0564  .|.j.k.rX|.j.|.d
+000014c0: 033c 007c 0545 0064 0148 0001 0064 0153  .<.|.E.d.H...d.S
+000014d0: 0029 0461 6801 0000 4974 6572 6174 6520  .).ah...Iterate 
+000014e0: 7468 726f 7567 6820 7468 6520 6164 7665  through the adve
+000014f0: 7274 6973 6564 2066 6964 656c 6974 7920  rtised fidelity 
+00001500: 7370 6163 6520 6f66 2074 6865 2062 656e  space of the ben
+00001510: 6368 6d61 726b 2e0a 0a20 2020 2020 2020  chmark...       
+00001520: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00001530: 2020 2066 726d 3a20 5374 6172 7420 6f66     frm: Start of
+00001540: 2074 6865 2063 7572 7665 2c20 6465 6661   the curve, defa
+00001550: 756c 7473 2074 6f20 7468 6520 6d69 6e69  ults to the mini
+00001560: 6d75 6d20 6669 6465 6c69 7479 0a20 2020  mum fidelity.   
+00001570: 2020 2020 2020 2020 2074 6f3a 2045 6e64           to: End
+00001580: 206f 6620 7468 6520 6375 7276 652c 2064   of the curve, d
+00001590: 6566 6175 6c74 7320 746f 2074 6865 206d  efaults to the m
+000015a0: 6178 696d 756d 2066 6964 656c 6974 790a  aximum fidelity.
+000015b0: 2020 2020 2020 2020 2020 2020 7374 6570              step
+000015c0: 3a20 5374 6570 2073 697a 652c 2064 6566  : Step size, def
+000015d0: 6175 6c74 7320 746f 2062 656e 6368 6d61  aults to benchma
+000015e0: 726b 2073 7461 6e64 6172 6420 2831 2066  rk standard (1 f
+000015f0: 6f72 2065 706f 6368 290a 0a20 2020 2020  or epoch)..     
+00001600: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00001610: 2020 2020 2020 2020 416e 2069 7465 7261          An itera
+00001620: 746f 7220 6f76 6572 2074 6865 2066 6964  tor over the fid
+00001630: 656c 6974 6965 730a 2020 2020 2020 2020  elities.        
+00001640: 4e29 0472 4400 0000 da04 7374 6f70 7248  N).rD.....stoprH
+00001650: 0000 00da 0564 7479 7065 e9ff ffff ff29  .....dtype.....)
+00001660: 0972 4400 0000 7246 0000 0072 4800 0000  .rD...rF...rH...
+00001670: 724d 0000 00da 0369 6e74 da05 666c 6f61  rM.....int..floa
+00001680: 74da 046c 6973 74da 026e 705a 0661 7261  t..list..npZ.ara
+00001690: 6e67 6529 0672 3b00 0000 7252 0000 0072  nge).r;...rR...r
+000016a0: 5400 0000 7248 0000 0072 5700 0000 5a0a  T...rH...rW...Z.
+000016b0: 6669 6465 6c69 7469 6573 7230 0000 0072  fidelitiesr0...r
+000016c0: 3000 0000 7232 0000 00da 0f69 7465 725f  0...r2.....iter_
+000016d0: 6669 6465 6c69 7469 6573 ce00 0000 7318  fidelities....s.
+000016e0: 0000 0002 8012 1012 0112 012a 0112 0202  ...........*....
+000016f0: 0114 0104 ff18 0b0a 010e 027a 1942 656e  ...........z.Ben
+00001700: 6368 6d61 726b 2e69 7465 725f 6669 6465  chmark.iter_fide
+00001710: 6c69 7469 6573 da04 4e6f 6e65 6301 0000  lities..Nonec...
+00001720: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+00001730: 0043 0000 01f3 0400 0000 6401 5300 2902  .C........d.S.).
+00001740: 7a38 4578 706c 6963 6974 6c79 206c 6f61  z8Explicitly loa
+00001750: 6420 7468 6520 6265 6e63 686d 6172 6b20  d the benchmark 
+00001760: 6265 666f 7265 2071 7565 7279 696e 672c  before querying,
+00001770: 206f 7074 696f 6e61 6c2e 4e72 3000 0000   optional.Nr0...
+00001780: 7240 0000 0072 3000 0000 7230 0000 0072  r@...r0...r0...r
+00001790: 3200 0000 da04 6c6f 6164 f400 0000 7302  2.....load....s.
+000017a0: 0000 0004 007a 0e42 656e 6368 6d61 726b  .....z.Benchmark
+000017b0: 2e6c 6f61 6429 03da 0261 7472 1f00 0000  .load)...atr....
+000017c0: 7220 0000 00da 0663 6f6e 6669 67fa 1543  r .....config..C
+000017d0: 207c 204d 6170 7069 6e67 5b73 7472 2c20   | Mapping[str, 
+000017e0: 416e 795d 7261 0000 0072 1500 0000 6302  Any]ra...r....c.
+000017f0: 0000 0000 0000 0003 0000 0007 0000 0008  ................
+00001800: 0000 0003 0000 0173 e200 0000 7c02 6401  .......s....|.d.
+00001810: 7501 7206 7c02 6e02 7c00 6a00 7d02 7c00  u.r.|.n.|.j.}.|.
+00001820: 6a01 7c02 0400 0300 6b01 7216 7c00 6a00  j.|.....k.r.|.j.
+00001830: 6b01 7319 4a00 8201 0100 4a00 8201 7402  k.s.J.....J...t.
+00001840: 7c01 7c00 6a03 8302 7329 7c00 6a03 6a04  |.|.j...s)|.j.j.
+00001850: 7c01 7c00 6a05 6402 8d02 7d05 6e02 7c01  |.|.j.d...}.n.|.
+00001860: 7d05 7406 7c05 8301 8900 7c00 6a05 6401  }.t.|.....|.j.d.
+00001870: 7501 7249 6403 6404 8400 7c00 6a05 a007  u.rId.d...|.j...
+00001880: a100 4400 8301 7d06 8700 6601 6405 6404  ..D...}...f.d.d.
+00001890: 8408 7c06 a007 a100 4400 8301 8900 7c03  ..|.....D.....|.
+000018a0: 6401 7501 724f 7c03 6e02 7c00 6a08 7d03  d.u.rO|.n.|.j.}.
+000018b0: 7c04 6401 7501 7258 7c04 6e02 7c00 6a09  |.d.u.rX|.n.|.j.
+000018c0: 7d04 7c00 6a0a 6a04 7c01 7c02 7c00 6a0b  }.|.j.j.|.|.|.j.
+000018d0: 8800 7c02 6406 8d02 740c 7c03 8301 740c  ..|.d...t.|...t.
+000018e0: 7c04 8301 7c00 6a0d 6407 8d06 5300 2908  |...|.j.d...S.).
+000018f0: 6199 0200 0053 7562 6d69 7420 6120 7175  a....Submit a qu
+00001900: 6572 7920 616e 6420 6765 7420 6120 7265  ery and get a re
+00001910: 7375 6c74 2e0a 0a20 2020 2020 2020 2041  sult...        A
+00001920: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00001930: 2063 6f6e 6669 673a 2054 6865 2071 7565   config: The que
+00001940: 7279 2074 6f20 7573 650a 2020 2020 2020  ry to use.      
+00001950: 2020 2020 2020 6174 3a20 5468 6520 6669        at: The fi
+00001960: 6465 6c69 7479 2061 7420 7768 6963 6820  delity at which 
+00001970: 746f 2071 7565 7279 2c20 6465 6661 756c  to query, defaul
+00001980: 7473 2074 6f20 4e6f 6e65 2077 6869 6368  ts to None which
+00001990: 206d 6561 6e73 202a 6d61 7869 6d75 6d2a   means *maximum*
+000019a0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+000019b0: 7565 5f6d 6574 7269 633a 2054 6865 206d  ue_metric: The m
+000019c0: 6574 7269 6320 746f 2075 7365 2066 6f72  etric to use for
+000019d0: 2074 6869 7320 7265 7375 6c74 2e20 5573   this result. Us
+000019e0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+000019f0: 2020 2074 6865 2076 616c 7565 206d 6574     the value met
+00001a00: 7269 6320 7061 7373 6564 2069 6e20 746f  ric passed in to
+00001a10: 2074 6865 2063 6f6e 7374 7275 6374 6f72   the constructor
+00001a20: 2069 6620 6e6f 7420 7370 6563 6966 6965   if not specifie
+00001a30: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00001a40: 2020 206f 7468 6572 7769 7365 2074 6865     otherwise the
+00001a50: 2064 6566 6175 6c74 206d 6574 7269 6320   default metric 
+00001a60: 6672 6f6d 2074 6865 2052 6573 756c 7420  from the Result 
+00001a70: 6966 204e 6f6e 652e 0a20 2020 2020 2020  if None..       
+00001a80: 2020 2020 2063 6f73 745f 6d65 7472 6963       cost_metric
+00001a90: 3a20 5468 6520 6d65 7472 6963 2074 6f20  : The metric to 
+00001aa0: 7573 6520 666f 7220 7468 6973 2072 6573  use for this res
+00001ab0: 756c 742e 2055 7365 730a 2020 2020 2020  ult. Uses.      
+00001ac0: 2020 2020 2020 2020 2020 7468 6520 636f            the co
+00001ad0: 7374 206d 6574 7269 6320 7061 7373 6564  st metric passed
+00001ae0: 2069 6e20 746f 2074 6865 2063 6f6e 7374   in to the const
+00001af0: 7275 6374 6f72 2069 6620 6e6f 7420 7370  ructor if not sp
+00001b00: 6563 6966 6965 642c 0a20 2020 2020 2020  ecified,.       
+00001b10: 2020 2020 2020 2020 206f 7468 6572 7769           otherwi
+00001b20: 7365 2074 6865 2064 6566 6175 6c74 206d  se the default m
+00001b30: 6574 7269 6320 6672 6f6d 2074 6865 2052  etric from the R
+00001b40: 6573 756c 7420 6966 204e 6f6e 652e 0a0a  esult if None...
+00001b50: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001b60: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00001b70: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
+00001b80: 7175 6572 790a 2020 2020 2020 2020 4e72  query.        Nr
+00001b90: 4b00 0000 6301 0000 0000 0000 0000 0000  K...c...........
+00001ba0: 0003 0000 0004 0000 0053 0000 01f3 1600  .........S......
+00001bb0: 0000 6900 7c00 5d07 5c02 7d01 7d02 7c02  ..i.|.].\.}.}.|.
+00001bc0: 7c01 9302 7102 5300 7230 0000 0072 3000  |...q.S.r0...r0.
+00001bd0: 0000 a903 7231 0000 00da 016b da01 7672  ....r1.....k..vr
+00001be0: 3000 0000 7230 0000 0072 3200 0000 7233  0...r0...r2...r3
+00001bf0: 0000 0019 0100 00f3 0200 0000 1600 7a23  ..............z#
+00001c00: 4265 6e63 686d 6172 6b2e 7175 6572 792e  Benchmark.query.
+00001c10: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
+00001c20: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
+00001c30: 0300 0000 0700 0000 1300 0001 f31e 0000  ................
+00001c40: 0069 007c 005d 0b5c 027d 017d 027c 0188  .i.|.].\.}.}.|..
+00001c50: 00a0 007c 027c 02a1 0293 0271 0253 0072  ...|.|.....q.S.r
+00001c60: 3000 0000 a901 da03 6765 7472 6500 0000  0.......getre...
+00001c70: a901 da12 5f42 656e 6368 6d61 726b 5f5f  ...._Benchmark__
+00001c80: 636f 6e66 6967 7230 0000 0072 3200 0000  configr0...r2...
+00001c90: 7233 0000 001a 0100 00f3 0200 0000 1e00  r3..............
+00001ca0: a901 7261 0000 00a9 0672 6200 0000 da08  ..ra.....rb.....
+00001cb0: 6669 6465 6c69 7479 da06 7265 7375 6c74  fidelity..result
+00001cc0: 721f 0000 0072 2000 0000 724c 0000 0029  r....r ...rL...)
+00001cd0: 0e72 4600 0000 7244 0000 0072 4d00 0000  .rF...rD...rM...
+00001ce0: 720f 0000 0072 4f00 0000 721a 0000 0072  r....rO...r....r
+00001cf0: 3f00 0000 7237 0000 0072 1f00 0000 7220  ?...r7...r....r 
+00001d00: 0000 0072 1000 0000 da13 5f6f 626a 6563  ...r......_objec
+00001d10: 7469 7665 5f66 756e 6374 696f 6e72 2200  tive_functionr".
+00001d20: 0000 7219 0000 0029 0772 3b00 0000 7262  ..r....).r;...rb
+00001d30: 0000 0072 6100 0000 721f 0000 0072 2000  ...ra...r....r .
+00001d40: 0000 5a07 5f63 6f6e 6669 67da 105f 7265  ..Z._config.._re
+00001d50: 7665 7273 655f 7265 6e61 6d65 7372 3000  verse_renamesr0.
+00001d60: 0000 726c 0000 0072 3200 0000 da05 7175  ..rl...r2.....qu
+00001d70: 6572 79f7 0000 0073 2600 0000 1218 2001  ery....s&..... .
+00001d80: 0c02 1401 0402 0802 0a01 1401 1601 1202  ................
+00001d90: 1201 0602 0201 0201 0c01 0601 0601 0401  ................
+00001da0: 06fa 7a0f 4265 6e63 686d 6172 6b2e 7175  ..z.Benchmark.qu
+00001db0: 6572 7929 0572 5200 0000 7254 0000 0072  ery).rR...rT...r
+00001dc0: 4800 0000 721f 0000 0072 2000 0000 fa07  H...r....r .....
+00001dd0: 6c69 7374 5b52 5d63 0200 0000 0000 0000  list[R]c........
+00001de0: 0500 0000 0800 0000 0700 0000 0300 0001  ................
+00001df0: 73bc 0000 007c 0364 0175 0172 067c 036e  s....|.d.u.r.|.n
+00001e00: 0288 036a 007d 037c 0264 0175 0172 0f7c  ...j.}.|.d.u.r.|
+00001e10: 026e 0288 036a 017d 027c 0464 0175 0172  .n...j.}.|.d.u.r
+00001e20: 187c 046e 0288 036a 027d 0474 0388 0183  .|.n...j.}.t....
+00001e30: 0189 0088 036a 0464 0175 0172 3964 0264  .....j.d.u.r9d.d
+00001e40: 0384 0088 036a 04a0 05a1 0044 0083 017d  .....j.....D...}
+00001e50: 0787 0066 0164 0464 0384 087c 07a0 05a1  ...f.d.d...|....
+00001e60: 0044 0083 0189 0088 0464 0175 0172 3f88  .D.......d.u.r?.
+00001e70: 046e 0288 036a 0689 0488 0264 0175 0172  .n...j.....d.u.r
+00001e80: 4888 026e 0288 036a 0789 0287 0187 0287  H..n...j........
+00001e90: 0387 0466 0464 0564 0684 0888 036a 0888  ...f.d.d.....j..
+00001ea0: 007c 027c 037c 0464 078d 0444 0083 0153  .|.|.|.d...D...S
+00001eb0: 0029 0861 1a03 0000 4765 7420 7468 6520  .).a....Get the 
+00001ec0: 6675 6c6c 2074 7261 6a65 6374 6f72 7920  full trajectory 
+00001ed0: 6f66 2061 2063 6f6e 6669 6775 7261 7469  of a configurati
+00001ee0: 6f6e 2e0a 0a20 2020 2020 2020 2041 7267  on...        Arg
+00001ef0: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+00001f00: 6f6e 6669 673a 2054 6865 2063 6f6e 6669  onfig: The confi
+00001f10: 6720 746f 2071 7565 7279 0a20 2020 2020  g to query.     
+00001f20: 2020 2020 2020 2066 726d 3a20 5374 6172         frm: Star
+00001f30: 7420 6f66 2074 6865 2063 7572 7665 2c20  t of the curve, 
+00001f40: 7368 6f75 6c64 2064 6566 6175 6c74 2074  should default t
+00001f50: 6f20 7468 6520 7374 6172 740a 2020 2020  o the start.    
+00001f60: 2020 2020 2020 2020 746f 3a20 456e 6420          to: End 
+00001f70: 6f66 2074 6865 2063 7572 7665 2c20 7368  of the curve, sh
+00001f80: 6f75 6c64 2064 6566 6175 6c74 2074 6f20  ould default to 
+00001f90: 7468 6520 746f 7461 6c0a 2020 2020 2020  the total.      
+00001fa0: 2020 2020 2020 7374 6570 3a20 5374 6570        step: Step
+00001fb0: 2073 697a 652c 2064 6566 6175 6c74 7320   size, defaults 
+00001fc0: 746f 2060 6063 6c73 2e64 6566 6175 6c74  to ``cls.default
+00001fd0: 5f73 7465 7060 600a 2020 2020 2020 2020  _step``.        
+00001fe0: 2020 2020 7661 6c75 655f 6d65 7472 6963      value_metric
+00001ff0: 3a20 5468 6520 6d65 7472 6963 2074 6f20  : The metric to 
+00002000: 7573 6520 666f 7220 7468 6973 2072 6573  use for this res
+00002010: 756c 742e 2055 7365 730a 2020 2020 2020  ult. Uses.      
+00002020: 2020 2020 2020 2020 2020 7468 6520 7661            the va
+00002030: 6c75 6520 6d65 7472 6963 2070 6173 7365  lue metric passe
+00002040: 6420 696e 2074 6f20 7468 6520 636f 6e73  d in to the cons
+00002050: 7472 7563 746f 7220 6966 206e 6f74 2073  tructor if not s
+00002060: 7065 6369 6669 6564 2c0a 2020 2020 2020  pecified,.      
+00002070: 2020 2020 2020 2020 2020 6f74 6865 7277            otherw
+00002080: 6973 6520 7468 6520 6465 6661 756c 7420  ise the default 
+00002090: 6d65 7472 6963 2066 726f 6d20 7468 6520  metric from the 
+000020a0: 5265 7375 6c74 2069 6620 4e6f 6e65 2e0a  Result if None..
+000020b0: 2020 2020 2020 2020 2020 2020 636f 7374              cost
+000020c0: 5f6d 6574 7269 633a 2054 6865 206d 6574  _metric: The met
+000020d0: 7269 6320 746f 2075 7365 2066 6f72 2074  ric to use for t
+000020e0: 6869 7320 7265 7375 6c74 2e20 5573 6573  his result. Uses
+000020f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002100: 2074 6865 2063 6f73 7420 6d65 7472 6963   the cost metric
+00002110: 2070 6173 7365 6420 696e 2074 6f20 7468   passed in to th
+00002120: 6520 636f 6e73 7472 7563 746f 7220 6966  e constructor if
+00002130: 206e 6f74 2073 7065 6369 6669 6564 2c0a   not specified,.
+00002140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002150: 6f74 6865 7277 6973 6520 7468 6520 6465  otherwise the de
+00002160: 6661 756c 7420 6d65 7472 6963 2066 726f  fault metric fro
+00002170: 6d20 7468 6520 5265 7375 6c74 2069 6620  m the Result if 
+00002180: 4e6f 6e65 2e0a 0a20 2020 2020 2020 2052  None...        R
+00002190: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+000021a0: 2020 2020 4120 6c69 7374 206f 6620 7468      A list of th
+000021b0: 6520 7265 7375 6c74 7320 666f 7220 7468  e results for th
+000021c0: 6973 2063 6f6e 6669 670a 2020 2020 2020  is config.      
+000021d0: 2020 4e63 0100 0000 0000 0000 0000 0000    Nc............
+000021e0: 0300 0000 0400 0000 5300 0001 7264 0000  ........S...rd..
+000021f0: 0072 3000 0000 7230 0000 0072 6500 0000  .r0...r0...re...
+00002200: 7230 0000 0072 3000 0000 7232 0000 0072  r0...r0...r2...r
+00002210: 3300 0000 4901 0000 7268 0000 007a 2842  3...I...rh...z(B
+00002220: 656e 6368 6d61 726b 2e74 7261 6a65 6374  enchmark.traject
+00002230: 6f72 792e 3c6c 6f63 616c 733e 2e3c 6469  ory.<locals>.<di
+00002240: 6374 636f 6d70 3e63 0100 0000 0000 0000  ctcomp>c........
+00002250: 0000 0000 0300 0000 0700 0000 1300 0001  ................
+00002260: 7269 0000 0072 3000 0000 726a 0000 0072  ri...r0...rj...r
+00002270: 6500 0000 726c 0000 0072 3000 0000 7232  e...rl...r0...r2
+00002280: 0000 0072 3300 0000 4a01 0000 726e 0000  ...r3...J...rn..
+00002290: 0063 0100 0000 0000 0000 0000 0000 0300  .c..............
+000022a0: 0000 0a00 0000 1300 0001 7332 0000 0067  ..........s2...g
+000022b0: 007c 005d 155c 027d 017d 0288 026a 006a  .|.].\.}.}...j.j
+000022c0: 0188 007c 017c 0274 0288 0383 0174 0288  ...|.|.t.....t..
+000022d0: 0183 0188 026a 0364 008d 0691 0271 0253  .....j.d.....q.S
+000022e0: 0029 0172 7000 0000 2904 7210 0000 0072  .).rp...).r....r
+000022f0: 4f00 0000 7222 0000 0072 1900 0000 2903  O...r"...r....).
+00002300: 7231 0000 0072 7100 0000 7272 0000 0029  r1...rq...rr...)
+00002310: 0472 6200 0000 7220 0000 0072 3b00 0000  .rb...r ...r;...
+00002320: 721f 0000 0072 3000 0000 7232 0000 00da  r....r0...r2....
+00002330: 0a3c 6c69 7374 636f 6d70 3e4f 0100 0073  .<listcomp>O...s
+00002340: 1600 0000 0600 0609 06f8 0201 0201 0201  ................
+00002350: 0601 0601 0401 04fa 06ff 7a28 4265 6e63  ..........z(Benc
+00002360: 686d 6172 6b2e 7472 616a 6563 746f 7279  hmark.trajectory
+00002370: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00002380: 6f6d 703e a903 7252 0000 0072 5400 0000  omp>..rR...rT...
+00002390: 7248 0000 0029 0972 4600 0000 7244 0000  rH...).rF...rD..
+000023a0: 0072 4800 0000 723f 0000 0072 1a00 0000  .rH...r?...r....
+000023b0: 7237 0000 0072 1f00 0000 7220 0000 00da  r7...r....r ....
+000023c0: 0b5f 7472 616a 6563 746f 7279 2908 723b  ._trajectory).r;
+000023d0: 0000 0072 6200 0000 7252 0000 0072 5400  ...rb...rR...rT.
+000023e0: 0000 7248 0000 0072 1f00 0000 7220 0000  ..rH...r....r ..
+000023f0: 0072 7400 0000 7230 0000 0029 0572 6d00  .rt...r0...).rm.
+00002400: 0000 7262 0000 0072 2000 0000 723b 0000  ..rb...r ...r;..
+00002410: 0072 1f00 0000 7232 0000 00da 0a74 7261  .r....r2.....tra
+00002420: 6a65 6374 6f72 7928 0100 0073 2200 0000  jectory(...s"...
+00002430: 121b 1201 1201 0802 0a01 1401 1601 1202  ................
+00002440: 1201 1002 0409 0201 0201 0201 0201 04fc  ................
+00002450: 06f7 7a14 4265 6e63 686d 6172 6b2e 7472  ..z.Benchmark.tr
+00002460: 616a 6563 746f 7279 fa11 4d61 7070 696e  ajectory..Mappin
+00002470: 675b 7374 722c 2041 6e79 5dfa 134d 6170  g[str, Any]..Map
+00002480: 7069 6e67 5b73 7472 2c20 666c 6f61 745d  ping[str, float]
+00002490: 6302 0000 0000 0000 0001 0000 0003 0000  c...............
+000024a0: 0001 0000 0043 0000 0172 5f00 0000 2902  .....C...r_...).
+000024b0: 7af6 4765 7420 7468 6520 7661 6c75 6520  z.Get the value 
+000024c0: 6f66 2074 6865 2062 656e 6368 6d61 726b  of the benchmark
+000024d0: 2066 6f72 2061 2063 6f6e 6669 6720 6174   for a config at
+000024e0: 2061 2066 6964 656c 6974 792e 0a0a 2020   a fidelity...  
+000024f0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00002500: 2020 2020 2020 2020 636f 6e66 6967 3a20          config: 
+00002510: 5468 6520 636f 6e66 6967 2074 6f20 7175  The config to qu
+00002520: 6572 790a 2020 2020 2020 2020 2020 2020  ery.            
+00002530: 6174 3a20 5468 6520 6669 6465 6c69 7479  at: The fidelity
+00002540: 2074 6f20 6765 7420 7468 6520 7265 7375   to get the resu
+00002550: 6c74 2061 740a 0a20 2020 2020 2020 2052  lt at..        R
+00002560: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00002570: 2020 2020 5468 6520 7265 7375 6c74 206f      The result o
+00002580: 6620 7468 6520 636f 6e66 6967 2061 7320  f the config as 
+00002590: 6b65 7920 7661 6c75 6520 7061 6972 730a  key value pairs.
+000025a0: 2020 2020 2020 2020 4e72 3000 0000 2903          Nr0...).
+000025b0: 723b 0000 0072 6200 0000 7261 0000 0072  r;...rb...ra...r
+000025c0: 3000 0000 7230 0000 0072 3200 0000 7273  0...r0...r2...rs
+000025d0: 0000 0060 0100 0073 0200 0000 0410 7a1d  ...`...s......z.
+000025e0: 4265 6e63 686d 6172 6b2e 5f6f 626a 6563  Benchmark._objec
+000025f0: 7469 7665 5f66 756e 6374 696f 6efa 2749  tive_function.'I
+00002600: 7465 7261 626c 655b 7475 706c 655b 462c  terable[tuple[F,
+00002610: 204d 6170 7069 6e67 5b73 7472 2c20 666c   Mapping[str, fl
+00002620: 6f61 745d 5d5d 6302 0000 0000 0000 0003  oat]]]c.........
+00002630: 0000 0005 0000 0006 0000 0003 0000 0173  ...............s
+00002640: 2000 0000 8700 8701 6602 6401 6402 8408   .......f.d.d...
+00002650: 8801 6a00 7c02 7c03 7c04 6403 8d03 4400  ..j.|.|.|.d...D.
+00002660: 8301 5300 2904 61d6 0100 0047 6574 2074  ..S.).a....Get t
+00002670: 6865 2074 7261 6a65 6374 6f72 7920 6f66  he trajectory of
+00002680: 2061 2063 6f6e 6669 672e 0a0a 2020 2020   a config...    
+00002690: 2020 2020 4279 2064 6566 6175 6c74 2074      By default t
+000026a0: 6869 7320 7769 6c6c 206a 7573 7420 6361  his will just ca
+000026b0: 6c6c 2074 6865 0a20 2020 2020 2020 205b  ll the.        [
+000026c0: 605f 6f62 6a65 6374 6976 655f 6675 6e63  `_objective_func
+000026d0: 7469 6f6e 2829 605d 5b6d 6670 6265 6e63  tion()`][mfpbenc
+000026e0: 682e 4265 6e63 686d 6172 6b2e 5f6f 626a  h.Benchmark._obj
+000026f0: 6563 7469 7665 5f66 756e 6374 696f 6e5d  ective_function]
+00002700: 2066 6f72 0a20 2020 2020 2020 2065 6163   for.        eac
+00002710: 6820 6669 6465 6c69 7479 2062 7574 2074  h fidelity but t
+00002720: 6869 7320 6361 6e20 6265 206f 7665 7277  his can be overw
+00002730: 7269 7474 656e 2069 6620 7468 6973 2063  ritten if this c
+00002740: 616e 2062 6520 646f 6e65 206d 6f72 6520  an be done more 
+00002750: 6f70 7469 6d61 6c79 2e0a 0a20 2020 2020  optimaly...     
+00002760: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00002770: 2020 2020 2063 6f6e 6669 673a 2054 6865       config: The
+00002780: 2063 6f6e 6669 6720 746f 2071 7565 7279   config to query
+00002790: 0a20 2020 2020 2020 2020 2020 2066 726d  .            frm
+000027a0: 3a20 5374 6172 7420 6f66 2074 6865 2063  : Start of the c
+000027b0: 7572 7665 2e0a 2020 2020 2020 2020 2020  urve..          
+000027c0: 2020 746f 3a20 456e 6420 6f66 2074 6865    to: End of the
+000027d0: 2063 7572 7665 2e0a 2020 2020 2020 2020   curve..        
+000027e0: 2020 2020 7374 6570 3a20 5374 6570 2073      step: Step s
+000027f0: 697a 652e 0a0a 2020 2020 2020 2020 5265  ize...        Re
+00002800: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00002810: 2020 2041 206c 6973 7420 6f66 2074 6865     A list of the
+00002820: 2072 6573 756c 7473 2066 6f72 2074 6869   results for thi
+00002830: 7320 636f 6e66 6967 0a20 2020 2020 2020  s config.       
+00002840: 2063 0100 0000 0000 0000 0000 0000 0200   c..............
+00002850: 0000 0700 0000 1300 0001 731e 0000 0067  ..........s....g
+00002860: 007c 005d 0b7d 017c 0188 016a 0088 007c  .|.].}.|...j...|
+00002870: 0164 008d 0266 0291 0271 0253 0029 0172  .d...f...q.S.).r
+00002880: 6f00 0000 2901 7273 0000 0029 0272 3100  o...).rs...).r1.
+00002890: 0000 7271 0000 00a9 0272 6200 0000 723b  ..rq.....rb...r;
+000028a0: 0000 0072 3000 0000 7232 0000 0072 7700  ...r0...r2...rw.
+000028b0: 0000 8901 0000 f308 0000 0006 0002 0210  ................
+000028c0: ff06 ff7a 2942 656e 6368 6d61 726b 2e5f  ...z)Benchmark._
+000028d0: 7472 616a 6563 746f 7279 2e3c 6c6f 6361  trajectory.<loca
+000028e0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7278  ls>.<listcomp>rx
+000028f0: 0000 0029 0172 5d00 0000 2905 723b 0000  ...).r]...).r;..
+00002900: 0072 6200 0000 7252 0000 0072 5400 0000  .rb...rR...rT...
+00002910: 7248 0000 0072 3000 0000 727e 0000 0072  rH...r0...r~...r
+00002920: 3200 0000 7279 0000 0072 0100 0073 0600  2...ry...r...s..
+00002930: 0000 0c17 0e02 06fe 7a15 4265 6e63 686d  ........z.Benchm
+00002940: 6172 6b2e 5f74 7261 6a65 6374 6f72 7929  ark._trajectory)
+00002950: 0172 1c00 0000 da01 6efa 2269 6e74 207c  .r......n."int |
+00002960: 206e 702e 7261 6e64 6f6d 2e52 616e 646f   np.random.Rando
+00002970: 6d53 7461 7465 207c 204e 6f6e 6563 0200  mState | Nonec..
+00002980: 0000 0000 0000 0100 0000 0300 0000 0100  ................
+00002990: 0000 4300 0001 f304 0000 0064 0053 00a9  ..C........d.S..
+000029a0: 014e 7230 0000 00a9 0372 3b00 0000 7280  .Nr0.....r;...r.
+000029b0: 0000 0072 1c00 0000 7230 0000 0072 3000  ...r....r0...r0.
+000029c0: 0000 7232 0000 00da 0673 616d 706c 658f  ..r2.....sample.
+000029d0: 0100 00f3 0200 0000 0407 7a10 4265 6e63  ..........z.Benc
+000029e0: 686d 6172 6b2e 7361 6d70 6c65 7259 0000  hmark.samplerY..
+000029f0: 00fa 076c 6973 745b 435d 6302 0000 0000  ...list[C]c.....
+00002a00: 0000 0001 0000 0003 0000 0001 0000 0043  ...............C
+00002a10: 0000 0172 8200 0000 7283 0000 0072 3000  ...r....r....r0.
+00002a20: 0000 7284 0000 0072 3000 0000 7230 0000  ..r....r0...r0..
+00002a30: 0072 3200 0000 7285 0000 0099 0100 0072  .r2...r........r
+00002a40: 8600 0000 fa0b 4320 7c20 6c69 7374 5b43  ......C | list[C
+00002a50: 5d63 0200 0000 0000 0000 0100 0000 0500  ]c..............
+00002a60: 0000 0400 0000 0300 0001 73a6 0000 0074  ..........s....t
+00002a70: 00a0 0188 006a 02a1 017d 0374 037c 0274  .....j...}.t.|.t
+00002a80: 046a 056a 0683 0272 147c 02a0 0764 0164  .j.j...r.|...d.d
+00002a90: 02a1 027d 046e 0f7c 0264 0375 0172 1a7c  ...}.n.|.d.u.r.|
+00002aa0: 026e 0874 046a 05a0 08a1 00a0 0964 0164  .n.t.j.......d.d
+00002ab0: 02a1 027d 047c 03a0 0a7c 04a1 0101 007c  ...}.|...|.....|
+00002ac0: 0164 0375 0072 3788 006a 0b6a 0c7c 03a0  .d.u.r7..j.j.|..
+00002ad0: 0da1 0088 006a 0e64 048d 0253 007c 0164  .....j.d...S.|.d
+00002ae0: 056b 0272 4788 006a 0b6a 0c7c 03a0 0da1  .k.rG..j.j.|....
+00002af0: 0088 006a 0e64 048d 0267 0153 0087 0066  ...j.d...g.S...f
+00002b00: 0164 0664 0784 087c 03a0 0d7c 01a1 0144  .d.d...|...|...D
+00002b10: 0083 0153 0029 0861 9601 0000 5361 6d70  ...S.).a....Samp
+00002b20: 6c65 2061 2072 616e 646f 6d20 706f 7373  le a random poss
+00002b30: 6962 6c65 2063 6f6e 6669 672e 0a0a 2020  ible config...  
+00002b40: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00002b50: 2020 2020 2020 2020 6e3a 2048 6f77 206d          n: How m
+00002b60: 616e 7920 7361 6d70 6c65 7320 746f 2074  any samples to t
+00002b70: 616b 652c 204e 6f6e 6520 6d65 616e 7320  ake, None means 
+00002b80: 6a73 7574 2061 2073 696e 676c 6520 6f6e  jsut a single on
+00002b90: 652c 206e 6f74 2069 6e20 6120 6c69 7374  e, not in a list
+00002ba0: 0a20 2020 2020 2020 2020 2020 2073 6565  .            see
+00002bb0: 643a 2054 6865 2073 6565 6420 746f 2075  d: The seed to u
+00002bc0: 7365 2066 6f72 2073 616d 706c 696e 670a  se for sampling.
+00002bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002be0: 2021 2121 206e 6f74 6520 2253 6565 6469   !!! note "Seedi
+00002bf0: 6e67 220a 0a20 2020 2020 2020 2020 2020  ng"..           
+00002c00: 2020 2020 2020 2020 2054 6869 7320 6973           This is
+00002c10: 2064 6966 6665 7265 6e74 2074 6861 6e20   different than 
+00002c20: 616e 7920 7365 6564 2070 6173 7365 6420  any seed passed 
+00002c30: 746f 2074 6865 2063 6f6e 7374 7275 6374  to the construct
+00002c40: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+00002c50: 2020 2020 2020 2020 6f66 2074 6865 2062          of the b
+00002c60: 656e 6368 6d61 726b 2e0a 0a20 2020 2020  enchmark...     
+00002c70: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00002c80: 2020 2020 2020 2020 4765 7420 6261 636b          Get back
+00002c90: 2061 2070 6f73 7369 626c 6520 436f 6e66   a possible Conf
+00002ca0: 6967 2074 6f20 7573 650a 2020 2020 2020  ig to use.      
+00002cb0: 2020 7201 0000 0069 ffff ff7f 4e72 4b00    r....i....NrK.
+00002cc0: 0000 7234 0000 0063 0100 0000 0000 0000  ..r4...c........
+00002cd0: 0000 0000 0200 0000 0600 0000 1300 0001  ................
+00002ce0: 731e 0000 0067 007c 005d 0b7d 0188 006a  s....g.|.].}...j
+00002cf0: 006a 017c 0188 006a 0264 008d 0291 0271  .j.|...j.d.....q
+00002d00: 0253 0029 0172 4b00 0000 2903 720f 0000  .S.).rK...).r...
+00002d10: 0072 4f00 0000 721a 0000 0029 0272 3100  .rO...r....).r1.
+00002d20: 0000 da01 6372 4000 0000 7230 0000 0072  ....cr@...r0...r
+00002d30: 3200 0000 7277 0000 00d0 0100 0072 7f00  2...rw.......r..
+00002d40: 0000 7a24 4265 6e63 686d 6172 6b2e 7361  ..z$Benchmark.sa
+00002d50: 6d70 6c65 2e3c 6c6f 6361 6c73 3e2e 3c6c  mple.<locals>.<l
+00002d60: 6973 7463 6f6d 703e 290f da04 636f 7079  istcomp>)...copy
+00002d70: 5a08 6465 6570 636f 7079 7223 0000 0072  Z.deepcopyr#...r
+00002d80: 4d00 0000 725c 0000 005a 0672 616e 646f  M...r\...Z.rando
+00002d90: 6d5a 0b52 616e 646f 6d53 7461 7465 5a07  mZ.RandomStateZ.
+00002da0: 7261 6e64 696e 745a 0b64 6566 6175 6c74  randintZ.default
+00002db0: 5f72 6e67 5a08 696e 7465 6765 7273 721c  _rngZ.integersr.
+00002dc0: 0000 0072 0f00 0000 724f 0000 005a 1473  ...r....rO...Z.s
+00002dd0: 616d 706c 655f 636f 6e66 6967 7572 6174  ample_configurat
+00002de0: 696f 6e72 1a00 0000 2905 723b 0000 0072  ionr....).r;...r
+00002df0: 8000 0000 721c 0000 0072 2300 0000 da03  ....r....r#.....
+00002e00: 726e 6772 3000 0000 7240 0000 0072 3200  rngr0...r@...r2.
+00002e10: 0000 7285 0000 00a2 0100 0073 2c00 0000  ..r........s,...
+00002e20: 0c14 0e01 0e01 0804 04ff 1002 02fd 0a06  ................
+00002e30: 0801 0601 0601 0401 06fe 0806 0602 0601  ................
+00002e40: 0401 04fe 04ff 0a07 0802 06fe fa14 5265  ..............Re
+00002e50: 7375 6c74 4672 616d 655b 432c 2046 2c20  sultFrame[C, F, 
+00002e60: 525d 6301 0000 0000 0000 0000 0000 0001  R]c.............
+00002e70: 0000 0004 0000 0043 0000 0173 1000 0000  .......C...s....
+00002e80: 7400 7401 7402 7403 6603 1900 8300 5300  t.t.t.t.f.....S.
+00002e90: 2901 7a22 4765 7420 616e 2065 6d70 7479  ).z"Get an empty
+00002ea0: 2066 7261 6d65 2074 6f20 7265 636f 7264   frame to record
+00002eb0: 2077 6974 682e 2904 7211 0000 0072 1400   with.).r....r..
+00002ec0: 0000 7216 0000 0072 1500 0000 7240 0000  ..r....r....r@..
+00002ed0: 0072 3000 0000 7230 0000 0072 3200 0000  .r0...r0...r2...
+00002ee0: da05 6672 616d 65d5 0100 0073 0200 0000  ..frame....s....
+00002ef0: 1002 7a0f 4265 6e63 686d 6172 6b2e 6672  ..z.Benchmark.fr
+00002f00: 616d 6529 1872 2100 0000 7222 0000 0072  ame).r!...r"...r
+00002f10: 2300 0000 7212 0000 0072 2400 0000 7225  #...r....r$...r%
+00002f20: 0000 0072 2600 0000 7227 0000 0072 2800  ...r&...r'...r(.
+00002f30: 0000 7229 0000 0072 2a00 0000 7222 0000  ..r)...r*...r"..
+00002f40: 0072 1b00 0000 722b 0000 0072 1c00 0000  .r....r+...r....
+00002f50: 722c 0000 0072 1d00 0000 722d 0000 0072  r,...r....r-...r
+00002f60: 1e00 0000 722e 0000 0072 1f00 0000 722f  ....r....r....r/
+00002f70: 0000 0072 2000 0000 722f 0000 0029 0272  ...r ...r/...).r
+00002f80: 3d00 0000 723e 0000 0029 0272 3d00 0000  =...r>...).r=...
+00002f90: 7216 0000 0072 8300 0000 2906 721d 0000  r....r....).r...
+00002fa0: 0072 4900 0000 7235 0000 0072 2f00 0000  .rI...r5...r/...
+00002fb0: 723d 0000 0072 1400 0000 2903 4e4e 4e29  r=...r....).NNN)
+00002fc0: 0872 5200 0000 7253 0000 0072 5400 0000  .rR...rS...rT...
+00002fd0: 7253 0000 0072 4800 0000 7253 0000 0072  rS...rH...rS...r
+00002fe0: 3d00 0000 7255 0000 0029 0272 3d00 0000  =...rU...).r=...
+00002ff0: 725e 0000 0029 0a72 6200 0000 7263 0000  r^...).rb...rc..
+00003000: 0072 6100 0000 7253 0000 0072 1f00 0000  .ra...rS...r....
+00003010: 722f 0000 0072 2000 0000 722f 0000 0072  r/...r ...r/...r
+00003020: 3d00 0000 7215 0000 0029 0e72 6200 0000  =...r....).rb...
+00003030: 7263 0000 0072 5200 0000 7253 0000 0072  rc...rR...rS...r
+00003040: 5400 0000 7253 0000 0072 4800 0000 7253  T...rS...rH...rS
+00003050: 0000 0072 1f00 0000 722f 0000 0072 2000  ...r....r/...r .
+00003060: 0000 722f 0000 0072 3d00 0000 7276 0000  ..r/...r=...rv..
+00003070: 0029 0672 6200 0000 727b 0000 0072 6100  .).rb...r{...ra.
+00003080: 0000 7216 0000 0072 3d00 0000 727c 0000  ..r....r=...r|..
+00003090: 0029 0a72 6200 0000 727b 0000 0072 5200  .).rb...r{...rR.
+000030a0: 0000 7216 0000 0072 5400 0000 7216 0000  ..r....rT...r...
+000030b0: 0072 4800 0000 7216 0000 0072 3d00 0000  .rH...r....r=...
+000030c0: 727d 0000 0029 0672 8000 0000 725e 0000  r}...).r....r^..
+000030d0: 0072 1c00 0000 7281 0000 0072 3d00 0000  .r....r....r=...
+000030e0: 7214 0000 0029 0672 8000 0000 7259 0000  r....).r....rY..
+000030f0: 0072 1c00 0000 7281 0000 0072 3d00 0000  .r....r....r=...
+00003100: 7287 0000 0029 0672 8000 0000 722c 0000  r....).r....r,..
+00003110: 0072 1c00 0000 7281 0000 0072 3d00 0000  .r....r....r=...
+00003120: 7288 0000 0029 0272 3d00 0000 728c 0000  r....).r=...r...
+00003130: 0029 1ada 085f 5f6e 616d 655f 5fda 0a5f  .)...__name__.._
+00003140: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00003150: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00003160: da09 5052 494f 525f 4449 5272 1800 0000  ..PRIOR_DIRr....
+00003170: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+00003180: 5f72 1900 0000 721a 0000 0072 3c00 0000  _r....r....r<...
+00003190: da08 7072 6f70 6572 7479 7241 0000 0072  ..propertyrA...r
+000031a0: 4400 0000 7246 0000 0072 4800 0000 723a  D...rF...rH...r:
+000031b0: 0000 0072 5d00 0000 7260 0000 0072 7500  ...r]...r`...ru.
+000031c0: 0000 727a 0000 0072 0400 0000 7273 0000  ..rz...r....rs..
+000031d0: 0072 7900 0000 720e 0000 0072 8500 0000  .ry...r....r....
+000031e0: 728d 0000 0072 3000 0000 7230 0000 0072  r....r0...r0...r
+000031f0: 3000 0000 7232 0000 0072 1700 0000 2a00  0...r2...r....*.
+00003200: 0000 7370 0000 000a 0004 010c 0202 010c  ..sp............
+00003210: 0202 010c 0602 0102 0f02 0102 0102 0102  ................
+00003220: 0102 010e f202 600c 0102 040c 0102 040c  ......`.........
+00003230: 0102 040c 0102 070c fd02 1e02 0102 010c  ................
+00003240: fc0a 2602 0702 0102 010e fa02 3502 0102  ..&.........5...
+00003250: 0102 0102 010e f802 380c 010a 1102 1d02  ........8.......
+00003260: 0302 fe02 0410 fc02 0902 0510 fc02 0a02  ................
+00003270: fe02 040e fc0e 3372 1700 0000 2928 da0a  ......3r....)(..
+00003280: 5f5f 6675 7475 7265 5f5f 7202 0000 0072  __future__r....r
+00003290: 8a00 0000 da03 6162 6372 0300 0000 7204  ......abcr....r.
+000032a0: 0000 005a 0770 6174 686c 6962 7205 0000  ...Z.pathlibr...
+000032b0: 00da 0674 7970 696e 6772 0600 0000 7207  ...typingr....r.
+000032c0: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+000032d0: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+000032e0: 0072 0e00 0000 5a05 6e75 6d70 7972 5c00  .r....Z.numpyr\.
+000032f0: 0000 da0f 6d66 7062 656e 6368 2e63 6f6e  ....mfpbench.con
+00003300: 6669 6772 0f00 0000 da0f 6d66 7062 656e  figr......mfpben
+00003310: 6368 2e72 6573 756c 7472 1000 0000 5a14  ch.resultr....Z.
+00003320: 6d66 7062 656e 6368 2e72 6573 756c 7466  mfpbench.resultf
+00003330: 7261 6d65 7211 0000 005a 0b43 6f6e 6669  ramer....Z.Confi
+00003340: 6753 7061 6365 7212 0000 00da 0f6d 6670  gSpacer......mfp
+00003350: 6265 6e63 682e 6d65 7472 6963 7213 0000  bench.metricr...
+00003360: 00da 085f 5f66 696c 655f 5fda 0670 6172  ...__file__..par
+00003370: 656e 745a 0448 4552 4572 9200 0000 7214  entZ.HEREr....r.
+00003380: 0000 0072 1500 0000 7259 0000 0072 5a00  ...r....rY...rZ.
+00003390: 0000 7216 0000 0072 1700 0000 7230 0000  ..r....r....r0..
+000033a0: 0072 3000 0000 7230 0000 0072 3200 0000  .r0...r0...r2...
+000033b0: da08 3c6d 6f64 756c 653e 0100 0000 7324  ..<module>....s$
+000033c0: 0000 000c 0008 0210 010c 012c 0108 0c0c  ...........,....
+000033d0: 020c 010c 0104 020c 010c 020c 0208 010c  ................
+000033e0: 030c 030c 0320 03                        ..... .
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/tabular_benchmark.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/tabular_benchmark.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/util.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/__pycache__/util.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/__pycache__/util.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/benchmark.py` & `mf_prior_bench-1.9.0/src/mfpbench/benchmark.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/config.py` & `mf_prior_bench-1.9.0/src/mfpbench/config.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/correlations.py` & `mf_prior_bench-1.9.0/src/mfpbench/correlations.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/get.py` & `mf_prior_bench-1.9.0/src/mfpbench/get.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/benchmark.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/benchmark.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 10960 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 d02a 0000  o........Coe.*..
+00000000: 6f0d 0d0a 0000 0000 70ea 3d66 c82a 0000  o.......p.=f.*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 2401 0000 6400  .....@...s$...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6400  m.Z.m.Z.m.Z...d.
@@ -123,16 +123,16 @@
 000007a0: 6443 642b 642c 8404 8301 5a0c 650d 6444  dCd+d,....Z.e.dD
 000007b0: 6432 6433 8404 8301 5a0e 650d 6445 8700  d2d3....Z.e.dE..
 000007c0: 6601 6438 6439 840c 8301 5a0f 6510 093a  f.d8d9....Z.e..:
 000007d0: 0915 6446 6447 643f 6440 8405 8301 5a11  ..dFdGd?d@....Z.
 000007e0: 8700 0400 5a12 5300 2948 da0d 4a41 4853  ....Z.S.)H..JAHS
 000007f0: 4265 6e63 686d 6172 6bda 0565 706f 6368  Benchmark..epoch
 00000800: 7235 0000 00da 124a 4148 535f 4649 4445  r5.....JAHS_FIDE
-00000810: 4c49 5459 5f4e 414d 4529 03e9 0300 0000  LITY_NAME)......
-00000820: e9c8 0000 00e9 0100 0000 7a1e 436c 6173  ..........z.Clas
+00000810: 4c49 5459 5f4e 414d 4529 03e9 0100 0000  LITY_NAME)......
+00000820: e9c8 0000 0072 4300 0000 7a1e 436c 6173  .....rC...z.Clas
 00000830: 7356 6172 5b74 7570 6c65 5b69 6e74 2c20  sVar[tuple[int, 
 00000840: 696e 742c 2069 6e74 5d5d da13 4a41 4853  int, int]]..JAHS
 00000850: 5f46 4944 454c 4954 595f 5241 4e47 4529  _FIDELITY_RANGE)
 00000860: 03fa 0976 616c 6964 2d61 6363 fa08 7465  ...valid-acc..te
 00000870: 7374 2d61 6363 7237 0000 007a 1943 6c61  st-accr7...z.Cla
 00000880: 7373 5661 725b 7475 706c 655b 7374 722c  ssVar[tuple[str,
 00000890: 202e 2e2e 5d5d da18 4a41 4853 5f4d 4554   ...]]..JAHS_MET
@@ -141,36 +141,36 @@
 000008c0: 6f72 6563 7461 6c48 6973 746f 6c6f 6779  orectalHistology
 000008d0: da0c 4661 7368 696f 6e4d 4e49 5354 7a1e  ..FashionMNISTz.
 000008e0: 436c 6173 7356 6172 5b74 7570 6c65 5b73  ClassVar[tuple[s
 000008f0: 7472 2c20 7374 722c 2073 7472 5d5d da08  tr, str, str]]..
 00000900: 7461 736b 5f69 6473 da04 7369 7a65 5a05  task_ids..sizeZ.
 00000910: 666c 6f70 7372 3400 0000 723c 0000 005a  flopsr4...r<...Z
 00000920: 0974 7261 696e 5f61 6363 2905 5a07 7369  .train_acc).Z.si
-00000930: 7a65 5f4d 425a 0546 4c4f 5053 7247 0000  ze_MBZ.FLOPSrG..
-00000940: 0072 4800 0000 7a09 7472 6169 6e2d 6163  .rH...z.train-ac
+00000930: 7a65 5f4d 425a 0546 4c4f 5053 7246 0000  ze_MBZ.FLOPSrF..
+00000940: 0072 4700 0000 7a09 7472 6169 6e2d 6163  .rG...z.train-ac
 00000950: 637a 1b43 6c61 7373 5661 725b 4d61 7070  cz.ClassVar[Mapp
 00000960: 696e 675b 7374 722c 2073 7472 5d5d da0f  ing[str, str]]..
 00000970: 5f72 6573 756c 745f 7265 6e61 6d65 734e  _result_renamesN
 00000980: 2906 da07 6461 7461 6469 72da 0473 6565  )...datadir..see
 00000990: 64da 0570 7269 6f72 da0d 7065 7274 7572  d..prior..pertur
 000009a0: 625f 7072 696f 72da 0c76 616c 7565 5f6d  b_prior..value_m
 000009b0: 6574 7269 63da 0b63 6f73 745f 6d65 7472  etric..cost_metr
 000009c0: 6963 da07 7461 736b 5f69 64fa 394c 6974  ic..task_id.9Lit
 000009d0: 6572 616c 5b27 4349 4641 5231 3027 2c20  eral['CIFAR10', 
 000009e0: 2743 6f6c 6f72 6563 7461 6c48 6973 746f  'ColorectalHisto
 000009f0: 6c6f 6779 272c 2027 4661 7368 696f 6e4d  logy', 'FashionM
-00000a00: 4e49 5354 275d 7251 0000 00fa 1173 7472  NIST']rQ.....str
-00000a10: 207c 2050 6174 6820 7c20 4e6f 6e65 7252   | Path | NonerR
+00000a00: 4e49 5354 275d 7250 0000 00fa 1173 7472  NIST']rP.....str
+00000a10: 207c 2050 6174 6820 7c20 4e6f 6e65 7251   | Path | NonerQ
 00000a20: 0000 00fa 0a69 6e74 207c 204e 6f6e 6572  .....int | Noner
-00000a30: 5300 0000 fa32 7374 7220 7c20 5061 7468  S....2str | Path
+00000a30: 5200 0000 fa32 7374 7220 7c20 5061 7468  R....2str | Path
 00000a40: 207c 204a 4148 5343 6f6e 6669 6720 7c20   | JAHSConfig | 
 00000a50: 4d61 7070 696e 675b 7374 722c 2041 6e79  Mapping[str, Any
-00000a60: 5d20 7c20 4e6f 6e65 7254 0000 00fa 0c66  ] | NonerT.....f
-00000a70: 6c6f 6174 207c 204e 6f6e 6572 5500 0000  loat | NonerU...
-00000a80: fa0a 7374 7220 7c20 4e6f 6e65 7256 0000  ..str | NonerV..
+00000a60: 5d20 7c20 4e6f 6e65 7253 0000 00fa 0c66  ] | NonerS.....f
+00000a70: 6c6f 6174 207c 204e 6f6e 6572 5400 0000  loat | NonerT...
+00000a80: fa0a 7374 7220 7c20 4e6f 6e65 7255 0000  ..str | NonerU..
 00000a90: 0063 0200 0000 0000 0000 0600 0000 0a00  .c..............
 00000aa0: 0000 0d00 0000 0300 0001 738c 0000 007c  ..........s....|
 00000ab0: 006a 007d 087c 0264 0175 0072 0b74 01a0  .j.}.|.d.u.r.t..
 00000ac0: 02a1 007d 0274 037c 0283 017d 027c 02a0  ...}.t.|...}.|..
 00000ad0: 04a1 0073 1e74 0564 027c 029b 0064 037c  ...s.t.d.|...d.|
 00000ae0: 029b 0064 049d 0583 0182 0164 017c 005f  ...d.......d.|._
 00000af0: 067c 027c 005f 077c 017c 005f 0864 057c  .|.|._.|.|._.d.|
@@ -241,263 +241,262 @@
 00000f00: 6620 4e6f 6e65 2e0a 2020 2020 2020 2020  f None..        
 00000f10: 4e7a 1543 616e 2774 2066 696e 6420 666f  Nz.Can't find fo
 00000f20: 6c64 6572 2061 7420 7a33 2e0a 6070 7974  lder at z3..`pyt
 00000f30: 686f 6e20 2d6d 206d 6670 6265 6e63 6820  hon -m mfpbench 
 00000f40: 646f 776e 6c6f 6164 202d 2d73 7461 7475  download --statu
 00000f50: 7320 2d2d 6461 7461 2d64 6972 20fa 0160  s --data-dir ..`
 00000f60: 5a05 6a61 6873 5fa9 02da 046e 616d 6572  Z.jahs_....namer
-00000f70: 5200 0000 290b 7252 0000 0072 6000 0000  R...).rR...r`...
+00000f70: 5100 0000 290b 7251 0000 0072 5f00 0000  Q...).rQ...r_...
 00000f80: da0b 636f 6e66 6967 5f74 7970 65da 0b72  ..config_type..r
 00000f90: 6573 756c 745f 7479 7065 da0d 6669 6465  esult_type..fide
 00000fa0: 6c69 7479 5f6e 616d 65da 0e66 6964 656c  lity_name..fidel
 00000fb0: 6974 795f 7261 6e67 65da 0573 7061 6365  ity_range..space
-00000fc0: 7253 0000 0072 5400 0000 7255 0000 0072  rS...rT...rU...r
-00000fd0: 5600 0000 2910 da09 5f5f 636c 6173 735f  V...)...__class_
+00000fc0: 7252 0000 0072 5300 0000 7254 0000 0072  rR...rS...rT...r
+00000fd0: 5500 0000 2910 da09 5f5f 636c 6173 735f  U...)...__class_
 00000fe0: 5f72 1500 0000 5a10 6465 6661 756c 745f  _r....Z.default_
 00000ff0: 6c6f 6361 7469 6f6e 7205 0000 00da 0665  locationr......e
 00001000: 7869 7374 73da 1146 696c 654e 6f74 466f  xists..FileNotFo
 00001010: 756e 6445 7272 6f72 da06 5f62 656e 6368  undError.._bench
-00001020: 7251 0000 0072 5700 0000 da05 7375 7065  rQ...rW.....supe
+00001020: 7250 0000 0072 5600 0000 da05 7375 7065  rP...rV.....supe
 00001030: 72da 085f 5f69 6e69 745f 5f72 1900 0000  r..__init__r....
-00001040: 7233 0000 0072 4200 0000 7246 0000 00da  r3...rB...rF....
+00001040: 7233 0000 0072 4200 0000 7245 0000 00da  r3...rB...rE....
 00001050: 115f 6a61 6873 5f63 6f6e 6669 6773 7061  ._jahs_configspa
-00001060: 6365 290a da04 7365 6c66 7257 0000 0072  ce)...selfrW...r
-00001070: 5100 0000 7252 0000 0072 5300 0000 7254  Q...rR...rS...rT
-00001080: 0000 0072 5500 0000 7256 0000 00da 0363  ...rU...rV.....c
-00001090: 6c73 7260 0000 00a9 0172 6600 0000 7231  lsr`.....rf...r1
-000010a0: 0000 0072 3200 0000 726b 0000 006b 0000  ...r2...rk...k..
+00001060: 6365 290a da04 7365 6c66 7256 0000 0072  ce)...selfrV...r
+00001070: 5000 0000 7251 0000 0072 5200 0000 7253  P...rQ...rR...rS
+00001080: 0000 0072 5400 0000 7255 0000 00da 0363  ...rT...rU.....c
+00001090: 6c73 725f 0000 00a9 0172 6500 0000 7231  lsr_.....re...r1
+000010a0: 0000 0072 3200 0000 726a 0000 006b 0000  ...r2...rj...k..
 000010b0: 0073 3600 0000 0620 0801 0801 0802 0802  .s6.... ........
 000010c0: 0201 0801 0201 06ff 04ff 0606 0601 0601  ................
 000010d0: 0a02 0601 0201 0201 0201 0201 0401 0401  ................
 000010e0: 0c01 0201 0201 0201 0201 0af5 7a16 4a41  ............z.JA
 000010f0: 4853 4265 6e63 686d 6172 6b2e 5f5f 696e  HSBenchmark.__in
 00001100: 6974 5f5f da06 7265 7475 726e da04 4e6f  it__..return..No
 00001110: 6e65 6301 0000 0000 0000 0000 0000 0002  nec.............
 00001120: 0000 0001 0000 0043 0000 0173 0a00 0000  .......C...s....
 00001130: 7c00 6a00 7d01 6401 5300 2902 7a3b 5072  |.j.}.d.S.).z;Pr
 00001140: 652d 6c6f 6164 204a 4148 5320 5847 426f  e-load JAHS XGBo
 00001150: 6f73 7420 6d6f 6465 6c20 6265 666f 7265  ost model before
 00001160: 2071 7565 7279 696e 6720 7468 6520 6669   querying the fi
 00001170: 7273 7420 7469 6d65 2e4e 2901 da05 6265  rst time.N)...be
-00001180: 6e63 6829 0272 6d00 0000 da01 5f72 3100  nch).rm....._r1.
+00001180: 6e63 6829 0272 6c00 0000 da01 5f72 3100  nch).rl....._r1.
 00001190: 0000 7231 0000 0072 3200 0000 da04 6c6f  ..r1...r2.....lo
 000011a0: 6164 ac00 0000 7302 0000 000a 037a 124a  ad....s......z.J
 000011b0: 4148 5342 656e 6368 6d61 726b 2e6c 6f61  AHSBenchmark.loa
 000011c0: 64fa 146a 6168 735f 6265 6e63 682e 4265  d..jahs_bench.Be
 000011d0: 6e63 686d 6172 6b63 0100 0000 0000 0000  nchmarkc........
 000011e0: 0000 0000 0500 0000 0a00 0000 4300 0001  ............C...
-000011f0: 73a2 0000 007c 006a 0073 4e7a 0664 0164  s....|.j.sNz.d.d
+000011f0: 73a0 0000 007c 006a 0073 4d7a 0664 0164  s....|.j.sMz.d.d
 00001200: 026c 017d 0157 006e 1104 0074 0279 1a01  .l.}.W.n...t.y..
 00001210: 007d 0201 007a 0574 0264 0383 017c 0282  .}...z.t.d...|..
 00001220: 0264 027d 027e 0277 0177 007c 016a 036a  .d.}.~.w.w.|.j.j
 00001230: 047c 016a 036a 057c 016a 036a 0664 049c  .|.j.j.|.j.j.d..
 00001240: 037d 037c 03a0 077c 006a 0864 02a1 027d  .}.|...|.j.d...}
 00001250: 047c 0464 0275 0072 4174 0964 057c 006a  .|.d.u.rAt.d.|.j
 00001260: 089b 0064 0674 0a7c 03a0 0ba1 0083 019b  ...d.t.|........
-00001270: 009d 0483 0182 017c 016a 0c7c 006a 087c  .......|.j.|.j.|
-00001280: 006a 0d64 077c 006a 0e64 088d 047c 005f  .j.d.|.j.d...|._
-00001290: 007c 006a 0053 0029 097a 1e54 6865 2075  .|.j.S.).z.The u
-000012a0: 6e64 6572 6c79 696e 6720 6265 6e63 686d  nderlying benchm
-000012b0: 6172 6b20 7573 6564 2e72 0100 0000 4efa  ark used.r....N.
-000012c0: 496a 6168 732d 6265 6e63 6820 6e6f 7420  Ijahs-bench not 
-000012d0: 696e 7374 616c 6c65 642c 2070 6c65 6173  installed, pleas
-000012e0: 6520 696e 7374 616c 6c20 6974 2077 6974  e install it wit
-000012f0: 6820 6070 6970 2069 6e73 7461 6c6c 206a  h `pip install j
-00001300: 6168 732d 6265 6e63 6860 724a 0000 007a  ahs-bench`rJ...z
-00001310: 0d55 6e6b 6e6f 776e 2074 6173 6b20 7a0d  .Unknown task z.
-00001320: 2c20 6d75 7374 2062 6520 696e 2046 2904  , must be in F).
-00001330: da04 7461 736b 5a08 7361 7665 5f64 6972  ..taskZ.save_dir
-00001340: 5a08 646f 776e 6c6f 6164 da07 6d65 7472  Z.download..metr
-00001350: 6963 7329 0f72 6900 0000 da0a 6a61 6873  ics).ri.....jahs
-00001360: 5f62 656e 6368 da0b 496d 706f 7274 4572  _bench..ImportEr
-00001370: 726f 725a 0e42 656e 6368 6d61 726b 5461  rorZ.BenchmarkTa
-00001380: 736b 7372 4b00 0000 724c 0000 0072 4d00  sksrK...rL...rM.
-00001390: 0000 da03 6765 7472 5700 0000 da0a 5661  ....getrW.....Va
-000013a0: 6c75 6545 7272 6f72 da04 6c69 7374 da04  lueError..list..
-000013b0: 6b65 7973 7211 0000 0072 5100 0000 7249  keysr....rQ...rI
-000013c0: 0000 0029 0572 6d00 0000 7279 0000 00da  ...).rm...ry....
-000013d0: 0165 da05 7461 736b 7372 7700 0000 7231  .e..tasksrw...r1
-000013e0: 0000 0072 3100 0000 7232 0000 0072 7200  ...r1...r2...rr.
-000013f0: 0000 b100 0000 7336 0000 0006 0302 010c  ......s6........
-00001400: 010e 0102 0102 0102 ff02 0302 fd08 8002  ................
-00001410: ff06 0706 0106 0106 fd0e 0508 0102 0118  ................
-00001420: 0104 ff04 0404 0104 0102 0104 0108 fc06  ................
-00001430: 077a 134a 4148 5342 656e 6368 6d61 726b  .z.JAHSBenchmark
-00001440: 2e62 656e 6368 da06 636f 6e66 6967 fa11  .bench..config..
-00001450: 4d61 7070 696e 675b 7374 722c 2041 6e79  Mapping[str, Any
-00001460: 5dda 0261 7472 1a00 0000 fa10 6469 6374  ]..atr......dict
-00001470: 5b73 7472 2c20 666c 6f61 745d 6303 0000  [str, float]c...
-00001480: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-00001490: 0043 0000 0173 2000 0000 7400 7c01 8301  .C...s ...t.|...
-000014a0: 7d03 7c00 6a01 6a02 7c03 7c02 6401 8d02  }.|.j.j.|.|.d...
-000014b0: 7d04 7c04 7c02 1900 5300 2902 4e29 01da  }.|.|...S.).N)..
-000014c0: 076e 6570 6f63 6873 2903 da04 6469 6374  .nepochs)...dict
-000014d0: 7272 0000 00da 085f 5f63 616c 6c5f 5f29  rr.....__call__)
-000014e0: 0572 6d00 0000 7281 0000 0072 8300 0000  .rm...r....r....
-000014f0: da05 7175 6572 79da 0772 6573 756c 7473  ..query..results
-00001500: 7231 0000 0072 3100 0000 7232 0000 00da  r1...r1...r2....
-00001510: 135f 6f62 6a65 6374 6976 655f 6675 6e63  ._objective_func
-00001520: 7469 6f6e d100 0000 7306 0000 0008 0610  tion....s.......
-00001530: 0108 017a 214a 4148 5342 656e 6368 6d61  ...z!JAHSBenchma
-00001540: 726b 2e5f 6f62 6a65 6374 6976 655f 6675  rk._objective_fu
-00001550: 6e63 7469 6f6e da03 6672 6dda 0274 6fda  nction..frm..to.
-00001560: 0473 7465 70fa 2949 7465 7261 626c 655b  .step.)Iterable[
-00001570: 7475 706c 655b 696e 742c 204d 6170 7069  tuple[int, Mappi
-00001580: 6e67 5b73 7472 2c20 666c 6f61 745d 5d5d  ng[str, float]]]
-00001590: 6302 0000 0000 0000 0003 0000 0006 0000  c...............
-000015a0: 0009 0000 0003 0000 0173 4800 0000 7400  .........sH...t.
-000015b0: 7c01 8301 7d05 7a0c 7c00 6a01 6a02 7c05  |...}.z.|.j.j.|.
-000015c0: 7c03 6401 6402 8d03 a003 a100 5700 5300  |.d.d.......W.S.
-000015d0: 0400 7404 7923 0100 0100 0100 7405 8300  ..t.y#......t...
-000015e0: 6a06 7c01 7c02 7c03 7c04 6403 8d04 0600  j.|.|.|.|.d.....
-000015f0: 5900 5300 7700 2904 4e54 2902 7285 0000  Y.S.w.).NT).r...
-00001600: 005a 0f66 756c 6c5f 7472 616a 6563 746f  .Z.full_trajecto
-00001610: 7279 2903 728b 0000 0072 8c00 0000 728d  ry).r....r....r.
-00001620: 0000 0029 0772 8600 0000 7272 0000 0072  ...).r....rr...r
-00001630: 8700 0000 da05 6974 656d 73da 0954 7970  ......items..Typ
-00001640: 6545 7272 6f72 726a 0000 00da 0b5f 7472  eErrorrj....._tr
-00001650: 616a 6563 746f 7279 2906 726d 0000 0072  ajectory).rm...r
-00001660: 8100 0000 728b 0000 0072 8c00 0000 728d  ....r....r....r.
-00001670: 0000 0072 8800 0000 726f 0000 0072 3100  ...r....ro...r1.
-00001680: 0000 7232 0000 0072 9100 0000 db00 0000  ..r2...r........
-00001690: 730c 0000 0008 0902 0218 010c 0118 0302  s...............
-000016a0: fd7a 194a 4148 5342 656e 6368 6d61 726b  .z.JAHSBenchmark
-000016b0: 2e5f 7472 616a 6563 746f 7279 da17 6a61  ._trajectory..ja
-000016c0: 6873 5f62 656e 6368 5f63 6f6e 6669 675f  hs_bench_config_
-000016d0: 7370 6163 6572 6000 0000 7225 0000 00fa  spacer`...r%....
-000016e0: 2269 6e74 207c 206e 702e 7261 6e64 6f6d  "int | np.random
-000016f0: 2e52 616e 646f 6d53 7461 7465 207c 204e  .RandomState | N
-00001700: 6f6e 6572 0e00 0000 6303 0000 0000 0000  oner....c.......
-00001710: 0000 0000 0009 0000 0011 0000 0043 0000  .............C..
-00001720: 0173 6001 0000 7400 7c02 7401 6a02 6a03  .s`...t.|.t.j.j.
-00001730: 8302 720b 7c02 a004 a100 7d02 7a08 6401  ..r.|.....}.z.d.
-00001740: 6402 6c05 6d06 7d03 0100 5700 6e11 0400  d.l.m.}...W.n...
-00001750: 7407 7924 0100 7d04 0100 7a05 7407 6403  t.y$..}...z.t.d.
-00001760: 8301 7c04 8202 6404 7d04 7e04 7701 7700  ..|...d.}.~.w.w.
-00001770: 7408 7c01 7c02 6405 8d02 7d05 7c05 a009  t.|.|.d...}.|...
-00001780: 740a 6406 6407 6408 8d02 740a 6409 640a  t.d.d.d...t.d.d.
-00001790: 6408 8d02 740b 640b 740c 740d 6407 8301  d...t.d.t.t.d...
-000017a0: 8301 6401 640c 8d03 740b 640d 740c 740d  ..d.d...t.d.t.t.
-000017b0: 6407 8301 8301 6401 640c 8d03 740b 640e  d.....d.d...t.d.
-000017c0: 740c 740d 6407 8301 8301 6401 640c 8d03  t.t.d.....d.d...
-000017d0: 740b 640f 740c 740d 6407 8301 8301 6401  t.d.t.t.d.....d.
-000017e0: 640c 8d03 740b 6410 740c 740d 6407 8301  d...t.d.t.t.d...
-000017f0: 8301 6401 640c 8d03 740b 6411 740c 740d  ..d.d...t.d.t.t.
-00001800: 6407 8301 8301 6401 640c 8d03 740a 6412  d.....d.d...t.d.
-00001810: 6413 6408 8d02 740b 6414 6415 6416 6702  d.d...t.d.d.d.g.
-00001820: 6416 640c 8d03 740b 6417 740c 7c03 6a0e  d.d...t.d.t.|.j.
-00001830: a00f a100 8301 6418 640c 8d03 670b a101  ......d.d...g...
-00001840: 0100 740a 6419 641a 6408 8d02 7d06 7410  ..t.d.d.d...}.t.
-00001850: 641b 641c 6413 641d 6415 641e 8d05 7d07  d.d.d.d.d.d...}.
-00001860: 7410 641f 6420 6421 6422 6415 641e 8d05  t.d.d d!d"d.d...
-00001870: 7d08 7c05 a009 7c06 7c07 7c08 6703 a101  }.|...|.|.|.g...
-00001880: 0100 7c05 5300 2923 7ae5 5468 6520 636f  ..|.S.)#z.The co
-00001890: 6e66 6967 7572 6174 696f 6e20 7370 6163  nfiguration spac
-000018a0: 6520 666f 7220 616c 6c20 6461 7461 7365  e for all datase
-000018b0: 7473 2069 6e20 4a41 4853 4265 6e63 682e  ts in JAHSBench.
-000018c0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000018d0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-000018e0: 3a20 5468 6520 6e61 6d65 2074 6f20 6769  : The name to gi
-000018f0: 7665 2074 6f20 7468 6520 636f 6e66 6967  ve to the config
-00001900: 2073 7061 6365 2e0a 2020 2020 2020 2020   space..        
-00001910: 2020 2020 7365 6564 3a20 5468 6520 7365      seed: The se
-00001920: 6564 2074 6f20 7573 6520 666f 7220 7468  ed to use for th
-00001930: 6520 636f 6e66 6967 2073 7061 6365 0a0a  e config space..
-00001940: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00001950: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-00001960: 2073 7061 6365 0a20 2020 2020 2020 2072   space.        r
-00001970: 0100 0000 2901 da0b 4163 7469 7661 7469  ....)...Activati
-00001980: 6f6e 7372 7600 0000 4e72 5f00 0000 721b  onsrv...Nr_...r.
-00001990: 0000 00e9 0500 0000 2901 da05 7661 6c75  ........)...valu
-000019a0: 6572 1c00 0000 e910 0000 0072 1d00 0000  er.........r....
-000019b0: 2902 da07 6368 6f69 6365 73da 0d64 6566  )...choices..def
-000019c0: 6175 6c74 5f76 616c 7565 721e 0000 0072  ault_valuer....r
-000019d0: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
-000019e0: 0000 0072 2900 0000 6700 0000 0000 00f0  ...r)...g.......
-000019f0: 3f72 2400 0000 5446 7226 0000 005a 0452  ?r$...TFr&...Z.R
-00001a00: 654c 5572 2700 0000 5a03 5347 4472 2a00  eLUr'...Z.SGDr*.
-00001a10: 0000 67fc a9f1 d24d 6250 3f67 9a99 9999  ..g....MbP?g....
-00001a20: 9999 b93f 2904 da05 6c6f 7765 72da 0575  ...?)...lower..u
-00001a30: 7070 6572 7299 0000 00da 036c 6f67 722b  pperr......logr+
-00001a40: 0000 0067 f168 e388 b5f8 e43e 677b 14ae  ...g.h.....>g{..
-00001a50: 47e1 7a84 3f67 fca9 f1d2 4d62 403f 2911  G.z.?g....Mb@?).
-00001a60: da0a 6973 696e 7374 616e 6365 723e 0000  ..isinstancer>..
-00001a70: 00da 0672 616e 646f 6dda 0b52 616e 646f  ...random..Rando
-00001a80: 6d53 7461 7465 da08 746f 6d61 7869 6e74  mState..tomaxint
-00001a90: 5a1d 6a61 6873 5f62 656e 6368 2e6c 6962  Z.jahs_bench.lib
-00001aa0: 2e63 6f72 652e 636f 6e73 7461 6e74 7372  .core.constantsr
-00001ab0: 9400 0000 727a 0000 0072 0e00 0000 da13  ....rz...r......
-00001ac0: 6164 645f 6879 7065 7270 6172 616d 6574  add_hyperparamet
-00001ad0: 6572 7372 0f00 0000 720d 0000 0072 7d00  ersr....r....r}.
-00001ae0: 0000 da05 7261 6e67 65da 0b5f 5f6d 656d  ....range..__mem
-00001af0: 6265 7273 5f5f 727e 0000 0072 1000 0000  bers__r~...r....
-00001b00: 2909 726e 0000 0072 6000 0000 7252 0000  ).rn...r`...rR..
-00001b10: 0072 9400 0000 727f 0000 0072 6500 0000  .r....r....re...
-00001b20: 5a0a 6f70 7469 6d69 7a65 7273 da02 6c72  Z.optimizers..lr
-00001b30: 5a0c 7765 6967 6874 5f64 6563 6179 7231  Z.weight_decayr1
-00001b40: 0000 0072 3100 0000 7232 0000 0072 6c00  ...r1...r2...rl.
-00001b50: 0000 ed00 0000 73a4 0000 000e 1108 0102  ......s.........
-00001b60: 0210 010e 0102 0102 0102 ff02 0302 fd08  ................
-00001b70: 8002 ff0c 0604 0102 0202 0102 0204 fd02  ................
-00001b80: 0502 0102 0204 fd02 0502 010a 0102 0104  ................
-00001b90: fd02 0502 010a 0102 0104 fd02 0502 010a  ................
-00001ba0: 0102 0104 fd02 0502 010a 0102 0104 fd02  ................
-00001bb0: 0502 010a 0102 0104 fd02 0502 010a 0102  ................
-00001bc0: 0104 fd0a 0a02 0102 0106 0102 0104 fd02  ................
-00001bd0: 0502 010c 0102 0104 fd02 cc04 ff0c 3e02  ..............>.
-00001be0: 0102 0102 0102 0102 0102 0106 fb02 0702  ................
-00001bf0: 0102 0102 0102 0102 0106 fb10 0804 017a  ...............z
-00001c00: 1f4a 4148 5342 656e 6368 6d61 726b 2e5f  .JAHSBenchmark._
-00001c10: 6a61 6873 5f63 6f6e 6669 6773 7061 6365  jahs_configspace
-00001c20: 290e 7257 0000 0072 5800 0000 7251 0000  ).rW...rX...rQ..
-00001c30: 0072 5900 0000 7252 0000 0072 5a00 0000  .rY...rR...rZ...
-00001c40: 7253 0000 0072 5b00 0000 7254 0000 0072  rS...r[...rT...r
-00001c50: 5c00 0000 7255 0000 0072 5d00 0000 7256  \...rU...r]...rV
-00001c60: 0000 0072 5d00 0000 2902 7270 0000 0072  ...r]...).rp...r
-00001c70: 7100 0000 2902 7270 0000 0072 7500 0000  q...).rp...ru...
-00001c80: 2906 7281 0000 0072 8200 0000 7283 0000  ).r....r....r...
-00001c90: 0072 1a00 0000 7270 0000 0072 8400 0000  .r....rp...r....
-00001ca0: 290a 7281 0000 0072 8200 0000 728b 0000  ).r....r....r...
-00001cb0: 0072 1a00 0000 728c 0000 0072 1a00 0000  .r....r....r....
-00001cc0: 728d 0000 0072 1a00 0000 7270 0000 0072  r....r....rp...r
-00001cd0: 8e00 0000 2902 7292 0000 004e 2906 7260  ....).r....N).r`
-00001ce0: 0000 0072 2500 0000 7252 0000 0072 9300  ...r%...rR...r..
-00001cf0: 0000 7270 0000 0072 0e00 0000 2913 722c  ..rp...r....).r,
-00001d00: 0000 0072 2d00 0000 722e 0000 0072 4200  ...r-...r....rB.
-00001d10: 0000 7230 0000 0072 4600 0000 7249 0000  ..r0...rF...rI..
-00001d20: 0072 4e00 0000 7250 0000 0072 6b00 0000  .rN...rP...rk...
-00001d30: 7274 0000 00da 0870 726f 7065 7274 7972  rt.....propertyr
-00001d40: 7200 0000 720c 0000 0072 8a00 0000 7291  r...r....r....r.
-00001d50: 0000 00da 0b63 6c61 7373 6d65 7468 6f64  .....classmethod
-00001d60: 726c 0000 00da 0d5f 5f63 6c61 7373 6365  rl.....__classce
-00001d70: 6c6c 5f5f 7231 0000 0072 3100 0000 726f  ll__r1...r1...ro
-00001d80: 0000 0072 3200 0000 7240 0000 004e 0000  ...r2...r@...N..
-00001d90: 0073 3c00 0000 0a00 0c01 0c01 0c01 0c06  .s<.............
-00001da0: 0205 0208 0201 0201 0201 0201 0efb 020c  ................
-00001db0: 0201 0201 0201 0201 0201 12f7 0a41 0205  .............A..
-00001dc0: 0c01 021f 0c01 0209 1001 0211 0203 0201  ................
-00001dd0: 16fd 7240 0000 0029 27da 0a5f 5f66 7574  ..r@...)'..__fut
-00001de0: 7572 655f 5f72 0200 0000 da03 6162 6372  ure__r......abcr
-00001df0: 0300 0000 da0b 6461 7461 636c 6173 7365  ......dataclasse
-00001e00: 7372 0400 0000 da07 7061 7468 6c69 6272  sr......pathlibr
-00001e10: 0500 0000 da06 7479 7069 6e67 7206 0000  ......typingr...
-00001e20: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
-00001e30: 720a 0000 0072 0b00 0000 da11 7479 7069  r....r......typi
-00001e40: 6e67 5f65 7874 656e 7369 6f6e 7372 0c00  ng_extensionsr..
-00001e50: 0000 da05 6e75 6d70 7972 3e00 0000 da0b  ....numpyr>.....
-00001e60: 436f 6e66 6967 5370 6163 6572 0d00 0000  ConfigSpacer....
-00001e70: 720e 0000 0072 0f00 0000 7210 0000 00da  r....r....r.....
-00001e80: 126d 6670 6265 6e63 682e 6265 6e63 686d  .mfpbench.benchm
-00001e90: 6172 6b72 1100 0000 da0f 6d66 7062 656e  arkr......mfpben
-00001ea0: 6368 2e63 6f6e 6669 6772 1200 0000 da0f  ch.configr......
-00001eb0: 6d66 7062 656e 6368 2e6d 6574 7269 6372  mfpbench.metricr
-00001ec0: 1300 0000 da0f 6d66 7062 656e 6368 2e72  ......mfpbench.r
-00001ed0: 6573 756c 7472 1400 0000 5a18 6d66 7062  esultr....Z.mfpb
-00001ee0: 656e 6368 2e73 6574 7570 5f62 656e 6368  ench.setup_bench
-00001ef0: 6d61 726b 7215 0000 0072 7900 0000 7219  markr....ry...r.
-00001f00: 0000 0072 1a00 0000 7233 0000 0072 4000  ...r....r3...r@.
-00001f10: 0000 7231 0000 0072 3100 0000 7231 0000  ..r1...r1...r1..
-00001f20: 0072 3200 0000 da08 3c6d 6f64 756c 653e  .r2.....<module>
-00001f30: 0100 0000 7328 0000 000c 000c 020c 010c  ....s(..........
-00001f40: 0120 010c 0108 0218 010c 070c 010c 010c  . ..............
-00001f50: 010c 0104 0208 010c 0312 0108 1b1a 0120  ............... 
-00001f60: 16                                       .
+00001270: 009d 0483 0182 017c 016a 0c7c 047c 006a  .......|.j.|.|.j
+00001280: 0d64 077c 006a 0e64 088d 047c 005f 007c  .d.|.j.d...|._.|
+00001290: 006a 0053 0029 097a 1e54 6865 2075 6e64  .j.S.).z.The und
+000012a0: 6572 6c79 696e 6720 6265 6e63 686d 6172  erlying benchmar
+000012b0: 6b20 7573 6564 2e72 0100 0000 4efa 496a  k used.r....N.Ij
+000012c0: 6168 732d 6265 6e63 6820 6e6f 7420 696e  ahs-bench not in
+000012d0: 7374 616c 6c65 642c 2070 6c65 6173 6520  stalled, please 
+000012e0: 696e 7374 616c 6c20 6974 2077 6974 6820  install it with 
+000012f0: 6070 6970 2069 6e73 7461 6c6c 206a 6168  `pip install jah
+00001300: 732d 6265 6e63 6860 7249 0000 007a 0d55  s-bench`rI...z.U
+00001310: 6e6b 6e6f 776e 2074 6173 6b20 7a0d 2c20  nknown task z., 
+00001320: 6d75 7374 2062 6520 696e 2046 2904 da04  must be in F)...
+00001330: 7461 736b 5a08 7361 7665 5f64 6972 5a08  taskZ.save_dirZ.
+00001340: 646f 776e 6c6f 6164 da07 6d65 7472 6963  download..metric
+00001350: 7329 0f72 6800 0000 da0a 6a61 6873 5f62  s).rh.....jahs_b
+00001360: 656e 6368 da0b 496d 706f 7274 4572 726f  ench..ImportErro
+00001370: 725a 0e42 656e 6368 6d61 726b 5461 736b  rZ.BenchmarkTask
+00001380: 7372 4a00 0000 724b 0000 0072 4c00 0000  srJ...rK...rL...
+00001390: da03 6765 7472 5600 0000 da0a 5661 6c75  ..getrV.....Valu
+000013a0: 6545 7272 6f72 da04 6c69 7374 da04 6b65  eError..list..ke
+000013b0: 7973 7211 0000 0072 5000 0000 7248 0000  ysr....rP...rH..
+000013c0: 0029 0572 6c00 0000 7278 0000 00da 0165  .).rl...rx.....e
+000013d0: 5a05 7461 736b 7372 7600 0000 7231 0000  Z.tasksrv...r1..
+000013e0: 0072 3100 0000 7232 0000 0072 7100 0000  .r1...r2...rq...
+000013f0: b100 0000 7336 0000 0006 0302 010c 010e  ....s6..........
+00001400: 0102 0102 0102 ff02 0302 fd08 8002 ff06  ................
+00001410: 0706 0106 0106 fd0e 0508 0102 0118 0104  ................
+00001420: ff04 0402 0104 0102 0104 0108 fc06 077a  ...............z
+00001430: 134a 4148 5342 656e 6368 6d61 726b 2e62  .JAHSBenchmark.b
+00001440: 656e 6368 da06 636f 6e66 6967 fa11 4d61  ench..config..Ma
+00001450: 7070 696e 675b 7374 722c 2041 6e79 5dda  pping[str, Any].
+00001460: 0261 7472 1a00 0000 fa10 6469 6374 5b73  .atr......dict[s
+00001470: 7472 2c20 666c 6f61 745d 6303 0000 0000  tr, float]c.....
+00001480: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
+00001490: 0000 0173 2000 0000 7400 7c01 8301 7d03  ...s ...t.|...}.
+000014a0: 7c00 6a01 6a02 7c03 7c02 6401 8d02 7d04  |.j.j.|.|.d...}.
+000014b0: 7c04 7c02 1900 5300 2902 4e29 01da 076e  |.|...S.).N)...n
+000014c0: 6570 6f63 6873 2903 da04 6469 6374 7271  epochs)...dictrq
+000014d0: 0000 00da 085f 5f63 616c 6c5f 5f29 0572  .....__call__).r
+000014e0: 6c00 0000 727f 0000 0072 8100 0000 da05  l...r....r......
+000014f0: 7175 6572 79da 0772 6573 756c 7473 7231  query..resultsr1
+00001500: 0000 0072 3100 0000 7232 0000 00da 135f  ...r1...r2....._
+00001510: 6f62 6a65 6374 6976 655f 6675 6e63 7469  objective_functi
+00001520: 6f6e d100 0000 7306 0000 0008 0610 0108  on....s.........
+00001530: 017a 214a 4148 5342 656e 6368 6d61 726b  .z!JAHSBenchmark
+00001540: 2e5f 6f62 6a65 6374 6976 655f 6675 6e63  ._objective_func
+00001550: 7469 6f6e da03 6672 6dda 0274 6fda 0473  tion..frm..to..s
+00001560: 7465 70fa 2949 7465 7261 626c 655b 7475  tep.)Iterable[tu
+00001570: 706c 655b 696e 742c 204d 6170 7069 6e67  ple[int, Mapping
+00001580: 5b73 7472 2c20 666c 6f61 745d 5d5d 6302  [str, float]]]c.
+00001590: 0000 0000 0000 0003 0000 0006 0000 0009  ................
+000015a0: 0000 0003 0000 0173 4800 0000 7400 7c01  .......sH...t.|.
+000015b0: 8301 7d05 7a0c 7c00 6a01 6a02 7c05 7c03  ..}.z.|.j.j.|.|.
+000015c0: 6401 6402 8d03 a003 a100 5700 5300 0400  d.d.......W.S...
+000015d0: 7404 7923 0100 0100 0100 7405 8300 6a06  t.y#......t...j.
+000015e0: 7c01 7c02 7c03 7c04 6403 8d04 0600 5900  |.|.|.|.d.....Y.
+000015f0: 5300 7700 2904 4e54 2902 7283 0000 005a  S.w.).NT).r....Z
+00001600: 0f66 756c 6c5f 7472 616a 6563 746f 7279  .full_trajectory
+00001610: 2903 7289 0000 0072 8a00 0000 728b 0000  ).r....r....r...
+00001620: 0029 0772 8400 0000 7271 0000 0072 8500  .).r....rq...r..
+00001630: 0000 da05 6974 656d 73da 0954 7970 6545  ....items..TypeE
+00001640: 7272 6f72 7269 0000 00da 0b5f 7472 616a  rrorri....._traj
+00001650: 6563 746f 7279 2906 726c 0000 0072 7f00  ectory).rl...r..
+00001660: 0000 7289 0000 0072 8a00 0000 728b 0000  ..r....r....r...
+00001670: 0072 8600 0000 726e 0000 0072 3100 0000  .r....rn...r1...
+00001680: 7232 0000 0072 8f00 0000 db00 0000 730c  r2...r........s.
+00001690: 0000 0008 0902 0218 010c 0118 0302 fd7a  ...............z
+000016a0: 194a 4148 5342 656e 6368 6d61 726b 2e5f  .JAHSBenchmark._
+000016b0: 7472 616a 6563 746f 7279 da17 6a61 6873  trajectory..jahs
+000016c0: 5f62 656e 6368 5f63 6f6e 6669 675f 7370  _bench_config_sp
+000016d0: 6163 6572 5f00 0000 7225 0000 00fa 2269  acer_...r%...."i
+000016e0: 6e74 207c 206e 702e 7261 6e64 6f6d 2e52  nt | np.random.R
+000016f0: 616e 646f 6d53 7461 7465 207c 204e 6f6e  andomState | Non
+00001700: 6572 0e00 0000 6303 0000 0000 0000 0000  er....c.........
+00001710: 0000 0009 0000 0011 0000 0043 0000 0173  ...........C...s
+00001720: 6001 0000 7400 7c02 7401 6a02 6a03 8302  `...t.|.t.j.j...
+00001730: 720b 7c02 a004 a100 7d02 7a08 6401 6402  r.|.....}.z.d.d.
+00001740: 6c05 6d06 7d03 0100 5700 6e11 0400 7407  l.m.}...W.n...t.
+00001750: 7924 0100 7d04 0100 7a05 7407 6403 8301  y$..}...z.t.d...
+00001760: 7c04 8202 6404 7d04 7e04 7701 7700 7408  |...d.}.~.w.w.t.
+00001770: 7c01 7c02 6405 8d02 7d05 7c05 a009 740a  |.|.d...}.|...t.
+00001780: 6406 6407 6408 8d02 740a 6409 640a 6408  d.d.d...t.d.d.d.
+00001790: 8d02 740b 640b 740c 740d 6407 8301 8301  ..t.d.t.t.d.....
+000017a0: 6401 640c 8d03 740b 640d 740c 740d 6407  d.d...t.d.t.t.d.
+000017b0: 8301 8301 6401 640c 8d03 740b 640e 740c  ....d.d...t.d.t.
+000017c0: 740d 6407 8301 8301 6401 640c 8d03 740b  t.d.....d.d...t.
+000017d0: 640f 740c 740d 6407 8301 8301 6401 640c  d.t.t.d.....d.d.
+000017e0: 8d03 740b 6410 740c 740d 6407 8301 8301  ..t.d.t.t.d.....
+000017f0: 6401 640c 8d03 740b 6411 740c 740d 6407  d.d...t.d.t.t.d.
+00001800: 8301 8301 6401 640c 8d03 740a 6412 6413  ....d.d...t.d.d.
+00001810: 6408 8d02 740b 6414 6415 6416 6702 6416  d...t.d.d.d.g.d.
+00001820: 640c 8d03 740b 6417 740c 7c03 6a0e a00f  d...t.d.t.|.j...
+00001830: a100 8301 6418 640c 8d03 670b a101 0100  ....d.d...g.....
+00001840: 740a 6419 641a 6408 8d02 7d06 7410 641b  t.d.d.d...}.t.d.
+00001850: 641c 6413 641d 6415 641e 8d05 7d07 7410  d.d.d.d.d...}.t.
+00001860: 641f 6420 6421 6422 6415 641e 8d05 7d08  d.d d!d"d.d...}.
+00001870: 7c05 a009 7c06 7c07 7c08 6703 a101 0100  |...|.|.|.g.....
+00001880: 7c05 5300 2923 7ae5 5468 6520 636f 6e66  |.S.)#z.The conf
+00001890: 6967 7572 6174 696f 6e20 7370 6163 6520  iguration space 
+000018a0: 666f 7220 616c 6c20 6461 7461 7365 7473  for all datasets
+000018b0: 2069 6e20 4a41 4853 4265 6e63 682e 0a0a   in JAHSBench...
+000018c0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+000018d0: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
+000018e0: 5468 6520 6e61 6d65 2074 6f20 6769 7665  The name to give
+000018f0: 2074 6f20 7468 6520 636f 6e66 6967 2073   to the config s
+00001900: 7061 6365 2e0a 2020 2020 2020 2020 2020  pace..          
+00001910: 2020 7365 6564 3a20 5468 6520 7365 6564    seed: The seed
+00001920: 2074 6f20 7573 6520 666f 7220 7468 6520   to use for the 
+00001930: 636f 6e66 6967 2073 7061 6365 0a0a 2020  config space..  
+00001940: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00001950: 2020 2020 2020 2020 2020 2054 6865 2073             The s
+00001960: 7061 6365 0a20 2020 2020 2020 2072 0100  pace.        r..
+00001970: 0000 2901 da0b 4163 7469 7661 7469 6f6e  ..)...Activation
+00001980: 7372 7500 0000 4e72 5e00 0000 721b 0000  sru...Nr^...r...
+00001990: 00e9 0500 0000 2901 da05 7661 6c75 6572  ......)...valuer
+000019a0: 1c00 0000 e910 0000 0072 1d00 0000 2902  .........r....).
+000019b0: da07 6368 6f69 6365 73da 0d64 6566 6175  ..choices..defau
+000019c0: 6c74 5f76 616c 7565 721e 0000 0072 1f00  lt_valuer....r..
+000019d0: 0000 7220 0000 0072 2100 0000 7222 0000  ..r ...r!...r"..
+000019e0: 0072 2900 0000 6700 0000 0000 00f0 3f72  .r)...g.......?r
+000019f0: 2400 0000 5446 7226 0000 005a 0452 654c  $...TFr&...Z.ReL
+00001a00: 5572 2700 0000 5a03 5347 4472 2a00 0000  Ur'...Z.SGDr*...
+00001a10: 67fc a9f1 d24d 6250 3f67 9a99 9999 9999  g....MbP?g......
+00001a20: b93f 2904 da05 6c6f 7765 72da 0575 7070  .?)...lower..upp
+00001a30: 6572 7297 0000 00da 036c 6f67 722b 0000  err......logr+..
+00001a40: 0067 f168 e388 b5f8 e43e 677b 14ae 47e1  .g.h.....>g{..G.
+00001a50: 7a84 3f67 fca9 f1d2 4d62 403f 2911 da0a  z.?g....Mb@?)...
+00001a60: 6973 696e 7374 616e 6365 723e 0000 00da  isinstancer>....
+00001a70: 0672 616e 646f 6dda 0b52 616e 646f 6d53  .random..RandomS
+00001a80: 7461 7465 da08 746f 6d61 7869 6e74 5a1d  tate..tomaxintZ.
+00001a90: 6a61 6873 5f62 656e 6368 2e6c 6962 2e63  jahs_bench.lib.c
+00001aa0: 6f72 652e 636f 6e73 7461 6e74 7372 9200  ore.constantsr..
+00001ab0: 0000 7279 0000 0072 0e00 0000 da13 6164  ..ry...r......ad
+00001ac0: 645f 6879 7065 7270 6172 616d 6574 6572  d_hyperparameter
+00001ad0: 7372 0f00 0000 720d 0000 0072 7c00 0000  sr....r....r|...
+00001ae0: da05 7261 6e67 65da 0b5f 5f6d 656d 6265  ..range..__membe
+00001af0: 7273 5f5f 727d 0000 0072 1000 0000 2909  rs__r}...r....).
+00001b00: 726d 0000 0072 5f00 0000 7251 0000 0072  rm...r_...rQ...r
+00001b10: 9200 0000 727e 0000 0072 6400 0000 5a0a  ....r~...rd...Z.
+00001b20: 6f70 7469 6d69 7a65 7273 da02 6c72 5a0c  optimizers..lrZ.
+00001b30: 7765 6967 6874 5f64 6563 6179 7231 0000  weight_decayr1..
+00001b40: 0072 3100 0000 7232 0000 0072 6b00 0000  .r1...r2...rk...
+00001b50: ed00 0000 73a4 0000 000e 1108 0102 0210  ....s...........
+00001b60: 010e 0102 0102 0102 ff02 0302 fd08 8002  ................
+00001b70: ff0c 0604 0102 0202 0102 0204 fd02 0502  ................
+00001b80: 0102 0204 fd02 0502 010a 0102 0104 fd02  ................
+00001b90: 0502 010a 0102 0104 fd02 0502 010a 0102  ................
+00001ba0: 0104 fd02 0502 010a 0102 0104 fd02 0502  ................
+00001bb0: 010a 0102 0104 fd02 0502 010a 0102 0104  ................
+00001bc0: fd0a 0a02 0102 0106 0102 0104 fd02 0502  ................
+00001bd0: 010c 0102 0104 fd02 cc04 ff0c 3e02 0102  ............>...
+00001be0: 0102 0102 0102 0102 0106 fb02 0702 0102  ................
+00001bf0: 0102 0102 0102 0106 fb10 0804 017a 1f4a  .............z.J
+00001c00: 4148 5342 656e 6368 6d61 726b 2e5f 6a61  AHSBenchmark._ja
+00001c10: 6873 5f63 6f6e 6669 6773 7061 6365 290e  hs_configspace).
+00001c20: 7256 0000 0072 5700 0000 7250 0000 0072  rV...rW...rP...r
+00001c30: 5800 0000 7251 0000 0072 5900 0000 7252  X...rQ...rY...rR
+00001c40: 0000 0072 5a00 0000 7253 0000 0072 5b00  ...rZ...rS...r[.
+00001c50: 0000 7254 0000 0072 5c00 0000 7255 0000  ..rT...r\...rU..
+00001c60: 0072 5c00 0000 2902 726f 0000 0072 7000  .r\...).ro...rp.
+00001c70: 0000 2902 726f 0000 0072 7400 0000 2906  ..).ro...rt...).
+00001c80: 727f 0000 0072 8000 0000 7281 0000 0072  r....r....r....r
+00001c90: 1a00 0000 726f 0000 0072 8200 0000 290a  ....ro...r....).
+00001ca0: 727f 0000 0072 8000 0000 7289 0000 0072  r....r....r....r
+00001cb0: 1a00 0000 728a 0000 0072 1a00 0000 728b  ....r....r....r.
+00001cc0: 0000 0072 1a00 0000 726f 0000 0072 8c00  ...r....ro...r..
+00001cd0: 0000 2902 7290 0000 004e 2906 725f 0000  ..).r....N).r_..
+00001ce0: 0072 2500 0000 7251 0000 0072 9100 0000  .r%...rQ...r....
+00001cf0: 726f 0000 0072 0e00 0000 2913 722c 0000  ro...r....).r,..
+00001d00: 0072 2d00 0000 722e 0000 0072 4200 0000  .r-...r....rB...
+00001d10: 7230 0000 0072 4500 0000 7248 0000 0072  r0...rE...rH...r
+00001d20: 4d00 0000 724f 0000 0072 6a00 0000 7273  M...rO...rj...rs
+00001d30: 0000 00da 0870 726f 7065 7274 7972 7100  .....propertyrq.
+00001d40: 0000 720c 0000 0072 8800 0000 728f 0000  ..r....r....r...
+00001d50: 00da 0b63 6c61 7373 6d65 7468 6f64 726b  ...classmethodrk
+00001d60: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
+00001d70: 5f5f 7231 0000 0072 3100 0000 726e 0000  __r1...r1...rn..
+00001d80: 0072 3200 0000 7240 0000 004e 0000 0073  .r2...r@...N...s
+00001d90: 3c00 0000 0a00 0c01 0c01 0c01 0c06 0205  <...............
+00001da0: 0208 0201 0201 0201 0201 0efb 020c 0201  ................
+00001db0: 0201 0201 0201 0201 12f7 0a41 0205 0c01  ...........A....
+00001dc0: 021f 0c01 0209 1001 0211 0203 0201 16fd  ................
+00001dd0: 7240 0000 0029 27da 0a5f 5f66 7574 7572  r@...)'..__futur
+00001de0: 655f 5f72 0200 0000 da03 6162 6372 0300  e__r......abcr..
+00001df0: 0000 da0b 6461 7461 636c 6173 7365 7372  ....dataclassesr
+00001e00: 0400 0000 da07 7061 7468 6c69 6272 0500  ......pathlibr..
+00001e10: 0000 da06 7479 7069 6e67 7206 0000 0072  ....typingr....r
+00001e20: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
+00001e30: 0000 0072 0b00 0000 da11 7479 7069 6e67  ...r......typing
+00001e40: 5f65 7874 656e 7369 6f6e 7372 0c00 0000  _extensionsr....
+00001e50: da05 6e75 6d70 7972 3e00 0000 da0b 436f  ..numpyr>.....Co
+00001e60: 6e66 6967 5370 6163 6572 0d00 0000 720e  nfigSpacer....r.
+00001e70: 0000 0072 0f00 0000 7210 0000 00da 126d  ...r....r......m
+00001e80: 6670 6265 6e63 682e 6265 6e63 686d 6172  fpbench.benchmar
+00001e90: 6b72 1100 0000 da0f 6d66 7062 656e 6368  kr......mfpbench
+00001ea0: 2e63 6f6e 6669 6772 1200 0000 da0f 6d66  .configr......mf
+00001eb0: 7062 656e 6368 2e6d 6574 7269 6372 1300  pbench.metricr..
+00001ec0: 0000 da0f 6d66 7062 656e 6368 2e72 6573  ....mfpbench.res
+00001ed0: 756c 7472 1400 0000 5a18 6d66 7062 656e  ultr....Z.mfpben
+00001ee0: 6368 2e73 6574 7570 5f62 656e 6368 6d61  ch.setup_benchma
+00001ef0: 726b 7215 0000 0072 7800 0000 7219 0000  rkr....rx...r...
+00001f00: 0072 1a00 0000 7233 0000 0072 4000 0000  .r....r3...r@...
+00001f10: 7231 0000 0072 3100 0000 7231 0000 0072  r1...r1...r1...r
+00001f20: 3200 0000 da08 3c6d 6f64 756c 653e 0100  2.....<module>..
+00001f30: 0000 7328 0000 000c 000c 020c 010c 0120  ..s(........... 
+00001f40: 010c 0108 0218 010c 070c 010c 010c 010c  ................
+00001f50: 0104 0208 010c 0312 0108 1b1a 0120 16    ............. .
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/benchmark.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/benchmark.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/config.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/config.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/result.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/result.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/result.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/result.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/spaces.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/spaces.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/jahs/__pycache__/spaces.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/jahs/__pycache__/spaces.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/jahs/benchmark.py` & `mf_prior_bench-1.9.0/src/mfpbench/jahs/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     valid_acc: Metric.Value
     test_acc: Metric.Value
     # train_acc: float # remove
 
 
 class JAHSBenchmark(Benchmark[JAHSConfig, JAHSResult, int], ABC):
     JAHS_FIDELITY_NAME: ClassVar[str] = "epoch"
-    JAHS_FIDELITY_RANGE: ClassVar[tuple[int, int, int]] = (3, 200, 1)
+    JAHS_FIDELITY_RANGE: ClassVar[tuple[int, int, int]] = (1, 200, 1)
     JAHS_METRICS_TO_ACTIVATE: ClassVar[tuple[str, ...]] = (
         "valid-acc",
         "test-acc",
         "runtime",
     )
 
     task_ids: ClassVar[tuple[str, str, str]] = (
@@ -194,15 +194,15 @@
             task = tasks.get(self.task_id, None)
             if task is None:
                 raise ValueError(
                     f"Unknown task {self.task_id}, must be in {list(tasks.keys())}",
                 )
 
             self._bench = jahs_bench.Benchmark(
-                task=self.task_id,
+                task=task,
                 save_dir=self.datadir,
                 download=False,
                 metrics=self.JAHS_METRICS_TO_ACTIVATE,
             )
 
         return self._bench
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/lcbench_tabular/__pycache__/benchmark.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/lcbench_tabular/__pycache__/benchmark.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 9870 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 8e26 0000  o........Coe.&..
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 8e26 0000  o.......m.=f.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 0c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 5a0b 6400  m.Z...d.d.l.Z.d.
 00000070: 6405 6c0c 5a0d 6400 6406 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -219,15 +219,15 @@
 00000da0: 726c 696e 6573 5a06 616c 6265 7274 5a16  rlinesZ.albertZ.
 00000db0: 416d 617a 6f6e 5f65 6d70 6c6f 7965 655f  Amazon_employee_
 00000dc0: 6163 6365 7373 5a0a 4150 5346 6169 6c75  accessZ.APSFailu
 00000dd0: 7265 5a0a 4175 7374 7261 6c69 616e 7a0e  reZ.Australianz.
 00000de0: 6261 6e6b 2d6d 6172 6b65 7469 6e67 7a20  bank-marketingz 
 00000df0: 626c 6f6f 642d 7472 616e 7366 7573 696f  blood-transfusio
 00000e00: 6e2d 7365 7276 6963 652d 6365 6e74 6572  n-service-center
-00000e10: da03 6361 725a 0963 6872 6973 7469 6e65  ..carZ.christine
+00000e10: 5a03 6361 725a 0963 6872 6973 7469 6e65  Z.carZ.christine
 00000e20: 7a06 636e 6165 2d39 7a09 636f 6e6e 6563  z.cnae-9z.connec
 00000e30: 742d 345a 0963 6f76 6572 7479 7065 7a08  t-4Z.covertypez.
 00000e40: 6372 6564 6974 2d67 5a06 6469 6f6e 6973  credit-gZ.dionis
 00000e50: 5a06 6661 6265 7274 7a0d 4661 7368 696f  Z.fabertz.Fashio
 00000e60: 6e2d 4d4e 4953 545a 0668 656c 656e 615a  n-MNISTZ.helenaZ
 00000e70: 0568 6967 6773 5a06 6a61 6e6e 6973 5a07  .higgsZ.jannisZ.
 00000e80: 6a61 736d 696e 655a 266a 756e 676c 655f  jasmineZ&jungle_
@@ -247,21 +247,21 @@
 00000f60: 1072 656d 6f76 655f 636f 6e73 7461 6e74  .remove_constant
 00000f70: 7372 1400 0000 da05 7072 696f 72da 0d70  sr......prior..p
 00000f80: 6572 7475 7262 5f70 7269 6f72 da0c 7661  erturb_prior..va
 00000f90: 6c75 655f 6d65 7472 6963 da0b 636f 7374  lue_metric..cost
 00000fa0: 5f6d 6574 7269 63da 0774 6173 6b5f 6964  _metric..task_id
 00000fb0: 7213 0000 00da 0764 6174 6164 6972 fa11  r......datadir..
 00000fc0: 7374 7220 7c20 5061 7468 207c 204e 6f6e  str | Path | Non
-00000fd0: 6572 5b00 0000 7216 0000 0072 1400 0000  er[...r....r....
-00000fe0: 7215 0000 0072 5c00 0000 fa3c 7374 7220  r....r\....<str 
+00000fd0: 6572 5a00 0000 7216 0000 0072 1400 0000  erZ...r....r....
+00000fe0: 7215 0000 0072 5b00 0000 fa3c 7374 7220  r....r[....<str 
 00000ff0: 7c20 5061 7468 207c 204c 4342 656e 6368  | Path | LCBench
 00001000: 5461 6275 6c61 7243 6f6e 6669 6720 7c20  TabularConfig | 
 00001010: 4d61 7070 696e 675b 7374 722c 2041 6e79  Mapping[str, Any
-00001020: 5d20 7c20 4e6f 6e65 725d 0000 0072 4200  ] | Noner]...rB.
-00001030: 0000 725e 0000 0072 4000 0000 725f 0000  ..r^...r@...r_..
+00001020: 5d20 7c20 4e6f 6e65 725c 0000 0072 4200  ] | Noner\...rB.
+00001030: 0000 725d 0000 0072 4000 0000 725e 0000  ..r]...r@...r^..
 00001040: 0072 1700 0000 da04 4e6f 6e65 6303 0000  .r......Nonec...
 00001050: 0000 0000 0006 0000 000f 0000 000e 0000  ................
 00001060: 0003 0000 0173 e600 0000 7c00 6a00 7d09  .....s....|.j.}.
 00001070: 7c01 7c09 6a01 7601 7213 7402 6401 7c01  |.|.j.v.r.t.d.|.
 00001080: 9b00 6402 7c09 6a01 9b00 9d04 8301 8201  ..d.|.j.........
 00001090: 7c02 6403 7500 721b 7403 a004 a100 7d02  |.d.u.r.t.....}.
 000010a0: 7405 7c02 8301 7c01 9b00 6404 9d02 1b00  t.|...|...d.....
@@ -367,65 +367,65 @@
 000016e0: 6829 02da 0569 6e64 6578 da05 6c65 7665  h)...index..leve
 000016f0: 6c7a 106c 6362 656e 6368 5f74 6162 756c  lz.lcbench_tabul
 00001700: 6172 2d29 0372 1200 0000 7214 0000 0072  ar-).r....r....r
 00001710: 1100 0000 da02 6964 290c da05 7461 626c  ......id)...tabl
 00001720: 6572 1200 0000 5a06 6964 5f6b 6579 5a0c  er....Z.id_keyZ.
 00001730: 6669 6465 6c69 7479 5f6b 6579 da0b 7265  fidelity_key..re
 00001740: 7375 6c74 5f74 7970 65da 0b63 6f6e 6669  sult_type..confi
-00001750: 675f 7479 7065 725e 0000 0072 5f00 0000  g_typer^...r_...
-00001760: da05 7370 6163 6572 1400 0000 725c 0000  ..spacer....r\..
-00001770: 0072 5d00 0000 2914 da09 5f5f 636c 6173  .r]...)...__clas
-00001780: 735f 5f72 5a00 0000 da0a 5661 6c75 6545  s__rZ.....ValueE
+00001750: 675f 7479 7065 725d 0000 0072 5e00 0000  g_typer]...r^...
+00001760: da05 7370 6163 6572 1400 0000 725b 0000  ..spacer....r[..
+00001770: 0072 5c00 0000 2914 da09 5f5f 636c 6173  .r\...)...__clas
+00001780: 735f 5f72 5900 0000 da0a 5661 6c75 6545  s__rY.....ValueE
 00001790: 7272 6f72 720f 0000 00da 1064 6566 6175  rrorr......defau
 000017a0: 6c74 5f6c 6f63 6174 696f 6e72 0400 0000  lt_locationr....
 000017b0: da06 6578 6973 7473 da11 4669 6c65 4e6f  ..exists..FileNo
-000017c0: 7446 6f75 6e64 4572 726f 7272 6000 0000  tFoundErrorr`...
+000017c0: 7446 6f75 6e64 4572 726f 7272 5f00 0000  tFoundErrorr_...
 000017d0: da0a 6973 696e 7374 616e 6365 7213 0000  ..isinstancer...
-000017e0: 0072 6100 0000 da02 7064 da0c 7265 6164  .ra.....pd..read
+000017e0: 0072 6000 0000 da02 7064 da0c 7265 6164  .r`.....pd..read
 000017f0: 5f70 6172 7175 6574 da04 6472 6f70 7239  _parquet..dropr9
 00001800: 0000 00da 0573 7570 6572 da08 5f5f 696e  .....super..__in
 00001810: 6974 5f5f 7247 0000 0072 3d00 0000 290f  it__rG...r=...).
-00001820: da04 7365 6c66 7260 0000 0072 6100 0000  ..selfr`...ra...
-00001830: 725b 0000 0072 1400 0000 725c 0000 0072  r[...r....r\...r
-00001840: 5d00 0000 725e 0000 0072 5f00 0000 da03  ]...r^...r_.....
+00001820: da04 7365 6c66 725f 0000 0072 6000 0000  ..selfr_...r`...
+00001830: 725a 0000 0072 1400 0000 725b 0000 0072  rZ...r....r[...r
+00001840: 5c00 0000 725d 0000 0072 5e00 0000 da03  \...r]...r^.....
 00001850: 636c 73da 0a74 6162 6c65 5f70 6174 6872  cls..table_pathr
-00001860: 6900 0000 5a0a 6472 6f70 5f65 706f 6368  i...Z.drop_epoch
+00001860: 6800 0000 5a0a 6472 6f70 5f65 706f 6368  h...Z.drop_epoch
 00001870: 5a13 6265 6e63 686d 6172 6b5f 7461 736b  Z.benchmark_task
-00001880: 5f6e 616d 6572 6c00 0000 a901 726d 0000  _namerl.....rm..
-00001890: 0072 3700 0000 7238 0000 0072 7700 0000  .r7...r8...rw...
+00001880: 5f6e 616d 6572 6b00 0000 a901 726c 0000  _namerk.....rl..
+00001890: 0072 3700 0000 7238 0000 0072 7600 0000  .r7...r8...rv...
 000018a0: cf00 0000 734a 0000 0006 230a 0116 0108  ....sJ....#.....
 000018b0: 0208 0112 0208 0102 0108 0102 0104 ff04  ................
 000018c0: ff06 0518 010a 0204 080e 010a 0202 0108  ................
 000018d0: 0102 0104 0106 fd06 0602 0102 0102 0102  ................
 000018e0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 000018f0: 010a f47a 204c 4342 656e 6368 5461 6275  ...z LCBenchTabu
 00001900: 6c61 7242 656e 6368 6d61 726b 2e5f 5f69  larBenchmark.__i
-00001910: 6e69 745f 5fa9 014e 2912 7260 0000 0072  nit__..N).r`...r
-00001920: 1300 0000 7261 0000 0072 6200 0000 725b  ....ra...rb...r[
+00001910: 6e69 745f 5fa9 014e 2912 725f 0000 0072  nit__..N).r_...r
+00001920: 1300 0000 7260 0000 0072 6100 0000 725a  ....r`...ra...rZ
 00001930: 0000 0072 1600 0000 7214 0000 0072 1500  ...r....r....r..
-00001940: 0000 725c 0000 0072 6300 0000 725d 0000  ..r\...rc...r]..
-00001950: 0072 4200 0000 725e 0000 0072 4000 0000  .rB...r^...r@...
-00001960: 725f 0000 0072 4000 0000 7217 0000 0072  r_...r@...r....r
-00001970: 6400 0000 2907 7243 0000 0072 4400 0000  d...).rC...rD...
-00001980: 7245 0000 0072 5a00 0000 7246 0000 0072  rE...rZ...rF...r
-00001990: 7700 0000 da0d 5f5f 636c 6173 7363 656c  w.....__classcel
-000019a0: 6c5f 5f72 3700 0000 7237 0000 0072 7b00  l__r7...r7...r{.
+00001940: 0000 725b 0000 0072 6200 0000 725c 0000  ..r[...rb...r\..
+00001950: 0072 4200 0000 725d 0000 0072 4000 0000  .rB...r]...r@...
+00001960: 725e 0000 0072 4000 0000 7217 0000 0072  r^...r@...r....r
+00001970: 6300 0000 2907 7243 0000 0072 4400 0000  c...).rC...rD...
+00001980: 7245 0000 0072 5900 0000 7246 0000 0072  rE...rY...rF...r
+00001990: 7600 0000 da0d 5f5f 636c 6173 7363 656c  v.....__classcel
+000019a0: 6c5f 5f72 3700 0000 7237 0000 0072 7a00  l__r7...r7...rz.
 000019b0: 0000 7238 0000 0072 5700 0000 a200 0000  ..r8...rW.......
 000019c0: 7318 0000 000a 000c 0102 2502 0a02 fd02  s.........%.....
 000019d0: 0502 0102 0102 0102 0102 011a f672 5700  .............rW.
-000019e0: 0000 727c 0000 0029 0872 1200 0000 7213  ..r|...).r....r.
+000019e0: 0000 727b 0000 0029 0872 1200 0000 7213  ..r{...).r....r.
 000019f0: 0000 0072 1400 0000 7215 0000 0072 1100  ...r....r....r..
 00001a00: 0000 7216 0000 0072 1700 0000 7208 0000  ..r....r....r...
 00001a10: 0029 23da 0a5f 5f66 7574 7572 655f 5f72  .)#..__future__r
 00001a20: 0200 0000 da0b 6461 7461 636c 6173 7365  ......dataclasse
 00001a30: 7372 0300 0000 da07 7061 7468 6c69 6272  sr......pathlibr
 00001a40: 0400 0000 da06 7479 7069 6e67 7205 0000  ......typingr...
 00001a50: 0072 0600 0000 7207 0000 00da 056e 756d  .r....r......num
 00001a60: 7079 7255 0000 00da 0670 616e 6461 7372  pyrU.....pandasr
-00001a70: 7300 0000 da0b 436f 6e66 6967 5370 6163  s.....ConfigSpac
+00001a70: 7200 0000 da0b 436f 6e66 6967 5370 6163  r.....ConfigSpac
 00001a80: 6572 0800 0000 da1b 436f 6e66 6967 5370  er......ConfigSp
 00001a90: 6163 652e 6879 7065 7270 6172 616d 6574  ace.hyperparamet
 00001aa0: 6572 7372 0900 0000 720a 0000 0072 0b00  ersr....r....r..
 00001ab0: 0000 da0f 6d66 7062 656e 6368 2e63 6f6e  ....mfpbench.con
 00001ac0: 6669 6772 0c00 0000 da0f 6d66 7062 656e  figr......mfpben
 00001ad0: 6368 2e6d 6574 7269 6372 0d00 0000 da0f  ch.metricr......
 00001ae0: 6d66 7062 656e 6368 2e72 6573 756c 7472  mfpbench.resultr
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/lcbench_tabular/benchmark.py` & `mf_prior_bench-1.9.0/src/mfpbench/lcbench_tabular/benchmark.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/metric.py` & `mf_prior_bench-1.9.0/src/mfpbench/metric.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/benchmark.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/benchmark.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 7119 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 cf1b 0000  o........Coe....
+00000000: 6f0d 0d0a 0000 0000 70ea 3d66 fe1b 0000  o.......p.=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 5401 0000 6400  .....@...sT...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6400  m.Z.m.Z.m.Z...d.
@@ -58,404 +58,406 @@
 00000390: 6e74 6966 792f 636f 6465 2f6d 662d 7072  ntify/code/mf-pr
 000003a0: 696f 722d 6265 6e63 682f 7372 632f 6d66  ior-bench/src/mf
 000003b0: 7062 656e 6368 2f70 6431 2f62 656e 6368  pbench/pd1/bench
 000003c0: 6d61 726b 2e70 7972 1900 0000 1900 0000  mark.pyr........
 000003d0: 730c 0000 000a 0004 0208 0208 0108 010c  s...............
 000003e0: 0172 1900 0000 2901 7216 0000 0063 0000  .r....).r....c..
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0600  ................
-00000400: 0000 4000 0001 7380 0000 0065 005a 0164  ..@...s....e.Z.d
-00000410: 005a 0255 0064 015a 0365 0464 0264 0365  .Z.U.d.Z.e.d.d.e
-00000420: 056a 0666 0264 048d 0265 0464 0264 0365  .j.f.d...e.d.d.e
-00000430: 056a 0666 0264 048d 0265 0464 0264 0365  .j.f.d...e.d.d.e
-00000440: 056a 0666 0264 048d 0264 059c 035a 0764  .j.f.d...d...Z.d
-00000450: 0665 0864 073c 0064 085a 0964 0965 0864  .e.d.<.d.Z.d.e.d
-00000460: 0a3c 0064 0b5a 0a64 0965 0864 0c3c 0064  .<.d.Z.d.e.d.<.d
-00000470: 0d65 0864 083c 0064 0d65 0864 0e3c 0064  .e.d.<.d.e.d.<.d
-00000480: 0d65 0864 0b3c 0064 0f53 0029 10da 0f50  .e.d.<.d.S.)...P
-00000490: 4431 5265 7375 6c74 5369 6d70 6c65 7a4c  D1ResultSimplezL
-000004a0: 5573 6564 2066 6f72 2061 6c6c 2050 4431  Used for all PD1
-000004b0: 2062 656e 6368 6d61 726b 732c 2065 7863   benchmarks, exc
-000004c0: 6570 7420 696d 6167 656e 6574 2c20 6c6d  ept imagenet, lm
-000004d0: 3162 2c20 7472 616e 736c 6174 655f 776d  1b, translate_wm
-000004e0: 742c 2075 6e69 7265 6635 302e 5472 0100  t, uniref50.Tr..
-000004f0: 0000 a902 da08 6d69 6e69 6d69 7a65 da06  ......minimize..
-00000500: 626f 756e 6473 2903 da10 7661 6c69 645f  bounds)...valid_
+00000400: 0000 4000 0001 7374 0000 0065 005a 0164  ..@...st...e.Z.d
+00000410: 005a 0255 0064 015a 0365 0464 0264 0364  .Z.U.d.Z.e.d.d.d
+00000420: 048d 0265 0464 0264 0364 048d 0265 0464  ...e.d.d.d...e.d
+00000430: 0264 0565 056a 0666 0264 048d 0264 069c  .d.e.j.f.d...d..
+00000440: 035a 0764 0765 0864 083c 0064 095a 0964  .Z.d.e.d.<.d.Z.d
+00000450: 0a65 0864 0b3c 0064 0c5a 0a64 0a65 0864  .e.d.<.d.Z.d.e.d
+00000460: 0d3c 0064 0e65 0864 093c 0064 0e65 0864  .<.d.e.d.<.d.e.d
+00000470: 0f3c 0064 0e65 0864 0c3c 0064 1053 0029  .<.d.e.d.<.d.S.)
+00000480: 11da 0f50 4431 5265 7375 6c74 5369 6d70  ...PD1ResultSimp
+00000490: 6c65 7a4c 5573 6564 2066 6f72 2061 6c6c  lezLUsed for all
+000004a0: 2050 4431 2062 656e 6368 6d61 726b 732c   PD1 benchmarks,
+000004b0: 2065 7863 6570 7420 696d 6167 656e 6574   except imagenet
+000004c0: 2c20 6c6d 3162 2c20 7472 616e 736c 6174  , lm1b, translat
+000004d0: 655f 776d 742c 2075 6e69 7265 6635 302e  e_wmt, uniref50.
+000004e0: 54a9 0272 0100 0000 e901 0000 00a9 02da  T..r............
+000004f0: 086d 696e 696d 697a 65da 0662 6f75 6e64  .minimize..bound
+00000500: 7372 0100 0000 2903 da10 7661 6c69 645f  sr....)...valid_
 00000510: 6572 726f 725f 7261 7465 da0f 7465 7374  error_rate..test
 00000520: 5f65 7272 6f72 5f72 6174 65da 0a74 7261  _error_rate..tra
 00000530: 696e 5f63 6f73 74fa 1e43 6c61 7373 5661  in_cost..ClassVa
 00000540: 725b 4d61 7070 696e 675b 7374 722c 204d  r[Mapping[str, M
 00000550: 6574 7269 635d 5dda 0b6d 6574 7269 635f  etric]]..metric_
-00000560: 6465 6673 7226 0000 00fa 0d43 6c61 7373  defsr&.....Class
+00000560: 6465 6673 7228 0000 00fa 0d43 6c61 7373  defsr(.....Class
 00000570: 5661 725b 7374 725d da14 6465 6661 756c  Var[str]..defaul
-00000580: 745f 7661 6c75 655f 6d65 7472 6963 7228  t_value_metricr(
+00000580: 745f 7661 6c75 655f 6d65 7472 6963 722a  t_value_metricr*
 00000590: 0000 00da 1364 6566 6175 6c74 5f63 6f73  .....default_cos
 000005a0: 745f 6d65 7472 6963 fa0c 4d65 7472 6963  t_metric..Metric
-000005b0: 2e56 616c 7565 7227 0000 004e a90b 721b  .Valuer'...N..r.
+000005b0: 2e56 616c 7565 7229 0000 004e a90b 721b  .Valuer)...N..r.
 000005c0: 0000 0072 1c00 0000 721d 0000 0072 1e00  ...r....r....r..
 000005d0: 0000 720f 0000 00da 026e 70da 0369 6e66  ..r......np..inf
-000005e0: 722a 0000 0072 1f00 0000 722c 0000 0072  r*...r....r,...r
-000005f0: 2d00 0000 7220 0000 0072 2000 0000 7220  -...r ...r ...r 
+000005e0: 722c 0000 0072 1f00 0000 722e 0000 0072  r,...r....r....r
+000005f0: 2f00 0000 7220 0000 0072 2000 0000 7220  /...r ...r ...r 
 00000600: 0000 0072 2100 0000 7222 0000 0023 0000  ...r!...r"...#..
-00000610: 0073 1600 0000 0a00 0402 1003 1001 1001  .s..............
+00000610: 0073 1600 0000 0a00 0402 0a03 0a01 1001  .s..............
 00000620: 0efd 0c05 0c01 0802 0801 0c01 7222 0000  ............r"..
 00000630: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000640: 0000 0500 0000 4000 0001 7368 0000 0065  ......@...sh...e
+00000640: 0000 0500 0000 4000 0001 7362 0000 0065  ......@...sb...e
 00000650: 005a 0164 005a 0255 0064 015a 0365 0464  .Z.d.Z.U.d.Z.e.d
-00000660: 0264 0365 056a 0666 0264 048d 0265 0464  .d.e.j.f.d...e.d
-00000670: 0264 0365 056a 0666 0264 048d 0264 059c  .d.e.j.f.d...d..
-00000680: 025a 0764 0665 0864 073c 0064 085a 0964  .Z.d.e.d.<.d.Z.d
-00000690: 0965 0864 0a3c 0064 0b5a 0a64 0965 0864  .e.d.<.d.Z.d.e.d
-000006a0: 0c3c 0064 0d65 0864 083c 0064 0d65 0864  .<.d.e.d.<.d.e.d
-000006b0: 0b3c 0064 0e53 0029 0fda 1450 4431 5265  .<.d.S.)...PD1Re
-000006c0: 7375 6c74 5472 616e 7366 6f72 6d65 727a  sultTransformerz
-000006d0: 4949 6d61 6765 6e65 742c 206c 6d31 622c  IImagenet, lm1b,
-000006e0: 2074 7261 6e73 6c61 7465 5f77 6d74 2c20   translate_wmt, 
-000006f0: 756e 6972 6566 3530 2c20 6369 6661 7231  uniref50, cifar1
-00000700: 3030 2063 6f6e 7461 696e 7320 6e6f 2074  00 contains no t
-00000710: 6573 7420 6572 726f 722e 5472 0100 0000  est error.Tr....
-00000720: 7223 0000 0029 0272 2600 0000 7228 0000  r#...).r&...r(..
-00000730: 0072 2900 0000 722a 0000 0072 2600 0000  .r)...r*...r&...
-00000740: 722b 0000 0072 2c00 0000 7228 0000 0072  r+...r,...r(...r
-00000750: 2d00 0000 722e 0000 004e 722f 0000 0072  -...r....Nr/...r
-00000760: 2000 0000 7220 0000 0072 2000 0000 7221   ...r ...r ...r!
-00000770: 0000 0072 3200 0000 3400 0000 7312 0000  ...r2...4...s...
-00000780: 000a 0004 0210 0310 010e fe0c 040c 0108  ................
-00000790: 020c 0172 3200 0000 da01 5229 01da 0562  ...r2.....R)...b
-000007a0: 6f75 6e64 6300 0000 0000 0000 0000 0000  oundc...........
-000007b0: 0000 0000 0007 0000 0000 0000 0173 bc00  .............s..
-000007c0: 0000 6500 5a01 6400 5a02 5500 6401 6503  ..e.Z.d.Z.U.d.e.
-000007d0: 6402 3c00 0900 6403 6503 6404 3c00 0900  d.<...d.e.d.<...
-000007e0: 6405 6503 6406 3c00 0900 6407 6407 6407  d.e.d.<...d.d.d.
-000007f0: 6407 6407 6407 6408 9c06 6438 8700 6601  d.d.d.d...d8..f.
-00000800: 6414 6415 840e 5a04 6439 6418 6419 8404  d.d...Z.d9d.d...
-00000810: 5a05 6506 643a 641b 641c 8404 8301 5a07  Z.e.d:d.d.....Z.
-00000820: 6506 643b 641e 641f 8404 8301 5a08 6506  e.d;d.d.....Z.e.
-00000830: 643c 6421 6422 8404 8301 5a09 650a 643d  d<d!d"....Z.e.d=
-00000840: 6428 6429 8404 8301 5a0b 650a 643e 642e  d(d)....Z.e.d>d.
-00000850: 642f 8404 8301 5a0c 643f 6433 6434 8404  d/....Z.d?d3d4..
-00000860: 5a0d 650e 650f 6440 6441 6436 6437 8405  Z.e.e.d@dAd6d7..
-00000870: 8301 8301 5a10 8700 0400 5a11 5300 2942  ....Z.....Z.S.)B
-00000880: da0c 5044 3142 656e 6368 6d61 726b 7a1e  ..PD1Benchmarkz.
-00000890: 436c 6173 7356 6172 5b74 7570 6c65 5b69  ClassVar[tuple[i
-000008a0: 6e74 2c20 696e 742c 2069 6e74 5d5d da12  nt, int, int]]..
-000008b0: 7064 315f 6669 6465 6c69 7479 5f72 616e  pd1_fidelity_ran
-000008c0: 6765 722b 0000 00da 0870 6431 5f6e 616d  ger+.....pd1_nam
-000008d0: 657a 0774 7970 655b 525d da0f 7064 315f  ez.type[R]..pd1_
-000008e0: 7265 7375 6c74 5f74 7970 654e 2906 da07  result_typeN)...
-000008f0: 6461 7461 6469 72da 0473 6565 64da 0570  datadir..seed..p
-00000900: 7269 6f72 da0d 7065 7274 7572 625f 7072  rior..perturb_pr
-00000910: 696f 72da 0c76 616c 7565 5f6d 6574 7269  ior..value_metri
-00000920: 63da 0b63 6f73 745f 6d65 7472 6963 7239  c..cost_metricr9
-00000930: 0000 00fa 1173 7472 207c 2050 6174 6820  .....str | Path 
-00000940: 7c20 4e6f 6e65 723a 0000 00fa 0a69 6e74  | Noner:.....int
-00000950: 207c 204e 6f6e 6572 3b00 0000 fa31 7374   | Noner;....1st
-00000960: 7220 7c20 5061 7468 207c 2050 4431 436f  r | Path | PD1Co
-00000970: 6e66 6967 207c 204d 6170 7069 6e67 5b73  nfig | Mapping[s
-00000980: 7472 2c20 416e 795d 207c 204e 6f6e 6572  tr, Any] | Noner
-00000990: 3c00 0000 fa0c 666c 6f61 7420 7c20 4e6f  <.....float | No
-000009a0: 6e65 723d 0000 00fa 0a73 7472 207c 204e  ner=.....str | N
-000009b0: 6f6e 6572 3e00 0000 6301 0000 0000 0000  oner>...c.......
-000009c0: 0006 0000 0009 0000 000d 0000 0003 0000  ................
-000009d0: 0173 9000 0000 7c00 6a00 7d07 7c07 6a01  .s....|.j.}.|.j.
-000009e0: 7c02 6401 8d01 7d08 7c01 6402 7500 7211  |.d...}.|.d.u.r.
-000009f0: 7402 a003 a100 7d01 7404 7c01 7405 8302  t.....}.t.|.t...
-00000a00: 721a 7406 7c01 8301 6e01 7c01 7d01 7c01  r.t.|...n.|.}.|.
-00000a10: a007 a100 732c 7408 6403 7c01 9b00 6404  ....s,t.d.|...d.
-00000a20: 7c01 6a09 9b00 6405 9d05 8301 8201 6402  |.j...d.......d.
-00000a30: 7c00 5f0a 7c01 7c00 5f0b 740c 8300 6a0d  |._.|.|._.t...j.
-00000a40: 7c02 7c00 6a0e 740f 7410 7c07 6a11 7c07  |.|.j.t.t.|.j.|.
-00000a50: 6a12 7c03 7c04 7c08 7c05 7c06 6406 8d0b  j.|.|.|.|.|.d...
-00000a60: 0100 6402 5300 2907 61db 0200 0043 7265  ..d.S.).a....Cre
-00000a70: 6174 6520 6120 5044 3120 4265 6e63 686d  ate a PD1 Benchm
-00000a80: 6172 6b2e 0a0a 2020 2020 2020 2020 4172  ark...        Ar
-00000a90: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00000aa0: 6461 7461 6469 723a 2050 6174 6820 746f  datadir: Path to
-00000ab0: 2074 6865 2064 6174 6120 6469 7265 6374   the data direct
-00000ac0: 6f72 790a 2020 2020 2020 2020 2020 2020  ory.            
-00000ad0: 7365 6564 3a20 5468 6520 7365 6564 2074  seed: The seed t
-00000ae0: 6f20 7573 6520 666f 7220 7468 6520 7370  o use for the sp
-00000af0: 6163 650a 2020 2020 2020 2020 2020 2020  ace.            
-00000b00: 7072 696f 723a 2041 6e79 2070 7269 6f72  prior: Any prior
-00000b10: 2074 6f20 7573 6520 666f 7220 7468 6520   to use for the 
-00000b20: 6265 6e63 686d 6172 6b0a 2020 2020 2020  benchmark.      
-00000b30: 2020 2020 2020 7065 7274 7572 625f 7072        perturb_pr
-00000b40: 696f 723a 2057 6865 7468 6572 2074 6f20  ior: Whether to 
-00000b50: 7065 7274 7572 6220 7468 6520 7072 696f  perturb the prio
-00000b60: 722e 2049 6620 7370 6563 6966 6965 642c  r. If specified,
-00000b70: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
-00000b80: 2020 2020 2020 6973 2069 6e74 6572 7072        is interpr
-00000b90: 6574 6564 2061 7320 7468 6520 7374 6420  eted as the std 
-00000ba0: 6f66 2061 206e 6f72 6d61 6c20 6672 6f6d  of a normal from
-00000bb0: 2077 6869 6368 2074 6f20 7065 7274 7572   which to pertur
-00000bc0: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
-00000bd0: 2020 6e75 6d65 7269 6361 6c20 6879 7065    numerical hype
-00000be0: 7270 6172 616d 6574 6572 7320 6f66 2074  rparameters of t
-00000bf0: 6865 2070 7269 6f72 2c20 616e 6420 7468  he prior, and th
-00000c00: 6520 7261 7720 7072 6f62 6162 696c 6974  e raw probabilit
-00000c10: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-00000c20: 2020 6f66 2073 7761 7070 696e 6720 6120    of swapping a 
-00000c30: 6361 7465 676f 7269 6361 6c20 7661 6c75  categorical valu
-00000c40: 652e 0a20 2020 2020 2020 2020 2020 2076  e..            v
-00000c50: 616c 7565 5f6d 6574 7269 633a 2054 6865  alue_metric: The
-00000c60: 206d 6574 7269 6320 746f 2075 7365 2066   metric to use f
-00000c70: 6f72 2074 6869 7320 6265 6e63 686d 6172  or this benchmar
-00000c80: 6b2e 2055 7365 730a 2020 2020 2020 2020  k. Uses.        
-00000c90: 2020 2020 2020 2020 7468 6520 6465 6661          the defa
-00000ca0: 756c 7420 6d65 7472 6963 2066 726f 6d20  ult metric from 
-00000cb0: 7468 6520 5265 7375 6c74 2069 6620 4e6f  the Result if No
-00000cc0: 6e65 2e0a 2020 2020 2020 2020 2020 2020  ne..            
-00000cd0: 636f 7374 5f6d 6574 7269 633a 2054 6865  cost_metric: The
-00000ce0: 2063 6f73 7420 746f 2075 7365 2066 6f72   cost to use for
-00000cf0: 2074 6869 7320 6265 6e63 686d 6172 6b2e   this benchmark.
-00000d00: 2055 7365 730a 2020 2020 2020 2020 2020   Uses.          
-00000d10: 2020 2020 2020 7468 6520 6465 6661 756c        the defaul
-00000d20: 7420 636f 7374 2066 726f 6d20 7468 6520  t cost from the 
-00000d30: 5265 7375 6c74 2069 6620 4e6f 6e65 2e0a  Result if None..
-00000d40: 2020 2020 2020 2020 2901 723a 0000 004e          ).r:...N
-00000d50: 7a15 4361 6e27 7420 6669 6e64 2066 6f6c  z.Can't find fol
-00000d60: 6465 7220 6174 207a 332e 0a60 7079 7468  der at z3..`pyth
-00000d70: 6f6e 202d 6d20 6d66 7062 656e 6368 2064  on -m mfpbench d
-00000d80: 6f77 6e6c 6f61 6420 2d2d 7374 6174 7573  ownload --status
-00000d90: 202d 2d64 6174 612d 6469 7220 fa01 6029   --data-dir ..`)
-00000da0: 0b72 3a00 0000 da04 6e61 6d65 da0b 636f  .r:.....name..co
-00000db0: 6e66 6967 5f74 7970 65da 0d66 6964 656c  nfig_type..fidel
-00000dc0: 6974 795f 6e61 6d65 da0e 6669 6465 6c69  ity_name..fideli
-00000dd0: 7479 5f72 616e 6765 da0b 7265 7375 6c74  ty_range..result
-00000de0: 5f74 7970 6572 3b00 0000 723c 0000 00da  _typer;...r<....
-00000df0: 0573 7061 6365 723d 0000 0072 3e00 0000  .spacer=...r>...
-00000e00: 2913 da09 5f5f 636c 6173 735f 5fda 0d5f  )...__class__.._
-00000e10: 6372 6561 7465 5f73 7061 6365 7211 0000  create_spacer...
-00000e20: 00da 1064 6566 6175 6c74 5f6c 6f63 6174  ...default_locat
-00000e30: 696f 6eda 0a69 7369 6e73 7461 6e63 65da  ion..isinstance.
-00000e40: 0373 7472 7205 0000 00da 0665 7869 7374  .strr......exist
-00000e50: 73da 1146 696c 654e 6f74 466f 756e 6445  s..FileNotFoundE
-00000e60: 7272 6f72 da06 7061 7265 6e74 da0b 5f73  rror..parent.._s
-00000e70: 7572 726f 6761 7465 7372 3900 0000 da05  urrogatesr9.....
-00000e80: 7375 7065 72da 085f 5f69 6e69 745f 5f72  super..__init__r
-00000e90: 3700 0000 7219 0000 00da 1150 4431 5f46  7...r......PD1_F
-00000ea0: 4944 454c 4954 595f 4e41 4d45 7236 0000  IDELITY_NAMEr6..
-00000eb0: 0072 3800 0000 2909 da04 7365 6c66 7239  .r8...)...selfr9
-00000ec0: 0000 0072 3a00 0000 723b 0000 0072 3c00  ...r:...r;...r<.
-00000ed0: 0000 723d 0000 0072 3e00 0000 da03 636c  ..r=...r>.....cl
-00000ee0: 7372 4a00 0000 a901 724b 0000 0072 2000  srJ.....rK...r .
-00000ef0: 0000 7221 0000 0072 5500 0000 5000 0000  ..r!...rU...P...
-00000f00: 7334 0000 0006 190c 0108 0108 0116 0208  s4..............
-00000f10: 0102 0108 0104 0106 ff04 ff06 0406 0106  ................
-00000f20: 0202 0104 0102 0102 0104 0104 0102 0102  ................
-00000f30: 0102 0102 0102 010a f57a 1550 4431 4265  .........z.PD1Be
-00000f40: 6e63 686d 6172 6b2e 5f5f 696e 6974 5f5f  nchmark.__init__
-00000f50: da06 7265 7475 726e da04 4e6f 6e65 6301  ..return..Nonec.
-00000f60: 0000 0000 0000 0000 0000 0002 0000 0001  ................
-00000f70: 0000 0043 0000 0173 0a00 0000 7c00 6a00  ...C...s....|.j.
-00000f80: 7d01 6401 5300 2902 7a13 4c6f 6164 2074  }.d.S.).z.Load t
-00000f90: 6865 2062 656e 6368 6d61 726b 2e4e 2901  he benchmark.N).
-00000fa0: da0a 7375 7272 6f67 6174 6573 2902 7257  ..surrogates).rW
-00000fb0: 0000 00da 015f 7220 0000 0072 2000 0000  ....._r ...r ...
-00000fc0: 7221 0000 00da 046c 6f61 6485 0000 0073  r!.....load....s
-00000fd0: 0200 0000 0a02 7a11 5044 3142 656e 6368  ......z.PD1Bench
-00000fe0: 6d61 726b 2e6c 6f61 64fa 1764 6963 745b  mark.load..dict[
-00000ff0: 7374 722c 2058 4742 5265 6772 6573 736f  str, XGBRegresso
-00001000: 725d 6301 0000 0000 0000 0000 0000 0005  r]c.............
-00001010: 0000 0006 0000 0043 0000 0173 7000 0000  .......C...sp...
-00001020: 7c00 6a00 6401 7500 7235 6402 6403 6c01  |.j.d.u.r5d.d.l.
-00001030: 6d02 7d01 0100 6900 7c00 5f00 7c00 6a03  m.}...i.|._.|.j.
-00001040: a004 a100 4400 5d21 5c02 7d02 7d03 7c03  ....D.]!\.}.}.|.
-00001050: a005 a100 7327 7406 6404 7c03 9b00 6405  ....s't.d.|...d.
-00001060: 7c00 6a07 6a08 9b00 9d04 8301 8201 7c01  |.j.j.........|.
-00001070: 8300 7d04 7c04 a009 7c03 a101 0100 7c04  ..}.|...|.....|.
-00001080: 7c00 6a00 7c02 3c00 7113 7c00 6a00 5300  |.j.|.<.q.|.j.S.
-00001090: 2906 7a32 5468 6520 7375 7272 6f67 6174  ).z2The surrogat
-000010a0: 6573 2066 6f72 2074 6869 7320 6265 6e63  es for this benc
-000010b0: 686d 6172 6b2c 206f 6e65 2070 6572 206d  hmark, one per m
-000010c0: 6574 7269 632e 4e72 0100 0000 7213 0000  etric.Nr....r...
-000010d0: 007a 1843 616e 2774 2066 696e 6420 7375  .z.Can't find su
-000010e0: 7272 6f67 6174 6520 6174 207a 342e 0a60  rrogate at z4..`
-000010f0: 7079 7468 6f6e 202d 6d20 6d66 7062 656e  python -m mfpben
-00001100: 6368 2064 6f77 6e6c 6f61 6420 2d2d 7374  ch download --st
-00001110: 6174 7573 202d 2d64 6174 612d 6469 7220  atus --data-dir 
-00001120: 2029 0a72 5300 0000 da07 7867 626f 6f73   ).rS.....xgboos
-00001130: 7472 1400 0000 da0f 7375 7272 6f67 6174  tr......surrogat
-00001140: 655f 7061 7468 73da 0569 7465 6d73 7250  e_paths..itemsrP
-00001150: 0000 0072 5100 0000 7239 0000 0072 5200  ...rQ...r9...rR.
-00001160: 0000 5a0a 6c6f 6164 5f6d 6f64 656c 2905  ..Z.load_model).
-00001170: 7257 0000 0072 1400 0000 da06 6d65 7472  rW...r......metr
-00001180: 6963 da04 7061 7468 da05 6d6f 6465 6c72  ic..path..modelr
-00001190: 2000 0000 7220 0000 0072 2100 0000 725c   ...r ...r!...r\
-000011a0: 0000 0089 0000 0073 1c00 0000 0a03 0c01  .......s........
-000011b0: 0602 1201 0801 0201 0801 0602 04fe 04ff  ................
-000011c0: 0605 0a01 0c01 0602 7a17 5044 3142 656e  ........z.PD1Ben
-000011d0: 6368 6d61 726b 2e73 7572 726f 6761 7465  chmark.surrogate
-000011e0: 7372 0500 0000 6301 0000 0000 0000 0000  sr....c.........
-000011f0: 0000 0001 0000 0002 0000 0043 0000 0173  ...........C...s
-00001200: 0a00 0000 7c00 6a00 6401 1b00 5300 2902  ....|.j.d...S.).
-00001210: 7a2e 5468 6520 6469 7265 6374 6f72 7920  z.The directory 
-00001220: 7768 6572 6520 7468 6520 7375 7272 6f67  where the surrog
-00001230: 6174 6573 2061 7265 2073 746f 7265 642e  ates are stored.
-00001240: 725c 0000 0029 0172 3900 0000 a901 7257  r\...).r9.....rW
-00001250: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00001260: 0000 da0d 7375 7272 6f67 6174 655f 6469  ....surrogate_di
-00001270: 729d 0000 0073 0200 0000 0a03 7a1a 5044  r....s......z.PD
-00001280: 3142 656e 6368 6d61 726b 2e73 7572 726f  1Benchmark.surro
-00001290: 6761 7465 5f64 6972 fa0f 6469 6374 5b73  gate_dir..dict[s
-000012a0: 7472 2c20 5061 7468 5d63 0100 0000 0000  tr, Path]c......
-000012b0: 0000 0000 0000 0100 0000 0300 0000 0300  ................
-000012c0: 0001 7316 0000 0087 0066 0164 0164 0284  ..s......f.d.d..
-000012d0: 0888 006a 006a 0144 0083 0153 0029 037a  ...j.j.D...S.).z
-000012e0: 1c54 6865 2070 6174 6873 2074 6f20 7468  .The paths to th
-000012f0: 6520 7375 7272 6f67 6174 6573 2e63 0100  e surrogates.c..
-00001300: 0000 0000 0000 0000 0000 0200 0000 0800  ................
-00001310: 0000 1300 0001 7326 0000 0069 007c 005d  ......s&...i.|.]
-00001320: 0f7d 017c 0188 006a 0088 006a 019b 0064  .}.|...j...j...d
-00001330: 007c 019b 0064 019d 041b 0093 0271 0253  .|...d.......q.S
-00001340: 0029 02fa 012d 7a05 2e6a 736f 6e29 0272  .)...-z..json).r
-00001350: 6700 0000 7245 0000 0029 02da 022e 3072  g...rE...)....0r
-00001360: 6300 0000 7266 0000 0072 2000 0000 7221  c...rf...r ...r!
-00001370: 0000 00da 0a3c 6469 6374 636f 6d70 3ea5  .....<dictcomp>.
-00001380: 0000 0073 0800 0000 0600 0202 18ff 06ff  ...s............
-00001390: 7a30 5044 3142 656e 6368 6d61 726b 2e73  z0PD1Benchmark.s
-000013a0: 7572 726f 6761 7465 5f70 6174 6873 2e3c  urrogate_paths.<
-000013b0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
-000013c0: 703e 2902 7210 0000 0072 2a00 0000 7266  p>).r....r*...rf
-000013d0: 0000 0072 2000 0000 7266 0000 0072 2100  ...r ...rf...r!.
-000013e0: 0000 7261 0000 00a2 0000 0073 0600 0000  ..ra.......s....
-000013f0: 0a03 0602 06fe 7a1c 5044 3142 656e 6368  ......z.PD1Bench
-00001400: 6d61 726b 2e73 7572 726f 6761 7465 5f70  mark.surrogate_p
-00001410: 6174 6873 da06 636f 6e66 6967 fa11 4d61  aths..config..Ma
-00001420: 7070 696e 675b 7374 722c 2041 6e79 5dda  pping[str, Any].
-00001430: 0261 74da 0369 6e74 fa10 6469 6374 5b73  .at..int..dict[s
-00001440: 7472 2c20 666c 6f61 745d 6303 0000 0000  tr, float]c.....
-00001450: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00001460: 0000 0173 1400 0000 7c00 6a00 7c01 7c02  ...s....|.j.|.|.
-00001470: 6701 6401 8d02 6402 1900 5300 2903 4e29  g.d...d...S.).N)
-00001480: 01da 0a66 6964 656c 6974 6965 7372 0100  ...fidelitiesr..
-00001490: 0000 2901 da0c 5f72 6573 756c 7473 5f66  ..)..._results_f
-000014a0: 6f72 2903 7257 0000 0072 6c00 0000 726e  or).rW...rl...rn
-000014b0: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-000014c0: 0000 da13 5f6f 626a 6563 7469 7665 5f66  ...._objective_f
-000014d0: 756e 6374 696f 6eaa 0000 0073 0200 0000  unction....s....
-000014e0: 1406 7a20 5044 3142 656e 6368 6d61 726b  ..z PD1Benchmark
-000014f0: 2e5f 6f62 6a65 6374 6976 655f 6675 6e63  ._objective_func
-00001500: 7469 6f6e da03 6672 6dda 0274 6fda 0473  tion..frm..to..s
-00001510: 7465 70fa 2949 7465 7261 626c 655b 7475  tep.)Iterable[tu
-00001520: 706c 655b 696e 742c 204d 6170 7069 6e67  ple[int, Mapping
-00001530: 5b73 7472 2c20 666c 6f61 745d 5d5d 6302  [str, float]]]c.
-00001540: 0000 0000 0000 0003 0000 0006 0000 0006  ................
-00001550: 0000 0043 0000 0173 2400 0000 7400 7c00  ...C...s$...t.|.
-00001560: a001 7c02 7c03 7c04 a103 8301 7d05 7402  ..|.|.|.....}.t.
-00001570: 7c05 7c00 a003 7c01 7c05 a102 8302 5300  |.|...|.|.....S.
-00001580: a901 4e29 04da 046c 6973 74da 0f69 7465  ..N)...list..ite
-00001590: 725f 6669 6465 6c69 7469 6573 da03 7a69  r_fidelities..zi
-000015a0: 7072 7200 0000 2906 7257 0000 0072 6c00  prr...).rW...rl.
-000015b0: 0000 7274 0000 0072 7500 0000 7276 0000  ..rt...ru...rv..
-000015c0: 0072 7100 0000 7220 0000 0072 2000 0000  .rq...r ...r ...
-000015d0: 7221 0000 00da 0b5f 7472 616a 6563 746f  r!....._trajecto
-000015e0: 7279 b200 0000 7304 0000 0012 0912 017a  ry....s........z
-000015f0: 1850 4431 4265 6e63 686d 6172 6b2e 5f74  .PD1Benchmark._t
-00001600: 7261 6a65 6374 6f72 7972 7100 0000 fa0d  rajectoryrq.....
-00001610: 4974 6572 6162 6c65 5b69 6e74 5dfa 166c  Iterable[int]..l
-00001620: 6973 745b 6469 6374 5b73 7472 2c20 666c  ist[dict[str, fl
-00001630: 6f61 745d 5d63 0300 0000 0000 0000 0000  oat]]c..........
-00001640: 0000 0800 0000 0500 0000 0300 0001 737e  ..............s~
-00001650: 0000 0074 007c 0183 0189 0087 0087 0266  ...t.|.........f
-00001660: 0264 0164 0284 087c 0244 0083 017d 0374  .d.d...|.D...}.t
-00001670: 01a0 027c 03a1 017d 047c 046a 037d 0588  ...|...}.|.j.}..
-00001680: 026a 04a0 05a1 0044 005d 115c 027d 067d  .j.....D.].\.}.}
-00001690: 077c 07a0 067c 047c 0519 00a1 016a 0764  .|...|.|.....j.d
-000016a0: 0364 048d 017c 047c 063c 0071 1b74 0888  .d...|.|.<.q.t..
-000016b0: 026a 04a0 09a1 0083 0189 0187 0166 0164  .j...........f.d
-000016c0: 0564 0284 087c 04a0 0aa1 0044 0083 0153  .d...|.....D...S
-000016d0: 0029 064e 6301 0000 0000 0000 0000 0000  .).Nc...........
-000016e0: 0002 0000 0005 0000 0013 0000 0173 1e00  .............s..
-000016f0: 0000 6700 7c00 5d0b 7d01 6900 8800 a501  ..g.|.].}.i.....
-00001700: 8801 6a00 7c01 6901 a501 9102 7102 5300  ..j.|.i.....q.S.
-00001710: 7220 0000 0029 0172 4700 0000 2902 726a  r ...).rG...).rj
-00001720: 0000 00da 0166 2902 da01 6372 5700 0000  .....f)...crW...
-00001730: 7220 0000 0072 2100 0000 da0a 3c6c 6973  r ...r!.....<lis
-00001740: 7463 6f6d 703e c500 0000 7302 0000 001e  tcomp>....s.....
-00001750: 007a 2d50 4431 4265 6e63 686d 6172 6b2e  .z-PD1Benchmark.
-00001760: 5f72 6573 756c 7473 5f66 6f72 2e3c 6c6f  _results_for.<lo
-00001770: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00001780: 7201 0000 0029 01da 036d 696e 6301 0000  r....)...minc...
-00001790: 0000 0000 0000 0000 0003 0000 0005 0000  ................
-000017a0: 0013 0000 0173 1c00 0000 6700 7c00 5d0a  .....s....g.|.].
-000017b0: 5c02 7d01 7d02 7400 7c02 8800 1900 8301  \.}.}.t.|.......
-000017c0: 9102 7102 5300 7220 0000 0029 01da 0464  ..q.S.r ...)...d
-000017d0: 6963 7429 0372 6a00 0000 725d 0000 00da  ict).rj...r]....
-000017e0: 0172 2901 da07 6d65 7472 6963 7372 2000  .r)...metricsr .
-000017f0: 0000 7221 0000 0072 8100 0000 cf00 0000  ..r!...r........
-00001800: 7302 0000 001c 0029 0b72 8300 0000 da02  s......).r......
-00001810: 7064 da09 4461 7461 4672 616d 65da 0763  pd..DataFrame..c
-00001820: 6f6c 756d 6e73 725c 0000 0072 6200 0000  olumnsr\...rb...
-00001830: 5a07 7072 6564 6963 74da 0463 6c69 7072  Z.predict..clipr
-00001840: 7900 0000 da04 6b65 7973 da08 6974 6572  y.....keys..iter
-00001850: 726f 7773 2908 7257 0000 0072 6c00 0000  rows).rW...rl...
-00001860: 7271 0000 005a 0771 7565 7269 6573 da02  rq...Z.queries..
-00001870: 7873 da08 6665 6174 7572 6573 7263 0000  xs..featuresrc..
-00001880: 005a 0973 7572 726f 6761 7465 7220 0000  .Z.surrogater ..
-00001890: 0029 0372 8000 0000 7285 0000 0072 5700  .).r....r....rW.
-000018a0: 0000 7221 0000 0072 7200 0000 be00 0000  ..r!...rr.......
-000018b0: 7310 0000 0008 0614 010a 0106 0312 011c  s...............
-000018c0: 020e 0216 017a 1950 4431 4265 6e63 686d  .....z.PD1Benchm
-000018d0: 6172 6b2e 5f72 6573 756c 7473 5f66 6f72  ark._results_for
-000018e0: 7212 0000 0063 0200 0000 0000 0000 0000  r....c..........
-000018f0: 0000 0200 0000 0100 0000 4300 0001 7304  ..........C...s.
-00001900: 0000 0064 0053 0072 7800 0000 7220 0000  ...d.S.rx...r ..
-00001910: 0029 0272 5800 0000 723a 0000 0072 2000  .).rX...r:...r .
-00001920: 0000 7220 0000 0072 2100 0000 724c 0000  ..r ...r!...rL..
-00001930: 00d1 0000 0073 0200 0000 0403 7a1a 5044  .....s......z.PD
-00001940: 3142 656e 6368 6d61 726b 2e5f 6372 6561  1Benchmark._crea
-00001950: 7465 5f73 7061 6365 290c 7239 0000 0072  te_space).r9...r
-00001960: 3f00 0000 723a 0000 0072 4000 0000 723b  ?...r:...r@...r;
-00001970: 0000 0072 4100 0000 723c 0000 0072 4200  ...rA...r<...rB.
-00001980: 0000 723d 0000 0072 4300 0000 723e 0000  ..r=...rC...r>..
-00001990: 0072 4300 0000 2902 725a 0000 0072 5b00  .rC...).rZ...r[.
-000019a0: 0000 2902 725a 0000 0072 5f00 0000 2902  ..).rZ...r_...).
-000019b0: 725a 0000 0072 0500 0000 2902 725a 0000  rZ...r....).rZ..
-000019c0: 0072 6800 0000 2906 726c 0000 0072 6d00  .rh...).rl...rm.
-000019d0: 0000 726e 0000 0072 6f00 0000 725a 0000  ..rn...ro...rZ..
-000019e0: 0072 7000 0000 290a 726c 0000 0072 6d00  .rp...).rl...rm.
-000019f0: 0000 7274 0000 0072 6f00 0000 7275 0000  ..rt...ro...ru..
-00001a00: 0072 6f00 0000 7276 0000 0072 6f00 0000  .ro...rv...ro...
-00001a10: 725a 0000 0072 7700 0000 2906 726c 0000  rZ...rw...).rl..
-00001a20: 0072 6d00 0000 7271 0000 0072 7d00 0000  .rm...rq...r}...
-00001a30: 725a 0000 0072 7e00 0000 7278 0000 0029  rZ...r~...rx...)
-00001a40: 0472 3a00 0000 7240 0000 0072 5a00 0000  .r:...r@...rZ...
-00001a50: 7212 0000 0029 1272 1b00 0000 721c 0000  r....).r....r...
-00001a60: 0072 1d00 0000 721f 0000 0072 5500 0000  .r....r....rU...
-00001a70: 725e 0000 00da 0870 726f 7065 7274 7972  r^.....propertyr
-00001a80: 5c00 0000 7267 0000 0072 6100 0000 720c  \...rg...ra...r.
-00001a90: 0000 0072 7300 0000 727c 0000 0072 7200  ...rs...r|...rr.
-00001aa0: 0000 da0b 636c 6173 736d 6574 686f 6472  ....classmethodr
-00001ab0: 0300 0000 724c 0000 00da 0d5f 5f63 6c61  ....rL.....__cla
-00001ac0: 7373 6365 6c6c 5f5f 7220 0000 0072 2000  sscell__r ...r .
-00001ad0: 0000 7259 0000 0072 2100 0000 7235 0000  ..rY...r!...r5..
-00001ae0: 0046 0000 0073 3a00 0000 0a00 0801 0201  .F...s:.........
-00001af0: 0802 0201 0802 0201 0205 0201 0201 0201  ................
-00001b00: 0201 0201 12f8 0a35 0204 0c01 0213 0c01  .......5........
-00001b10: 0204 0c01 0207 0c01 0207 0c01 0a0b 0213  ................
-00001b20: 0201 1801 7235 0000 0029 2ada 0a5f 5f66  ....r5...)*..__f
-00001b30: 7574 7572 655f 5f72 0200 0000 da03 6162  uture__r......ab
-00001b40: 6372 0300 0000 da0b 6461 7461 636c 6173  cr......dataclas
-00001b50: 7365 7372 0400 0000 da07 7061 7468 6c69  sesr......pathli
-00001b60: 6272 0500 0000 da06 7479 7069 6e67 7206  br......typingr.
-00001b70: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00001b80: 0000 720a 0000 0072 0b00 0000 da11 7479  ..r....r......ty
-00001b90: 7069 6e67 5f65 7874 656e 7369 6f6e 7372  ping_extensionsr
-00001ba0: 0c00 0000 da05 6e75 6d70 7972 3000 0000  ......numpyr0...
-00001bb0: da06 7061 6e64 6173 7286 0000 00da 126d  ..pandasr......m
-00001bc0: 6670 6265 6e63 682e 6265 6e63 686d 6172  fpbench.benchmar
-00001bd0: 6b72 0d00 0000 da0f 6d66 7062 656e 6368  kr......mfpbench
-00001be0: 2e63 6f6e 6669 6772 0e00 0000 da0f 6d66  .configr......mf
-00001bf0: 7062 656e 6368 2e6d 6574 7269 6372 0f00  pbench.metricr..
-00001c00: 0000 da0f 6d66 7062 656e 6368 2e72 6573  ....mfpbench.res
-00001c10: 756c 7472 1000 0000 da18 6d66 7062 656e  ultr......mfpben
-00001c20: 6368 2e73 6574 7570 5f62 656e 6368 6d61  ch.setup_benchma
-00001c30: 726b 7211 0000 00da 0b43 6f6e 6669 6753  rkr......ConfigS
-00001c40: 7061 6365 7212 0000 0072 6000 0000 7214  pacer....r`...r.
-00001c50: 0000 0072 5600 0000 7219 0000 0072 6f00  ...rV...r....ro.
-00001c60: 0000 7222 0000 0072 3200 0000 7233 0000  ..r"...r2...r3..
-00001c70: 0072 3500 0000 7220 0000 0072 2000 0000  .r5...r ...r ...
-00001c80: 7220 0000 0072 2100 0000 da08 3c6d 6f64  r ...r!.....<mod
-00001c90: 756c 653e 0100 0000 7332 0000 000c 000c  ule>....s2......
-00001ca0: 020c 010c 0120 010c 0108 0208 010c 020c  ..... ..........
-00001cb0: 010c 010c 010c 0104 020c 010c 0104 020c  ................
-00001cc0: 0312 0108 091a 0108 101a 010c 0e1e 03    ...............
+00000660: 0264 0364 048d 0265 0464 0264 0565 056a  .d.d...e.d.d.e.j
+00000670: 0666 0264 048d 0264 069c 025a 0764 0765  .f.d...d...Z.d.e
+00000680: 0864 083c 0064 095a 0964 0a65 0864 0b3c  .d.<.d.Z.d.e.d.<
+00000690: 0064 0c5a 0a64 0a65 0864 0d3c 0064 0e65  .d.Z.d.e.d.<.d.e
+000006a0: 0864 093c 0064 0e65 0864 0c3c 0064 0f53  .d.<.d.e.d.<.d.S
+000006b0: 0029 10da 1450 4431 5265 7375 6c74 5472  .)...PD1ResultTr
+000006c0: 616e 7366 6f72 6d65 727a 4949 6d61 6765  ansformerzIImage
+000006d0: 6e65 742c 206c 6d31 622c 2074 7261 6e73  net, lm1b, trans
+000006e0: 6c61 7465 5f77 6d74 2c20 756e 6972 6566  late_wmt, uniref
+000006f0: 3530 2c20 6369 6661 7231 3030 2063 6f6e  50, cifar100 con
+00000700: 7461 696e 7320 6e6f 2074 6573 7420 6572  tains no test er
+00000710: 726f 722e 5472 2300 0000 7225 0000 0072  ror.Tr#...r%...r
+00000720: 0100 0000 2902 7228 0000 0072 2a00 0000  ....).r(...r*...
+00000730: 722b 0000 0072 2c00 0000 7228 0000 0072  r+...r,...r(...r
+00000740: 2d00 0000 722e 0000 0072 2a00 0000 722f  -...r....r*...r/
+00000750: 0000 0072 3000 0000 4e72 3100 0000 7220  ...r0...Nr1...r 
+00000760: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
+00000770: 0000 7234 0000 0034 0000 0073 1200 0000  ..r4...4...s....
+00000780: 0a00 0402 0a03 1001 0efe 0c04 0c01 0802  ................
+00000790: 0c01 7234 0000 00da 0152 2901 da05 626f  ..r4.....R)...bo
+000007a0: 756e 6463 0000 0000 0000 0000 0000 0000  undc............
+000007b0: 0000 0000 0700 0000 0000 0001 73bc 0000  ............s...
+000007c0: 0065 005a 0164 005a 0255 0064 0165 0364  .e.Z.d.Z.U.d.e.d
+000007d0: 023c 0009 0064 0365 0364 043c 0009 0064  .<...d.e.d.<...d
+000007e0: 0565 0364 063c 0009 0064 0764 0764 0764  .e.d.<...d.d.d.d
+000007f0: 0764 0764 0764 089c 0664 3887 0066 0164  .d.d.d...d8..f.d
+00000800: 1464 1584 0e5a 0464 3964 1864 1984 045a  .d...Z.d9d.d...Z
+00000810: 0565 0664 3a64 1b64 1c84 0483 015a 0765  .e.d:d.d.....Z.e
+00000820: 0664 3b64 1e64 1f84 0483 015a 0865 0664  .d;d.d.....Z.e.d
+00000830: 3c64 2164 2284 0483 015a 0965 0a64 3d64  <d!d"....Z.e.d=d
+00000840: 2864 2984 0483 015a 0b65 0a64 3e64 2e64  (d)....Z.e.d>d.d
+00000850: 2f84 0483 015a 0c64 3f64 3364 3484 045a  /....Z.d?d3d4..Z
+00000860: 0d65 0e65 0f64 4064 4164 3664 3784 0583  .e.e.d@dAd6d7...
+00000870: 0183 015a 1087 0004 005a 1153 0029 42da  ...Z.....Z.S.)B.
+00000880: 0c50 4431 4265 6e63 686d 6172 6b7a 1e43  .PD1Benchmarkz.C
+00000890: 6c61 7373 5661 725b 7475 706c 655b 696e  lassVar[tuple[in
+000008a0: 742c 2069 6e74 2c20 696e 745d 5dda 1270  t, int, int]]..p
+000008b0: 6431 5f66 6964 656c 6974 795f 7261 6e67  d1_fidelity_rang
+000008c0: 6572 2d00 0000 da08 7064 315f 6e61 6d65  er-.....pd1_name
+000008d0: 7a07 7479 7065 5b52 5dda 0f70 6431 5f72  z.type[R]..pd1_r
+000008e0: 6573 756c 745f 7479 7065 4e29 06da 0764  esult_typeN)...d
+000008f0: 6174 6164 6972 da04 7365 6564 da05 7072  atadir..seed..pr
+00000900: 696f 72da 0d70 6572 7475 7262 5f70 7269  ior..perturb_pri
+00000910: 6f72 da0c 7661 6c75 655f 6d65 7472 6963  or..value_metric
+00000920: da0b 636f 7374 5f6d 6574 7269 6372 3b00  ..cost_metricr;.
+00000930: 0000 fa11 7374 7220 7c20 5061 7468 207c  ....str | Path |
+00000940: 204e 6f6e 6572 3c00 0000 fa0a 696e 7420   Noner<.....int 
+00000950: 7c20 4e6f 6e65 723d 0000 00fa 3173 7472  | Noner=....1str
+00000960: 207c 2050 6174 6820 7c20 5044 3143 6f6e   | Path | PD1Con
+00000970: 6669 6720 7c20 4d61 7070 696e 675b 7374  fig | Mapping[st
+00000980: 722c 2041 6e79 5d20 7c20 4e6f 6e65 723e  r, Any] | Noner>
+00000990: 0000 00fa 0c66 6c6f 6174 207c 204e 6f6e  .....float | Non
+000009a0: 6572 3f00 0000 fa0a 7374 7220 7c20 4e6f  er?.....str | No
+000009b0: 6e65 7240 0000 0063 0100 0000 0000 0000  ner@...c........
+000009c0: 0600 0000 0900 0000 0d00 0000 0300 0001  ................
+000009d0: 7390 0000 007c 006a 007d 077c 076a 017c  s....|.j.}.|.j.|
+000009e0: 0264 018d 017d 087c 0164 0275 0072 1174  .d...}.|.d.u.r.t
+000009f0: 02a0 03a1 007d 0174 047c 0174 0583 0272  .....}.t.|.t...r
+00000a00: 1a74 067c 0183 016e 017c 017d 017c 01a0  .t.|...n.|.}.|..
+00000a10: 07a1 0073 2c74 0864 037c 019b 0064 047c  ...s,t.d.|...d.|
+00000a20: 016a 099b 0064 059d 0583 0182 0164 027c  .j...d.......d.|
+00000a30: 005f 0a7c 017c 005f 0b74 0c83 006a 0d7c  ._.|.|._.t...j.|
+00000a40: 027c 006a 0e74 0f74 107c 076a 117c 076a  .|.j.t.t.|.j.|.j
+00000a50: 127c 037c 047c 087c 057c 0664 068d 0b01  .|.|.|.|.|.d....
+00000a60: 0064 0253 0029 0761 db02 0000 4372 6561  .d.S.).a....Crea
+00000a70: 7465 2061 2050 4431 2042 656e 6368 6d61  te a PD1 Benchma
+00000a80: 726b 2e0a 0a20 2020 2020 2020 2041 7267  rk...        Arg
+00000a90: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
+00000aa0: 6174 6164 6972 3a20 5061 7468 2074 6f20  atadir: Path to 
+00000ab0: 7468 6520 6461 7461 2064 6972 6563 746f  the data directo
+00000ac0: 7279 0a20 2020 2020 2020 2020 2020 2073  ry.            s
+00000ad0: 6565 643a 2054 6865 2073 6565 6420 746f  eed: The seed to
+00000ae0: 2075 7365 2066 6f72 2074 6865 2073 7061   use for the spa
+00000af0: 6365 0a20 2020 2020 2020 2020 2020 2070  ce.            p
+00000b00: 7269 6f72 3a20 416e 7920 7072 696f 7220  rior: Any prior 
+00000b10: 746f 2075 7365 2066 6f72 2074 6865 2062  to use for the b
+00000b20: 656e 6368 6d61 726b 0a20 2020 2020 2020  enchmark.       
+00000b30: 2020 2020 2070 6572 7475 7262 5f70 7269       perturb_pri
+00000b40: 6f72 3a20 5768 6574 6865 7220 746f 2070  or: Whether to p
+00000b50: 6572 7475 7262 2074 6865 2070 7269 6f72  erturb the prior
+00000b60: 2e20 4966 2073 7065 6369 6669 6564 2c20  . If specified, 
+00000b70: 7468 6973 0a20 2020 2020 2020 2020 2020  this.           
+00000b80: 2020 2020 2069 7320 696e 7465 7270 7265       is interpre
+00000b90: 7465 6420 6173 2074 6865 2073 7464 206f  ted as the std o
+00000ba0: 6620 6120 6e6f 726d 616c 2066 726f 6d20  f a normal from 
+00000bb0: 7768 6963 6820 746f 2070 6572 7475 7262  which to perturb
+00000bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000bd0: 206e 756d 6572 6963 616c 2068 7970 6572   numerical hyper
+00000be0: 7061 7261 6d65 7465 7273 206f 6620 7468  parameters of th
+00000bf0: 6520 7072 696f 722c 2061 6e64 2074 6865  e prior, and the
+00000c00: 2072 6177 2070 726f 6261 6269 6c69 7479   raw probability
+00000c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c20: 206f 6620 7377 6170 7069 6e67 2061 2063   of swapping a c
+00000c30: 6174 6567 6f72 6963 616c 2076 616c 7565  ategorical value
+00000c40: 2e0a 2020 2020 2020 2020 2020 2020 7661  ..            va
+00000c50: 6c75 655f 6d65 7472 6963 3a20 5468 6520  lue_metric: The 
+00000c60: 6d65 7472 6963 2074 6f20 7573 6520 666f  metric to use fo
+00000c70: 7220 7468 6973 2062 656e 6368 6d61 726b  r this benchmark
+00000c80: 2e20 5573 6573 0a20 2020 2020 2020 2020  . Uses.         
+00000c90: 2020 2020 2020 2074 6865 2064 6566 6175         the defau
+00000ca0: 6c74 206d 6574 7269 6320 6672 6f6d 2074  lt metric from t
+00000cb0: 6865 2052 6573 756c 7420 6966 204e 6f6e  he Result if Non
+00000cc0: 652e 0a20 2020 2020 2020 2020 2020 2063  e..            c
+00000cd0: 6f73 745f 6d65 7472 6963 3a20 5468 6520  ost_metric: The 
+00000ce0: 636f 7374 2074 6f20 7573 6520 666f 7220  cost to use for 
+00000cf0: 7468 6973 2062 656e 6368 6d61 726b 2e20  this benchmark. 
+00000d00: 5573 6573 0a20 2020 2020 2020 2020 2020  Uses.           
+00000d10: 2020 2020 2074 6865 2064 6566 6175 6c74       the default
+00000d20: 2063 6f73 7420 6672 6f6d 2074 6865 2052   cost from the R
+00000d30: 6573 756c 7420 6966 204e 6f6e 652e 0a20  esult if None.. 
+00000d40: 2020 2020 2020 2029 0172 3c00 0000 4e7a         ).r<...Nz
+00000d50: 1543 616e 2774 2066 696e 6420 666f 6c64  .Can't find fold
+00000d60: 6572 2061 7420 7a33 2e0a 6070 7974 686f  er at z3..`pytho
+00000d70: 6e20 2d6d 206d 6670 6265 6e63 6820 646f  n -m mfpbench do
+00000d80: 776e 6c6f 6164 202d 2d73 7461 7475 7320  wnload --status 
+00000d90: 2d2d 6461 7461 2d64 6972 20fa 0160 290b  --data-dir ..`).
+00000da0: 723c 0000 00da 046e 616d 65da 0b63 6f6e  r<.....name..con
+00000db0: 6669 675f 7479 7065 da0d 6669 6465 6c69  fig_type..fideli
+00000dc0: 7479 5f6e 616d 65da 0e66 6964 656c 6974  ty_name..fidelit
+00000dd0: 795f 7261 6e67 65da 0b72 6573 756c 745f  y_range..result_
+00000de0: 7479 7065 723d 0000 0072 3e00 0000 da05  typer=...r>.....
+00000df0: 7370 6163 6572 3f00 0000 7240 0000 0029  spacer?...r@...)
+00000e00: 13da 095f 5f63 6c61 7373 5f5f da0d 5f63  ...__class__.._c
+00000e10: 7265 6174 655f 7370 6163 6572 1100 0000  reate_spacer....
+00000e20: da10 6465 6661 756c 745f 6c6f 6361 7469  ..default_locati
+00000e30: 6f6e da0a 6973 696e 7374 616e 6365 da03  on..isinstance..
+00000e40: 7374 7272 0500 0000 da06 6578 6973 7473  strr......exists
+00000e50: da11 4669 6c65 4e6f 7446 6f75 6e64 4572  ..FileNotFoundEr
+00000e60: 726f 72da 0670 6172 656e 74da 0b5f 7375  ror..parent.._su
+00000e70: 7272 6f67 6174 6573 723b 0000 00da 0573  rrogatesr;.....s
+00000e80: 7570 6572 da08 5f5f 696e 6974 5f5f 7239  uper..__init__r9
+00000e90: 0000 0072 1900 0000 da11 5044 315f 4649  ...r......PD1_FI
+00000ea0: 4445 4c49 5459 5f4e 414d 4572 3800 0000  DELITY_NAMEr8...
+00000eb0: 723a 0000 0029 09da 0473 656c 6672 3b00  r:...)...selfr;.
+00000ec0: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
+00000ed0: 0072 3f00 0000 7240 0000 00da 0363 6c73  .r?...r@.....cls
+00000ee0: 724c 0000 00a9 0172 4d00 0000 7220 0000  rL.....rM...r ..
+00000ef0: 0072 2100 0000 7257 0000 0050 0000 0073  .r!...rW...P...s
+00000f00: 3400 0000 0619 0c01 0801 0801 1602 0801  4...............
+00000f10: 0201 0801 0401 06ff 04ff 0604 0601 0602  ................
+00000f20: 0201 0401 0201 0201 0401 0401 0201 0201  ................
+00000f30: 0201 0201 0201 0af5 7a15 5044 3142 656e  ........z.PD1Ben
+00000f40: 6368 6d61 726b 2e5f 5f69 6e69 745f 5fda  chmark.__init__.
+00000f50: 0672 6574 7572 6eda 044e 6f6e 6563 0100  .return..Nonec..
+00000f60: 0000 0000 0000 0000 0000 0200 0000 0100  ................
+00000f70: 0000 4300 0001 730a 0000 007c 006a 007d  ..C...s....|.j.}
+00000f80: 0164 0153 0029 027a 134c 6f61 6420 7468  .d.S.).z.Load th
+00000f90: 6520 6265 6e63 686d 6172 6b2e 4e29 01da  e benchmark.N)..
+00000fa0: 0a73 7572 726f 6761 7465 7329 0272 5900  .surrogates).rY.
+00000fb0: 0000 da01 5f72 2000 0000 7220 0000 0072  ...._r ...r ...r
+00000fc0: 2100 0000 da04 6c6f 6164 8500 0000 7302  !.....load....s.
+00000fd0: 0000 000a 027a 1150 4431 4265 6e63 686d  .....z.PD1Benchm
+00000fe0: 6172 6b2e 6c6f 6164 fa17 6469 6374 5b73  ark.load..dict[s
+00000ff0: 7472 2c20 5847 4252 6567 7265 7373 6f72  tr, XGBRegressor
+00001000: 5d63 0100 0000 0000 0000 0000 0000 0500  ]c..............
+00001010: 0000 0600 0000 4300 0001 7370 0000 007c  ......C...sp...|
+00001020: 006a 0064 0175 0072 3564 0264 036c 016d  .j.d.u.r5d.d.l.m
+00001030: 027d 0101 0069 007c 005f 007c 006a 03a0  .}...i.|._.|.j..
+00001040: 04a1 0044 005d 215c 027d 027d 037c 03a0  ...D.]!\.}.}.|..
+00001050: 05a1 0073 2774 0664 047c 039b 0064 057c  ...s't.d.|...d.|
+00001060: 006a 076a 089b 009d 0483 0182 017c 0183  .j.j.........|..
+00001070: 007d 047c 04a0 097c 03a1 0101 007c 047c  .}.|...|.....|.|
+00001080: 006a 007c 023c 0071 137c 006a 0053 0029  .j.|.<.q.|.j.S.)
+00001090: 067a 3254 6865 2073 7572 726f 6761 7465  .z2The surrogate
+000010a0: 7320 666f 7220 7468 6973 2062 656e 6368  s for this bench
+000010b0: 6d61 726b 2c20 6f6e 6520 7065 7220 6d65  mark, one per me
+000010c0: 7472 6963 2e4e 7201 0000 0072 1300 0000  tric.Nr....r....
+000010d0: 7a18 4361 6e27 7420 6669 6e64 2073 7572  z.Can't find sur
+000010e0: 726f 6761 7465 2061 7420 7a34 2e0a 6070  rogate at z4..`p
+000010f0: 7974 686f 6e20 2d6d 206d 6670 6265 6e63  ython -m mfpbenc
+00001100: 6820 646f 776e 6c6f 6164 202d 2d73 7461  h download --sta
+00001110: 7475 7320 2d2d 6461 7461 2d64 6972 2020  tus --data-dir  
+00001120: 290a 7255 0000 00da 0778 6762 6f6f 7374  ).rU.....xgboost
+00001130: 7214 0000 00da 0f73 7572 726f 6761 7465  r......surrogate
+00001140: 5f70 6174 6873 da05 6974 656d 7372 5200  _paths..itemsrR.
+00001150: 0000 7253 0000 0072 3b00 0000 7254 0000  ..rS...r;...rT..
+00001160: 005a 0a6c 6f61 645f 6d6f 6465 6c29 0572  .Z.load_model).r
+00001170: 5900 0000 7214 0000 00da 066d 6574 7269  Y...r......metri
+00001180: 63da 0470 6174 685a 056d 6f64 656c 7220  c..pathZ.modelr 
+00001190: 0000 0072 2000 0000 7221 0000 0072 5e00  ...r ...r!...r^.
+000011a0: 0000 8900 0000 731c 0000 000a 030c 0106  ......s.........
+000011b0: 0212 0108 0102 0108 0106 0204 fe04 ff06  ................
+000011c0: 050a 010c 0106 027a 1750 4431 4265 6e63  .......z.PD1Benc
+000011d0: 686d 6172 6b2e 7375 7272 6f67 6174 6573  hmark.surrogates
+000011e0: 7205 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000011f0: 0000 0100 0000 0200 0000 4300 0001 730a  ..........C...s.
+00001200: 0000 007c 006a 0064 011b 0053 0029 027a  ...|.j.d...S.).z
+00001210: 2e54 6865 2064 6972 6563 746f 7279 2077  .The directory w
+00001220: 6865 7265 2074 6865 2073 7572 726f 6761  here the surroga
+00001230: 7465 7320 6172 6520 7374 6f72 6564 2e72  tes are stored.r
+00001240: 5e00 0000 2901 723b 0000 00a9 0172 5900  ^...).r;.....rY.
+00001250: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
+00001260: 00da 0d73 7572 726f 6761 7465 5f64 6972  ...surrogate_dir
+00001270: 9d00 0000 7302 0000 000a 037a 1a50 4431  ....s......z.PD1
+00001280: 4265 6e63 686d 6172 6b2e 7375 7272 6f67  Benchmark.surrog
+00001290: 6174 655f 6469 72fa 0f64 6963 745b 7374  ate_dir..dict[st
+000012a0: 722c 2050 6174 685d 6301 0000 0000 0000  r, Path]c.......
+000012b0: 0000 0000 0001 0000 0003 0000 0003 0000  ................
+000012c0: 0173 1600 0000 8700 6601 6401 6402 8408  .s......f.d.d...
+000012d0: 8800 6a00 6a01 4400 8301 5300 2903 7a1c  ..j.j.D...S.).z.
+000012e0: 5468 6520 7061 7468 7320 746f 2074 6865  The paths to the
+000012f0: 2073 7572 726f 6761 7465 732e 6301 0000   surrogates.c...
+00001300: 0000 0000 0000 0000 0002 0000 0008 0000  ................
+00001310: 0013 0000 0173 2600 0000 6900 7c00 5d0f  .....s&...i.|.].
+00001320: 7d01 7c01 8800 6a00 8800 6a01 9b00 6400  }.|...j...j...d.
+00001330: 7c01 9b00 6401 9d04 1b00 9302 7102 5300  |...d.......q.S.
+00001340: 2902 fa01 2d7a 052e 6a73 6f6e 2902 7268  )...-z..json).rh
+00001350: 0000 0072 4700 0000 2902 da02 2e30 7265  ...rG...)....0re
+00001360: 0000 0072 6700 0000 7220 0000 0072 2100  ...rg...r ...r!.
+00001370: 0000 da0a 3c64 6963 7463 6f6d 703e a500  ....<dictcomp>..
+00001380: 0000 7308 0000 0006 0002 0218 ff06 ff7a  ..s............z
+00001390: 3050 4431 4265 6e63 686d 6172 6b2e 7375  0PD1Benchmark.su
+000013a0: 7272 6f67 6174 655f 7061 7468 732e 3c6c  rrogate_paths.<l
+000013b0: 6f63 616c 733e 2e3c 6469 6374 636f 6d70  ocals>.<dictcomp
+000013c0: 3e29 0272 1000 0000 722c 0000 0072 6700  >).r....r,...rg.
+000013d0: 0000 7220 0000 0072 6700 0000 7221 0000  ..r ...rg...r!..
+000013e0: 0072 6300 0000 a200 0000 7306 0000 000a  .rc.......s.....
+000013f0: 0306 0206 fe7a 1c50 4431 4265 6e63 686d  .....z.PD1Benchm
+00001400: 6172 6b2e 7375 7272 6f67 6174 655f 7061  ark.surrogate_pa
+00001410: 7468 73da 0663 6f6e 6669 67fa 114d 6170  ths..config..Map
+00001420: 7069 6e67 5b73 7472 2c20 416e 795d da02  ping[str, Any]..
+00001430: 6174 da03 696e 74fa 1064 6963 745b 7374  at..int..dict[st
+00001440: 722c 2066 6c6f 6174 5d63 0300 0000 0000  r, float]c......
+00001450: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+00001460: 0001 7314 0000 007c 006a 007c 017c 0267  ..s....|.j.|.|.g
+00001470: 0164 018d 0264 0219 0053 0029 034e 2901  .d...d...S.).N).
+00001480: da0a 6669 6465 6c69 7469 6573 7201 0000  ..fidelitiesr...
+00001490: 0029 01da 0c5f 7265 7375 6c74 735f 666f  .)..._results_fo
+000014a0: 7229 0372 5900 0000 726d 0000 0072 6f00  r).rY...rm...ro.
+000014b0: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
+000014c0: 00da 135f 6f62 6a65 6374 6976 655f 6675  ..._objective_fu
+000014d0: 6e63 7469 6f6e aa00 0000 7302 0000 0014  nction....s.....
+000014e0: 067a 2050 4431 4265 6e63 686d 6172 6b2e  .z PD1Benchmark.
+000014f0: 5f6f 626a 6563 7469 7665 5f66 756e 6374  _objective_funct
+00001500: 696f 6eda 0366 726d da02 746f da04 7374  ion..frm..to..st
+00001510: 6570 fa29 4974 6572 6162 6c65 5b74 7570  ep.)Iterable[tup
+00001520: 6c65 5b69 6e74 2c20 4d61 7070 696e 675b  le[int, Mapping[
+00001530: 7374 722c 2066 6c6f 6174 5d5d 5d63 0200  str, float]]]c..
+00001540: 0000 0000 0000 0300 0000 0600 0000 0600  ................
+00001550: 0000 4300 0001 7324 0000 0074 007c 00a0  ..C...s$...t.|..
+00001560: 017c 027c 037c 04a1 0383 017d 0574 027c  .|.|.|.....}.t.|
+00001570: 057c 00a0 037c 017c 05a1 0283 0253 00a9  .|...|.|.....S..
+00001580: 014e 2904 da04 6c69 7374 da0f 6974 6572  .N)...list..iter
+00001590: 5f66 6964 656c 6974 6965 73da 037a 6970  _fidelities..zip
+000015a0: 7273 0000 0029 0672 5900 0000 726d 0000  rs...).rY...rm..
+000015b0: 0072 7500 0000 7276 0000 0072 7700 0000  .ru...rv...rw...
+000015c0: 7272 0000 0072 2000 0000 7220 0000 0072  rr...r ...r ...r
+000015d0: 2100 0000 da0b 5f74 7261 6a65 6374 6f72  !....._trajector
+000015e0: 79b2 0000 0073 0400 0000 1209 1201 7a18  y....s........z.
+000015f0: 5044 3142 656e 6368 6d61 726b 2e5f 7472  PD1Benchmark._tr
+00001600: 616a 6563 746f 7279 7272 0000 00fa 0d49  ajectoryrr.....I
+00001610: 7465 7261 626c 655b 696e 745d fa16 6c69  terable[int]..li
+00001620: 7374 5b64 6963 745b 7374 722c 2066 6c6f  st[dict[str, flo
+00001630: 6174 5d5d 6303 0000 0000 0000 0000 0000  at]]c...........
+00001640: 0009 0000 0005 0000 0003 0000 0173 8a00  .............s..
+00001650: 0000 7400 7c01 8301 8900 8700 8702 6602  ..t.|.........f.
+00001660: 6401 6402 8408 7c02 4400 8301 7d03 7401  d.d...|.D...}.t.
+00001670: a002 7c03 a101 7d04 7c04 6a03 7d05 8802  ..|...}.|.j.}...
+00001680: 6a04 a005 a100 4400 5d17 5c02 7d06 7d07  j.....D.].\.}.}.
+00001690: 8802 6a06 6a07 7c06 1900 6a08 7d08 7c07  ..j.j.|...j.}.|.
+000016a0: a009 7c04 7c05 1900 a101 6a0a 7c08 8e00  ..|.|.....j.|...
+000016b0: 7c04 7c06 3c00 711b 740b 8802 6a04 a00c  |.|.<.q.t...j...
+000016c0: a100 8301 8901 8701 6601 6403 6402 8408  ........f.d.d...
+000016d0: 7c04 a00d a100 4400 8301 5300 2904 4e63  |.....D...S.).Nc
+000016e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000016f0: 0500 0000 1300 0001 731e 0000 0067 007c  ........s....g.|
+00001700: 005d 0b7d 0169 0088 00a5 0188 016a 007c  .].}.i.......j.|
+00001710: 0169 01a5 0191 0271 0253 0072 2000 0000  .i.....q.S.r ...
+00001720: 2901 7249 0000 0029 0272 6b00 0000 da01  ).rI...).rk.....
+00001730: 6629 02da 0163 7259 0000 0072 2000 0000  f)...crY...r ...
+00001740: 7221 0000 00da 0a3c 6c69 7374 636f 6d70  r!.....<listcomp
+00001750: 3ec5 0000 0073 0200 0000 1e00 7a2d 5044  >....s......z-PD
+00001760: 3142 656e 6368 6d61 726b 2e5f 7265 7375  1Benchmark._resu
+00001770: 6c74 735f 666f 722e 3c6c 6f63 616c 733e  lts_for.<locals>
+00001780: 2e3c 6c69 7374 636f 6d70 3e63 0100 0000  .<listcomp>c....
+00001790: 0000 0000 0000 0000 0300 0000 0500 0000  ................
+000017a0: 1300 0001 731c 0000 0067 007c 005d 0a5c  ....s....g.|.].\
+000017b0: 027d 017d 0274 007c 0288 0019 0083 0191  .}.}.t.|........
+000017c0: 0271 0253 0072 2000 0000 2901 da04 6469  .q.S.r ...)...di
+000017d0: 6374 2903 726b 0000 0072 5f00 0000 da01  ct).rk...r_.....
+000017e0: 7229 01da 076d 6574 7269 6373 7220 0000  r)...metricsr ..
+000017f0: 0072 2100 0000 7282 0000 00d0 0000 0073  .r!...r........s
+00001800: 0200 0000 1c00 290e 7283 0000 00da 0270  ......).r......p
+00001810: 64da 0944 6174 6146 7261 6d65 da07 636f  d..DataFrame..co
+00001820: 6c75 6d6e 7372 5e00 0000 7264 0000 0072  lumnsr^...rd...r
+00001830: 1000 0000 722c 0000 0072 2700 0000 5a07  ....r,...r'...Z.
+00001840: 7072 6564 6963 74da 0463 6c69 7072 7a00  predict..cliprz.
+00001850: 0000 da04 6b65 7973 da08 6974 6572 726f  ....keys..iterro
+00001860: 7773 2909 7259 0000 0072 6d00 0000 7272  ws).rY...rm...rr
+00001870: 0000 005a 0771 7565 7269 6573 da02 7873  ...Z.queries..xs
+00001880: da08 6665 6174 7572 6573 7265 0000 005a  ..featuresre...Z
+00001890: 0973 7572 726f 6761 7465 7227 0000 0072  .surrogater'...r
+000018a0: 2000 0000 2903 7281 0000 0072 8500 0000   ...).r....r....
+000018b0: 7259 0000 0072 2100 0000 7273 0000 00be  rY...r!...rs....
+000018c0: 0000 0073 1200 0000 0806 1401 0a01 0603  ...s............
+000018d0: 1201 0e02 1a01 0e02 1601 7a19 5044 3142  ..........z.PD1B
+000018e0: 656e 6368 6d61 726b 2e5f 7265 7375 6c74  enchmark._result
+000018f0: 735f 666f 7272 1200 0000 6302 0000 0000  s_forr....c.....
+00001900: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
+00001910: 0000 0173 0400 0000 6400 5300 7279 0000  ...s....d.S.ry..
+00001920: 0072 2000 0000 2902 725a 0000 0072 3c00  .r ...).rZ...r<.
+00001930: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
+00001940: 0072 4e00 0000 d200 0000 7302 0000 0004  .rN.......s.....
+00001950: 037a 1a50 4431 4265 6e63 686d 6172 6b2e  .z.PD1Benchmark.
+00001960: 5f63 7265 6174 655f 7370 6163 6529 0c72  _create_space).r
+00001970: 3b00 0000 7241 0000 0072 3c00 0000 7242  ;...rA...r<...rB
+00001980: 0000 0072 3d00 0000 7243 0000 0072 3e00  ...r=...rC...r>.
+00001990: 0000 7244 0000 0072 3f00 0000 7245 0000  ..rD...r?...rE..
+000019a0: 0072 4000 0000 7245 0000 0029 0272 5c00  .r@...rE...).r\.
+000019b0: 0000 725d 0000 0029 0272 5c00 0000 7261  ..r]...).r\...ra
+000019c0: 0000 0029 0272 5c00 0000 7205 0000 0029  ...).r\...r....)
+000019d0: 0272 5c00 0000 7269 0000 0029 0672 6d00  .r\...ri...).rm.
+000019e0: 0000 726e 0000 0072 6f00 0000 7270 0000  ..rn...ro...rp..
+000019f0: 0072 5c00 0000 7271 0000 0029 0a72 6d00  .r\...rq...).rm.
+00001a00: 0000 726e 0000 0072 7500 0000 7270 0000  ..rn...ru...rp..
+00001a10: 0072 7600 0000 7270 0000 0072 7700 0000  .rv...rp...rw...
+00001a20: 7270 0000 0072 5c00 0000 7278 0000 0029  rp...r\...rx...)
+00001a30: 0672 6d00 0000 726e 0000 0072 7200 0000  .rm...rn...rr...
+00001a40: 727e 0000 0072 5c00 0000 727f 0000 0072  r~...r\...r....r
+00001a50: 7900 0000 2904 723c 0000 0072 4200 0000  y...).r<...rB...
+00001a60: 725c 0000 0072 1200 0000 2912 721b 0000  r\...r....).r...
+00001a70: 0072 1c00 0000 721d 0000 0072 1f00 0000  .r....r....r....
+00001a80: 7257 0000 0072 6000 0000 da08 7072 6f70  rW...r`.....prop
+00001a90: 6572 7479 725e 0000 0072 6800 0000 7263  ertyr^...rh...rc
+00001aa0: 0000 0072 0c00 0000 7274 0000 0072 7d00  ...r....rt...r}.
+00001ab0: 0000 7273 0000 00da 0b63 6c61 7373 6d65  ..rs.....classme
+00001ac0: 7468 6f64 7203 0000 0072 4e00 0000 da0d  thodr....rN.....
+00001ad0: 5f5f 636c 6173 7363 656c 6c5f 5f72 2000  __classcell__r .
+00001ae0: 0000 7220 0000 0072 5b00 0000 7221 0000  ..r ...r[...r!..
+00001af0: 0072 3700 0000 4600 0000 733a 0000 000a  .r7...F...s:....
+00001b00: 0008 0102 0108 0202 0108 0202 0102 0502  ................
+00001b10: 0102 0102 0102 0102 0112 f80a 3502 040c  ............5...
+00001b20: 0102 130c 0102 040c 0102 070c 0102 070c  ................
+00001b30: 010a 0b02 1402 0118 0172 3700 0000 292a  .........r7...)*
+00001b40: da0a 5f5f 6675 7475 7265 5f5f 7202 0000  ..__future__r...
+00001b50: 00da 0361 6263 7203 0000 00da 0b64 6174  ...abcr......dat
+00001b60: 6163 6c61 7373 6573 7204 0000 00da 0770  aclassesr......p
+00001b70: 6174 686c 6962 7205 0000 00da 0674 7970  athlibr......typ
+00001b80: 696e 6772 0600 0000 7207 0000 0072 0800  ingr....r....r..
+00001b90: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00001ba0: 00da 1174 7970 696e 675f 6578 7465 6e73  ...typing_extens
+00001bb0: 696f 6e73 720c 0000 00da 056e 756d 7079  ionsr......numpy
+00001bc0: 7232 0000 00da 0670 616e 6461 7372 8600  r2.....pandasr..
+00001bd0: 0000 da12 6d66 7062 656e 6368 2e62 656e  ....mfpbench.ben
+00001be0: 6368 6d61 726b 720d 0000 00da 0f6d 6670  chmarkr......mfp
+00001bf0: 6265 6e63 682e 636f 6e66 6967 720e 0000  bench.configr...
+00001c00: 00da 0f6d 6670 6265 6e63 682e 6d65 7472  ...mfpbench.metr
+00001c10: 6963 720f 0000 00da 0f6d 6670 6265 6e63  icr......mfpbenc
+00001c20: 682e 7265 7375 6c74 7210 0000 00da 186d  h.resultr......m
+00001c30: 6670 6265 6e63 682e 7365 7475 705f 6265  fpbench.setup_be
+00001c40: 6e63 686d 6172 6b72 1100 0000 da0b 436f  nchmarkr......Co
+00001c50: 6e66 6967 5370 6163 6572 1200 0000 7262  nfigSpacer....rb
+00001c60: 0000 0072 1400 0000 7258 0000 0072 1900  ...r....rX...r..
+00001c70: 0000 7270 0000 0072 2200 0000 7234 0000  ..rp...r"...r4..
+00001c80: 0072 3500 0000 7237 0000 0072 2000 0000  .r5...r7...r ...
+00001c90: 7220 0000 0072 2000 0000 7221 0000 00da  r ...r ...r!....
+00001ca0: 083c 6d6f 6475 6c65 3e01 0000 0073 3200  .<module>....s2.
+00001cb0: 0000 0c00 0c02 0c01 0c01 2001 0c01 0802  .......... .....
+00001cc0: 0801 0c02 0c01 0c01 0c01 0c01 0402 0c01  ................
+00001cd0: 0c01 0402 0c03 1201 0809 1a01 0810 1a01  ................
+00001ce0: 0c0e 1e03                                ....
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/benchmark.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/benchmark.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/config.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/config.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/result.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/result.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/__pycache__/result.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/__pycache__/result.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmark.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,15 +197,16 @@
         queries = [{**c, self.fidelity_name: f} for f in fidelities]
         xs = pd.DataFrame(queries)
 
         # Predict the metric for everything in the dataframe
         features = xs.columns
         for metric, surrogate in self.surrogates.items():
             # We clip as sometimes the surrogate produces negative values
-            xs[metric] = surrogate.predict(xs[features]).clip(min=0)
+            bounds = self.Result.metric_defs[metric].bounds
+            xs[metric] = surrogate.predict(xs[features]).clip(*bounds)
 
         metrics = list(self.surrogates.keys())
         return [dict(r[metrics]) for _, r in xs.iterrows()]
 
     @classmethod
     @abstractmethod
     def _create_space(cls, seed: int | None = None) -> ConfigurationSpace:
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__init__.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/__init__.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/__init__.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/cifar100.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/imagenet.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 1318 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 2605 0000  o........Coe&...
+00000000: 6f0d 0d0a 0000 0000 70ea 3d66 1a05 0000  o.......p.=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6506 8303 5a08 6406 5300 2907  ..d.e...Z.d.S.).
 00000070: e900 0000 0029 01da 0b61 6e6e 6f74 6174  .....)...annotat
@@ -10,69 +10,68 @@
 00000090: 6174 696f 6e53 7061 6365 da1a 556e 6966  ationSpace..Unif
 000000a0: 6f72 6d46 6c6f 6174 4879 7065 7270 6172  ormFloatHyperpar
 000000b0: 616d 6574 6572 2902 da0c 5044 3142 656e  ameter)...PD1Ben
 000000c0: 6368 6d61 726b da14 5044 3152 6573 756c  chmark..PD1Resul
 000000d0: 7454 7261 6e73 666f 726d 6572 6300 0000  tTransformerc...
 000000e0: 0000 0000 0000 0000 0000 0000 0005 0000  ................
 000000f0: 0040 0000 0173 2800 0000 6500 5a01 6400  .@...s(...e.Z.d.
-00000100: 5a02 6401 5a03 6504 5a05 6402 5a06 6507  Z.d.Z.e.Z.d.Z.e.
+00000100: 5a02 6503 5a04 6401 5a05 6402 5a06 6507  Z.e.Z.d.Z.d.Z.e.
 00000110: 640a 640b 6408 6409 8405 8301 5a08 6403  d.d.d.d.....Z.d.
-00000120: 5300 290c da1b 5044 3163 6966 6172 3130  S.)...PD1cifar10
-00000130: 305f 7769 6465 7265 736e 6574 5f32 3034  0_wideresnet_204
-00000140: 3829 03e9 2d00 0000 e9c7 0000 00e9 0100  8)..-...........
-00000150: 0000 7a18 6369 6661 7231 3030 2d77 6964  ..z.cifar100-wid
-00000160: 6572 6573 6e65 742d 3230 3438 4eda 0473  eresnet-2048N..s
-00000170: 6565 64fa 0a69 6e74 207c 204e 6f6e 65da  eed..int | None.
-00000180: 0672 6574 7572 6e72 0300 0000 6302 0000  .returnr....c...
-00000190: 0000 0000 0000 0000 0003 0000 000b 0000  ................
-000001a0: 0043 0000 0173 4c00 0000 7400 7c01 6401  .C...sL...t.|.d.
-000001b0: 8d01 7d02 7c02 a001 7402 6402 6403 6404  ..}.|...t.d.d.d.
-000001c0: 6405 8d03 7402 6406 6407 6408 6409 640a  d...t.d.d.d.d.d.
-000001d0: 8d04 7402 640b 640c 640d 6405 8d03 7402  ..t.d.d.d.d...t.
-000001e0: 640e 640f 6410 6409 640a 8d04 6704 a101  d.d.d.d.d...g...
-000001f0: 0100 7c02 5300 2911 4e29 0172 0b00 0000  ..|.S.).N).r....
-00000200: da0f 6c72 5f64 6563 6179 5f66 6163 746f  ..lr_decay_facto
-00000210: 7267 3525 5987 a3ab 843f 67ea 3f6b 7efc  rg5%Y....?g.?k~.
-00000220: a5ef 3f29 02da 056c 6f77 6572 da05 7570  ..?)...lower..up
-00000230: 7065 72da 0a6c 725f 696e 6974 6961 6c67  per..lr_initialg
-00000240: f168 e388 b5f8 e43e 67fc a71b 28f0 8e23  .h.....>g...(..#
-00000250: 4054 2903 720f 0000 0072 1000 0000 da03  @T).r....r......
-00000260: 6c6f 67da 086c 725f 706f 7765 7267 bf10  log..lr_powerg..
-00000270: 72de ffc7 b93f 6749 8446 b071 fdff 3fda  r....?gI.F.q..?.
-00000280: 0c6f 7074 5f6d 6f6d 656e 7475 6d67 fc6d  .opt_momentumg.m
-00000290: 4f90 d8ee 0e3f 678c dafd 2ac0 f7ef 3f29  O....?g...*...?)
-000002a0: 0372 0300 0000 da13 6164 645f 6879 7065  .r......add_hype
-000002b0: 7270 6172 616d 6574 6572 7372 0400 0000  rparametersr....
-000002c0: 2903 da03 636c 7372 0b00 0000 da02 6373  )...clsr......cs
-000002d0: a900 7218 0000 00fa 4a2f 686f 6d65 2f73  ..r.....J/home/s
-000002e0: 6b61 6e74 6966 792f 636f 6465 2f6d 662d  kantify/code/mf-
-000002f0: 7072 696f 722d 6265 6e63 682f 7372 632f  prior-bench/src/
-00000300: 6d66 7062 656e 6368 2f70 6431 2f62 656e  mfpbench/pd1/ben
-00000310: 6368 6d61 726b 732f 6369 6661 7231 3030  chmarks/cifar100
-00000320: 2e70 79da 0d5f 6372 6561 7465 5f73 7061  .py.._create_spa
-00000330: 6365 0d00 0000 7336 0000 000a 0204 0102  ce....s6........
-00000340: 0202 0102 0102 0104 fd02 0502 0102 0102  ................
-00000350: 0102 0104 fc02 0602 0102 0102 0104 fd02  ................
-00000360: 0502 0102 0102 0102 0104 fc02 ef04 ff04  ................
-00000370: 1a7a 2950 4431 6369 6661 7231 3030 5f77  .z)PD1cifar100_w
-00000380: 6964 6572 6573 6e65 745f 3230 3438 2e5f  ideresnet_2048._
-00000390: 6372 6561 7465 5f73 7061 6365 2901 4e29  create_space).N)
-000003a0: 0472 0b00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000003b0: 7203 0000 0029 09da 085f 5f6e 616d 655f  r....)...__name_
-000003c0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000003d0: 5f71 7561 6c6e 616d 655f 5fda 1270 6431  _qualname__..pd1
-000003e0: 5f66 6964 656c 6974 795f 7261 6e67 6572  _fidelity_ranger
-000003f0: 0600 0000 da0f 7064 315f 7265 7375 6c74  ......pd1_result
-00000400: 5f74 7970 65da 0870 6431 5f6e 616d 65da  _type..pd1_name.
-00000410: 0b63 6c61 7373 6d65 7468 6f64 721a 0000  .classmethodr...
-00000420: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-00000430: 7219 0000 0072 0700 0000 0800 0000 730c  r....r........s.
-00000440: 0000 0008 0004 0104 0104 0102 0212 0172  ...............r
-00000450: 0700 0000 4e29 09da 0a5f 5f66 7574 7572  ....N)...__futur
-00000460: 655f 5f72 0200 0000 da0b 436f 6e66 6967  e__r......Config
-00000470: 5370 6163 6572 0300 0000 7204 0000 00da  Spacer....r.....
-00000480: 166d 6670 6265 6e63 682e 7064 312e 6265  .mfpbench.pd1.be
-00000490: 6e63 686d 6172 6b72 0500 0000 7206 0000  nchmarkr....r...
-000004a0: 0072 0700 0000 7218 0000 0072 1800 0000  .r....r....r....
-000004b0: 7218 0000 0072 1900 0000 da08 3c6d 6f64  r....r......<mod
-000004c0: 756c 653e 0100 0000 7308 0000 000c 0010  ule>....s.......
-000004d0: 0210 0214 03                             .....
+00000120: 5300 290c da16 5044 3169 6d61 6765 6e65  S.)...PD1imagene
+00000130: 745f 7265 736e 6574 5f35 3132 2903 e901  t_resnet_512)...
+00000140: 0000 00e9 6300 0000 7208 0000 007a 1369  ....c...r....z.i
+00000150: 6d61 6765 6e65 742d 7265 736e 6574 2d35  magenet-resnet-5
+00000160: 3132 4eda 0473 6565 64fa 0a69 6e74 207c  12N..seed..int |
+00000170: 204e 6f6e 65da 0672 6574 7572 6e72 0300   None..returnr..
+00000180: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
+00000190: 0000 000b 0000 0043 0000 0173 4c00 0000  .......C...sL...
+000001a0: 7400 7c01 6401 8d01 7d02 7c02 a001 7402  t.|.d...}.|...t.
+000001b0: 6402 6403 6404 6405 8d03 7402 6406 6407  d.d.d.d...t.d.d.
+000001c0: 6408 6409 640a 8d04 7402 640b 640c 640d  d.d.d...t.d.d.d.
+000001d0: 6405 8d03 7402 640e 640f 6410 6409 640a  d...t.d.d.d.d.d.
+000001e0: 8d04 6704 a101 0100 7c02 5300 2911 4e29  ..g.....|.S.).N)
+000001f0: 0172 0a00 0000 da0f 6c72 5f64 6563 6179  .r......lr_decay
+00000200: 5f66 6163 746f 7267 f19b c24a 0515 853f  _factorg...J...?
+00000210: 67bd c5c3 7b0e acef 3f29 02da 056c 6f77  g...{...?)...low
+00000220: 6572 da05 7570 7065 72da 0a6c 725f 696e  er..upper..lr_in
+00000230: 6974 6961 6c67 f168 e388 b5f8 e43e 67fb  itialg.h.....>g.
+00000240: cc59 9f72 8c23 4054 2903 720e 0000 0072  .Y.r.#@T).r....r
+00000250: 0f00 0000 da03 6c6f 67da 086c 725f 706f  ......log..lr_po
+00000260: 7765 7267 7fd9 3d79 58a8 b93f 6710 ae80  werg..=yX..?g...
+00000270: 423d fdff 3fda 0c6f 7074 5f6d 6f6d 656e  B=..?..opt_momen
+00000280: 7475 6d67 fc6d 4f90 d8ee 0e3f 678c dafd  tumg.mO....?g...
+00000290: 2ac0 f7ef 3f29 0372 0300 0000 da13 6164  *...?).r......ad
+000002a0: 645f 6879 7065 7270 6172 616d 6574 6572  d_hyperparameter
+000002b0: 7372 0400 0000 2903 da03 636c 7372 0a00  sr....)...clsr..
+000002c0: 0000 da02 6373 a900 7217 0000 00fa 4a2f  ....cs..r.....J/
+000002d0: 686f 6d65 2f73 6b61 6e74 6966 792f 636f  home/skantify/co
+000002e0: 6465 2f6d 662d 7072 696f 722d 6265 6e63  de/mf-prior-benc
+000002f0: 682f 7372 632f 6d66 7062 656e 6368 2f70  h/src/mfpbench/p
+00000300: 6431 2f62 656e 6368 6d61 726b 732f 696d  d1/benchmarks/im
+00000310: 6167 656e 6574 2e70 79da 0d5f 6372 6561  agenet.py.._crea
+00000320: 7465 5f73 7061 6365 0d00 0000 7336 0000  te_space....s6..
+00000330: 000a 0204 0102 0202 0102 0102 0104 fd02  ................
+00000340: 0502 0102 0102 0102 0104 fc02 0602 0102  ................
+00000350: 0102 0104 fd02 0502 0102 0102 0102 0104  ................
+00000360: fc02 ef04 ff04 1a7a 2450 4431 696d 6167  .......z$PD1imag
+00000370: 656e 6574 5f72 6573 6e65 745f 3531 322e  enet_resnet_512.
+00000380: 5f63 7265 6174 655f 7370 6163 6529 014e  _create_space).N
+00000390: 2904 720a 0000 0072 0b00 0000 720c 0000  ).r....r....r...
+000003a0: 0072 0300 0000 2909 da08 5f5f 6e61 6d65  .r....)...__name
+000003b0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000003c0: 5f5f 7175 616c 6e61 6d65 5f5f 7206 0000  __qualname__r...
+000003d0: 00da 0f70 6431 5f72 6573 756c 745f 7479  ...pd1_result_ty
+000003e0: 7065 da12 7064 315f 6669 6465 6c69 7479  pe..pd1_fidelity
+000003f0: 5f72 616e 6765 da08 7064 315f 6e61 6d65  _range..pd1_name
+00000400: da0b 636c 6173 736d 6574 686f 6472 1900  ..classmethodr..
+00000410: 0000 7217 0000 0072 1700 0000 7217 0000  ..r....r....r...
+00000420: 0072 1800 0000 7207 0000 0008 0000 0073  .r....r........s
+00000430: 0c00 0000 0800 0401 0401 0401 0202 1201  ................
+00000440: 7207 0000 004e 2909 da0a 5f5f 6675 7475  r....N)...__futu
+00000450: 7265 5f5f 7202 0000 00da 0b43 6f6e 6669  re__r......Confi
+00000460: 6753 7061 6365 7203 0000 0072 0400 0000  gSpacer....r....
+00000470: da16 6d66 7062 656e 6368 2e70 6431 2e62  ..mfpbench.pd1.b
+00000480: 656e 6368 6d61 726b 7205 0000 0072 0600  enchmarkr....r..
+00000490: 0000 7207 0000 0072 1700 0000 7217 0000  ..r....r....r...
+000004a0: 0072 1700 0000 7218 0000 00da 083c 6d6f  .r....r......<mo
+000004b0: 6475 6c65 3e01 0000 0073 0800 0000 0c00  dule>....s......
+000004c0: 1002 1002 1403                           ......
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/cifar100.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/cifar100.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/imagenet.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/translate_wmt.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 1306 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 1a05 0000  o........Coe....
+00000000: 6f0d 0d0a 0000 0000 70ea 3d66 4a05 0000  o.......p.=fJ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6506 8303 5a08 6406 5300 2907  ..d.e...Z.d.S.).
 00000070: e900 0000 0029 01da 0b61 6e6e 6f74 6174  .....)...annotat
@@ -10,68 +10,70 @@
 00000090: 6174 696f 6e53 7061 6365 da1a 556e 6966  ationSpace..Unif
 000000a0: 6f72 6d46 6c6f 6174 4879 7065 7270 6172  ormFloatHyperpar
 000000b0: 616d 6574 6572 2902 da0c 5044 3142 656e  ameter)...PD1Ben
 000000c0: 6368 6d61 726b da14 5044 3152 6573 756c  chmark..PD1Resul
 000000d0: 7454 7261 6e73 666f 726d 6572 6300 0000  tTransformerc...
 000000e0: 0000 0000 0000 0000 0000 0000 0005 0000  ................
 000000f0: 0040 0000 0173 2800 0000 6500 5a01 6400  .@...s(...e.Z.d.
-00000100: 5a02 6503 5a04 6401 5a05 6402 5a06 6507  Z.e.Z.d.Z.d.Z.e.
+00000100: 5a02 6401 5a03 6504 5a05 6402 5a06 6507  Z.d.Z.e.Z.d.Z.e.
 00000110: 640a 640b 6408 6409 8405 8301 5a08 6403  d.d.d.d.....Z.d.
-00000120: 5300 290c da16 5044 3169 6d61 6765 6e65  S.)...PD1imagene
-00000130: 745f 7265 736e 6574 5f35 3132 2903 e903  t_resnet_512)...
-00000140: 0000 00e9 6300 0000 e901 0000 007a 1369  ....c........z.i
-00000150: 6d61 6765 6e65 742d 7265 736e 6574 2d35  magenet-resnet-5
-00000160: 3132 4eda 0473 6565 64fa 0a69 6e74 207c  12N..seed..int |
-00000170: 204e 6f6e 65da 0672 6574 7572 6e72 0300   None..returnr..
-00000180: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
-00000190: 0000 000b 0000 0043 0000 0173 4c00 0000  .......C...sL...
-000001a0: 7400 7c01 6401 8d01 7d02 7c02 a001 7402  t.|.d...}.|...t.
-000001b0: 6402 6403 6404 6405 8d03 7402 6406 6407  d.d.d.d...t.d.d.
-000001c0: 6408 6409 640a 8d04 7402 640b 640c 640d  d.d.d...t.d.d.d.
-000001d0: 6405 8d03 7402 640e 640f 6410 6409 640a  d...t.d.d.d.d.d.
-000001e0: 8d04 6704 a101 0100 7c02 5300 2911 4e29  ..g.....|.S.).N)
-000001f0: 0172 0b00 0000 da0f 6c72 5f64 6563 6179  .r......lr_decay
-00000200: 5f66 6163 746f 7267 f19b c24a 0515 853f  _factorg...J...?
-00000210: 67bd c5c3 7b0e acef 3f29 02da 056c 6f77  g...{...?)...low
-00000220: 6572 da05 7570 7065 72da 0a6c 725f 696e  er..upper..lr_in
-00000230: 6974 6961 6c67 f168 e388 b5f8 e43e 67fb  itialg.h.....>g.
-00000240: cc59 9f72 8c23 4054 2903 720f 0000 0072  .Y.r.#@T).r....r
-00000250: 1000 0000 da03 6c6f 67da 086c 725f 706f  ......log..lr_po
-00000260: 7765 7267 7fd9 3d79 58a8 b93f 6710 ae80  werg..=yX..?g...
-00000270: 423d fdff 3fda 0c6f 7074 5f6d 6f6d 656e  B=..?..opt_momen
-00000280: 7475 6d67 fc6d 4f90 d8ee 0e3f 678c dafd  tumg.mO....?g...
-00000290: 2ac0 f7ef 3f29 0372 0300 0000 da13 6164  *...?).r......ad
-000002a0: 645f 6879 7065 7270 6172 616d 6574 6572  d_hyperparameter
-000002b0: 7372 0400 0000 2903 da03 636c 7372 0b00  sr....)...clsr..
-000002c0: 0000 da02 6373 a900 7218 0000 00fa 4a2f  ....cs..r.....J/
-000002d0: 686f 6d65 2f73 6b61 6e74 6966 792f 636f  home/skantify/co
-000002e0: 6465 2f6d 662d 7072 696f 722d 6265 6e63  de/mf-prior-benc
-000002f0: 682f 7372 632f 6d66 7062 656e 6368 2f70  h/src/mfpbench/p
-00000300: 6431 2f62 656e 6368 6d61 726b 732f 696d  d1/benchmarks/im
-00000310: 6167 656e 6574 2e70 79da 0d5f 6372 6561  agenet.py.._crea
-00000320: 7465 5f73 7061 6365 0d00 0000 7336 0000  te_space....s6..
-00000330: 000a 0204 0102 0202 0102 0102 0104 fd02  ................
-00000340: 0502 0102 0102 0102 0104 fc02 0602 0102  ................
-00000350: 0102 0104 fd02 0502 0102 0102 0102 0104  ................
-00000360: fc02 ef04 ff04 1a7a 2450 4431 696d 6167  .......z$PD1imag
-00000370: 656e 6574 5f72 6573 6e65 745f 3531 322e  enet_resnet_512.
-00000380: 5f63 7265 6174 655f 7370 6163 6529 014e  _create_space).N
-00000390: 2904 720b 0000 0072 0c00 0000 720d 0000  ).r....r....r...
-000003a0: 0072 0300 0000 2909 da08 5f5f 6e61 6d65  .r....)...__name
-000003b0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-000003c0: 5f5f 7175 616c 6e61 6d65 5f5f 7206 0000  __qualname__r...
-000003d0: 00da 0f70 6431 5f72 6573 756c 745f 7479  ...pd1_result_ty
-000003e0: 7065 da12 7064 315f 6669 6465 6c69 7479  pe..pd1_fidelity
-000003f0: 5f72 616e 6765 da08 7064 315f 6e61 6d65  _range..pd1_name
-00000400: da0b 636c 6173 736d 6574 686f 6472 1a00  ..classmethodr..
-00000410: 0000 7218 0000 0072 1800 0000 7218 0000  ..r....r....r...
-00000420: 0072 1900 0000 7207 0000 0008 0000 0073  .r....r........s
-00000430: 0c00 0000 0800 0401 0401 0401 0202 1201  ................
-00000440: 7207 0000 004e 2909 da0a 5f5f 6675 7475  r....N)...__futu
-00000450: 7265 5f5f 7202 0000 00da 0b43 6f6e 6669  re__r......Confi
-00000460: 6753 7061 6365 7203 0000 0072 0400 0000  gSpacer....r....
-00000470: da16 6d66 7062 656e 6368 2e70 6431 2e62  ..mfpbench.pd1.b
-00000480: 656e 6368 6d61 726b 7205 0000 0072 0600  enchmarkr....r..
-00000490: 0000 7207 0000 0072 1800 0000 7218 0000  ..r....r....r...
-000004a0: 0072 1800 0000 7219 0000 00da 083c 6d6f  .r....r......<mo
-000004b0: 6475 6c65 3e01 0000 0073 0800 0000 0c00  dule>....s......
-000004c0: 1002 1002 1403                           ......
+00000120: 5300 290c da1a 5044 3174 7261 6e73 6c61  S.)...PD1transla
+00000130: 7465 776d 745f 7866 6f72 6d65 725f 3634  tewmt_xformer_64
+00000140: 2903 e901 0000 00e9 1300 0000 7208 0000  )...........r...
+00000150: 007a 2274 7261 6e73 6c61 7465 5f77 6d74  .z"translate_wmt
+00000160: 2d78 666f 726d 6572 5f74 7261 6e73 6c61  -xformer_transla
+00000170: 7465 2d36 344e da04 7365 6564 fa0a 696e  te-64N..seed..in
+00000180: 7420 7c20 4e6f 6e65 da06 7265 7475 726e  t | None..return
+00000190: 7203 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000001a0: 0000 0300 0000 0b00 0000 4300 0001 734c  ..........C...sL
+000001b0: 0000 0074 007c 0164 018d 017d 027c 02a0  ...t.|.d...}.|..
+000001c0: 0174 0264 0264 0364 0464 058d 0374 0264  .t.d.d.d.d...t.d
+000001d0: 0664 0764 0864 0964 0a8d 0474 0264 0b64  .d.d.d.d...t.d.d
+000001e0: 0c64 0d64 058d 0374 0264 0e64 0f64 1064  .d.d...t.d.d.d.d
+000001f0: 0964 0a8d 0467 04a1 0101 007c 0253 0029  .d...g.....|.S.)
+00000200: 114e 2901 720a 0000 00da 0f6c 725f 6465  .N).r......lr_de
+00000210: 6361 795f 6661 6374 6f72 6723 76f1 f07a  cay_factorg#v..z
+00000220: 8684 3f67 117e 519e 53a2 ef3f 2902 da05  ..?g.~Q.S..?)...
+00000230: 6c6f 7765 72da 0575 7070 6572 da0a 6c72  lower..upper..lr
+00000240: 5f69 6e69 7469 616c 673d d78e d986 07e5  _initialg=......
+00000250: 3e67 bea2 ee12 3baf 2340 5429 0372 0e00  >g....;.#@T).r..
+00000260: 0000 720f 0000 00da 036c 6f67 da08 6c72  ..r......log..lr
+00000270: 5f70 6f77 6572 67d1 e830 9575 b5b9 3f67  _powerg..0.u..?g
+00000280: ef37 4958 3cfa ff3f da0c 6f70 745f 6d6f  .7IX<..?..opt_mo
+00000290: 6d65 6e74 756d 67e0 d48f 5eb0 ba0e 3f67  mentumg...^...?g
+000002a0: 1e94 73cb cef7 ef3f 2903 7203 0000 00da  ..s....?).r.....
+000002b0: 1361 6464 5f68 7970 6572 7061 7261 6d65  .add_hyperparame
+000002c0: 7465 7273 7204 0000 0029 03da 0363 6c73  tersr....)...cls
+000002d0: 720a 0000 00da 0263 73a9 0072 1700 0000  r......cs..r....
+000002e0: fa4f 2f68 6f6d 652f 736b 616e 7469 6679  .O/home/skantify
+000002f0: 2f63 6f64 652f 6d66 2d70 7269 6f72 2d62  /code/mf-prior-b
+00000300: 656e 6368 2f73 7263 2f6d 6670 6265 6e63  ench/src/mfpbenc
+00000310: 682f 7064 312f 6265 6e63 686d 6172 6b73  h/pd1/benchmarks
+00000320: 2f74 7261 6e73 6c61 7465 5f77 6d74 2e70  /translate_wmt.p
+00000330: 79da 0d5f 6372 6561 7465 5f73 7061 6365  y.._create_space
+00000340: 0d00 0000 7336 0000 000a 0204 0102 0202  ....s6..........
+00000350: 0102 0102 0104 fd02 0502 0102 0102 0102  ................
+00000360: 0104 fc02 0602 0102 0102 0104 fd02 0502  ................
+00000370: 0102 0102 0102 0104 fc02 ef04 ff04 1a7a  ...............z
+00000380: 2850 4431 7472 616e 736c 6174 6577 6d74  (PD1translatewmt
+00000390: 5f78 666f 726d 6572 5f36 342e 5f63 7265  _xformer_64._cre
+000003a0: 6174 655f 7370 6163 6529 014e 2904 720a  ate_space).N).r.
+000003b0: 0000 0072 0b00 0000 720c 0000 0072 0300  ...r....r....r..
+000003c0: 0000 2909 da08 5f5f 6e61 6d65 5f5f da0a  ..)...__name__..
+000003d0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000003e0: 616c 6e61 6d65 5f5f da12 7064 315f 6669  alname__..pd1_fi
+000003f0: 6465 6c69 7479 5f72 616e 6765 7206 0000  delity_ranger...
+00000400: 00da 0f70 6431 5f72 6573 756c 745f 7479  ...pd1_result_ty
+00000410: 7065 da08 7064 315f 6e61 6d65 da0b 636c  pe..pd1_name..cl
+00000420: 6173 736d 6574 686f 6472 1900 0000 7217  assmethodr....r.
+00000430: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000440: 0000 7207 0000 0008 0000 0073 0c00 0000  ..r........s....
+00000450: 0800 0401 0401 0401 0202 1201 7207 0000  ............r...
+00000460: 004e 2909 da0a 5f5f 6675 7475 7265 5f5f  .N)...__future__
+00000470: 7202 0000 00da 0b43 6f6e 6669 6753 7061  r......ConfigSpa
+00000480: 6365 7203 0000 0072 0400 0000 da16 6d66  cer....r......mf
+00000490: 7062 656e 6368 2e70 6431 2e62 656e 6368  pbench.pd1.bench
+000004a0: 6d61 726b 7205 0000 0072 0600 0000 7207  markr....r....r.
+000004b0: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
+000004c0: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000004d0: 3e01 0000 0073 0800 0000 0c00 1002 1002  >....s..........
+000004e0: 1403                                     ..
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/imagenet.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/imagenet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/lm1b.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/lm1b.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/lm1b.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/lm1b.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/translate_wmt.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/cifar100.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 1344 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 4005 0000  o........Coe@...
+00000000: 6f0d 0d0a 0000 0000 70ea 3d66 2605 0000  o.......p.=f&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6506 8303 5a08 6406 5300 2907  ..d.e...Z.d.S.).
 00000070: e900 0000 0029 01da 0b61 6e6e 6f74 6174  .....)...annotat
@@ -12,67 +12,67 @@
 000000b0: 616d 6574 6572 2902 da0c 5044 3142 656e  ameter)...PD1Ben
 000000c0: 6368 6d61 726b da14 5044 3152 6573 756c  chmark..PD1Resul
 000000d0: 7454 7261 6e73 666f 726d 6572 6300 0000  tTransformerc...
 000000e0: 0000 0000 0000 0000 0000 0000 0005 0000  ................
 000000f0: 0040 0000 0173 2800 0000 6500 5a01 6400  .@...s(...e.Z.d.
 00000100: 5a02 6401 5a03 6504 5a05 6402 5a06 6507  Z.d.Z.e.Z.d.Z.e.
 00000110: 640a 640b 6408 6409 8405 8301 5a08 6403  d.d.d.d.....Z.d.
-00000120: 5300 290c da1a 5044 3174 7261 6e73 6c61  S.)...PD1transla
-00000130: 7465 776d 745f 7866 6f72 6d65 725f 3634  tewmt_xformer_64
-00000140: 2903 e901 0000 00e9 1300 0000 7208 0000  )...........r...
-00000150: 007a 1874 7261 6e73 6c61 7465 2d77 6d74  .z.translate-wmt
-00000160: 2d78 666f 726d 6572 2d36 344e da04 7365  -xformer-64N..se
-00000170: 6564 fa0a 696e 7420 7c20 4e6f 6e65 da06  ed..int | None..
-00000180: 7265 7475 726e 7203 0000 0063 0200 0000  returnr....c....
-00000190: 0000 0000 0000 0000 0300 0000 0b00 0000  ................
-000001a0: 4300 0001 734c 0000 0074 007c 0164 018d  C...sL...t.|.d..
-000001b0: 017d 027c 02a0 0174 0264 0264 0364 0464  .}.|...t.d.d.d.d
-000001c0: 058d 0374 0264 0664 0764 0864 0964 0a8d  ...t.d.d.d.d.d..
-000001d0: 0474 0264 0b64 0c64 0d64 058d 0374 0264  .t.d.d.d.d...t.d
-000001e0: 0e64 0f64 1064 0964 0a8d 0467 04a1 0101  .d.d.d.d...g....
-000001f0: 007c 0253 0029 114e 2901 720a 0000 00da  .|.S.).N).r.....
-00000200: 0f6c 725f 6465 6361 795f 6661 6374 6f72  .lr_decay_factor
-00000210: 6723 76f1 f07a 8684 3f67 117e 519e 53a2  g#v..z..?g.~Q.S.
-00000220: ef3f 2902 da05 6c6f 7765 72da 0575 7070  .?)...lower..upp
-00000230: 6572 da0a 6c72 5f69 6e69 7469 616c 673d  er..lr_initialg=
-00000240: d78e d986 07e5 3e67 bea2 ee12 3baf 2340  ......>g....;.#@
-00000250: 5429 0372 0e00 0000 720f 0000 00da 036c  T).r....r......l
-00000260: 6f67 da08 6c72 5f70 6f77 6572 67d1 e830  og..lr_powerg..0
-00000270: 9575 b5b9 3f67 ef37 4958 3cfa ff3f da0c  .u..?g.7IX<..?..
-00000280: 6f70 745f 6d6f 6d65 6e74 756d 67e0 d48f  opt_momentumg...
-00000290: 5eb0 ba0e 3f67 1e94 73cb cef7 ef3f 2903  ^...?g..s....?).
-000002a0: 7203 0000 00da 1361 6464 5f68 7970 6572  r......add_hyper
-000002b0: 7061 7261 6d65 7465 7273 7204 0000 0029  parametersr....)
-000002c0: 03da 0363 6c73 720a 0000 00da 0263 73a9  ...clsr......cs.
-000002d0: 0072 1700 0000 fa4f 2f68 6f6d 652f 736b  .r.....O/home/sk
-000002e0: 616e 7469 6679 2f63 6f64 652f 6d66 2d70  antify/code/mf-p
-000002f0: 7269 6f72 2d62 656e 6368 2f73 7263 2f6d  rior-bench/src/m
-00000300: 6670 6265 6e63 682f 7064 312f 6265 6e63  fpbench/pd1/benc
-00000310: 686d 6172 6b73 2f74 7261 6e73 6c61 7465  hmarks/translate
-00000320: 5f77 6d74 2e70 79da 0d5f 6372 6561 7465  _wmt.py.._create
-00000330: 5f73 7061 6365 0d00 0000 7336 0000 000a  _space....s6....
-00000340: 0204 0102 0202 0102 0102 0104 fd02 0502  ................
-00000350: 0102 0102 0102 0104 fc02 0602 0102 0102  ................
-00000360: 0104 fd02 0502 0102 0102 0102 0104 fc02  ................
-00000370: ef04 ff04 1a7a 2850 4431 7472 616e 736c  .....z(PD1transl
-00000380: 6174 6577 6d74 5f78 666f 726d 6572 5f36  atewmt_xformer_6
-00000390: 342e 5f63 7265 6174 655f 7370 6163 6529  4._create_space)
-000003a0: 014e 2904 720a 0000 0072 0b00 0000 720c  .N).r....r....r.
-000003b0: 0000 0072 0300 0000 2909 da08 5f5f 6e61  ...r....)...__na
-000003c0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000003d0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da12  ..__qualname__..
-000003e0: 7064 315f 6669 6465 6c69 7479 5f72 616e  pd1_fidelity_ran
-000003f0: 6765 7206 0000 00da 0f70 6431 5f72 6573  ger......pd1_res
-00000400: 756c 745f 7479 7065 da08 7064 315f 6e61  ult_type..pd1_na
-00000410: 6d65 da0b 636c 6173 736d 6574 686f 6472  me..classmethodr
-00000420: 1900 0000 7217 0000 0072 1700 0000 7217  ....r....r....r.
-00000430: 0000 0072 1800 0000 7207 0000 0008 0000  ...r....r.......
-00000440: 0073 0c00 0000 0800 0401 0401 0401 0202  .s..............
-00000450: 1201 7207 0000 004e 2909 da0a 5f5f 6675  ..r....N)...__fu
-00000460: 7475 7265 5f5f 7202 0000 00da 0b43 6f6e  ture__r......Con
-00000470: 6669 6753 7061 6365 7203 0000 0072 0400  figSpacer....r..
-00000480: 0000 da16 6d66 7062 656e 6368 2e70 6431  ....mfpbench.pd1
-00000490: 2e62 656e 6368 6d61 726b 7205 0000 0072  .benchmarkr....r
-000004a0: 0600 0000 7207 0000 0072 1700 0000 7217  ....r....r....r.
-000004b0: 0000 0072 1700 0000 7218 0000 00da 083c  ...r....r......<
-000004c0: 6d6f 6475 6c65 3e01 0000 0073 0800 0000  module>....s....
-000004d0: 0c00 1002 1002 1403                      ........
+00000120: 5300 290c da1b 5044 3163 6966 6172 3130  S.)...PD1cifar10
+00000130: 305f 7769 6465 7265 736e 6574 5f32 3034  0_wideresnet_204
+00000140: 3829 03e9 0100 0000 e9c7 0000 0072 0800  8)...........r..
+00000150: 0000 7a19 6369 6661 7231 3030 2d77 6964  ..z.cifar100-wid
+00000160: 655f 7265 736e 6574 2d32 3034 384e da04  e_resnet-2048N..
+00000170: 7365 6564 fa0a 696e 7420 7c20 4e6f 6e65  seed..int | None
+00000180: da06 7265 7475 726e 7203 0000 0063 0200  ..returnr....c..
+00000190: 0000 0000 0000 0000 0000 0300 0000 0b00  ................
+000001a0: 0000 4300 0001 734c 0000 0074 007c 0164  ..C...sL...t.|.d
+000001b0: 018d 017d 027c 02a0 0174 0264 0264 0364  ...}.|...t.d.d.d
+000001c0: 0464 058d 0374 0264 0664 0764 0864 0964  .d...t.d.d.d.d.d
+000001d0: 0a8d 0474 0264 0b64 0c64 0d64 058d 0374  ...t.d.d.d.d...t
+000001e0: 0264 0e64 0f64 1064 0964 0a8d 0467 04a1  .d.d.d.d.d...g..
+000001f0: 0101 007c 0253 0029 114e 2901 720a 0000  ...|.S.).N).r...
+00000200: 00da 0f6c 725f 6465 6361 795f 6661 6374  ...lr_decay_fact
+00000210: 6f72 6735 2559 87a3 ab84 3f67 ea3f 6b7e  org5%Y....?g.?k~
+00000220: fca5 ef3f 2902 da05 6c6f 7765 72da 0575  ...?)...lower..u
+00000230: 7070 6572 da0a 6c72 5f69 6e69 7469 616c  pper..lr_initial
+00000240: 67f1 68e3 88b5 f8e4 3e67 fca7 1b28 f08e  g.h.....>g...(..
+00000250: 2340 5429 0372 0e00 0000 720f 0000 00da  #@T).r....r.....
+00000260: 036c 6f67 da08 6c72 5f70 6f77 6572 67bf  .log..lr_powerg.
+00000270: 1072 deff c7b9 3f67 4984 46b0 71fd ff3f  .r....?gI.F.q..?
+00000280: da0c 6f70 745f 6d6f 6d65 6e74 756d 67fc  ..opt_momentumg.
+00000290: 6d4f 90d8 ee0e 3f67 8cda fd2a c0f7 ef3f  mO....?g...*...?
+000002a0: 2903 7203 0000 00da 1361 6464 5f68 7970  ).r......add_hyp
+000002b0: 6572 7061 7261 6d65 7465 7273 7204 0000  erparametersr...
+000002c0: 0029 03da 0363 6c73 720a 0000 00da 0263  .)...clsr......c
+000002d0: 73a9 0072 1700 0000 fa4a 2f68 6f6d 652f  s..r.....J/home/
+000002e0: 736b 616e 7469 6679 2f63 6f64 652f 6d66  skantify/code/mf
+000002f0: 2d70 7269 6f72 2d62 656e 6368 2f73 7263  -prior-bench/src
+00000300: 2f6d 6670 6265 6e63 682f 7064 312f 6265  /mfpbench/pd1/be
+00000310: 6e63 686d 6172 6b73 2f63 6966 6172 3130  nchmarks/cifar10
+00000320: 302e 7079 da0d 5f63 7265 6174 655f 7370  0.py.._create_sp
+00000330: 6163 650d 0000 0073 3600 0000 0a02 0401  ace....s6.......
+00000340: 0202 0201 0201 0201 04fd 0205 0201 0201  ................
+00000350: 0201 0201 04fc 0206 0201 0201 0201 04fd  ................
+00000360: 0205 0201 0201 0201 0201 04fc 02ef 04ff  ................
+00000370: 041a 7a29 5044 3163 6966 6172 3130 305f  ..z)PD1cifar100_
+00000380: 7769 6465 7265 736e 6574 5f32 3034 382e  wideresnet_2048.
+00000390: 5f63 7265 6174 655f 7370 6163 6529 014e  _create_space).N
+000003a0: 2904 720a 0000 0072 0b00 0000 720c 0000  ).r....r....r...
+000003b0: 0072 0300 0000 2909 da08 5f5f 6e61 6d65  .r....)...__name
+000003c0: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+000003d0: 5f5f 7175 616c 6e61 6d65 5f5f da12 7064  __qualname__..pd
+000003e0: 315f 6669 6465 6c69 7479 5f72 616e 6765  1_fidelity_range
+000003f0: 7206 0000 00da 0f70 6431 5f72 6573 756c  r......pd1_resul
+00000400: 745f 7479 7065 da08 7064 315f 6e61 6d65  t_type..pd1_name
+00000410: da0b 636c 6173 736d 6574 686f 6472 1900  ..classmethodr..
+00000420: 0000 7217 0000 0072 1700 0000 7217 0000  ..r....r....r...
+00000430: 0072 1800 0000 7207 0000 0008 0000 0073  .r....r........s
+00000440: 0c00 0000 0800 0401 0401 0401 0202 1201  ................
+00000450: 7207 0000 004e 2909 da0a 5f5f 6675 7475  r....N)...__futu
+00000460: 7265 5f5f 7202 0000 00da 0b43 6f6e 6669  re__r......Confi
+00000470: 6753 7061 6365 7203 0000 0072 0400 0000  gSpacer....r....
+00000480: da16 6d66 7062 656e 6368 2e70 6431 2e62  ..mfpbench.pd1.b
+00000490: 656e 6368 6d61 726b 7205 0000 0072 0600  enchmarkr....r..
+000004a0: 0000 7207 0000 0072 1700 0000 7217 0000  ..r....r....r...
+000004b0: 0072 1700 0000 7218 0000 00da 083c 6d6f  .r....r......<mo
+000004c0: 6475 6c65 3e01 0000 0073 0800 0000 0c00  dule>....s......
+000004d0: 1002 1002 1403                           ......
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/translate_wmt.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/translate_wmt.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/uniref50.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/uniref50.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/__pycache__/uniref50.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/__pycache__/uniref50.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/cifar100.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/cifar100.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from ConfigSpace import ConfigurationSpace, UniformFloatHyperparameter
 
 from mfpbench.pd1.benchmark import PD1Benchmark, PD1ResultTransformer
 
 
 class PD1cifar100_wideresnet_2048(PD1Benchmark):
-    pd1_fidelity_range = (45, 199, 1)
+    pd1_fidelity_range = (1, 199, 1)
     pd1_result_type = PD1ResultTransformer
-    pd1_name = "cifar100-wideresnet-2048"
+    pd1_name = "cifar100-wide_resnet-2048"
 
     @classmethod
     def _create_space(cls, seed: int | None = None) -> ConfigurationSpace:
         cs = ConfigurationSpace(seed=seed)
         cs.add_hyperparameters(
             [
                 UniformFloatHyperparameter(
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/imagenet.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/imagenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ConfigSpace import ConfigurationSpace, UniformFloatHyperparameter
 
 from mfpbench.pd1.benchmark import PD1Benchmark, PD1ResultTransformer
 
 
 class PD1imagenet_resnet_512(PD1Benchmark):
     pd1_result_type = PD1ResultTransformer
-    pd1_fidelity_range = (3, 99, 1)
+    pd1_fidelity_range = (1, 99, 1)
     pd1_name = "imagenet-resnet-512"
 
     @classmethod
     def _create_space(cls, seed: int | None = None) -> ConfigurationSpace:
         cs = ConfigurationSpace(seed=seed)
         cs.add_hyperparameters(
             [
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/lm1b.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/lm1b.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/translate_wmt.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/uniref50.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from __future__ import annotations
 
 from ConfigSpace import ConfigurationSpace, UniformFloatHyperparameter
 
 from mfpbench.pd1.benchmark import PD1Benchmark, PD1ResultTransformer
 
 
-class PD1translatewmt_xformer_64(PD1Benchmark):
-    pd1_fidelity_range = (1, 19, 1)
+class PD1uniref50_transformer_128(PD1Benchmark):
+    pd1_fidelity_range = (1, 22, 1)
     pd1_result_type = PD1ResultTransformer
-    pd1_name = "translate-wmt-xformer-64"
+    pd1_name = "uniref50-transformer-128"
 
     @classmethod
     def _create_space(cls, seed: int | None = None) -> ConfigurationSpace:
         cs = ConfigurationSpace(seed=seed)
         cs.add_hyperparameters(
             [
                 UniformFloatHyperparameter(
                     "lr_decay_factor",
-                    lower=0.0100221257,
-                    upper=0.988565263,
+                    lower=0.0111588123,
+                    upper=0.9898713967,
                 ),
                 UniformFloatHyperparameter(
                     "lr_initial",
-                    lower=1.00276e-05,
-                    upper=9.8422475735,
+                    lower=1.00564e-05,
+                    upper=0.4429248972,
                     log=True,
                 ),
                 UniformFloatHyperparameter(
                     "lr_power",
-                    lower=0.1004250993,
-                    upper=1.9985927056,
+                    lower=0.1001570089,
+                    upper=1.9989163336,
                 ),
                 UniformFloatHyperparameter(
                     "opt_momentum",
                     lower=5.86114e-05,
-                    upper=0.9989999746,
+                    upper=0.9989940217,
                     log=True,
                 ),
             ],
         )
         return cs
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/benchmarks/uniref50.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/benchmarks/translate_wmt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from __future__ import annotations
 
 from ConfigSpace import ConfigurationSpace, UniformFloatHyperparameter
 
 from mfpbench.pd1.benchmark import PD1Benchmark, PD1ResultTransformer
 
 
-class PD1uniref50_transformer_128(PD1Benchmark):
-    pd1_fidelity_range = (1, 22, 1)
+class PD1translatewmt_xformer_64(PD1Benchmark):
+    pd1_fidelity_range = (1, 19, 1)
     pd1_result_type = PD1ResultTransformer
-    pd1_name = "uniref50-transformer-128"
+    pd1_name = "translate_wmt-xformer_translate-64"
 
     @classmethod
     def _create_space(cls, seed: int | None = None) -> ConfigurationSpace:
         cs = ConfigurationSpace(seed=seed)
         cs.add_hyperparameters(
             [
                 UniformFloatHyperparameter(
                     "lr_decay_factor",
-                    lower=0.0111588123,
-                    upper=0.9898713967,
+                    lower=0.0100221257,
+                    upper=0.988565263,
                 ),
                 UniformFloatHyperparameter(
                     "lr_initial",
-                    lower=1.00564e-05,
-                    upper=0.4429248972,
+                    lower=1.00276e-05,
+                    upper=9.8422475735,
                     log=True,
                 ),
                 UniformFloatHyperparameter(
                     "lr_power",
-                    lower=0.1001570089,
-                    upper=1.9989163336,
+                    lower=0.1004250993,
+                    upper=1.9985927056,
                 ),
                 UniformFloatHyperparameter(
                     "opt_momentum",
                     lower=5.86114e-05,
-                    upper=0.9989940217,
+                    upper=0.9989999746,
                     log=True,
                 ),
             ],
         )
         return cs
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/__pycache__/columns.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/__pycache__/columns.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/__pycache__/process_script.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/__pycache__/process_script.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/columns.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/columns.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/processing/process_script.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/processing/process_script.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/__pycache__/training.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/__pycache__/training.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/__pycache__/xgboost_space.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/__pycache__/xgboost_space.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/train_xgboost.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/train_xgboost.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/training.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/training.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/pd1/surrogate/xgboost_space.py` & `mf_prior_bench-1.9.0/src/mfpbench/pd1/surrogate/xgboost_space.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/priors.py` & `mf_prior_bench-1.9.0/src/mfpbench/priors.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/result.py` & `mf_prior_bench-1.9.0/src/mfpbench/result.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/resultframe.py` & `mf_prior_bench-1.9.0/src/mfpbench/resultframe.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/setup_benchmark.py` & `mf_prior_bench-1.9.0/src/mfpbench/setup_benchmark.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/stats.py` & `mf_prior_bench-1.9.0/src/mfpbench/stats.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/__init__.py` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/__pycache__/__init__.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/__pycache__/__init__.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__init__.py` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__init__.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/__init__.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/__init__.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/benchmark.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/benchmark.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 7935 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 ff1e 0000  o........Coe....
+00000000: 6f0d 0d0a 0000 0000 70ea 3d66 ff1e 0000  o.......p.=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0173 2e02 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6401 6406 6c0d 6d0e 5a0e 0100 6401  ..d.d.l.m.Z...d.
@@ -190,17 +190,17 @@
 00000bd0: 7c08 6a04 7c09 7c00 6a03 7c00 6a02 7c01  |.j.|.|.j.|.j.|.
 00000be0: 6405 8d04 7c00 5f05 7c08 6a06 6406 6b03  d...|._.|.j.d.k.
 00000bf0: 7238 6407 7c08 6a07 9b00 6408 7c08 6a06  r8d.|.j...d.|.j.
 00000c00: 9b00 9d04 6e05 6407 7c08 6a07 9b00 9d02  ....n.d.|.j.....
 00000c10: 7d0a 7408 7c0a 7c01 6409 8d02 7d0b 7c0b  }.t.|.|.d...}.|.
 00000c20: a009 640a 640b 8400 740a 7c08 6a07 8301  ..d.d...t.|.j...
 00000c30: 4400 8301 a101 0100 740b 8300 6a0c 7c0a  D.......t...j.|.
-00000c40: 7c00 6a0d 7c00 6a0e 640c 640d 7c09 6403  |.j.|.j.d.d.|.d.
-00000c50: 6603 7c0b 7c01 7c04 7c05 7c06 7c07 640e  f.|.|.|.|.|.|.d.
-00000c60: 8d0b 0100 6401 5300 290f 6157 0300 0049  ....d.S.).aW...I
+00000c40: 7c00 6a0d 7c00 6a0e 640c 6403 7c09 6403  |.j.|.j.d.d.|.d.
+00000c50: 6603 7c0b 7c01 7c04 7c05 7c06 7c07 640d  f.|.|.|.|.|.|.d.
+00000c60: 8d0b 0100 6401 5300 290e 6157 0300 0049  ....d.S.).aW...I
 00000c70: 6e69 7469 616c 697a 6520 7468 6520 6265  nitialize the be
 00000c80: 6e63 686d 6172 6b2e 0a0a 2020 2020 2020  nchmark...      
 00000c90: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
 00000ca0: 2020 2020 7365 6564 3a20 5468 6520 7365      seed: The se
 00000cb0: 6564 2074 6f20 7573 652e 0a20 2020 2020  ed to use..     
 00000cc0: 2020 2020 2020 2062 6961 733a 2048 6f77         bias: How
 00000cd0: 206d 7563 6820 6269 6173 2074 6f20 696e   much bias to in
@@ -265,252 +265,252 @@
 00001080: da05 7570 7065 7229 0172 0c00 0000 2902  ..upper).r....).
 00001090: da02 2e30 da01 6972 2300 0000 7223 0000  ...0..ir#...r#..
 000010a0: 0072 2400 0000 da0a 3c6c 6973 7463 6f6d  .r$.....<listcom
 000010b0: 703e 9900 0000 7308 0000 0006 0002 0212  p>....s.........
 000010c0: ff06 ff7a 304d 4648 6172 746d 616e 6e42  ...z0MFHartmannB
 000010d0: 656e 6368 6d61 726b 2e5f 5f69 6e69 745f  enchmark.__init_
 000010e0: 5f2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  _.<locals>.<list
-000010f0: 636f 6d70 3eda 017a e903 0000 0029 0b72  comp>..z.....).r
-00001100: 5400 0000 da0b 636f 6e66 6967 5f74 7970  T.....config_typ
-00001110: 65da 0b72 6573 756c 745f 7479 7065 da0d  e..result_type..
-00001120: 6669 6465 6c69 7479 5f6e 616d 65da 0e66  fidelity_name..f
-00001130: 6964 656c 6974 795f 7261 6e67 65da 0573  idelity_range..s
-00001140: 7061 6365 7245 0000 0072 4800 0000 7249  pacerE...rH...rI
-00001150: 0000 0072 4a00 0000 724b 0000 0029 0fda  ...rJ...rK...)..
-00001160: 095f 5f63 6c61 7373 5f5f 7244 0000 0072  .__class__rD...r
-00001170: 4600 0000 7247 0000 0072 3f00 0000 7252  F...rG...r?...rR
-00001180: 0000 0072 4300 0000 7242 0000 0072 0b00  ...rC...rB...r..
-00001190: 0000 da13 6164 645f 6879 7065 7270 6172  ....add_hyperpar
-000011a0: 616d 6574 6572 73da 0572 616e 6765 da05  ameters..range..
-000011b0: 7375 7065 72da 085f 5f69 6e69 745f 5f72  super..__init__r
-000011c0: 4000 0000 7241 0000 0029 0cda 0473 656c  @...rA...)...sel
-000011d0: 6672 4500 0000 7246 0000 0072 4700 0000  frE...rF...rG...
-000011e0: 7248 0000 0072 4900 0000 724a 0000 0072  rH...rI...rJ...r
-000011f0: 4b00 0000 da03 636c 735a 0d5f 6d61 785f  K.....clsZ._max_
-00001200: 6669 6465 6c69 7479 7254 0000 0072 6100  fidelityrT...ra.
-00001210: 0000 a901 7262 0000 0072 2300 0000 7224  ....rb...r#...r$
-00001220: 0000 0072 6600 0000 6600 0000 7342 0000  ...rf...f...sB..
-00001230: 0006 1f18 0118 0104 0204 0202 0104 0104  ................
-00001240: 0102 0108 fc0a 0914 ff0a 0202 fd0c 0504  ................
-00001250: 0106 0108 0204 fe04 ff06 0602 0104 0104  ................
-00001260: 0102 0108 0102 0102 0102 0102 0102 0102  ................
-00001270: 010a f57a 1c4d 4648 6172 746d 616e 6e42  ...z.MFHartmannB
-00001280: 656e 6368 6d61 726b 2e5f 5f69 6e69 745f  enchmark.__init_
-00001290: 5fda 0663 6f6e 6669 67fa 114d 6170 7069  _..config..Mappi
-000012a0: 6e67 5b73 7472 2c20 416e 795d da02 6174  ng[str, Any]..at
-000012b0: da03 696e 74da 0672 6574 7572 6efa 1064  ..int..return..d
-000012c0: 6963 745b 7374 722c 2066 6c6f 6174 5d63  ict[str, float]c
-000012d0: 0200 0000 0000 0000 0100 0000 0400 0000  ................
-000012e0: 0600 0000 0300 0001 7344 0000 0074 007c  ........sD...t.|
-000012f0: 0183 0189 0074 0187 0066 0164 0164 0284  .....t...f.d.d..
-00001300: 0874 0288 0064 0364 0484 0064 058d 0244  .t...d.d...d...D
-00001310: 0083 0183 017d 037c 006a 037c 027c 0364  .....}.|.j.|.|.d
-00001320: 068d 027c 00a0 047c 02a1 0164 079c 0253  ...|...|...d...S
-00001330: 0029 084e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00001340: 0002 0000 0003 0000 0033 0000 0173 1800  .........3...s..
-00001350: 0000 8100 7c00 5d07 7d01 8800 7c01 1900  ....|.].}...|...
-00001360: 5600 0100 7102 6400 5300 2901 4e72 2300  V...q.d.S.).Nr#.
-00001370: 0000 2902 7258 0000 00da 0173 a901 da05  ..).rX.....s....
-00001380: 7175 6572 7972 2300 0000 7224 0000 00da  queryr#...r$....
-00001390: 093c 6765 6e65 7870 723e b700 0000 7304  .<genexpr>....s.
-000013a0: 0000 0002 8016 007a 3a4d 4648 6172 746d  .......z:MFHartm
-000013b0: 616e 6e42 656e 6368 6d61 726b 2e5f 6f62  annBenchmark._ob
-000013c0: 6a65 6374 6976 655f 6675 6e63 7469 6f6e  jective_function
-000013d0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-000013e0: 7072 3e63 0100 0000 0000 0000 0000 0000  pr>c............
-000013f0: 0100 0000 0400 0000 5300 0001 7312 0000  ........S...s...
-00001400: 0074 007c 00a0 0164 01a1 0164 0219 0083  .t.|...d...d....
-00001410: 0153 0029 034e 7253 0000 00e9 ffff ffff  .S.).NrS........
-00001420: 2902 726d 0000 00da 0573 706c 6974 2901  ).rm.....split).
-00001430: da01 6b72 2300 0000 7223 0000 0072 2400  ..kr#...r#...r$.
-00001440: 0000 da08 3c6c 616d 6264 613e b700 0000  ....<lambda>....
-00001450: 7302 0000 0012 007a 394d 4648 6172 746d  s......z9MFHartm
-00001460: 616e 6e42 656e 6368 6d61 726b 2e5f 6f62  annBenchmark._ob
-00001470: 6a65 6374 6976 655f 6675 6e63 7469 6f6e  jective_function
-00001480: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00001490: 613e 2901 da03 6b65 7929 0272 5b00 0000  a>)...key).r[...
-000014a0: da02 5873 722e 0000 0029 05da 0464 6963  ..Xsr....)...dic
-000014b0: 74da 0574 7570 6c65 da06 736f 7274 6564  t..tuple..sorted
-000014c0: 7252 0000 00da 0e5f 6669 6465 6c69 7479  rR....._fidelity
-000014d0: 5f63 6f73 7429 0472 6700 0000 726a 0000  _cost).rg...rj..
-000014e0: 0072 6c00 0000 7279 0000 0072 2300 0000  .rl...ry...r#...
-000014f0: 7271 0000 0072 2400 0000 da13 5f6f 626a  rq...r$....._obj
-00001500: 6563 7469 7665 5f66 756e 6374 696f 6eac  ective_function.
-00001510: 0000 0073 0600 0000 0807 2204 1a01 7a27  ...s......"...z'
-00001520: 4d46 4861 7274 6d61 6e6e 4265 6e63 686d  MFHartmannBenchm
-00001530: 6172 6b2e 5f6f 626a 6563 7469 7665 5f66  ark._objective_f
-00001540: 756e 6374 696f 6e72 1a00 0000 6302 0000  unctionr....c...
-00001550: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00001560: 0043 0000 0173 1a00 0000 6401 6402 7c01  .C...s....d.d.|.
-00001570: 7c00 6a00 6403 1900 1b00 6404 1300 1400  |.j.d.....d.....
-00001580: 1700 5300 2905 4e72 2c00 0000 6766 6666  ..S.).Nr,...gfff
-00001590: 6666 66ee 3f72 2d00 0000 e902 0000 0029  fff.?r-........)
-000015a0: 0172 6000 0000 2902 7267 0000 0072 6c00  .r`...).rg...rl.
-000015b0: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
-000015c0: 0072 7d00 0000 ba00 0000 7302 0000 001a  .r}.......s.....
-000015d0: 027a 224d 4648 6172 746d 616e 6e42 656e  .z"MFHartmannBen
-000015e0: 6368 6d61 726b 2e5f 6669 6465 6c69 7479  chmark._fidelity
-000015f0: 5f63 6f73 7472 3c00 0000 6301 0000 0000  _costr<...c.....
-00001600: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-00001610: 0000 0173 2200 0000 6401 6402 8400 7400  ...s"...d.d...t.
-00001620: 7c00 6a01 6a02 8301 4400 8301 7d01 7c00  |.j.j...D...}.|.
-00001630: 6a03 a004 7c01 a101 5300 2903 7a1d 5468  j...|...S.).z.Th
-00001640: 6520 6f70 7469 6d75 6d20 6f66 2074 6865  e optimum of the
-00001650: 2062 656e 6368 6d61 726b 2e63 0100 0000   benchmark.c....
-00001660: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00001670: 5300 0001 731c 0000 0069 007c 005d 0a5c  S...s....i.|.].\
-00001680: 027d 017d 0264 007c 019b 009d 027c 0293  .}.}.d.|.....|..
-00001690: 0271 0253 0029 0172 5500 0000 7223 0000  .q.S.).rU...r#..
-000016a0: 0029 0372 5800 0000 7259 0000 00da 0178  .).rX...rY.....x
-000016b0: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
-000016c0: 0a3c 6469 6374 636f 6d70 3ec1 0000 0073  .<dictcomp>....s
-000016d0: 0200 0000 1c00 7a2f 4d46 4861 7274 6d61  ......z/MFHartma
-000016e0: 6e6e 4265 6e63 686d 6172 6b2e 6f70 7469  nnBenchmark.opti
-000016f0: 6d75 6d2e 3c6c 6f63 616c 733e 2e3c 6469  mum.<locals>.<di
-00001700: 6374 636f 6d70 3e29 05da 0965 6e75 6d65  ctcomp>)...enume
-00001710: 7261 7465 723f 0000 00da 076f 7074 696d  rater?.....optim
-00001720: 756d 720e 0000 00da 0966 726f 6d5f 6469  umr......from_di
-00001730: 6374 2902 7267 0000 0072 8300 0000 7223  ct).rg...r....r#
-00001740: 0000 0072 2300 0000 7224 0000 0072 8300  ...r#...r$...r..
-00001750: 0000 be00 0000 7304 0000 0016 030c 017a  ......s........z
-00001760: 1b4d 4648 6172 746d 616e 6e42 656e 6368  .MFHartmannBench
-00001770: 6d61 726b 2e6f 7074 696d 756d 290e 7245  mark.optimum).rE
-00001780: 0000 0072 4c00 0000 7246 0000 0072 4d00  ...rL...rF...rM.
-00001790: 0000 7247 0000 0072 4d00 0000 7248 0000  ..rG...rM...rH..
-000017a0: 0072 4e00 0000 7249 0000 0072 4d00 0000  .rN...rI...rM...
-000017b0: 724a 0000 0072 4f00 0000 724b 0000 0072  rJ...rO...rK...r
-000017c0: 4f00 0000 2906 726a 0000 0072 6b00 0000  O...).rj...rk...
-000017d0: 726c 0000 0072 6d00 0000 726e 0000 0072  rl...rm...rn...r
-000017e0: 6f00 0000 2904 726c 0000 0072 6d00 0000  o...).rl...rm...
-000017f0: 726e 0000 0072 1a00 0000 2902 726e 0000  rn...r....).rn..
-00001800: 0072 3c00 0000 290c 721f 0000 0072 2000  .r<...).r....r .
-00001810: 0000 7221 0000 0072 2200 0000 7244 0000  ..r!...r"...rD..
-00001820: 0072 6600 0000 720a 0000 0072 7e00 0000  .rf...r....r~...
-00001830: 727d 0000 00da 0870 726f 7065 7274 7972  r}.....propertyr
-00001840: 8300 0000 da0d 5f5f 636c 6173 7363 656c  ......__classcel
-00001850: 6c5f 5f72 2300 0000 7223 0000 0072 6900  l__r#...r#...ri.
-00001860: 0000 7224 0000 0072 3e00 0000 5300 0000  ..r$...r>...S...
-00001870: 7334 0000 000a 0008 0102 0108 0202 0108  s4..............
-00001880: 0202 0108 0202 0108 0202 010c 0202 0102  ................
-00001890: 0502 0102 0102 0102 0102 0102 0112 f702  ................
-000018a0: 460c 010a 0d02 0414 0172 3e00 0000 6300  F........r>...c.
-000018b0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-000018c0: 0000 0040 0000 01f3 2200 0000 6500 5a01  ...@...."...e.Z.
-000018d0: 6400 5a02 6503 5a04 6505 5a06 6507 5a08  d.Z.e.Z.e.Z.e.Z.
-000018e0: 6503 6a09 5a0a 6401 5a0b 6402 5300 2903  e.j.Z.d.Z.d.S.).
-000018f0: da14 4d46 4861 7274 6d61 6e6e 3342 656e  ..MFHartmann3Ben
-00001900: 6368 6d61 726b 7251 0000 004e 290c 721f  chmarkrQ...N).r.
-00001910: 0000 0072 2000 0000 7221 0000 0072 1100  ...r ...r!...r..
-00001920: 0000 723f 0000 0072 1900 0000 7240 0000  ..r?...r....r@..
-00001930: 0072 2700 0000 7241 0000 00da 0464 696d  .r'...rA.....dim
-00001940: 7372 4200 0000 7243 0000 0072 2300 0000  srB...rC...r#...
-00001950: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
-00001960: 8800 0000 c800 0000 f30c 0000 0008 0004  ................
-00001970: 0704 0104 0106 0108 0172 8800 0000 6300  .........r....c.
-00001980: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00001990: 0000 0040 0000 01f3 1400 0000 6500 5a01  ...@........e.Z.
-000019a0: 6400 5a02 6401 5a03 6402 5a04 6403 5300  d.Z.d.Z.d.Z.d.S.
-000019b0: 2904 da1c 4d46 4861 7274 6d61 6e6e 3342  )...MFHartmann3B
-000019c0: 656e 6368 6d61 726b 5465 7272 6962 6c65  enchmarkTerrible
-000019d0: a902 e700 0000 0000 0010 4067 0000 0000  ..........@g....
-000019e0: 0000 1440 da08 7465 7272 6962 6c65 4ea9  ...@..terribleN.
-000019f0: 0572 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00001a00: 7244 0000 0072 4300 0000 7223 0000 0072  rD...rC...r#...r
-00001a10: 2300 0000 7223 0000 0072 2400 0000 728c  #...r#...r$...r.
-00001a20: 0000 00d6 0000 00f3 0600 0000 0800 0401  ................
-00001a30: 0801 728c 0000 0063 0000 0000 0000 0000  ..r....c........
-00001a40: 0000 0000 0000 0000 0100 0000 4000 0001  ............@...
-00001a50: 728b 0000 0029 04da 174d 4648 6172 746d  r....)...MFHartm
-00001a60: 616e 6e33 4265 6e63 686d 6172 6b42 6164  ann3BenchmarkBad
-00001a70: a902 6700 0000 0000 000c 4072 8e00 0000  ..g.......@r....
-00001a80: da03 6261 644e 7290 0000 0072 2300 0000  ..badNr....r#...
-00001a90: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
-00001aa0: 9200 0000 db00 0000 7291 0000 0072 9200  ........r....r..
-00001ab0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00001ac0: 0000 0001 0000 0040 0000 0172 8b00 0000  .......@...r....
-00001ad0: 2904 da1c 4d46 4861 7274 6d61 6e6e 3342  )...MFHartmann3B
-00001ae0: 656e 6368 6d61 726b 4d6f 6465 7261 7465  enchmarkModerate
-00001af0: a902 e700 0000 0000 0008 4072 9700 0000  ..........@r....
-00001b00: da08 6d6f 6465 7261 7465 4e72 9000 0000  ..moderateNr....
-00001b10: 7223 0000 0072 2300 0000 7223 0000 0072  r#...r#...r#...r
-00001b20: 2400 0000 7295 0000 00e0 0000 0072 9100  $...r........r..
-00001b30: 0000 7295 0000 0063 0000 0000 0000 0000  ..r....c........
-00001b40: 0000 0000 0000 0000 0100 0000 4000 0001  ............@...
-00001b50: 728b 0000 0029 04da 184d 4648 6172 746d  r....)...MFHartm
-00001b60: 616e 6e33 4265 6e63 686d 6172 6b47 6f6f  ann3BenchmarkGoo
-00001b70: 64a9 0267 0000 0000 0000 0440 6700 0000  d..g.......@g...
-00001b80: 0000 0000 40da 0467 6f6f 644e 7290 0000  ....@..goodNr...
-00001b90: 0072 2300 0000 7223 0000 0072 2300 0000  .r#...r#...r#...
-00001ba0: 7224 0000 0072 9900 0000 e500 0000 7291  r$...r........r.
-00001bb0: 0000 0072 9900 0000 6300 0000 0000 0000  ...r....c.......
-00001bc0: 0000 0000 0000 0000 0001 0000 0040 0000  .............@..
-00001bd0: 0172 8700 0000 2903 da14 4d46 4861 7274  .r....)...MFHart
-00001be0: 6d61 6e6e 3642 656e 6368 6d61 726b 7251  mann6BenchmarkrQ
-00001bf0: 0000 004e 290c 721f 0000 0072 2000 0000  ...N).r....r ...
-00001c00: 7221 0000 0072 1200 0000 723f 0000 0072  r!...r....r?...r
-00001c10: 2500 0000 7240 0000 0072 3b00 0000 7241  %...r@...r;...rA
-00001c20: 0000 0072 8900 0000 7242 0000 0072 4300  ...r....rB...rC.
-00001c30: 0000 7223 0000 0072 2300 0000 7223 0000  ..r#...r#...r#..
-00001c40: 0072 2400 0000 729c 0000 00ed 0000 0072  .r$...r........r
-00001c50: 8a00 0000 729c 0000 0063 0000 0000 0000  ....r....c......
-00001c60: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
-00001c70: 0001 728b 0000 0029 04da 1c4d 4648 6172  ..r....)...MFHar
-00001c80: 746d 616e 6e36 4265 6e63 686d 6172 6b54  tmann6BenchmarkT
-00001c90: 6572 7269 626c 6572 8d00 0000 728f 0000  erribler....r...
-00001ca0: 004e 7290 0000 0072 2300 0000 7223 0000  .Nr....r#...r#..
-00001cb0: 0072 2300 0000 7224 0000 0072 9d00 0000  .r#...r$...r....
-00001cc0: fb00 0000 7291 0000 0072 9d00 0000 6300  ....r....r....c.
-00001cd0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00001ce0: 0000 0040 0000 0172 8b00 0000 2904 da17  ...@...r....)...
-00001cf0: 4d46 4861 7274 6d61 6e6e 3642 656e 6368  MFHartmann6Bench
-00001d00: 6d61 726b 4261 6472 9300 0000 7294 0000  markBadr....r...
-00001d10: 004e 7290 0000 0072 2300 0000 7223 0000  .Nr....r#...r#..
-00001d20: 0072 2300 0000 7224 0000 0072 9e00 0000  .r#...r$...r....
-00001d30: 0001 0000 7291 0000 0072 9e00 0000 6300  ....r....r....c.
-00001d40: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00001d50: 0000 0040 0000 0172 8b00 0000 2904 da1c  ...@...r....)...
-00001d60: 4d46 4861 7274 6d61 6e6e 3642 656e 6368  MFHartmann6Bench
-00001d70: 6d61 726b 4d6f 6465 7261 7465 7296 0000  markModerater...
-00001d80: 0072 9800 0000 4e72 9000 0000 7223 0000  .r....Nr....r#..
-00001d90: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
-00001da0: 729f 0000 0005 0100 0072 9100 0000 729f  r........r....r.
-00001db0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001dc0: 0000 0000 0100 0000 4000 0001 728b 0000  ........@...r...
-00001dd0: 0029 04da 184d 4648 6172 746d 616e 6e36  .)...MFHartmann6
-00001de0: 4265 6e63 686d 6172 6b47 6f6f 6472 9a00  BenchmarkGoodr..
-00001df0: 0000 729b 0000 004e 7290 0000 0072 2300  ..r....Nr....r#.
-00001e00: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
-00001e10: 0072 a000 0000 0a01 0000 7291 0000 0072  .r........r....r
-00001e20: a000 0000 2933 da07 5f5f 646f 635f 5fda  ....)3..__doc__.
-00001e30: 0a5f 5f66 7574 7572 655f 5f72 0200 0000  .__future__r....
-00001e40: da0b 6461 7461 636c 6173 7365 7372 0300  ..dataclassesr..
-00001e50: 0000 da07 7061 7468 6c69 6272 0400 0000  ....pathlibr....
-00001e60: da06 7479 7069 6e67 7205 0000 0072 0600  ..typingr....r..
-00001e70: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
-00001e80: 00da 1174 7970 696e 675f 6578 7465 6e73  ...typing_extens
-00001e90: 696f 6e73 720a 0000 00da 056e 756d 7079  ionsr......numpy
-00001ea0: 7238 0000 00da 0b43 6f6e 6669 6753 7061  r8.....ConfigSpa
-00001eb0: 6365 720b 0000 0072 0c00 0000 da12 6d66  cer....r......mf
-00001ec0: 7062 656e 6368 2e62 656e 6368 6d61 726b  pbench.benchmark
-00001ed0: 720d 0000 00da 0f6d 6670 6265 6e63 682e  r......mfpbench.
-00001ee0: 636f 6e66 6967 720e 0000 00da 0f6d 6670  configr......mfp
-00001ef0: 6265 6e63 682e 6d65 7472 6963 720f 0000  bench.metricr...
-00001f00: 00da 0f6d 6670 6265 6e63 682e 7265 7375  ...mfpbench.resu
-00001f10: 6c74 7210 0000 00da 266d 6670 6265 6e63  ltr.....&mfpbenc
-00001f20: 682e 7379 6e74 6865 7469 632e 6861 7274  h.synthetic.hart
-00001f30: 6d61 6e6e 2e67 656e 6572 6174 6f72 7372  mann.generatorsr
-00001f40: 1100 0000 7212 0000 0072 1300 0000 7214  ....r....r....r.
-00001f50: 0000 0072 1900 0000 7225 0000 0072 6d00  ...r....r%...rm.
-00001f60: 0000 7227 0000 0072 3b00 0000 723c 0000  ..r'...r;...r<..
-00001f70: 0072 3d00 0000 723e 0000 0072 8800 0000  .r=...r>...r....
-00001f80: 728c 0000 0072 9200 0000 7295 0000 0072  r....r....r....r
-00001f90: 9900 0000 729c 0000 0072 9d00 0000 729e  ....r....r....r.
-00001fa0: 0000 0072 9f00 0000 72a0 0000 0072 2300  ...r....r....r#.
-00001fb0: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
-00001fc0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00001fd0: 6200 0000 0400 0c0a 0c02 0c01 1c01 0c01  b...............
-00001fe0: 0802 1001 0c02 0c01 0c01 0c01 1401 0c06  ................
-00001ff0: 0c03 1201 0c06 1201 0809 1a01 080d 1a01  ................
-00002000: 0c0d 0c01 2603 0a75 0201 0201 0201 0201  ....&..u........
-00002010: 02fe 02ff 04ff 100e 1005 1005 1005 0a08  ................
-00002020: 0201 0201 0201 0201 02fe 02ff 04ff 100e  ................
-00002030: 1005 1005 1405                           ......
+000010f0: 636f 6d70 3eda 017a 290b 7254 0000 00da  comp>..z).rT....
+00001100: 0b63 6f6e 6669 675f 7479 7065 da0b 7265  .config_type..re
+00001110: 7375 6c74 5f74 7970 65da 0d66 6964 656c  sult_type..fidel
+00001120: 6974 795f 6e61 6d65 da0e 6669 6465 6c69  ity_name..fideli
+00001130: 7479 5f72 616e 6765 da05 7370 6163 6572  ty_range..spacer
+00001140: 4500 0000 7248 0000 0072 4900 0000 724a  E...rH...rI...rJ
+00001150: 0000 0072 4b00 0000 290f da09 5f5f 636c  ...rK...)...__cl
+00001160: 6173 735f 5f72 4400 0000 7246 0000 0072  ass__rD...rF...r
+00001170: 4700 0000 723f 0000 0072 5200 0000 7243  G...r?...rR...rC
+00001180: 0000 0072 4200 0000 720b 0000 00da 1361  ...rB...r......a
+00001190: 6464 5f68 7970 6572 7061 7261 6d65 7465  dd_hyperparamete
+000011a0: 7273 da05 7261 6e67 65da 0573 7570 6572  rs..range..super
+000011b0: da08 5f5f 696e 6974 5f5f 7240 0000 0072  ..__init__r@...r
+000011c0: 4100 0000 290c da04 7365 6c66 7245 0000  A...)...selfrE..
+000011d0: 0072 4600 0000 7247 0000 0072 4800 0000  .rF...rG...rH...
+000011e0: 7249 0000 0072 4a00 0000 724b 0000 00da  rI...rJ...rK....
+000011f0: 0363 6c73 5a0d 5f6d 6178 5f66 6964 656c  .clsZ._max_fidel
+00001200: 6974 7972 5400 0000 7260 0000 00a9 0172  ityrT...r`.....r
+00001210: 6100 0000 7223 0000 0072 2400 0000 7265  a...r#...r$...re
+00001220: 0000 0066 0000 0073 4200 0000 061f 1801  ...f...sB.......
+00001230: 1801 0402 0402 0201 0401 0401 0201 08fc  ................
+00001240: 0a09 14ff 0a02 02fd 0c05 0401 0601 0802  ................
+00001250: 04fe 04ff 0606 0201 0401 0401 0201 0801  ................
+00001260: 0201 0201 0201 0201 0201 0201 0af5 7a1c  ..............z.
+00001270: 4d46 4861 7274 6d61 6e6e 4265 6e63 686d  MFHartmannBenchm
+00001280: 6172 6b2e 5f5f 696e 6974 5f5f da06 636f  ark.__init__..co
+00001290: 6e66 6967 fa11 4d61 7070 696e 675b 7374  nfig..Mapping[st
+000012a0: 722c 2041 6e79 5dda 0261 74da 0369 6e74  r, Any]..at..int
+000012b0: da06 7265 7475 726e fa10 6469 6374 5b73  ..return..dict[s
+000012c0: 7472 2c20 666c 6f61 745d 6302 0000 0000  tr, float]c.....
+000012d0: 0000 0001 0000 0004 0000 0006 0000 0003  ................
+000012e0: 0000 0173 4400 0000 7400 7c01 8301 8900  ...sD...t.|.....
+000012f0: 7401 8700 6601 6401 6402 8408 7402 8800  t...f.d.d...t...
+00001300: 6403 6404 8400 6405 8d02 4400 8301 8301  d.d...d...D.....
+00001310: 7d03 7c00 6a03 7c02 7c03 6406 8d02 7c00  }.|.j.|.|.d...|.
+00001320: a004 7c02 a101 6407 9c02 5300 2908 4e63  ..|...d...S.).Nc
+00001330: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001340: 0300 0000 3300 0001 7318 0000 0081 007c  ....3...s......|
+00001350: 005d 077d 0188 007c 0119 0056 0001 0071  .].}...|...V...q
+00001360: 0264 0053 0029 014e 7223 0000 0029 0272  .d.S.).Nr#...).r
+00001370: 5800 0000 da01 73a9 01da 0571 7565 7279  X.....s....query
+00001380: 7223 0000 0072 2400 0000 da09 3c67 656e  r#...r$.....<gen
+00001390: 6578 7072 3eb7 0000 0073 0400 0000 0280  expr>....s......
+000013a0: 1600 7a3a 4d46 4861 7274 6d61 6e6e 4265  ..z:MFHartmannBe
+000013b0: 6e63 686d 6172 6b2e 5f6f 626a 6563 7469  nchmark._objecti
+000013c0: 7665 5f66 756e 6374 696f 6e2e 3c6c 6f63  ve_function.<loc
+000013d0: 616c 733e 2e3c 6765 6e65 7870 723e 6301  als>.<genexpr>c.
+000013e0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000013f0: 0000 0053 0000 0173 1200 0000 7400 7c00  ...S...s....t.|.
+00001400: a001 6401 a101 6402 1900 8301 5300 2903  ..d...d.....S.).
+00001410: 4e72 5300 0000 e9ff ffff ff29 0272 6c00  NrS........).rl.
+00001420: 0000 da05 7370 6c69 7429 01da 016b 7223  ....split)...kr#
+00001430: 0000 0072 2300 0000 7224 0000 00da 083c  ...r#...r$.....<
+00001440: 6c61 6d62 6461 3eb7 0000 0073 0200 0000  lambda>....s....
+00001450: 1200 7a39 4d46 4861 7274 6d61 6e6e 4265  ..z9MFHartmannBe
+00001460: 6e63 686d 6172 6b2e 5f6f 626a 6563 7469  nchmark._objecti
+00001470: 7665 5f66 756e 6374 696f 6e2e 3c6c 6f63  ve_function.<loc
+00001480: 616c 733e 2e3c 6c61 6d62 6461 3e29 01da  als>.<lambda>)..
+00001490: 036b 6579 2902 725b 0000 00da 0258 7372  .key).r[.....Xsr
+000014a0: 2e00 0000 2905 da04 6469 6374 da05 7475  ....)...dict..tu
+000014b0: 706c 65da 0673 6f72 7465 6472 5200 0000  ple..sortedrR...
+000014c0: da0e 5f66 6964 656c 6974 795f 636f 7374  .._fidelity_cost
+000014d0: 2904 7266 0000 0072 6900 0000 726b 0000  ).rf...ri...rk..
+000014e0: 0072 7800 0000 7223 0000 0072 7000 0000  .rx...r#...rp...
+000014f0: 7224 0000 00da 135f 6f62 6a65 6374 6976  r$....._objectiv
+00001500: 655f 6675 6e63 7469 6f6e ac00 0000 7306  e_function....s.
+00001510: 0000 0008 0722 041a 017a 274d 4648 6172  ....."...z'MFHar
+00001520: 746d 616e 6e42 656e 6368 6d61 726b 2e5f  tmannBenchmark._
+00001530: 6f62 6a65 6374 6976 655f 6675 6e63 7469  objective_functi
+00001540: 6f6e 721a 0000 0063 0200 0000 0000 0000  onr....c........
+00001550: 0000 0000 0200 0000 0500 0000 4300 0001  ............C...
+00001560: 731a 0000 0064 0164 027c 017c 006a 0064  s....d.d.|.|.j.d
+00001570: 0319 001b 0064 0413 0014 0017 0053 0029  .....d.......S.)
+00001580: 054e 722c 0000 0067 6666 6666 6666 ee3f  .Nr,...gffffff.?
+00001590: 722d 0000 00e9 0200 0000 2901 725f 0000  r-........).r_..
+000015a0: 0029 0272 6600 0000 726b 0000 0072 2300  .).rf...rk...r#.
+000015b0: 0000 7223 0000 0072 2400 0000 727c 0000  ..r#...r$...r|..
+000015c0: 00ba 0000 0073 0200 0000 1a02 7a22 4d46  .....s......z"MF
+000015d0: 4861 7274 6d61 6e6e 4265 6e63 686d 6172  HartmannBenchmar
+000015e0: 6b2e 5f66 6964 656c 6974 795f 636f 7374  k._fidelity_cost
+000015f0: 723c 0000 0063 0100 0000 0000 0000 0000  r<...c..........
+00001600: 0000 0200 0000 0300 0000 4300 0001 7322  ..........C...s"
+00001610: 0000 0064 0164 0284 0074 007c 006a 016a  ...d.d...t.|.j.j
+00001620: 0283 0144 0083 017d 017c 006a 03a0 047c  ...D...}.|.j...|
+00001630: 01a1 0153 0029 037a 1d54 6865 206f 7074  ...S.).z.The opt
+00001640: 696d 756d 206f 6620 7468 6520 6265 6e63  imum of the benc
+00001650: 686d 6172 6b2e 6301 0000 0000 0000 0000  hmark.c.........
+00001660: 0000 0003 0000 0004 0000 0053 0000 0173  ...........S...s
+00001670: 1c00 0000 6900 7c00 5d0a 5c02 7d01 7d02  ....i.|.].\.}.}.
+00001680: 6400 7c01 9b00 9d02 7c02 9302 7102 5300  d.|.....|...q.S.
+00001690: 2901 7255 0000 0072 2300 0000 2903 7258  ).rU...r#...).rX
+000016a0: 0000 0072 5900 0000 da01 7872 2300 0000  ...rY.....xr#...
+000016b0: 7223 0000 0072 2400 0000 da0a 3c64 6963  r#...r$.....<dic
+000016c0: 7463 6f6d 703e c100 0000 7302 0000 001c  tcomp>....s.....
+000016d0: 007a 2f4d 4648 6172 746d 616e 6e42 656e  .z/MFHartmannBen
+000016e0: 6368 6d61 726b 2e6f 7074 696d 756d 2e3c  chmark.optimum.<
+000016f0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
+00001700: 703e 2905 da09 656e 756d 6572 6174 6572  p>)...enumerater
+00001710: 3f00 0000 da07 6f70 7469 6d75 6d72 0e00  ?.....optimumr..
+00001720: 0000 da09 6672 6f6d 5f64 6963 7429 0272  ....from_dict).r
+00001730: 6600 0000 7282 0000 0072 2300 0000 7223  f...r....r#...r#
+00001740: 0000 0072 2400 0000 7282 0000 00be 0000  ...r$...r.......
+00001750: 0073 0400 0000 1603 0c01 7a1b 4d46 4861  .s........z.MFHa
+00001760: 7274 6d61 6e6e 4265 6e63 686d 6172 6b2e  rtmannBenchmark.
+00001770: 6f70 7469 6d75 6d29 0e72 4500 0000 724c  optimum).rE...rL
+00001780: 0000 0072 4600 0000 724d 0000 0072 4700  ...rF...rM...rG.
+00001790: 0000 724d 0000 0072 4800 0000 724e 0000  ..rM...rH...rN..
+000017a0: 0072 4900 0000 724d 0000 0072 4a00 0000  .rI...rM...rJ...
+000017b0: 724f 0000 0072 4b00 0000 724f 0000 0029  rO...rK...rO...)
+000017c0: 0672 6900 0000 726a 0000 0072 6b00 0000  .ri...rj...rk...
+000017d0: 726c 0000 0072 6d00 0000 726e 0000 0029  rl...rm...rn...)
+000017e0: 0472 6b00 0000 726c 0000 0072 6d00 0000  .rk...rl...rm...
+000017f0: 721a 0000 0029 0272 6d00 0000 723c 0000  r....).rm...r<..
+00001800: 0029 0c72 1f00 0000 7220 0000 0072 2100  .).r....r ...r!.
+00001810: 0000 7222 0000 0072 4400 0000 7265 0000  ..r"...rD...re..
+00001820: 0072 0a00 0000 727d 0000 0072 7c00 0000  .r....r}...r|...
+00001830: da08 7072 6f70 6572 7479 7282 0000 00da  ..propertyr.....
+00001840: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7223  .__classcell__r#
+00001850: 0000 0072 2300 0000 7268 0000 0072 2400  ...r#...rh...r$.
+00001860: 0000 723e 0000 0053 0000 0073 3400 0000  ..r>...S...s4...
+00001870: 0a00 0801 0201 0802 0201 0802 0201 0802  ................
+00001880: 0201 0802 0201 0c02 0201 0205 0201 0201  ................
+00001890: 0201 0201 0201 0201 12f7 0246 0c01 0a0d  ...........F....
+000018a0: 0204 1401 723e 0000 0063 0000 0000 0000  ....r>...c......
+000018b0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+000018c0: 0001 f322 0000 0065 005a 0164 005a 0265  ..."...e.Z.d.Z.e
+000018d0: 035a 0465 055a 0665 075a 0865 036a 095a  .Z.e.Z.e.Z.e.j.Z
+000018e0: 0a64 015a 0b64 0253 0029 03da 144d 4648  .d.Z.d.S.)...MFH
+000018f0: 6172 746d 616e 6e33 4265 6e63 686d 6172  artmann3Benchmar
+00001900: 6b72 5100 0000 4e29 0c72 1f00 0000 7220  krQ...N).r....r 
+00001910: 0000 0072 2100 0000 7211 0000 0072 3f00  ...r!...r....r?.
+00001920: 0000 7219 0000 0072 4000 0000 7227 0000  ..r....r@...r'..
+00001930: 0072 4100 0000 da04 6469 6d73 7242 0000  .rA.....dimsrB..
+00001940: 0072 4300 0000 7223 0000 0072 2300 0000  .rC...r#...r#...
+00001950: 7223 0000 0072 2400 0000 7287 0000 00c8  r#...r$...r.....
+00001960: 0000 00f3 0c00 0000 0800 0407 0401 0401  ................
+00001970: 0601 0801 7287 0000 0063 0000 0000 0000  ....r....c......
+00001980: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00001990: 0001 f314 0000 0065 005a 0164 005a 0264  .......e.Z.d.Z.d
+000019a0: 015a 0364 025a 0464 0353 0029 04da 1c4d  .Z.d.Z.d.S.)...M
+000019b0: 4648 6172 746d 616e 6e33 4265 6e63 686d  FHartmann3Benchm
+000019c0: 6172 6b54 6572 7269 626c 65a9 02e7 0000  arkTerrible.....
+000019d0: 0000 0000 1040 6700 0000 0000 0014 40da  .....@g.......@.
+000019e0: 0874 6572 7269 626c 654e a905 721f 0000  .terribleN..r...
+000019f0: 0072 2000 0000 7221 0000 0072 4400 0000  .r ...r!...rD...
+00001a00: 7243 0000 0072 2300 0000 7223 0000 0072  rC...r#...r#...r
+00001a10: 2300 0000 7224 0000 0072 8b00 0000 d600  #...r$...r......
+00001a20: 0000 f306 0000 0008 0004 0108 0172 8b00  .............r..
+00001a30: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00001a40: 0000 0001 0000 0040 0000 0172 8a00 0000  .......@...r....
+00001a50: 2904 da17 4d46 4861 7274 6d61 6e6e 3342  )...MFHartmann3B
+00001a60: 656e 6368 6d61 726b 4261 64a9 0267 0000  enchmarkBad..g..
+00001a70: 0000 0000 0c40 728d 0000 00da 0362 6164  .....@r......bad
+00001a80: 4e72 8f00 0000 7223 0000 0072 2300 0000  Nr....r#...r#...
+00001a90: 7223 0000 0072 2400 0000 7291 0000 00db  r#...r$...r.....
+00001aa0: 0000 0072 9000 0000 7291 0000 0063 0000  ...r....r....c..
+00001ab0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+00001ac0: 0000 4000 0001 728a 0000 0029 04da 1c4d  ..@...r....)...M
+00001ad0: 4648 6172 746d 616e 6e33 4265 6e63 686d  FHartmann3Benchm
+00001ae0: 6172 6b4d 6f64 6572 6174 65a9 02e7 0000  arkModerate.....
+00001af0: 0000 0000 0840 7296 0000 00da 086d 6f64  .....@r......mod
+00001b00: 6572 6174 654e 728f 0000 0072 2300 0000  erateNr....r#...
+00001b10: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
+00001b20: 9400 0000 e000 0000 7290 0000 0072 9400  ........r....r..
+00001b30: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00001b40: 0000 0001 0000 0040 0000 0172 8a00 0000  .......@...r....
+00001b50: 2904 da18 4d46 4861 7274 6d61 6e6e 3342  )...MFHartmann3B
+00001b60: 656e 6368 6d61 726b 476f 6f64 a902 6700  enchmarkGood..g.
+00001b70: 0000 0000 0004 4067 0000 0000 0000 0040  ......@g.......@
+00001b80: da04 676f 6f64 4e72 8f00 0000 7223 0000  ..goodNr....r#..
+00001b90: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00001ba0: 7298 0000 00e5 0000 0072 9000 0000 7298  r........r....r.
+00001bb0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00001bc0: 0000 0000 0100 0000 4000 0001 7286 0000  ........@...r...
+00001bd0: 0029 03da 144d 4648 6172 746d 616e 6e36  .)...MFHartmann6
+00001be0: 4265 6e63 686d 6172 6b72 5100 0000 4e29  BenchmarkrQ...N)
+00001bf0: 0c72 1f00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+00001c00: 7212 0000 0072 3f00 0000 7225 0000 0072  r....r?...r%...r
+00001c10: 4000 0000 723b 0000 0072 4100 0000 7288  @...r;...rA...r.
+00001c20: 0000 0072 4200 0000 7243 0000 0072 2300  ...rB...rC...r#.
+00001c30: 0000 7223 0000 0072 2300 0000 7224 0000  ..r#...r#...r$..
+00001c40: 0072 9b00 0000 ed00 0000 7289 0000 0072  .r........r....r
+00001c50: 9b00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00001c60: 0000 0000 0001 0000 0040 0000 0172 8a00  .........@...r..
+00001c70: 0000 2904 da1c 4d46 4861 7274 6d61 6e6e  ..)...MFHartmann
+00001c80: 3642 656e 6368 6d61 726b 5465 7272 6962  6BenchmarkTerrib
+00001c90: 6c65 728c 0000 0072 8e00 0000 4e72 8f00  ler....r....Nr..
+00001ca0: 0000 7223 0000 0072 2300 0000 7223 0000  ..r#...r#...r#..
+00001cb0: 0072 2400 0000 729c 0000 00fb 0000 0072  .r$...r........r
+00001cc0: 9000 0000 729c 0000 0063 0000 0000 0000  ....r....c......
+00001cd0: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00001ce0: 0001 728a 0000 0029 04da 174d 4648 6172  ..r....)...MFHar
+00001cf0: 746d 616e 6e36 4265 6e63 686d 6172 6b42  tmann6BenchmarkB
+00001d00: 6164 7292 0000 0072 9300 0000 4e72 8f00  adr....r....Nr..
+00001d10: 0000 7223 0000 0072 2300 0000 7223 0000  ..r#...r#...r#..
+00001d20: 0072 2400 0000 729d 0000 0000 0100 0072  .r$...r........r
+00001d30: 9000 0000 729d 0000 0063 0000 0000 0000  ....r....c......
+00001d40: 0000 0000 0000 0000 0000 0100 0000 4000  ..............@.
+00001d50: 0001 728a 0000 0029 04da 1c4d 4648 6172  ..r....)...MFHar
+00001d60: 746d 616e 6e36 4265 6e63 686d 6172 6b4d  tmann6BenchmarkM
+00001d70: 6f64 6572 6174 6572 9500 0000 7297 0000  oderater....r...
+00001d80: 004e 728f 0000 0072 2300 0000 7223 0000  .Nr....r#...r#..
+00001d90: 0072 2300 0000 7224 0000 0072 9e00 0000  .r#...r$...r....
+00001da0: 0501 0000 7290 0000 0072 9e00 0000 6300  ....r....r....c.
+00001db0: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+00001dc0: 0000 0040 0000 0172 8a00 0000 2904 da18  ...@...r....)...
+00001dd0: 4d46 4861 7274 6d61 6e6e 3642 656e 6368  MFHartmann6Bench
+00001de0: 6d61 726b 476f 6f64 7299 0000 0072 9a00  markGoodr....r..
+00001df0: 0000 4e72 8f00 0000 7223 0000 0072 2300  ..Nr....r#...r#.
+00001e00: 0000 7223 0000 0072 2400 0000 729f 0000  ..r#...r$...r...
+00001e10: 000a 0100 0072 9000 0000 729f 0000 0029  .....r....r....)
+00001e20: 33da 075f 5f64 6f63 5f5f da0a 5f5f 6675  3..__doc__..__fu
+00001e30: 7475 7265 5f5f 7202 0000 00da 0b64 6174  ture__r......dat
+00001e40: 6163 6c61 7373 6573 7203 0000 00da 0770  aclassesr......p
+00001e50: 6174 686c 6962 7204 0000 00da 0674 7970  athlibr......typ
+00001e60: 696e 6772 0500 0000 7206 0000 0072 0700  ingr....r....r..
+00001e70: 0000 7208 0000 0072 0900 0000 da11 7479  ..r....r......ty
+00001e80: 7069 6e67 5f65 7874 656e 7369 6f6e 7372  ping_extensionsr
+00001e90: 0a00 0000 da05 6e75 6d70 7972 3800 0000  ......numpyr8...
+00001ea0: da0b 436f 6e66 6967 5370 6163 6572 0b00  ..ConfigSpacer..
+00001eb0: 0000 720c 0000 00da 126d 6670 6265 6e63  ..r......mfpbenc
+00001ec0: 682e 6265 6e63 686d 6172 6b72 0d00 0000  h.benchmarkr....
+00001ed0: da0f 6d66 7062 656e 6368 2e63 6f6e 6669  ..mfpbench.confi
+00001ee0: 6772 0e00 0000 da0f 6d66 7062 656e 6368  gr......mfpbench
+00001ef0: 2e6d 6574 7269 6372 0f00 0000 da0f 6d66  .metricr......mf
+00001f00: 7062 656e 6368 2e72 6573 756c 7472 1000  pbench.resultr..
+00001f10: 0000 da26 6d66 7062 656e 6368 2e73 796e  ...&mfpbench.syn
+00001f20: 7468 6574 6963 2e68 6172 746d 616e 6e2e  thetic.hartmann.
+00001f30: 6765 6e65 7261 746f 7273 7211 0000 0072  generatorsr....r
+00001f40: 1200 0000 7213 0000 0072 1400 0000 7219  ....r....r....r.
+00001f50: 0000 0072 2500 0000 726c 0000 0072 2700  ...r%...rl...r'.
+00001f60: 0000 723b 0000 0072 3c00 0000 723d 0000  ..r;...r<...r=..
+00001f70: 0072 3e00 0000 7287 0000 0072 8b00 0000  .r>...r....r....
+00001f80: 7291 0000 0072 9400 0000 7298 0000 0072  r....r....r....r
+00001f90: 9b00 0000 729c 0000 0072 9d00 0000 729e  ....r....r....r.
+00001fa0: 0000 0072 9f00 0000 7223 0000 0072 2300  ...r....r#...r#.
+00001fb0: 0000 7223 0000 0072 2400 0000 da08 3c6d  ..r#...r$.....<m
+00001fc0: 6f64 756c 653e 0100 0000 7362 0000 0004  odule>....sb....
+00001fd0: 000c 0a0c 020c 011c 010c 0108 0210 010c  ................
+00001fe0: 020c 010c 010c 0114 010c 060c 0312 010c  ................
+00001ff0: 0612 0108 091a 0108 0d1a 010c 0d0c 0126  ...............&
+00002000: 030a 7502 0102 0102 0102 0102 fe02 ff04  ..u.............
+00002010: ff10 0e10 0510 0510 050a 0802 0102 0102  ................
+00002020: 0102 0102 fe02 ff04 ff10 0e10 0510 0514  ................
+00002030: 05                                       .
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/benchmark.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/benchmark.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/config.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/config.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/generators.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/generators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/generators.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/generators.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/result.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/result.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/__pycache__/result.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/__pycache__/result.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/benchmark.py` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             ],
         )
         super().__init__(
             name=name,
             config_type=self.mfh_config_type,
             result_type=self.mfh_result_type,
             fidelity_name="z",
-            fidelity_range=(3, _max_fidelity, 1),
+            fidelity_range=(1, _max_fidelity, 1),
             space=space,
             seed=seed,
             prior=prior,
             perturb_prior=perturb_prior,
             value_metric=value_metric,
             cost_metric=cost_metric,
         )
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/synthetic/hartmann/generators.py` & `mf_prior_bench-1.9.0/src/mfpbench/synthetic/hartmann/generators.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/tabular.py` & `mf_prior_bench-1.9.0/src/mfpbench/tabular.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/util.py` & `mf_prior_bench-1.9.0/src/mfpbench/util.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/__init__.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/__init__.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/__init__.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/__init__.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/benchmark.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/benchmark.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/benchmark.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/benchmark.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/config.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/config.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/config.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/result.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/result.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/__pycache__/result.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/__pycache__/result.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmark.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmark.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__init__.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/__init__.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/__init__.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/lcbench.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/lcbench.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 2821 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 050b 0000  o........Coe....
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 050b 0000  o.......m.=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 a400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 5a08 6400  m.Z...d.d.l.Z.d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6400 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6503  m.Z.m.Z.m.Z...e.
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/lcbench.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/lcbench.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/nb301.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/nb301.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 3927 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 570f 0000  o........CoeW...
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 570f 0000  o.......m.=fW...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 d800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c09 6d0a 5a0a 6d0b 5a0b 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6405 6c0c 5a0d 6400 6406 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/__pycache__/nb301.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/__pycache__/nb301.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__init__.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__init__.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/__init__.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/__init__.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 2698 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 8a0a 0000  o........Coe....
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 8a0a 0000  o.......m.=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 e600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0c 5a0d 6400 6406 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_glmnet.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_glmnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_glmnet.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_glmnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_ranger.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_ranger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_ranger.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_ranger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_rpart.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_rpart.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_rpart.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_rpart.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_super.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_super.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_super.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_super.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_xgboost.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_xgboost.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_xgboost.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/__pycache__/iaml_xgboost.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml_glmnet.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml_glmnet.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml_ranger.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml_ranger.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml_rpart.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml_rpart.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml_super.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml_super.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/iaml/iaml_xgboost.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/iaml/iaml_xgboost.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/lcbench.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/lcbench.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/nb301.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/nb301.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__init__.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/__init__.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/__init__.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Dec  5 15:34:32 2023 UTC, .py size: 2544 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0843 6f65 f009 0000  o........Coe....
+00000000: 6f0d 0d0a 0000 0000 6dea 3d66 f009 0000  o.......m.=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0173 e600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6400 6404 6c0a 6d0b 5a0b 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6405 6c0c 5a0d 6400 6406 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
```

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_aknn.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_aknn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_aknn.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_aknn.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_glmnet.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_glmnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_glmnet.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_glmnet.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_ranger.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_ranger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_ranger.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_ranger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_rpart.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_rpart.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_rpart.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_rpart.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_super.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_super.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_super.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_super.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_svm.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_svm.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_svm.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_svm.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_xgboost.cpython-310.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_xgboost.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_xgboost.cpython-38.pyc` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/__pycache__/rbv2_xgboost.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_aknn.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_aknn.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_glmnet.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_glmnet.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_ranger.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_ranger.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_rpart.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_rpart.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_super.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_super.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_svm.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_svm.py`

 * *Files identical despite different names*

### Comparing `mf-prior-bench-1.8.1/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_xgboost.py` & `mf_prior_bench-1.9.0/src/mfpbench/yahpo/benchmarks/rbv2/rbv2_xgboost.py`

 * *Files identical despite different names*

