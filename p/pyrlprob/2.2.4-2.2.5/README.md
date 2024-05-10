# Comparing `tmp/pyrlprob-2.2.4.tar.gz` & `tmp/pyrlprob-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrlprob-2.2.4.tar", last modified: Tue Apr 30 22:29:31 2024, max compression
+gzip compressed data, was "pyrlprob-2.2.5.tar", last modified: Fri May 10 20:48:30 2024, max compression
```

## Comparing `pyrlprob-2.2.4.tar` & `pyrlprob-2.2.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/LICENSE.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/MANIFEST.in
--rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2808 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/PKG-INFO
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1787 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/README.md
--rw-------   0 lorenzof (332258323) domainusers (245600513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyproject.toml
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.082611 pyrlprob-2.2.4/pyrlprob/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/__main__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)    16762 2024-04-29 20:54:47.000000 pyrlprob-2.2.4/pyrlprob/base_funs.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/commands.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.082611 pyrlprob-2.2.4/pyrlprob/include/
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.086611 pyrlprob-2.2.4/pyrlprob/include/pyrlprob/
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/include/pyrlprob/binding.cpp
--rw-------   0 lorenzof (332258323) domainusers (245600513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/include/pyrlprob/mdp.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/include/pyrlprob/mdp_vec.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/include/pyrlprob/py_mdp.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     7733 2024-02-16 19:04:09.000000 pyrlprob-2.2.4/pyrlprob/mdp.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.086611 pyrlprob-2.2.4/pyrlprob/models/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      151 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/models/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)    29760 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/models/models.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)    14323 2024-04-29 20:57:36.000000 pyrlprob-2.2.4/pyrlprob/problem.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.086611 pyrlprob-2.2.4/pyrlprob/tests/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/__init__.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.086611 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/binding.cpp
--rw-------   0 lorenzof (332258323) domainusers (245600513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.cpp
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.py
--rwx------   0 lorenzof (332258323) domainusers (245600513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
--rw-------   0 lorenzof (332258323) domainusers (245600513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d_dyn.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/rk4.h
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1358 2024-02-16 18:24:51.000000 pyrlprob-2.2.4/pyrlprob/tests/landing1d_cpp.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1961 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/tests/landing1d_gtrxl_py.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1637 2024-02-16 19:31:26.000000 pyrlprob-2.2.4/pyrlprob/tests/landing1d_load.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1811 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/tests/landing1d_lstm_py.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1341 2024-02-16 19:10:05.000000 pyrlprob-2.2.4/pyrlprob/tests/landing1d_py.yaml
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.094611 pyrlprob-2.2.4/pyrlprob/tests/py_tests/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     4931 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d_dyn.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     6379 2024-02-16 18:26:17.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d_gym.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
--rw-------   0 lorenzof (332258323) domainusers (245600513)     5902 2024-04-29 20:57:24.000000 pyrlprob-2.2.4/pyrlprob/tests/test_landing1d.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2813 2024-02-16 17:36:47.000000 pyrlprob-2.2.4/pyrlprob/tests/test_multiple_gym.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/pyrlprob/tune/
--rw-------   0 lorenzof (332258323) domainusers (245600513)       87 2024-02-16 18:28:30.000000 pyrlprob-2.2.4/pyrlprob/tune/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     3393 2024-02-16 18:35:28.000000 pyrlprob-2.2.4/pyrlprob/tune/tune.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/pyrlprob/utils/
--rw-------   0 lorenzof (332258323) domainusers (245600513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.2.4/pyrlprob/utils/__init__.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     3446 2024-04-29 19:06:24.000000 pyrlprob-2.2.4/pyrlprob/utils/auxiliary.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     4722 2024-02-16 19:07:37.000000 pyrlprob-2.2.4/pyrlprob/utils/callbacks.py
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2835 2024-02-16 19:07:46.000000 pyrlprob-2.2.4/pyrlprob/utils/plots.py
-drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-04-30 22:29:31.086611 pyrlprob-2.2.4/pyrlprob.egg-info/
--rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2808 2024-04-30 22:29:30.000000 pyrlprob-2.2.4/pyrlprob.egg-info/PKG-INFO
--rw-------   0 lorenzof (332258323) domainusers (245600513)     2633 2024-04-30 22:29:30.000000 pyrlprob-2.2.4/pyrlprob.egg-info/SOURCES.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)        1 2024-04-30 22:29:30.000000 pyrlprob-2.2.4/pyrlprob.egg-info/dependency_links.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)      227 2024-04-30 22:29:30.000000 pyrlprob-2.2.4/pyrlprob.egg-info/requires.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)        9 2024-04-30 22:29:30.000000 pyrlprob-2.2.4/pyrlprob.egg-info/top_level.txt
--rw-------   0 lorenzof (332258323) domainusers (245600513)       38 2024-04-30 22:29:31.098610 pyrlprob-2.2.4/setup.cfg
--rw-------   0 lorenzof (332258323) domainusers (245600513)     1286 2024-04-30 22:29:06.000000 pyrlprob-2.2.4/setup.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.093879 pyrlprob-2.2.5/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/LICENSE.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/MANIFEST.in
+-rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2808 2024-05-10 20:48:30.093879 pyrlprob-2.2.5/PKG-INFO
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1787 2024-05-02 02:18:25.000000 pyrlprob-2.2.5/README.md
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyproject.toml
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.081879 pyrlprob-2.2.5/pyrlprob/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/__main__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    16784 2024-05-10 20:47:21.000000 pyrlprob-2.2.5/pyrlprob/base_funs.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/commands.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.069879 pyrlprob-2.2.5/pyrlprob/include/
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.085879 pyrlprob-2.2.5/pyrlprob/include/pyrlprob/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/include/pyrlprob/binding.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/include/pyrlprob/mdp.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/include/pyrlprob/mdp_vec.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/include/pyrlprob/py_mdp.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     7733 2024-02-16 19:04:09.000000 pyrlprob-2.2.5/pyrlprob/mdp.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.085879 pyrlprob-2.2.5/pyrlprob/models/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      151 2024-05-02 02:18:25.000000 pyrlprob-2.2.5/pyrlprob/models/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    29760 2024-05-02 02:18:25.000000 pyrlprob-2.2.5/pyrlprob/models/models.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)    14768 2024-05-10 20:46:43.000000 pyrlprob-2.2.5/pyrlprob/problem.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.085879 pyrlprob-2.2.5/pyrlprob/tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/__init__.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.089879 pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/binding.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/landing1d.cpp
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/landing1d.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/landing1d.py
+-rwx------   0 lorenzof (332258323) domainusers (245600513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/landing1d_dyn.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/rk4.h
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1358 2024-02-16 18:24:51.000000 pyrlprob-2.2.5/pyrlprob/tests/landing1d_cpp.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1961 2024-05-02 02:18:25.000000 pyrlprob-2.2.5/pyrlprob/tests/landing1d_gtrxl_py.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1637 2024-02-16 19:31:26.000000 pyrlprob-2.2.5/pyrlprob/tests/landing1d_load.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1811 2024-05-02 02:18:25.000000 pyrlprob-2.2.5/pyrlprob/tests/landing1d_lstm_py.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1341 2024-02-16 19:10:05.000000 pyrlprob-2.2.5/pyrlprob/tests/landing1d_py.yaml
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.089879 pyrlprob-2.2.5/pyrlprob/tests/py_tests/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4931 2024-05-02 02:18:25.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/landing1d.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/landing1d_dyn.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     6379 2024-02-16 18:26:17.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/landing1d_gym.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.093879 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     5902 2024-05-02 02:18:25.000000 pyrlprob-2.2.5/pyrlprob/tests/test_landing1d.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2813 2024-02-16 17:36:47.000000 pyrlprob-2.2.5/pyrlprob/tests/test_multiple_gym.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.093879 pyrlprob-2.2.5/pyrlprob/tune/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)       87 2024-02-16 18:28:30.000000 pyrlprob-2.2.5/pyrlprob/tune/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3393 2024-02-16 18:35:28.000000 pyrlprob-2.2.5/pyrlprob/tune/tune.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.093879 pyrlprob-2.2.5/pyrlprob/utils/
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.2.5/pyrlprob/utils/__init__.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     3446 2024-05-02 02:18:25.000000 pyrlprob-2.2.5/pyrlprob/utils/auxiliary.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     4722 2024-02-16 19:07:37.000000 pyrlprob-2.2.5/pyrlprob/utils/callbacks.py
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2835 2024-02-16 19:07:46.000000 pyrlprob-2.2.5/pyrlprob/utils/plots.py
+drwx------   0 lorenzof (332258323) domainusers (245600513)        0 2024-05-10 20:48:30.081879 pyrlprob-2.2.5/pyrlprob.egg-info/
+-rw-r--r--   0 lorenzof (332258323) domainusers (245600513)     2808 2024-05-10 20:48:29.000000 pyrlprob-2.2.5/pyrlprob.egg-info/PKG-INFO
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     2633 2024-05-10 20:48:29.000000 pyrlprob-2.2.5/pyrlprob.egg-info/SOURCES.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)        1 2024-05-10 20:48:29.000000 pyrlprob-2.2.5/pyrlprob.egg-info/dependency_links.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)      227 2024-05-10 20:48:29.000000 pyrlprob-2.2.5/pyrlprob.egg-info/requires.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)        9 2024-05-10 20:48:29.000000 pyrlprob-2.2.5/pyrlprob.egg-info/top_level.txt
+-rw-------   0 lorenzof (332258323) domainusers (245600513)       38 2024-05-10 20:48:30.093879 pyrlprob-2.2.5/setup.cfg
+-rw-------   0 lorenzof (332258323) domainusers (245600513)     1286 2024-05-10 20:47:32.000000 pyrlprob-2.2.5/setup.py
```

### Comparing `pyrlprob-2.2.4/LICENSE.txt` & `pyrlprob-2.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/PKG-INFO` & `pyrlprob-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.2.4
+Version: 2.2.5
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrlprob-2.2.4/README.md` & `pyrlprob-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/__main__.py` & `pyrlprob-2.2.5/pyrlprob/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/base_funs.py` & `pyrlprob-2.2.5/pyrlprob/base_funs.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from pyrlprob.utils.auxiliary import *
 import pyrlprob.utils.callbacks as callbacks
 
 
 def training(trainer: Union[str, Callable, Type], 
              config: Dict[str, Any], 
              stop: Dict[str, Any], 
+             best_metric: str="episode_reward_mean",
+             min_or_max: str="max",
              num_cp_to_keep: str="all",
              evaluation_active: bool=False,
              logdir: Optional[str]=None,
              create_out_file: bool=True, 
              load: Optional[Dict[str, Any]]=None, 
              debug: bool=False,
              open_ray: bool=True,
@@ -29,14 +31,16 @@
     """
     Train the current model with ray.tune, using the specified trainer and configs.
 
     Args:
         trainer (str or callable): trainer (i.e., RL algorithm) to train the model with
         config (dict): config file (dictionary)
         stop (dict): stopping conditions (dictionary)
+        best_metric (str): metric to be used to determine the best result.
+        min_or_max (str): if best_metric must be minimized or maximized
         num_cp_to_keep (str): number of checkpoints to keep. If "all", all checkpoints are kept, if "best", only the best checkpoint is kept
         evaluation_active (bool): whether evaluation is active
         logdir (str): name of the directory where training results are saved
         create_out_file (bool): whether to create an outfile with run time and best result
         load (dict): dictionary containing the directory and checkpoint where the 
             pre-trained model to load is located
         debug (bool): whether to print worker's logs.
@@ -76,30 +80,30 @@
     # Checkpoint saving
     if num_cp_to_keep == "all":
         keep_checkpoints_num = None
         checkpoint_score_attr = None
     elif num_cp_to_keep == "best":
         keep_checkpoints_num = 1
         if evaluation_active:
-            checkpoint_score_attr = "evaluation/episode_reward_mean"
+            checkpoint_score_attr = "evaluation/" + best_metric
         else:
-            checkpoint_score_attr = "episode_reward_mean"
+            checkpoint_score_attr = best_metric
     else:
         keep_checkpoints_num = None
         checkpoint_score_attr = None
 
     # Train the model
     start_time = time.time()
     analysis = tune.run(trainer,
                         config=config,
                         local_dir=outdir,
                         restore=restore,
                         stop=stop,
-                        metric="episode_reward_mean",
-                        mode="max",
+                        metric=best_metric,
+                        mode=min_or_max,
                         checkpoint_freq=1,
                         checkpoint_at_end=True,
                         keep_checkpoints_num=keep_checkpoints_num,
                         checkpoint_score_attr=checkpoint_score_attr)
     end_time = time.time()
     run_time = end_time - start_time
 
@@ -119,22 +123,20 @@
     
     # Run time per iter
     run_time_per_iter = last_result["time_this_iter_s"]
 
     # Save elapsed time and results
     if create_out_file:
         f_out_res = open(best_exp_dir + "result.txt", "w")
-        f_out_res.write("%22s %22s %22s %22s %22s\n" \
+        f_out_res.write("%22s %22s %22s\n" \
             % ("# elapsed time [s]", "training_iteration", \
-            "episode_reward_mean", "episode_reward_max", "episode_reward_min"))
-        f_out_res.write("%22.7f %22d %22.7f %22.7f %22.7f\n" \
+            best_metric))
+        f_out_res.write("%22.7f %22d %22.7f\n" \
             % (run_time, best_result["training_iteration"], \
-                best_result["episode_reward_mean"], \
-                best_result["episode_reward_max"], \
-                best_result["episode_reward_min"]))
+                best_result[best_metric]))
         f_out_res.close()
 
     # Terminate ray
     if open_ray:
         ray.shutdown()
 
     # Return trainer and best experiment directory + last checkpoint saved
```

### Comparing `pyrlprob-2.2.4/pyrlprob/commands.py` & `pyrlprob-2.2.5/pyrlprob/commands.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/include/pyrlprob/binding.cpp` & `pyrlprob-2.2.5/pyrlprob/include/pyrlprob/binding.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/include/pyrlprob/mdp.h` & `pyrlprob-2.2.5/pyrlprob/include/pyrlprob/mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/include/pyrlprob/mdp_vec.h` & `pyrlprob-2.2.5/pyrlprob/include/pyrlprob/mdp_vec.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/include/pyrlprob/py_mdp.h` & `pyrlprob-2.2.5/pyrlprob/include/pyrlprob/py_mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/mdp.py` & `pyrlprob-2.2.5/pyrlprob/mdp.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/models/models.py` & `pyrlprob-2.2.5/pyrlprob/models/models.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/problem.py` & `pyrlprob-2.2.5/pyrlprob/problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,28 @@
         else:
             settings = config_file
         self.input_config = settings
 
         #Trainer definition
         if isinstance(settings["run"], dict):
             self.__method = settings["run"]["method"]
-            self.__algorithm = settings["run"]["algorithm"]
+            self.__algorithm = settings["run"]["algorithm"].upper()
+            default_config = self.__algorithm + "_DEFAULT_CONFIG"
         else:
             self.__method = settings["run"]
             self.__algorithm = self.__method.upper()
+            default_config = "DEFAULT_CONFIG"
         alg_module = importlib.import_module("ray.rllib.agents." + self.__method)
         self.trainer = getattr(alg_module, self.__algorithm + "Trainer")
 
         #Stopping criteria definition
         self.stop = settings["stop"]
 
         #Config definition
-        self.config = alg_module.DEFAULT_CONFIG.copy()
+        self.config = getattr(alg_module, default_config).copy()
         update(self.config, settings["config"])
 
         #Evironment definition
         if "." in self.config["env"]:
             mod_name, env_name = self.config["env"].rsplit('.',1)
             mod = importlib.import_module(mod_name)
             env = getattr(mod, env_name)
@@ -160,15 +162,14 @@
         and may include evaluation and post-processing.
 
         Args:
             logdir (str): name of the directory where training results are saved
             num_cp_to_keep (str): number of checkpoints to keep. If "all", all checkpoints are kept, if "best", only the best checkpoint is kept
             evaluate (bool): whether to do evaluation
             best_metric (str): metric to be used to determine the best checkpoint in exp_dir during evaluation.
-                It it is a number, that checkpoint will be used.
             min_or_max (str): if best_metric must be minimized or maximized
             postprocess (bool): whether to do postprocessing
             debug (bool): whether to print worker's logs.
             open_ray (bool): whether to open/close ray
             return_time (bool): whether to return run time per iter
         
         Return:
@@ -181,25 +182,29 @@
         """
         
         #Training
         if return_time:
             best_result, trainer_dir, best_exp_dir, last_checkpoint, run_time = training(trainer=self.trainer, 
                                                                             config=self.config, 
                                                                             stop=self.stop,
+                                                                            best_metric=best_metric,
+                                                                            min_or_max=min_or_max,
                                                                             num_cp_to_keep=num_cp_to_keep,
                                                                             evaluation_active=self.evaluation,
                                                                             logdir=logdir,
                                                                             load=self.load,
                                                                             debug=debug,
                                                                             open_ray=open_ray,
                                                                             return_time=return_time)
         else:
             best_result, trainer_dir, best_exp_dir, last_checkpoint = training(trainer=self.trainer, 
                                                                   config=self.config, 
                                                                   stop=self.stop,
+                                                                  best_metric=best_metric,
+                                                                  min_or_max=min_or_max,
                                                                   num_cp_to_keep=num_cp_to_keep,
                                                                   evaluation_active=self.evaluation,
                                                                   logdir=logdir,
                                                                   load=self.load,
                                                                   debug=debug,
                                                                   open_ray=open_ray,
                                                                   return_time=return_time)
```

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.cpp` & `pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/landing1d.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.h` & `pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/landing1d.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d.py` & `pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so` & `pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/landing1d_dyn.h` & `pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/landing1d_dyn.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/cpp_tests/rk4.h` & `pyrlprob-2.2.5/pyrlprob/tests/cpp_tests/rk4.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/landing1d_cpp.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/landing1d_cpp.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/landing1d_gtrxl_py.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/landing1d_gtrxl_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/landing1d_load.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/landing1d_load.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/landing1d_lstm_py.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/landing1d_lstm_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/landing1d_py.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/landing1d_py.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d.py` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d_dyn.py` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/landing1d_dyn.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/landing1d_gym.py` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/landing1d_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml` & `pyrlprob-2.2.5/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/test_landing1d.py` & `pyrlprob-2.2.5/pyrlprob/tests/test_landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tests/test_multiple_gym.py` & `pyrlprob-2.2.5/pyrlprob/tests/test_multiple_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/tune/tune.py` & `pyrlprob-2.2.5/pyrlprob/tune/tune.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/utils/__init__.py` & `pyrlprob-2.2.5/pyrlprob/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/utils/auxiliary.py` & `pyrlprob-2.2.5/pyrlprob/utils/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/utils/callbacks.py` & `pyrlprob-2.2.5/pyrlprob/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob/utils/plots.py` & `pyrlprob-2.2.5/pyrlprob/utils/plots.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/pyrlprob.egg-info/PKG-INFO` & `pyrlprob-2.2.5/pyrlprob.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.2.4
+Version: 2.2.5
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrlprob-2.2.4/pyrlprob.egg-info/SOURCES.txt` & `pyrlprob-2.2.5/pyrlprob.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.2.4/setup.py` & `pyrlprob-2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='pyrlprob',
-    version='2.2.4',
+    version='2.2.5',
     author='Lorenzo Federici',
     author_email = 'federicilorenzo94@gmail.com',
     description = 'Train Gym-derived environments in Python/C++ through Ray RLlib',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/LorenzoFederici/pyrlprob',
     classifiers = [
```

