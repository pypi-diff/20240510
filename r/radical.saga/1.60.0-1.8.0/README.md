# Comparing `tmp/radical_saga-1.60.0.tar.gz` & `tmp/radical.saga-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radical_saga-1.60.0.tar", last modified: Fri May 10 13:15:17 2024, max compression
+gzip compressed data, was "dist/radical.saga-1.8.0.tar", last modified: Thu Sep 23 11:55:47 2021, max compression
```

## Comparing `radical_saga-1.60.0.tar` & `radical.saga-1.8.0.tar`

### file list

```diff
@@ -1,277 +1,283 @@
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    46969 2024-05-10 13:14:56.000000 radical_saga-1.60.0/CHANGES.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1298 2022-12-16 11:59:15.000000 radical_saga-1.60.0/LICENSE.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      209 2022-12-16 13:13:22.000000 radical_saga-1.60.0/MANIFEST.in
--rw-r--r--   0 merzky    (1000) merzky    (1000)     2650 2024-05-10 13:15:17.447867 radical_saga-1.60.0/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1260 2021-09-24 08:23:25.000000 radical_saga-1.60.0/README.md
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        7 2024-05-10 13:14:30.000000 radical_saga-1.60.0/VERSION
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.427867 radical_saga-1.60.0/bin/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)       79 2021-09-24 08:23:25.000000 radical_saga-1.60.0/bin/radical-saga-version
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.427867 radical_saga-1.60.0/examples/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.431867 radical_saga-1.60.0/examples/context/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      624 2022-03-21 12:14:26.000000 radical_saga-1.60.0/examples/context/context_ssh.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.431867 radical_saga-1.60.0/examples/files/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     2102 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/files/go_file_copy.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1941 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/files/go_remotedir_list.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1119 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/files/http_file_copy.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1702 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/files/sftp_file_copy.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1607 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/files/sftp_remotedir_list.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1478 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/files/srm_get_size.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.431867 radical_saga-1.60.0/examples/jobs/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     5194 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/cobalt.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3278 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/condorjob.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     2843 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/loadlevelerjob.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3068 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/localjob.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3431 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/localjobcontainer.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3711 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/lsfjob.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3846 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/pbsgsisshjob.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3872 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/pbsjob.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3630 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/pbsprojob.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3433 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/sgejob.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     5234 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/slurmjob.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3624 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/slurmjobcontainer.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     3539 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/jobs/torque_gsissh_job.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.431867 radical_saga-1.60.0/examples/master_worker/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     4885 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/master_worker/master.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1438 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/master_worker/worker.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.431867 radical_saga-1.60.0/examples/misc/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)      505 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/misc/inherit_context.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.427867 radical_saga-1.60.0/examples/replica/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.431867 radical_saga-1.60.0/examples/replica/irods/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     5006 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/replica/irods/irods_test.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.431867 radical_saga-1.60.0/examples/resource/
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     5158 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/resource/amazon_ec2.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)    11695 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/resource/ec2.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.431867 radical_saga-1.60.0/examples/tutorial/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.431867 radical_saga-1.60.0/examples/tutorial/mandelbrot/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2880 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/tutorial/mandelbrot/mandelbrot.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     5448 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/tutorial/mandelbrot/saga_mandelbrot.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     3960 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/tutorial/mandelbrot/saga_mandelbrot_osg.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     1996 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/tutorial/saga_example_local.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     2385 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/tutorial/saga_example_remote.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     2532 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/tutorial/saga_example_remote_cluster_staging.py
--rwxrwxr-x   0 merzky    (1000) merzky    (1000)     2671 2021-09-24 08:23:25.000000 radical_saga-1.60.0/examples/tutorial/saga_example_remote_staging.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       88 2024-05-10 13:14:24.000000 radical_saga-1.60.0/pyproject.toml
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       58 2022-12-16 11:59:15.000000 radical_saga-1.60.0/requirements-docs.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       71 2022-12-16 11:59:15.000000 radical_saga-1.60.0/requirements-tests.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       44 2024-05-10 13:15:06.000000 radical_saga-1.60.0/requirements.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       38 2024-05-10 13:15:17.447867 radical_saga-1.60.0/setup.cfg
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     6980 2024-05-10 13:14:24.000000 radical_saga-1.60.0/setup.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.427867 radical_saga-1.60.0/src/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.427867 radical_saga-1.60.0/src/radical/
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.435867 radical_saga-1.60.0/src/radical/saga/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       51 2024-05-10 13:15:17.000000 radical_saga-1.60.0/src/radical/saga/VERSION
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1549 2024-05-10 13:14:24.000000 radical_saga-1.60.0/src/radical/saga/__init__.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.435867 radical_saga-1.60.0/src/radical/saga/adaptors/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      110 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/__init__.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.435867 radical_saga-1.60.0/src/radical/saga/adaptors/aws/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/aws/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    41488 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/aws/ec2_resource.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2774 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/base.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.435867 radical_saga-1.60.0/src/radical/saga/adaptors/cobalt/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      108 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cobalt/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    50714 2022-03-21 12:14:26.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cobalt/cobaltjob.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.435867 radical_saga-1.60.0/src/radical/saga/adaptors/condor/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      106 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/condor/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    65110 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/condor/condorjob.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     3713 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/condor/transferdirectives.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.435867 radical_saga-1.60.0/src/radical/saga/adaptors/context/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/context/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4852 2022-03-21 12:14:26.000000 radical_saga-1.60.0/src/radical/saga/adaptors/context/myproxy.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     9994 2024-05-10 13:14:24.000000 radical_saga-1.60.0/src/radical/saga/adaptors/context/ssh.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2717 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/context/userpass.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4351 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/context/x509.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.435867 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      139 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/__init__.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.435867 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/advert/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      172 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/advert/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1968 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/advert/directory.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1803 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/advert/entry.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      644 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/attributes.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2687 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/base.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      467 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/context.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4831 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/decorators.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/filesystem/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      258 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/filesystem/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1725 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/filesystem/directory.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     3102 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/filesystem/file.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/job/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      247 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/job/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4854 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/job/job.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2567 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/job/service.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/namespace/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      259 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/namespace/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     3531 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/namespace/directory.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2989 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/namespace/entry.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/replica/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      270 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/replica/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2102 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/replica/logical_directory.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2464 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/replica/logical_file.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/resource/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      351 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/resource/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2210 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/resource/manager.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2588 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/resource/resource.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      420 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/cpi/sasync.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/globus_online/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/globus_online/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    42822 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/globus_online/go_file.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/http/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      104 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/http/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     7867 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/http/http_file.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/irods/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      114 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/irods/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    32419 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/irods/irods_replica.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/loadl/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      104 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/loadl/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    41780 2022-03-21 12:14:26.000000 radical_saga-1.60.0/src/radical/saga/adaptors/loadl/loadljob.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/lsf/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      106 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/lsf/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    38885 2022-09-14 23:41:32.000000 radical_saga-1.60.0/src/radical/saga/adaptors/lsf/lsfjob.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/noop/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/noop/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    18449 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/noop/noop_job.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/pbs/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      106 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/pbs/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    46490 2023-06-22 10:43:02.000000 radical_saga-1.60.0/src/radical/saga/adaptors/pbs/pbsjob.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/pbspro/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      106 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/pbspro/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    44160 2023-06-22 10:43:02.000000 radical_saga-1.60.0/src/radical/saga/adaptors/pbspro/pbsprojob.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/redis/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/redis/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1584 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/redis/redis_1.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      904 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/redis/redis_2.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    15418 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/redis/redis_advert.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2896 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/redis/redis_cache.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    20614 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/redis/redis_namespace.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.439867 radical_saga-1.60.0/src/radical/saga/adaptors/sge/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      106 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/sge/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    50027 2022-03-21 12:14:26.000000 radical_saga-1.60.0/src/radical/saga/adaptors/sge/sgejob.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.443867 radical_saga-1.60.0/src/radical/saga/adaptors/shell/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/shell/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    47096 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/shell/shell_file.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    59910 2023-03-21 19:29:01.000000 radical_saga-1.60.0/src/radical/saga/adaptors/shell/shell_job.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    12225 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/shell/shell_resource.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      324 2023-02-01 21:02:40.000000 radical_saga-1.60.0/src/radical/saga/adaptors/shell/shell_wrapper.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    28870 2022-10-11 20:08:38.000000 radical_saga-1.60.0/src/radical/saga/adaptors/shell/shell_wrapper.sh
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.443867 radical_saga-1.60.0/src/radical/saga/adaptors/slurm/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/slurm/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    59568 2023-08-01 10:11:06.000000 radical_saga-1.60.0/src/radical/saga/adaptors/slurm/slurm_job.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.443867 radical_saga-1.60.0/src/radical/saga/adaptors/srm/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/srm/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    21845 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/srm/srmfile.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.443867 radical_saga-1.60.0/src/radical/saga/adaptors/torque/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      109 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/torque/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    50168 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/adaptors/torque/torquejob.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.443867 radical_saga-1.60.0/src/radical/saga/advert/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      203 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/advert/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      935 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/advert/constants.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     7433 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/advert/directory.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     7308 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/advert/entry.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)   100992 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/attributes.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4844 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/base.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.443867 radical_saga-1.60.0/src/radical/saga/configs/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      138 2022-03-21 12:14:26.000000 radical_saga-1.60.0/src/radical/saga/configs/adaptors_cobaltjob.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      115 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/adaptors_condorjob.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1055 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/adaptors_globus_online_file.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      360 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/adaptors_loadljob.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       34 2022-03-21 12:14:26.000000 radical_saga-1.60.0/src/radical/saga/configs/adaptors_myproxy.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      359 2022-03-21 12:14:26.000000 radical_saga-1.60.0/src/radical/saga/configs/adaptors_sgejob.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      701 2022-03-21 12:14:26.000000 radical_saga-1.60.0/src/radical/saga/configs/adaptors_shell_job.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1263 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/registry_default.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1311 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/session.json
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical/saga/configs/tests/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        0 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       46 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_advert_redis_local.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       74 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_advert_redis_repex1.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      296 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_condor_osg_engage.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      326 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_condor_ssh_osg.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      228 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_default.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       51 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_file_localhost.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      132 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_fork_localhost.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      169 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_gsisftp_kraken.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      138 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_gsissh_kraken.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      217 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_irods_replica.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      201 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_lsf_localhost_yellowstone.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      286 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_pbs_gsissh_kraken.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      233 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_pbs_gsissh_trestles.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      223 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_pbs_ssh_alamo.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      214 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_pbs_ssh_archer.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      223 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_pbs_ssh_hotel.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      223 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_pbs_ssh_india.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      224 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_pbs_ssh_sierra.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      230 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_pbs_ssh_trestles.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      157 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_sftp_india.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      161 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_sftp_stampede.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      323 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_sge_gsissh_lonestar.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      398 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_sge_ssh_lonestar.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      273 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_slurm_ssh_comet.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      358 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_slurm_ssh_stampede.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      345 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_ssh_boskop.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      132 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_ssh_gw86.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      118 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_ssh_india.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      172 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_ssh_localhost.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      169 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_ssh_silver.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      311 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/tests/test_torque_gsissh_supermic.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1314 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/configs/utils_default.json
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1377 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/constants.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     5895 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/context.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical/saga/engine/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      306 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/engine/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    22430 2024-05-10 13:14:24.000000 radical_saga-1.60.0/src/radical/saga/engine/engine.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    16066 2022-12-16 11:59:15.000000 radical_saga-1.60.0/src/radical/saga/exceptions.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical/saga/filesystem/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      202 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/filesystem/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      872 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/filesystem/constants.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     7788 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/filesystem/directory.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    11356 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/filesystem/file.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical/saga/job/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      320 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/job/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     7244 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/job/constants.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     1745 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/job/container.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     5730 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/job/description.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    27060 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/job/job.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    14806 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/job/service.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical/saga/messages/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     3240 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/messages/message.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2452 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/monitorable.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical/saga/namespace/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      206 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/namespace/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      492 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/namespace/constants.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    17201 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/namespace/directory.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    11856 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/namespace/entry.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical/saga/replica/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      237 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/replica/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      756 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/replica/constants.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     6918 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/replica/logical_directory.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     8558 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/replica/logical_file.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical/saga/resource/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      222 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/resource/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2952 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/resource/constants.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     9163 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/resource/description.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     9522 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/resource/manager.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    19649 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/resource/resource.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      390 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/sasync.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    10720 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/session.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    22267 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/task.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2112 2023-02-01 21:02:40.000000 radical_saga-1.60.0/src/radical/saga/url.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical/saga/utils/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      247 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/utils/__init__.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical/saga/utils/job/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)      166 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/utils/job/__init__.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     4594 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/utils/job/transfer_directives.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     8997 2022-08-15 10:42:21.000000 radical_saga-1.60.0/src/radical/saga/utils/misc.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2154 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/utils/pty_exceptions.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    31387 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/utils/pty_process.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    43171 2022-03-21 12:14:26.000000 radical_saga-1.60.0/src/radical/saga/utils/pty_shell.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)    30520 2022-08-15 10:42:21.000000 radical_saga-1.60.0/src/radical/saga/utils/pty_shell_factory.py
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     2551 2021-09-24 08:23:25.000000 radical_saga-1.60.0/src/radical/saga/utils/test_config.py
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/src/radical.saga.egg-info/
--rw-r--r--   0 merzky    (1000) merzky    (1000)     2650 2024-05-10 13:15:17.000000 radical_saga-1.60.0/src/radical.saga.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     9042 2024-05-10 13:15:17.000000 radical_saga-1.60.0/src/radical.saga.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-05-10 13:15:17.000000 radical_saga-1.60.0/src/radical.saga.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        1 2024-05-10 13:15:17.000000 radical_saga-1.60.0/src/radical.saga.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1000) merzky    (1000)       42 2024-05-10 13:15:17.000000 radical_saga-1.60.0/src/radical.saga.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1000) merzky    (1000)        8 2024-05-10 13:15:17.000000 radical_saga-1.60.0/src/radical.saga.egg-info/top_level.txt
-drwxrwxr-x   0 merzky    (1000) merzky    (1000)        0 2024-05-10 13:15:17.447867 radical_saga-1.60.0/tests/
--rw-rw-r--   0 merzky    (1000) merzky    (1000)     3641 2021-09-24 08:23:25.000000 radical_saga-1.60.0/tests/test_cheyenne.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.753540 radical.saga-1.8.0/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    41432 2021-09-23 11:53:53.000000 radical.saga-1.8.0/CHANGES.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1284 2021-04-14 10:16:16.000000 radical.saga-1.8.0/LICENSE.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      138 2021-04-14 10:16:16.000000 radical.saga-1.8.0/MANIFEST.in
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1092 2021-09-23 11:55:47.753540 radical.saga-1.8.0/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1260 2021-06-14 10:07:23.000000 radical.saga-1.8.0/README.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2021-09-23 11:53:02.000000 radical.saga-1.8.0/VERSION
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.717540 radical.saga-1.8.0/bin/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)       79 2021-04-14 10:16:16.000000 radical.saga-1.8.0/bin/radical-saga-version
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.713540 radical.saga-1.8.0/examples/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.717540 radical.saga-1.8.0/examples/context/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      919 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/context/context_ssh.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.717540 radical.saga-1.8.0/examples/files/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2102 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/go_file_copy.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1941 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/go_remotedir_list.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1119 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/http_file_copy.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1702 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/sftp_file_copy.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1607 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/sftp_remotedir_list.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1478 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/srm_get_size.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/jobs/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5194 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/cobalt.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3278 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/condorjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2843 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/loadlevelerjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3068 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/localjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3431 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/localjobcontainer.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3711 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/lsfjob.py
+-rwxr-xr-x   0 merzky    (1001) merzky    (1001)      943 2020-01-08 22:16:58.000000 radical.saga-1.8.0/examples/jobs/noopjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3846 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/pbsgsisshjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3872 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/pbsjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3630 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/pbsprojob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3433 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/sgejob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5234 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/slurmjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3624 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/slurmjobcontainer.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3539 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/torque_gsissh_job.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/master_worker/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4885 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/master_worker/master.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1438 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/master_worker/worker.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/misc/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      505 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/misc/inherit_context.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.713540 radical.saga-1.8.0/examples/replica/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/replica/irods/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5006 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/replica/irods/irods_test.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/resource/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5158 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/resource/amazon_ec2.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)    11695 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/resource/ec2.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/tutorial/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/tutorial/mandelbrot/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2880 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/mandelbrot/mandelbrot.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5448 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/mandelbrot/saga_mandelbrot.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3960 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/mandelbrot/saga_mandelbrot_osg.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1996 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/saga_example_local.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2385 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/saga_example_remote.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2532 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/saga_example_remote_cluster_staging.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2671 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/saga_example_remote_staging.py
+-rw-r--r--   0 merzky    (1001) merzky    (1001)       87 2021-09-23 11:55:47.753540 radical.saga-1.8.0/setup.cfg
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9101 2021-09-23 09:22:40.000000 radical.saga-1.8.0/setup.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.713540 radical.saga-1.8.0/src/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.713540 radical.saga-1.8.0/src/radical/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.725540 radical.saga-1.8.0/src/radical/saga/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       40 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical/saga/SDIST
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       20 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical/saga/VERSION
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1217 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.725540 radical.saga-1.8.0/src/radical/saga/adaptors/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      110 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.725540 radical.saga-1.8.0/src/radical/saga/adaptors/aws/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/aws/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    41488 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/aws/ec2_resource.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2774 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/base.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.725540 radical.saga-1.8.0/src/radical/saga/adaptors/cobalt/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      108 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cobalt/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    51241 2021-07-08 07:53:29.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cobalt/cobaltjob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.725540 radical.saga-1.8.0/src/radical/saga/adaptors/condor/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/condor/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    65110 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/condor/condorjob.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3713 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/condor/transferdirectives.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/context/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/context/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4880 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/context/myproxy.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9994 2021-09-23 09:22:40.000000 radical.saga-1.8.0/src/radical/saga/adaptors/context/ssh.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2717 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/context/userpass.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4351 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/context/x509.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      139 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      172 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1968 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1803 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/entry.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      644 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/attributes.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2687 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/base.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      467 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/context.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4831 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/decorators.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      258 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1725 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3102 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      247 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4854 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/job.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2567 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/service.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      259 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3531 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2989 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/entry.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      270 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2102 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/logical_directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2464 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/logical_file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      351 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2210 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/manager.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2588 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/resource.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      420 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/sasync.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/globus_online/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/globus_online/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    42822 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/globus_online/go_file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/http/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      104 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/http/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7867 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/http/http_file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/irods/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      114 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/irods/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    32419 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/irods/irods_replica.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/loadl/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      104 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/loadl/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    41758 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/loadl/loadljob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/lsf/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/lsf/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    38592 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/lsf/lsfjob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/mock/
+-rw-r--r--   0 merzky    (1001) merzky    (1001)        0 2020-12-21 14:02:41.000000 radical.saga-1.8.0/src/radical/saga/adaptors/mock/__init__.py
+-rw-r--r--   0 merzky    (1001) merzky    (1001)    43999 2020-12-21 14:05:37.000000 radical.saga-1.8.0/src/radical/saga/adaptors/mock/shell_file.py
+-rw-r--r--   0 merzky    (1001) merzky    (1001)    59601 2020-12-21 14:04:14.000000 radical.saga-1.8.0/src/radical/saga/adaptors/mock/shell_job.py
+-rw-r--r--   0 merzky    (1001) merzky    (1001)    12187 2020-12-21 14:04:03.000000 radical.saga-1.8.0/src/radical/saga/adaptors/mock/shell_resource.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/noop/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/noop/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    18449 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/noop/noop_job.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/pbs/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/pbs/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    46718 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/pbs/pbsjob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/pbspro/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/pbspro/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    46968 2021-09-23 09:22:40.000000 radical.saga-1.8.0/src/radical/saga/adaptors/pbspro/pbsprojob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/redis/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1584 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_1.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      904 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_2.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    15418 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_advert.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2896 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_cache.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    20614 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_namespace.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/sge/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/sge/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    50011 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/sge/sgejob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/shell/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    47096 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_file.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    59786 2021-08-25 14:26:29.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_job.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    12225 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_resource.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      307 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_wrapper.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    28614 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_wrapper.sh
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/slurm/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/slurm/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    52416 2021-09-23 11:52:49.000000 radical.saga-1.8.0/src/radical/saga/adaptors/slurm/slurm_job.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.741540 radical.saga-1.8.0/src/radical/saga/adaptors/srm/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/srm/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    21845 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/srm/srmfile.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.741540 radical.saga-1.8.0/src/radical/saga/adaptors/torque/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      109 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/torque/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    50168 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/torque/torquejob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.741540 radical.saga-1.8.0/src/radical/saga/advert/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      203 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/advert/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      935 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/advert/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7433 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/advert/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7308 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/advert/entry.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)   100992 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/attributes.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4844 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/base.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.741540 radical.saga-1.8.0/src/radical/saga/configs/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      238 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_cobaltjob.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      115 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_condorjob.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1055 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_globus_online_file.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      360 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_loadljob.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      247 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_myproxy.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      577 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_sgejob.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      919 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_shell_job.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1263 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/registry_default.json
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.741540 radical.saga-1.8.0/src/radical/saga/configs/resources/
+-rw-r--r--   0 merzky    (1001) merzky    (1001)       21 2020-02-03 15:02:11.000000 radical.saga-1.8.0/src/radical/saga/configs/resources/stampede.json
+-rw-r--r--   0 merzky    (1001) merzky    (1001)      175 2020-02-03 15:02:35.000000 radical.saga-1.8.0/src/radical/saga/configs/resources.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1311 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/session.json
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/configs/tests/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       46 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_advert_redis_local.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       74 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_advert_redis_repex1.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      296 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_condor_osg_engage.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      326 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_condor_ssh_osg.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      228 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_default.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       51 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_file_localhost.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      132 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_fork_localhost.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      169 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_gsisftp_kraken.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      138 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_gsissh_kraken.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      217 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_irods_replica.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      201 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_lsf_localhost_yellowstone.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      286 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_gsissh_kraken.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      233 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_gsissh_trestles.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      223 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_alamo.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      214 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_archer.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      223 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_hotel.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      223 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_india.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      224 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_sierra.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      230 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_trestles.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      157 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_sftp_india.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      161 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_sftp_stampede.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      323 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_sge_gsissh_lonestar.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      398 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_sge_ssh_lonestar.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      273 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_slurm_ssh_comet.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      358 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_slurm_ssh_stampede.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      345 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_ssh_boskop.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      132 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_ssh_gw86.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      118 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_ssh_india.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      172 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_ssh_localhost.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      169 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_ssh_silver.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      311 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_torque_gsissh_supermic.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1314 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/utils_default.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1377 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5895 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/context.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/engine/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      306 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/engine/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    22540 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/engine/engine.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    16389 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/exceptions.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/filesystem/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      202 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/filesystem/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      872 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/filesystem/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7788 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/filesystem/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    11356 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/filesystem/file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/job/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      320 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7244 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1745 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/container.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5730 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/description.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    27060 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/job.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    14806 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/service.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/messages/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3240 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/messages/message.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2452 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/monitorable.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/namespace/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      206 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/namespace/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      492 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/namespace/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    17201 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/namespace/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    11856 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/namespace/entry.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/replica/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      237 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/replica/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      756 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/replica/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     6918 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/replica/logical_directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     8558 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/replica/logical_file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.753540 radical.saga-1.8.0/src/radical/saga/resource/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      222 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/resource/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2952 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/resource/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9163 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/resource/description.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9522 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/resource/manager.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    19649 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/resource/resource.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/sasync.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    10720 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/session.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    22267 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/task.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2113 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/url.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.753540 radical.saga-1.8.0/src/radical/saga/utils/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      247 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.753540 radical.saga-1.8.0/src/radical/saga/utils/job/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      166 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/job/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4594 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/job/transfer_directives.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9454 2021-09-23 09:22:40.000000 radical.saga-1.8.0/src/radical/saga/utils/misc.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2154 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/pty_exceptions.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    31387 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/pty_process.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    43400 2021-09-23 11:52:49.000000 radical.saga-1.8.0/src/radical/saga/utils/pty_shell.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    30526 2021-09-23 09:22:40.000000 radical.saga-1.8.0/src/radical/saga/utils/pty_shell_factory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2551 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/test_config.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      413 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/version.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/src/radical.saga.egg-info/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1092 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9347 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/namespace_packages.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       36 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/top_level.txt
```

### Comparing `radical_saga-1.60.0/CHANGES.md` & `radical.saga-1.8.0/CHANGES.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,171 +1,12 @@
 
 
 For a list of open issues and known problems, see:
 https://github.com/radical-cybertools/radical.saga/issues
 
-1.60.0 Release                                                        2024-05-10
---------------------------------------------------------------------------------
-
-  - Provide a target for Sphinx :py:mod: role.
-  - set version requirement for RCT stack
-  - sync with RU
-
-
-1.52.0 Release                                                        2024-04-15
---------------------------------------------------------------------------------
-
-  - fix for setuptools upgrade
-
-
-1.47.0 Release                                                        2024-02-08
---------------------------------------------------------------------------------
-
-  - maintenance
-
-
-1.46.0 Release                                                        2024-01-11
---------------------------------------------------------------------------------
-
-  - pypi fix
-
-
-1.43.0 Release                                                        2024-01-10
---------------------------------------------------------------------------------
-
-  - maintenance
-
-
-1.42.0 Release                                                        2023-12-04
---------------------------------------------------------------------------------
-
-  - maintenance
-
-
-1.41.0 Release                                                        2023-10-17
---------------------------------------------------------------------------------
-
-  - fix RTD
-  - RU dep version bump
-
-
-1.36.0 Release                                                        2023-08-01
---------------------------------------------------------------------------------
-
-  - fixed request for GPUs on Amarel (SLURM)
-
-
-1.35.0 Release                                                        2023-07-11
---------------------------------------------------------------------------------
-
-  - support `partition[:qos]` as `queue` instead of `partition/queue`
-    for Perlmutter@NERSC
-  - fixed SLURM generation for Rivanna
-
-
-1.34.0 Release                                                        2023-06-22
---------------------------------------------------------------------------------
-
-  - adding `exclusive` arg to srun
-  - cleaned intermediate fix (PBSPro)
-  - fixed final state (PBSPro)
-  - fixed monitoring update interval (PBSPro)
-  - fixed option for Perlmutter
-  - fixed option(s) for PBSPro tool(s)
-
-
-1.33.0 Release                                                        2023-04-25
---------------------------------------------------------------------------------
-
-  - fix a race condition
-  - fix CI (removed codecov)
-  - fix `core-spec` with consideration of `threads-per-core` (Slurm)
-
-
-1.22.0 Release                                                        2023-03-21
---------------------------------------------------------------------------------
-
-  - support for Frontier
-  - added set of PPNs per queue
-  - add some job attributes to the shell adaptor but ignore them
-  
-
-1.21.0 Release                                                        2023-02-01
---------------------------------------------------------------------------------
-
-  - added core specialization option (SLURM)
-  - enforce to use `threads-per-core` only if `smt` is in `system_architecture`
-  - fixed value for `processes_per_host`
-  - let shell_wrapper.py close file more promptly.
-  - updated and cleaned PBSPro adapter
-
-
-1.20.0 Release                                                        2022-12-16
---------------------------------------------------------------------------------
-
-  - bump python test env to 3.7
-  - enhanced SMT control (same approach as for LSF adaptor)
-  - SAGA.Exception to not overwrite representation
-  - sync with ru
-
-
-1.18.0 Release                                                        2022-10-11
---------------------------------------------------------------------------------
-
-  - add namespace docs as they are not pulled via inheritance
-  - allow to trap `SIGTERM` before `SIGKILL` is sent
-
-
-1.17.0 Release                                                        2022-09-15
---------------------------------------------------------------------------------
-
-  - add resource `ascent` into LSF adaptor
-  - add `threads-per-core` parameter (Slurm)
-  - convince traverse to provide GPUs
-  - enforce a predefined directory for the batch-script
-  - fix SMT setup (in sync with RADICAL-Pilot SMT setup)
-  - keep sbatch script within job's working directory
-
-
-1.16.0 Release                                                        2022-08-15
---------------------------------------------------------------------------------
-
-  - move `host_is_local` to RU
-  - spock needs -N
-
-
-1.14.0 Release                                                        2022-04-13
---------------------------------------------------------------------------------
-
-  - Add notifications to slurm
-  - another attempt to fix traverse support
-
-
-1.13.0 Release                                                        2022-03-21
---------------------------------------------------------------------------------
-
-  - support node features (constraints) in SLURM
-  - clean temporary setup files
-  - updated slurm script for `crusher`
-  
-
-1.12.0 Release                                                        2022-02-28
---------------------------------------------------------------------------------
-
-  - adding SDSC expanse to slurm adaptor
-  - consistent use of radical_base
-
-
-1.11.1 Release                                                        2022-01-19
---------------------------------------------------------------------------------
-
-  - expanse support
-  - fix PBS host lookup
-
-
 Hotfix 1.8.0 Release                                                  2021-09-23
 --------------------------------------------------------------------------------
 
   - fix directory creation (recursive flag is set)
   - add longhorn GRES exception
```

### Comparing `radical_saga-1.60.0/LICENSE.md` & `radical.saga-1.8.0/LICENSE.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-
 radical.saga is licensed under the MIT License (MIT)
 ----------------------------------------------------
 
-    Copyright (C) 2011-2023 by the RADICAL-Cybertools Team
-    (info@radical-cybertools.org)
-    
+Copyright (C) 2011-2020 by the RADICAL-Cybertools Team 
+(info@radical-cybertools.org)
+
     Permission is hereby granted, free of charge, to any person obtaining a copy
     of this software and associated documentation files (the "Software"), to
     deal in the Software without restriction, including without limitation the
     rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
     sell copies of the Software, and to permit persons to whom the Software is
     furnished to do so, subject to the following conditions:
-    
-    The above copyright notice and this permission notice shall be included in
+
+    The above copyright notice and this permission notice shall be included in 
     all copies or substantial portions of the Software.
-    
-    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-    FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
-    IN THE SOFTWARE.
 
+    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
+    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
+    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
+    FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS 
+    IN THE SOFTWARE.
```

### Comparing `radical_saga-1.60.0/README.md` & `radical.saga-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/files/go_file_copy.py` & `radical.saga-1.8.0/examples/files/go_file_copy.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/files/go_remotedir_list.py` & `radical.saga-1.8.0/examples/files/go_remotedir_list.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/files/http_file_copy.py` & `radical.saga-1.8.0/examples/files/http_file_copy.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/files/sftp_file_copy.py` & `radical.saga-1.8.0/examples/files/sftp_file_copy.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/files/sftp_remotedir_list.py` & `radical.saga-1.8.0/examples/files/sftp_remotedir_list.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/files/srm_get_size.py` & `radical.saga-1.8.0/examples/files/srm_get_size.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/cobalt.py` & `radical.saga-1.8.0/examples/jobs/cobalt.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/condorjob.py` & `radical.saga-1.8.0/examples/jobs/condorjob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/loadlevelerjob.py` & `radical.saga-1.8.0/examples/jobs/loadlevelerjob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/localjob.py` & `radical.saga-1.8.0/examples/jobs/localjob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/localjobcontainer.py` & `radical.saga-1.8.0/examples/jobs/localjobcontainer.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/lsfjob.py` & `radical.saga-1.8.0/examples/jobs/lsfjob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/pbsgsisshjob.py` & `radical.saga-1.8.0/examples/jobs/pbsgsisshjob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/pbsjob.py` & `radical.saga-1.8.0/examples/jobs/pbsjob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/pbsprojob.py` & `radical.saga-1.8.0/examples/jobs/pbsprojob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/sgejob.py` & `radical.saga-1.8.0/examples/jobs/sgejob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/slurmjob.py` & `radical.saga-1.8.0/examples/jobs/slurmjob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/slurmjobcontainer.py` & `radical.saga-1.8.0/examples/jobs/slurmjobcontainer.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/jobs/torque_gsissh_job.py` & `radical.saga-1.8.0/examples/jobs/torque_gsissh_job.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/master_worker/master.py` & `radical.saga-1.8.0/examples/master_worker/master.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/master_worker/worker.py` & `radical.saga-1.8.0/examples/master_worker/worker.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/replica/irods/irods_test.py` & `radical.saga-1.8.0/examples/replica/irods/irods_test.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/resource/amazon_ec2.py` & `radical.saga-1.8.0/examples/resource/amazon_ec2.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/resource/ec2.py` & `radical.saga-1.8.0/examples/resource/ec2.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/tutorial/mandelbrot/mandelbrot.py` & `radical.saga-1.8.0/examples/tutorial/mandelbrot/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/tutorial/mandelbrot/saga_mandelbrot.py` & `radical.saga-1.8.0/examples/tutorial/mandelbrot/saga_mandelbrot.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/tutorial/mandelbrot/saga_mandelbrot_osg.py` & `radical.saga-1.8.0/examples/tutorial/mandelbrot/saga_mandelbrot_osg.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/tutorial/saga_example_local.py` & `radical.saga-1.8.0/examples/tutorial/saga_example_local.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/tutorial/saga_example_remote.py` & `radical.saga-1.8.0/examples/tutorial/saga_example_remote.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/tutorial/saga_example_remote_cluster_staging.py` & `radical.saga-1.8.0/examples/tutorial/saga_example_remote_cluster_staging.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/examples/tutorial/saga_example_remote_staging.py` & `radical.saga-1.8.0/examples/tutorial/saga_example_remote_staging.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/__init__.py` & `radical.saga-1.8.0/src/radical/saga/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 __author__    = "RADICAL-SAGA Development Team"
 __copyright__ = "Copyright 2013, RADICAL"
 __license__   = "MIT"
 
 
 # ------------------------------------------------------------------------------
 #
+
+from .version    import *
 from .constants  import *
 
 from .task       import Task, Container
 from .attributes import Attributes, Callback
 from .session    import Session, DefaultSession
 from .context    import Context
 from .url        import Url
@@ -34,21 +36,8 @@
 from .           import resource
 # from .           import messages
 
 from .           import utils
 
 
 # ------------------------------------------------------------------------------
-#
-import os            as _os
-import radical.utils as _ru
-
-_mod_root = _os.path.dirname (__file__)
-
-version_short, version_base, version_branch, version_tag, version_detail \
-             = _ru.get_version(_mod_root)
-version      = version_short
-__version__  = version_detail
-
-
-# ------------------------------------------------------------------------------
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/aws/ec2_resource.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/aws/ec2_resource.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/base.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/base.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cobalt/cobaltjob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cobalt/cobaltjob.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 from ...              import exceptions as rse
 from ...utils         import pty_shell  as rsups
 from ...              import job        as api
 from ..               import base       as a_base
 from ..cpi            import job        as cpi_job
 from ..cpi            import decorators as cpi_decs
 
-import radical.utils as ru
-
 
 SYNC_CALL  = cpi_decs.SYNC_CALL
 ASYNC_CALL = cpi_decs.ASYNC_CALL
 
 SYNC_WAIT_UPDATE_INTERVAL =  1  # seconds
 MONITOR_UPDATE_INTERVAL   = 60  # seconds
 
@@ -308,14 +306,24 @@
 # the adaptor name
 #
 _ADAPTOR_NAME          = "radical.saga.adaptors.cobaltjob"
 _ADAPTOR_SCHEMAS       = ["cobalt", "cobalt+ssh", "cobalt+gsissh"]
 _ADAPTOR_OPTIONS       = [
     {
         'category'         : 'radical.saga.adaptors.cobaltjob',
+        'name'             : 'base_workdir',
+        'type'             : str,
+        'default'          : "$HOME/.radical/saga/adaptors/cobaltjob/",
+        'documentation'    : '''The adaptor stores job state information on the
+                              filesystem on the target resource. This parameter
+                              specified what location should be used.''',
+        'env_variable'     : None
+    },
+    {
+        'category'         : 'radical.saga.adaptors.cobaltjob',
         'name'             : 'purge_on_start',
         'type'             : bool,
         'default'          : True,
         'valid_options'    : [True, False],
         'documentation'    : '''Purge temporary job information for all
                               jobs which are older than a number of days.
                               The number of days can be configured with
@@ -422,18 +430,19 @@
 
         a_base.Base.__init__(self, _ADAPTOR_INFO, _ADAPTOR_OPTIONS)
 
         self.id_re = re.compile('^\[(.*)\]-\[(.*?)\]$')
         self.epoch = datetime.datetime(1970,1,1)
 
         # Adaptor Options
+        self.base_workdir     = self._cfg['base_workdir']
         self.purge_on_start   = self._cfg['purge_on_start']
         self.purge_older_than = self._cfg['purge_older_than']
 
-        self.base_workdir = ru.get_radical_base('saga') + 'adaptors/cobalt'
+        self.base_workdir     = os.path.normpath(self.base_workdir)
 
         # dictionaries to keep track of certain Cobalt jobs data
         self._script_file         = dict()  # location of cobalt script file
         self._job_current_workdir = dict()  # working dir, for status checking
 
 
     # --------------------------------------------------------------------------
@@ -562,17 +571,16 @@
 
 
     # --------------------------------------------------------------------------
     #
     def initialize(self):
 
         # Create the staging directory
-        ret, out, _ = self.shell.run_sync("mkdir -p %s"
-                                          % self._adaptor.base_workdir)
-
+        ret, out, _ = self.shell.run_sync ("mkdir -p %s"
+                                                   % self._adaptor.base_workdir)
         if  ret != 0 :
             raise rse.NoSuccess("Error creating staging directory. (%s): (%s)"
                            % (ret, out))
 
         # Purge temporary files
         if self._adaptor.purge_on_start:
             cmd = "find %s -type f -mtime +%d -print -delete | wc -l" % (
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/condor/condorjob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/condor/condorjob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/condor/transferdirectives.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/condor/transferdirectives.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/context/myproxy.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/context/myproxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from ...exceptions import *
 from ..            import base
 from ..cpi         import SYNC_CALL, ASYNC_CALL
 from ..cpi         import context as cpi
 from ...           import context as api
 from ...exceptions import *
 
-import radical.utils as ru
-
 
 ######################################################################
 #
 # adaptor meta data
 #
 _ADAPTOR_NAME          = 'adaptor_myproxy'
 _ADAPTOR_SCHEMAS       = ['MyProxy']
@@ -64,15 +62,15 @@
 
     def __init__ (self) :
 
         base.Base.__init__ (self, _ADAPTOR_INFO)
 
         # there are no default myproxy contexts
         self._default_contexts = []
-        self.base_workdir = ru.get_radical_base('saga') + 'adaptors/myproxy'
+        self.base_workdir = self._cfg.get('base_workdir', os.getcwd())
 
 
     def sanity_check (self) :
         pass
 
 
     def _get_default_contexts (self) :
@@ -87,15 +85,14 @@
 #
 class ContextMyProxy (cpi.Context) :
 
     def __init__ (self, api, adaptor) :
 
         _cpi_base = super  (ContextMyProxy, self)
         _cpi_base.__init__ (api, adaptor)
-
         self.base_workdir = adaptor.base_workdir
 
 
     @SYNC_CALL
     def init_instance (self, adaptor_state, type) :
 
         if not type.lower () in (schema.lower() for schema in _ADAPTOR_SCHEMAS) :
@@ -137,18 +134,19 @@
         if  api.life_time and api.life_time > 0 :
             cmd += " --proxy_lifetime %s"  %  api.life_time
 
         # store the proxy in a private location
         proxy_store    = "%s" % self.base_workdir
         proxy_location = "%s/myproxy_%d.x509"  %  (proxy_store, id(self))
 
-        try:
-            ru.rec_makedir(proxy_store)
-        except OSError as e:
-            raise NoSuccess('could not create myproxy store') from e
+        if not os.path.exists (proxy_store) :
+            try :
+                os.makedirs (proxy_store)
+            except OSError as e :
+                raise NoSuccess ("could not create myproxy store") from e
 
         cmd += " --out %s"  %  proxy_location
 
         expected_result  = "A credential has been received for user %s in %s.\n" \
                          %  (api.user_id, proxy_location)
 
         process          = subprocess.Popen (cmd, shell=True,
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/context/ssh.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/context/ssh.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/context/userpass.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/context/userpass.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/context/x509.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/context/x509.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/advert/directory.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/directory.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/advert/entry.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/entry.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/attributes.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/attributes.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/base.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/base.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/decorators.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/decorators.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/filesystem/directory.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/directory.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/filesystem/file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/file.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/job/job.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/job.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/job/service.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/service.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/namespace/directory.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/directory.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/namespace/entry.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/entry.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/replica/logical_directory.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/logical_directory.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/replica/logical_file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/logical_file.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/resource/manager.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/manager.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/cpi/resource/resource.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/resource.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/globus_online/go_file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/globus_online/go_file.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/http/http_file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/http/http_file.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/irods/irods_replica.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/irods/irods_replica.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/loadl/loadljob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/loadl/loadljob.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         self.blocking = None
         self.job_type = 'MPICH'  # TODO: Is this a sane default?
         self.enforce_resource_submission = False
         self.enforce_consumable_cpus = False
         self.enforce_consumable_memory = False
         self.enforce_consumable_virtual_memory = False
         self.enforce_consumable_large_page_memory = False
-        self.temp_path = ru.get_radical_base('saga') + 'adaptors/loadl_job'
+        self.temp_path = "$HOME/.radical/saga/adaptors/loadl_job"
 
         # LoadLeveler has two ways of specifying the executable and arguments.
         # - Explicit: the executable and arguments are specified as parameters.
         # - Implicit: the (remainder of the) job script is the task.
         #
         # Currently we don't know how this policy can be detected at runtime.
         # We know that providing both will not work in all cases.
@@ -350,17 +350,17 @@
         # different queues, number of processes per node, etc.
         # TODO: this is quite a hack. however, it *seems* to work quite
         #       well in practice.
         # modi by hgkim
 
         # purge temporary files
         if self._adaptor.purge_on_start:
-            cmd  = "find %s" % self.temp_path
-            cmd += " -type f -mtime +%d -print -delete | wc -l" \
-                                               % self._adaptor.purge_older_than
+            cmd = "find $HOME/.radical/saga/adaptors/loadl_job" \
+                  " -type f -mtime +%d -print -delete | wc -l" \
+                % self._adaptor.purge_older_than
             ret, out, _ = self.shell.run_sync(cmd)
             if ret == 0 and out != "0":
                 self._logger.info("Purged %s temporary files" % out)
 
     # ----------------------------------------------------------------
     #
     def finalize(self, kill_shell=False):
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/lsf/lsfjob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/lsf/lsfjob.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,23 +44,14 @@
                'valid_alloc_flags': [
                    'gpumps',
                    'gpudefault',
                    'nvme',
                    'spectral',
                    'maximizegpfs'
                ]},
-    'ascent': {'cpn': 42,
-               'gpn': 6,
-               'valid_alloc_flags': [
-                   'gpumps',
-                   'gpudefault',
-                   'nvme',
-                   'spectral',
-                   'maximizegpfs'
-               ]},
     'lassen': {'cpn': 40,
                'gpn': 4,
                'valid_alloc_flags': [
                    'atsdisable',
                    'autonumaoff',
                    'cpublink',
                    'ipisolate'
@@ -224,32 +215,29 @@
         out, _, ret = ru.sh_callout('hostname -f')
         if ret: hostname = os.environ.get('HOSTNAME', '')
         else  : hostname = out.strip()
 
     if not hostname:
         raise RuntimeError('cannot determine target host f or %s' % url)
 
-    smt = int(jd.environment.get('RADICAL_SMT') or
-              jd.system_architecture.get('smt') or
-              SMT_DEFAULT)
-
-    if smt not in SMT_VALID_VALUES:
-        smt = SMT_DEFAULT
-
-    cpn, gpn, valid_alloc_flags = 0, 1, []
+    cpn, gpn, smt, valid_alloc_flags = 0, 1, SMT_DEFAULT, []
     for resource_name in RESOURCES:
         if resource_name in hostname:
+            smt = jd.system_architecture.get('smt') or smt
             cpn = RESOURCES[resource_name]['cpn'] * smt
             gpn = RESOURCES[resource_name]['gpn']
             valid_alloc_flags = RESOURCES[resource_name]['valid_alloc_flags']
             break
 
     if not cpn:
         raise ValueError('LSF host (%s) not yet supported' % hostname)
 
+    if smt not in SMT_VALID_VALUES:
+        smt = SMT_DEFAULT
+
     cpu_nodes = int(total_cpu_count / cpn)
     if total_cpu_count > (cpu_nodes * cpn):
         cpu_nodes += 1
 
     gpu_nodes = int(total_gpu_count / gpn)
     if total_gpu_count > (gpu_nodes * gpn):
         gpu_nodes += 1
@@ -260,16 +248,16 @@
     alloc_flags = []
     for flag in jd.system_architecture.get('options', []):
         if flag.lower() in valid_alloc_flags:
             alloc_flags.append(flag.lower())
     alloc_flags.append('smt%d' % smt)
     lsf_bsubs += "#BSUB -alloc_flags '%s' \n" % ' '.join(alloc_flags)
 
+    env_string += "export RADICAL_SAGA_SMT=%d" % smt
     if jd.environment:
-        env_string += "export"
         for k, v in jd.environment.items():
             env_string += " %s=%s" % (k, v)
 
     # escape double quotes and dollar signs, otherwise 'echo |'
     # further down won't work
     # only escape '$' in args and exe. not in the bsubs
     command   = command.replace('$', '\\$')
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/noop/noop_job.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/noop/noop_job.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/pbs/pbsjob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/pbs/pbsjob.py`

 * *Files 2% similar despite different names*

```diff
@@ -737,21 +737,24 @@
     #
     def _retrieve_job(self, job_id):
         """ see if we can get some info about a job that we don't
             know anything about
         """
         # rm, pid = self._adaptor.parse_id(job_id)
 
-        # # run the PBS 'qstat' command to get job's info
+        # # run the PBS 'qstat' command to get some infos about our job
+        # if 'PBSPro_1' in self._commands['qstat']['version']:
+        #     qstat_flag = '-f'
+        # else:
+        #     qstat_flag ='-f1'
         #
-        # qstat_flags = '-fx'
         # ret, out, _ = self.shell.run_sync("unset GREP_OPTIONS; %s %s %s | "\
         #         "grep -E -i '(job_state)|(exec_host)|(exit_status)|(ctime)|"\
         #         "(start_time)|(comp_time)|(stime)|(qtime)|(mtime)'" \
-        #       % (self._commands['qstat']['path'], qstat_flags, pid))
+        #       % (self._commands['qstat']['path'], qstat_flag, pid))
 
         # if ret != 0:
         #     raise NoSuccess("Couldn't reconnect job '%s': %s" % (job_id, out))
 
         # else:
         #     # the job seems to exist on the backend. let's gather some data
         #     job_info = {
@@ -800,22 +803,25 @@
                 'start_time':   None,
                 'end_time':     None,
                 'gone':         False
             }
 
         rm, pid = self._adaptor.parse_id(job_id)
 
-        # run the PBS 'qstat' command to get job's info
-        # options: "-f" - long format; "-x" - includes finished jobs
-        qstat_flags = '-fx'
+        # run the PBS 'qstat' command to get some infos about our job
+        # TODO: create a PBSPRO/TORQUE flag once
+        if 'PBSPro_1' in self._commands['qstat']['version']:
+            qstat_flag = '-fx'
+        else:
+            qstat_flag = '-f1'
 
         ret, out, _ = self.shell.run_sync("unset GREP_OPTIONS; %s %s %s | "
                 "grep -E -i '(job_state)|(exec_host)|(exit_status)|"
                  "(ctime)|(start_time)|(stime)|(mtime)'"
-                % (self._commands['qstat']['path'], qstat_flags, pid))
+                % (self._commands['qstat']['path'], qstat_flag, pid))
 
         if ret != 0:
 
             if reconnect:
                 raise rse.NoSuccess("Couldn't reconnect job %s: %s" % (job_id, out))
 
             if ("Unknown Job Id" in out):
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/pbspro/pbsprojob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/pbspro/pbsprojob.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 from ..cpi            import job        as cpi
 from ..cpi            import decorators as cpi_decs
 
 
 SYNC_CALL  = cpi_decs.SYNC_CALL
 ASYNC_CALL = cpi_decs.ASYNC_CALL
 
-SYNC_WAIT_UPDATE_INTERVAL = 1  # seconds
-MONITOR_UPDATE_INTERVAL   = 5  # seconds
+SYNC_WAIT_UPDATE_INTERVAL =  1  # seconds
+MONITOR_UPDATE_INTERVAL   = 60  # seconds
 
 
 # --------------------------------------------------------------------
 #
 class _job_state_monitor(threading.Thread):
     """ thread that periodically monitors job states
     """
@@ -75,15 +75,15 @@
                     if  job_info['state'] not in api.FINAL:
 
                         # Store the current state since the current state
                         # variable is updated when _job_get_info is called
                         pre_update_state = job_info['state']
 
                         new_job_info = self.js._job_get_info(job_id, reconnect=False)
-                        self.logger.debug("Job monitoring thread updating Job "
+                        self.logger.info ("Job monitoring thread updating Job "
                                           "%s (old state: %s, new state: %s)" %
                                           (job_id, pre_update_state, new_job_info['state']))
 
                         # fire job state callback if 'state' has changed
                         if  new_job_info['state'] != pre_update_state:
                             job_obj = job_info['obj']
                             job_obj._attributes_i_set('state',
@@ -126,14 +126,16 @@
     # R: Job is running.
     # E: Job is exiting after having run
     # T: Job is being moved to new location.
     # X: Subjob has completed execution or has been deleted (PBSPro)
     # F: Job is Finished (PBSPro)
     # C: Job is completed after having run (Torque)
 
+    ret = None
+
     if   job_state == 'C':     # Torque
         if retcode ==  0 : ret = api.DONE
         else             : ret = api.FAILED
     elif job_state == 'F':     # PBSPro
         if retcode ==  0 : ret = api.DONE
         else             : ret = api.FAILED
     elif job_state == 'H': ret = api.PENDING
@@ -155,150 +157,204 @@
 
 # --------------------------------------------------------------------
 #
 def _script_generator(url, logger, jd, ppn, gres, version, is_cray=False,
                       queue=None):
     """ generates a batch script from a SAGA job description
     """
-    pbs_params  = ''
+    pbs_params  = str()
+    exec_n_args = str()
+
+    if jd.processes_per_host:
+        logger.info("Override detected ppn (%d) with user ppn (%d)" % (ppn, jd.processes_per_host))
+        ppn = jd.processes_per_host
+
+    exec_n_args += 'export SAGA_PPN=%d\n' % ppn
+    if jd.executable:
+        exec_n_args += "%s " % (jd.executable)
+    if jd.arguments:
+        for arg in jd.arguments:
+            exec_n_args += "%s " % (arg)
 
     if jd.name:
-        pbs_params += '#PBS -N %s\n' % jd.name
+        pbs_params += "#PBS -N %s \n" % jd.name
+
+    if is_cray or 'Version: 4.2.7' not in version:
+        # qsub on Cray systems complains about the -V option:
+        # Warning:
+        # Your job uses the -V option, which requests that all of your
+        # current shell environment settings (9913 bytes) be exported to
+        # it.  This is not recommended, as it causes problems for the
+        # batch environment in some cases.
+        pbs_params += "#PBS -V \n"
+
+    if jd.environment:
+        pbs_params += "#PBS -v %s\n" % \
+                ','.join (["%s=%s" % (k,v)
+                           for k,v in jd.environment.items()])
+
+    # apparently this doesn't work with older PBS installations
+    #    if jd.working_directory:
+    #        pbs_params += "#PBS -d %s \n" % jd.working_directory
+    #
+    # a workaround is to do an explicit 'cd'
+    if jd.working_directory:
+        workdir_directives  = 'export    PBS_O_WORKDIR=%s \n' % jd.working_directory
+        workdir_directives += 'mkdir -p  %s\n' % jd.working_directory
+        workdir_directives += 'cd        %s\n' % jd.working_directory
+    else:
+        workdir_directives = ''
 
     if jd.output:
-        stdout_dir = ''
-        if jd.working_directory and not os.path.isabs(jd.output):
-            # user provided a relative path for STDOUT
-            stdout_dir = '%s/' % jd.working_directory
-        pbs_params += '#PBS -o %s%s\n' % (stdout_dir, jd.output)
+        # if working directory is set, we want stdout to end up in
+        # the working directory as well, unless it containes a specific
+        # path name.
+        if jd.working_directory:
+            if os.path.isabs(jd.output):
+                pbs_params += "#PBS -o %s \n" % jd.output
+            else:
+                # user provided a relative path for STDOUT. in this case
+                # we prepend the workind directory path before passing
+                # it on to PBS
+                pbs_params += "#PBS -o %s/%s \n" % (jd.working_directory, jd.output)
+        else:
+            pbs_params += "#PBS -o %s \n" % jd.output
 
     if jd.error:
-        stderr_dir = ''
-        if jd.working_directory and not os.path.isabs(jd.error):
-            # user provided a relative path for STDERR
-            stderr_dir = '%s/' % jd.working_directory
-        pbs_params += '#PBS -e %s%s\n' % (stderr_dir, jd.error)
+        # if working directory is set, we want stderr to end up in
+        # the working directory as well, unless it contains a specific
+        # path name.
+        if jd.working_directory:
+            if os.path.isabs(jd.error):
+                pbs_params += "#PBS -e %s \n" % jd.error
+            else:
+                # user provided a realtive path for STDERR. in this case
+                # we prepend the workind directory path before passing
+                # it on to PBS
+                pbs_params += "#PBS -e %s/%s \n" % (jd.working_directory, jd.error)
+        else:
+            pbs_params += "#PBS -e %s \n" % jd.error
 
-    if jd.wall_time_limit:
-        pbs_params += '#PBS -l walltime=%s:%s:00\n' \
-            % (int(jd.wall_time_limit / 60), jd.wall_time_limit % 60)
 
-    if jd.project:
-        pbs_params += '#PBS -A %s\n' % jd.project
-        if 'PBSPro_1' in version:
-            # set both parameters: -P(roject) and -A(accounting)
-            # depends on system configuration (check with site admin if needed)
-            pbs_params += '#PBS -P %s\n' % jd.project
-
-    if jd.job_contact:
-        pbs_params += '#PBS -M %s\n' % jd.job_contact
-        pbs_params += '#PBS -m abe\n'  # sends email on job abort, begin and end
+    if jd.wall_time_limit:
+        hours = int(jd.wall_time_limit / 60)
+        minutes = jd.wall_time_limit % 60
+        pbs_params += "#PBS -l walltime=%s:%s:00 \n" \
+            % (str(hours), str(minutes))
 
     # see https://gist.github.com/nobias/5b2373258e595e5242d5
     # The parameter to '-q' can have the following forms:
     #
     #   queue
     #   queue@server
     #   @server
     #
     # where 'server' is the target resource which can be *different* than the
     # submission host.  We interpret 'jd.candidate_hosts[0]' as such a target
     # resource - but only if exactly one `candidate_host` is given.
-    #
-    # We have to take care to filter out special cases where we abuse
+
+    # We haqve to take care to filter out special cases where we abise
     # `candidate_hosts` for node properties (those are appended to the nodes
     # argument in the resource_list).  This is currently only implemented for
     # "bigflash" on Gordon@SDSC
     #
     # https://github.com/radical-cybertools/radical.saga/issues/406
-    #
-    # Parse candidate_hosts, node properties are appended to the nodes
-    # argument in the resource_list.
-    queue_spec = queue or jd.queue or ''
 
+    queue_spec      = ''
     node_properties = []
-    if jd.candidate_hosts:
-        if 'BIG_FLASH' in jd.candidate_hosts:
-            node_properties.append('bigflash')
-        elif len(jd.candidate_hosts) == 1:
-            queue_spec += '@%s' % jd.candidate_hosts[0]
-        else:
-            raise rse.NotImplemented(
-                'unsupported candidate_hosts [%s]' % jd.candidate_hosts)
 
+    if      queue: queue_spec =    queue
+    elif jd.queue: queue_spec = jd.queue
+
+    # Parse candidate_hosts
+    #
+    # Node properties are appended to the nodes argument in the resource_list.
+    #
+    # Currently only implemented for "bigflash" on Gordon@SDSC
+    # https://github.com/radical-cybertools/saga-python/issues/406
+    #
     if queue_spec:
-        pbs_params += '#PBS -q %s\n' % queue_spec
+        pbs_params += "#PBS -q %s\n" % queue_spec
 
-    if jd.processes_per_host:
-        logger.info('Override detected ppn (%d) with user ppn (%d)' %
-                    (ppn, jd.processes_per_host))
-        ppn = jd.processes_per_host
+    if jd.project:
+        if 'PBSPro_1' in version:
+            # On PBS Pro we set both -P(roject) and -A(accounting),
+            # as we don't know what the admins decided, and just
+            # pray that this doesn't create problems.
+            pbs_params += "#PBS -P %s \n" % str(jd.project)
+            pbs_params += "#PBS -A %s \n" % str(jd.project)
+        else:
+            # Torque
+            pbs_params += "#PBS -A %s \n" % str(jd.project)
+
+    if jd.job_contact:
+        pbs_params += "#PBS -m abe \n"
 
     # if total_cpu_count is not defined, we assume 1
     if not jd.total_cpu_count:
         jd.total_cpu_count = 1
 
     # Request enough nodes to cater for the number of cores requested
     nnodes = jd.total_cpu_count / ppn
     if jd.total_cpu_count % ppn > 0:
         nnodes += 1
 
-    # TODO: Special cases for PBS/TORQUE on Cray
-    if any(v in version for v in ['PBSPro_10', '4.2.7']):       # edison, hopper
-        pbs_params += '#PBS -l mppwidth=%s\n' % jd.total_cpu_count
-    elif any(v in version for v in ['PBSPro_12', 'PBSPro_13']): # archer
-        pbs_params += '#PBS -l select=%d\n' % nnodes
-    elif is_cray:                                               # kraken, jaguar
-        pbs_params += '#PBS -l size=%s\n' % jd.total_cpu_count
-    elif node_properties:
-        pbs_params += '#PBS -l nodes=%d:ppn=%d%s\n' % (
-            nnodes, ppn, ''.join([':%s' % prop for prop in node_properties]))
-    else:
-        pbs_params += '#PBS -l select=%d:ncpus=%d\n' % (nnodes, ppn)
+    # use ncpus value for systems that need to specify ncpus as multiple of PPN
+    ncpus = nnodes * ppn
 
-    # Process Generic Resource specification request
-    if gres:
-        pbs_params += '#PBS -l gres=%s\n' % gres
-
-    for l_option in jd.system_architecture.get('options', []):
-        pbs_params += '#PBS -l %s\n' % l_option
+    # Node properties are appended to the nodes argument in the resource_list.
+    node_properties = []
 
-    if is_cray:
-        # qsub on Cray systems complains about the -V option:
-        # Warning:
-        # Your job uses the -V option, which requests that all of your
-        # current shell environment settings (9913 bytes) be exported to
-        # it.  This is not recommended, as it causes problems for the
-        # batch environment in some cases.
-        pbs_params += "#PBS -V \n"
+    # Parse candidate_hosts
+    #
+    # Currently only implemented for "bigflash" on Gordon@SDSC
+    # https://github.com/radical-cybertools/radical.saga/issues/406
+    #
+    if jd.candidate_hosts:
+        if 'BIG_FLASH' in jd.candidate_hosts:
+            node_properties.append('bigflash')
+        elif len(jd.candidate_hosts) == 1:
+            queue_spec += '@%s' % jd.candidate_hosts[0]
+        else:
+            raise rse.NotImplemented("unsupported candidate_hosts [%s]"
+                                      % jd.candidate_hosts)
 
-    if jd.environment:
-        pbs_params += '#PBS -v %s\n' % \
-            ','.join(['"%s=%s"' % (k, v) for k, v in jd.environment.items()])
+    if 'cheyenne'  in url.host.lower() or \
+       'cheyenne'  in os.uname()[1].lower():
+        is_cheyenne = True
+    else:
+        is_cheyenne = False
 
-    exec_script = '\nexport SAGA_PPN=%d\n' % ppn
-    if jd.working_directory:
-        # older PBS installations might not accept this option
-        # if jd.working_directory:
-        #     pbs_params += '#PBS -d %s \n' % jd.working_directory
-        # (*) a workaround is to do an explicit 'cd'
-        exec_script += 'export PBS_O_WORKDIR=%s \n' % jd.working_directory
-        exec_script += 'mkdir -p %s\n' % jd.working_directory
-        exec_script += 'cd       %s\n' % jd.working_directory
+    # TODO: Special cases for PBS/TORQUE on Cray. Different PBSes,
+    #       different flags. A complete nightmare...
+    #       The more we add, the more it screams for a refactoring
+    if   is_cheyenne                     : pbs_params += "#PBS -l select=%d:ncpus=%d\n" % (nnodes, 36)           # cheyenne, ppn=36
+    elif 'PBSPro_10'       in version: pbs_params += "#PBS -l mppwidth=%s \n"       % jd.total_cpu_count     # hopper
+    elif 'PBSPro_12'       in version: pbs_params += "#PBS -l select=%d\n"          % nnodes                 # pbspro 12, archer
+    elif 'PBSPro_13'       in version: pbs_params += "#PBS -l select=%d\n"          % nnodes                 # pbspro 13
+    elif '4.2.6'           in version: pbs_params += "#PBS -l nodes=%d\n"           % nnodes                 # titan
+    elif '4.2.7'           in version: pbs_params += "#PBS -l mppwidth=%s \n"       % jd.total_cpu_count     # edison, hopper
+    elif 'Version: 5.'     in version: pbs_params += "#PBS -l procs=%d\n"           % jd.total_cpu_count     # torqye 5
+    elif 'version: 2.3.13' in version: pbs_params += "#PBS -l ncpus=%d\n"           % ncpus                  # blacklight
+    elif '14.2'            in version: pbs_params += "#PBS -l select=%d:ncpus=%d\n" % (nnodes, ppn)          # pbspro 14
+    elif is_cray                     : pbs_params += "#PBS -l size=%s\n"            % jd.total_cpu_count     # kraken, jaguar
+    else                             : pbs_params += "#PBS -l nodes=%d:ppn=%d%s\n"  % (nnodes, ppn,          # default
+                                       ''.join([':%s' % prop for prop in node_properties]))
 
-    if jd.executable:
-        exec_script += '\n%s ' % jd.executable
-    if jd.arguments:
-        exec_script += ' '.join(jd.arguments)
+    # Process Generic Resource specification request
+    if gres:
+        pbs_params += "#PBS -l gres=%s\n" % gres
 
-    # escape all double quotes and dollar signs, otherwise 'echo |' further
-    # down won't work only escape '$' in args and exec, not in the params
-    exec_script = exec_script.replace('$', '\\$')
+    # escape all double quotes and dollarsigns, otherwise 'echo |'
+    # further down won't work
+    # only escape '$' in args and exe. not in the params
+    exec_n_args = workdir_directives + exec_n_args
+    exec_n_args = exec_n_args.replace('$', '\\$')
 
-    pbscript = '\n#!/bin/bash\n\n%s%s\n' % (pbs_params, exec_script)
+    pbscript = "\n#!/bin/bash \n%s%s" % (pbs_params, exec_n_args)
 
     pbscript = pbscript.replace('"', '\\"')
     return pbscript
 
 
 # --------------------------------------------------------------------
 # some private defs
@@ -327,18 +383,15 @@
                           api.QUEUE,
                           api.PROJECT,
                           api.WALL_TIME_LIMIT,
                           api.WORKING_DIRECTORY,
                           api.WALL_TIME_LIMIT,
                           api.SPMD_VARIATION,
                           api.PROCESSES_PER_HOST,
-                          api.TOTAL_CPU_COUNT,
-                          api.TOTAL_GPU_COUNT,
-                          api.SYSTEM_ARCHITECTURE,
-                          api.JOB_CONTACT],
+                          api.TOTAL_CPU_COUNT],
     "job_attributes":    [api.EXIT_CODE,
                           api.EXECUTION_HOSTS,
                           api.CREATED,
                           api.STARTED,
                           api.FINISHED],
     "metrics":           [api.STATE],
     "callbacks":         [api.STATE],
@@ -740,24 +793,25 @@
                 'start_time':   None,
                 'end_time':     None,
                 'gone':         False
             }
 
         rm, pid = self._adaptor.parse_id(job_id)
 
-        # run the PBS 'qstat' command to get job's info
-        # options: "-f" - long format; "-x" - includes finished jobs
+        # run the PBS 'qstat' command to get some infos about our job
+        # TODO: create a PBSPRO/TORQUE flag once
         pbs_version = self._commands['qstat']['version']
-        if 'PBSPro_1' in pbs_version: qstat_flags = '-f'
-        else                        : qstat_flags = '-fx'
+        if   '18.2'     in pbs_version: qstat_flag = '-fx'  # Cheyenne
+        elif 'PBSPro_1' in pbs_version: qstat_flag = '-f'
+        else                          : qstat_flag = '-f1'
 
         ret, out, _ = self.shell.run_sync("unset GREP_OPTIONS; %s %s %s | "
                 "grep -E -i '(job_state)|(Job_Name)|(exec_host)|(exit_status)|"
                  "(ctime)|(start_time)|(stime)|(mtime)'"
-                % (self._commands['qstat']['path'], qstat_flags, pid))
+                % (self._commands['qstat']['path'], qstat_flag, pid))
 
         if ret:
 
             if reconnect:
                 raise rse.NoSuccess("Couldn't reconnect job %s: %s" % (job_id, out))
 
             if ("Unknown Job Id" in out):
@@ -828,29 +882,38 @@
                   #        modification time) which is generally also end time.
                   #        TORQUE has an "comp_time" (completion? time), that is
                   #        generally the same as mtime.
                   #
                   #        For now we use mtime for both TORQUE and PBS Pro.
 
             # split exec hosts list if set
-            if job_info.get('exec_host'):
+            if job_info['exec_host']:
                 job_info['exec_hosts'] = job_info['exec_hosts'].split('+')
 
+            # TORQUE doesn't allow us to distinguish DONE/FAILED on final state
+            # alone, we need to consider the exit_status.
             retcode = job_info.get('returncode', -1)
             job_info['state'] = _to_saga_jobstate(job_state, retcode)
 
             # FIXME: workaround for time zone problem described above
             if job_info['state'] in [api.RUNNING] + api.FINAL \
                 and not job_info['start_time']:
                 job_info['start_time'] = time.time()
 
             if job_info['state'] in api.FINAL \
                 and not job_info['end_time']:
                 job_info['end_time'] = time.time()
 
+
+        # PBSPRO state does not indicate error or success -- we derive that from
+        # the exit code
+        if job_info['returncode'] not in [None, 0]:
+            job_info['state'] = api.FAILED
+
+
         # return the updated job info
         return job_info
 
 
     # ----------------------------------------------------------------
     #
     def _job_get_state(self, job_id):
@@ -897,27 +960,23 @@
         return self.jobs[job_id]['end_time']
 
     # ----------------------------------------------------------------
     #
     def _job_cancel(self, job_id):
         """ cancel the job via 'qdel'
         """
-        if self.jobs[job_id]['state'] in api.FINAL:
-            # job is already final - nothing to do
-            return
-
         rm, pid = self._adaptor.parse_id(job_id)
 
         ret, out, _ = self.shell.run_sync("%s %s\n"
                     % (self._commands['qdel']['path'], pid))
 
         if ret:
             raise rse.NoSuccess("Error canceling job via 'qdel': %s" % out)
 
-        # assume the job was successfully canceled
+        # assume the job was succesfully canceled
         self.jobs[job_id]['state'] = api.CANCELED
 
         if not self.jobs[job_id]['end_time']:
             self.jobs[job_id]['end_time'] = time.time()
 
 
     # ----------------------------------------------------------------
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/redis/redis_1.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_1.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/redis/redis_2.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_2.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/redis/redis_advert.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_advert.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/redis/redis_cache.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_cache.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/redis/redis_namespace.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_namespace.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/sge/sgejob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/sge/sgejob.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,16 +213,15 @@
         a_base.Base.__init__(self, _ADAPTOR_INFO)
 
         self.id_re = re.compile('^\[(.*)\]-\[(.*?)\]$')
         self.epoch = datetime(1970,1,1)
 
         self.purge_on_start   = self._cfg['purge_on_start']
         self.purge_older_than = self._cfg['purge_older_than']
-
-        self.base_workdir = ru.get_radical_base('saga') + 'adaptors/sge'
+        self.base_workdir     = self._cfg['base_workdir']
 
 
     # ----------------------------------------------------------------
     #
     def sanity_check(self):
         # FIXME: also check for gsissh
         pass
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/shell/shell_file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_file.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/shell/shell_job.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,44 +152,41 @@
 
 
 # ------------------------------------------------------------------------------
 # the adaptor capabilities & supported attributes
 #
 _ADAPTOR_CAPABILITIES  = {
     "jdes_attributes" : [api.NAME,
-                         api.EXECUTABLE,
-                         api.PRE_EXEC,
-                         api.POST_EXEC,
-                         api.ARGUMENTS,
-                         api.ENVIRONMENT,
-                         api.WORKING_DIRECTORY,
-                         api.FILE_TRANSFER,
-                         api.INPUT,
-                         api.OUTPUT,
-                         api.ERROR,
-                         api.NAME,
-                         api.WALL_TIME_LIMIT,
-                         api.TOTAL_CPU_COUNT,
-                         api.TOTAL_GPU_COUNT,
-                         api.PROCESSES_PER_HOST,
-                         api.SPMD_VARIATION,
-                         api.QUEUE,
-                         api.PROJECT,
-                         api.SYSTEM_ARCHITECTURE,
-                        ],
+                          api.EXECUTABLE,
+                          api.PRE_EXEC,
+                          api.POST_EXEC,
+                          api.ARGUMENTS,
+                          api.ENVIRONMENT,
+                          api.WORKING_DIRECTORY,
+                          api.FILE_TRANSFER,
+                          api.INPUT,
+                          api.OUTPUT,
+                          api.ERROR,
+                          api.NAME,
+                          api.WALL_TIME_LIMIT,
+                          api.TOTAL_CPU_COUNT,
+                          api.TOTAL_GPU_COUNT,
+                          api.PROCESSES_PER_HOST,
+                          api.SPMD_VARIATION,
+                         ],
     "job_attributes"  : [api.EXIT_CODE,
-                         api.EXECUTION_HOSTS,
-                         api.CREATED,
-                         api.STARTED,
-                         api.FINISHED],
+                          api.EXECUTION_HOSTS,
+                          api.CREATED,
+                          api.STARTED,
+                          api.FINISHED],
     "metrics"         : [api.STATE,
-                         api.STATE_DETAIL],
+                          api.STATE_DETAIL],
     "contexts"        : {"ssh"     : "public/private keypair",
-                         "x509"    : "X509 proxy for gsissh",
-                         "userpass": "username/password pair for ssh"}
+                          "x509"    : "X509 proxy for gsissh",
+                          "userpass": "username/password pair for ssh"}
 }
 
 # ------------------------------------------------------------------------------
 # the adaptor documentation
 #
 _ADAPTOR_DOC           = {
     "name"            : _ADAPTOR_NAME,
@@ -262,15 +259,15 @@
                          /bin/sh: fork: retry: Resource temporarily unavailable
               NoSuccess: failed to run job \
                          backend error
 
           * number of files are limited, as is disk space: the job.service will
 
             keep job state on the remote disk, in
-            `$RADICAL_BASE/.radical/saga/adaptors/shell_job/`.
+            ``~/.radical/saga/adaptors/shell_job/``.
             Quota limitations may limit the number of files created there,
             and/or the total size of that directory.
 
             On quota or disk space limits, you may see error messages similar to
             the following ones::
 
               NoSuccess: read from pty process failed ([Errno 5] Quota exceeded)
@@ -556,30 +553,31 @@
                 env[key] = val
 
         cfg = self._adaptor._cfg
 
         # expand those config entries we want to use(where needed)
         self.notifications  = cfg.enable_notifications
         self.purge_on_start = cfg.purge_on_star
+        self.base_workdir   = ru.expand_env(cfg.base_workdir, env)
 
-        self.base_workdir   = ru.get_radical_base('saga') + 'adaptors/shell_job'
 
         # start the shell, find its prompt.  If that is up and running, we can
         # bootstrap our wrapper script, and then run jobs etc.
 
         # -- now stage the shell wrapper script, and run it.  Once that is up
         # and running, we can requests job start / management operations via its
         # stdio.
 
         base = self.base_workdir
+
         with self._shell_lock:
-            ret, out, _ = self.shell.run_sync(' mkdir -p %s' % base)
+            ret, out, _ = self.shell.run_sync(" mkdir -p %s" % base)
 
         if ret != 0:
-            raise rse.NoSuccess('host setup failed (%s):(%s)' % (ret, out))
+            raise rse.NoSuccess("host setup failed(%s):(%s)" % (ret, out))
 
         # TODO: replace some constants in the script with values from config
         # files, such as 'timeout' or 'purge_on_quit' ...
         tgt = "%s/wrapper.sh" % base
 
         # lets check if we actually need to stage the wrapper script.  We need
         # an adaptor lock on this one.
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/shell/shell_resource.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_resource.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/shell/shell_wrapper.sh` & `radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_wrapper.sh`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 # this script uses only POSIX shell functionality, and does not rely on bash or
 # other shell extensions.  It expects /bin/sh to be a POSIX compliant shell
 # thought.
 #
 # The invocation passes one (optional) parameter, the base workdir.  That
 # directory will be used to keep job state data. Its default value is set to
-# $RADICAL_BASE/.radical/saga/adaptors/shell_job/ (defaults to $HOME)
-test -z "$RADICAL_BASE" && export RADICAL_BASE="$HOME"
+# $HOME/.radical/saga/adaptors/shell_job/
+
 
 # --------------------------------------------------------------------
 # on argument quoting
 #
 #   method "a b c" 'd e' f g
 #   method() {
 #     echo $*     # 'a' 'b' 'c' 'd' 'e' 'f' 'g'
@@ -65,15 +65,15 @@
 GID="$$"
 export GID
 
 # this is where this 'daemon' keeps state for all started jobs
 BASE="$1"; shift
 if test -z "$BASE"
 then
-  BASE=$RADICAL_BASE/.radical/saga/adaptors/shell_job/
+  BASE=$HOME/.radical/saga/adaptors/shell_job/
 fi
 NOTIFICATIONS="$BASE/notifications"
 LOG="$BASE/log"
 
 # this process will terminate when idle for longer than TIMEOUT seconds
 TIMEOUT=300
 
@@ -97,20 +97,14 @@
 \trap idle_handler ALRM
 #\trap '' ALRM
 
 \trap cleanup_handler_sighup  HUP
 \trap cleanup_handler_sigint  INT
 \trap cleanup_handler_sigterm TERM
 
-usleep(){
-  # slip for a minute amount of time
-  head -c $((1024 * 1024)) /dev/urandom > /dev/null 2>&1
-# head -c 1 /dev/random > /dev/null 2>&1
-}
-
 cleanup_handler_quit (){
   \printf "trapped QUIT\n"
   cmd_quit $IDLE
 }
 
 cleanup_handler_term (){
   \printf "trapped TERM\n"
@@ -717,29 +711,27 @@
   DIR="$BASE/$1"
 
   rpid=`\cat "$DIR/rpid"`
   mpid=`\cat "$DIR/mpid"`
 
   # first kill monitor, so that it does not interfer with state management
   /bin/kill -TERM $mpid 2>/dev/null
-  usleep
   /bin/kill -KILL $mpid 2>/dev/null
 
   # now make sure that job did not reach final state before monitor died
   state=`\grep -e ' $' "$DIR/state" | \tail -n 1 | \tr -d ' '`
   if test "$state" = "FAILED" -o "$state" = "DONE" -o "$state" = "CANCELED"
   then
     ERROR="state: $state\n job $1 is in final state"
     RETVAL="$1 $state"
     return
   fi
 
   # now kill the job process group, and to be sure also the job shell
   /bin/kill -TERM $KILL_DASHES -$rpid 2>/dev/null
-  usleep
   /bin/kill -KILL $KILL_DASHES -$rpid 2>/dev/null
 
   # FIXME: how can we check for success?  ps?
   \printf "CANCELED \n" >> "$DIR/state"
   RETVAL="$1 CANCELED"
 }
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/slurm/slurm_job.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/slurm/slurm_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,53 +8,33 @@
 SLURM job adaptor implementation
 '''
 
 import re
 import os
 import math
 import time
-import threading
 import datetime
 import tempfile
 
 import radical.utils as ru
 
 from ...job           import constants   as c
 from ...utils         import pty_shell   as rsups
 from ...              import job         as api_job
 from ...              import exceptions  as rse
+from ...              import filesystem  as sfs
 from ..               import base        as a_base
 from ..cpi            import job         as cpi_job
 from ..cpi            import decorators  as cpi_decs
 
 from ...utils.job     import TransferDirectives
 
 SYNC_CALL  = cpi_decs.SYNC_CALL
 ASYNC_CALL = cpi_decs.ASYNC_CALL
 
-MONITOR_UPDATE_INTERVAL = 3  # seconds
-
-SMT_DEFAULT = 1
-
-PPN_PER_QUEUE = {
-    'bridges2': {
-        'rm'    : 128,
-        'rm-512': 128,
-        'em'    : 96
-    },
-    'rivanna': {
-        'standard': 40,
-        'parallel': 40,
-        'bii'     : 40,
-        'largemem': 16,
-        'gpu'     : 10,
-        'dev'     : 4
-    }
-}
-
 
 # ------------------------------------------------------------------------------
 # some private defs
 #
 _PTY_TIMEOUT = 2.0
 
 # ------------------------------------------------------------------------------
@@ -220,90 +200,14 @@
             "type"     : "radical.saga.job.Job",
             "class"    : "SLURMJob"
         }
     ]
 }
 
 
-# ------------------------------------------------------------------------------
-#
-class _job_state_monitor(threading.Thread):
-    """
-    thread that periodically monitors job states
-    """
-
-    # --------------------------------------------------------------------------
-    #
-    def __init__(self, job_service):
-
-        self.logger = job_service._logger
-        self.js     = job_service
-        self._term  = threading.Event()
-
-        super(_job_state_monitor, self).__init__()
-        self.setDaemon(True)
-
-
-    # --------------------------------------------------------------------------
-    #
-    def stop(self):
-
-        self.logger.info('stop  thread for %s', self.js.get_url())
-        self._term.set()
-
-
-    # --------------------------------------------------------------------------
-    #
-    def run(self):
-
-        self.logger.info('start thread for %s', self.js.get_url())
-        while not self._term.is_set():
-
-            try:
-                # do bulk updates here! we don't want to pull information
-                # job by job. that would be too inefficient!
-                jobs = self.js.jobs
-                for job_id in jobs:
-
-                    job_info = jobs[job_id]
-                    # we only need to monitor jobs that are not in a
-                    # terminal state, so we can skip the ones that are
-                    # either done, failed or canceled
-                    old_state = job_info['old_state']
-                    if old_state in api_job.FINAL:
-                        continue
-
-                    # job is not final and we got new info - replace job info
-                    new_info = self.js._job_get_info(job_id)
-                    self.js.jobs[job_id] = new_info
-
-                    # we only care to state updates though when the state
-                    # actually changed from last time
-                    new_state = new_info['state']
-                    if new_state == old_state:
-                        continue
-
-                    # fire job state callback if 'state' has changed
-                    self.logger.info("update Job %s (state: %s)"
-                                    % (job_id, new_state))
-                    new_info['old_state'] = new_state
-                    job_obj = new_info['job_obj']
-                    if job_obj:
-                        job_obj._api()._attributes_i_set('state', new_state,
-                                                       job_obj._api()._UP, True)
-
-                time.sleep(MONITOR_UPDATE_INTERVAL)
-
-            except Exception:
-                self.logger.exception("job_id monitoring thread failed")
-                raise
-
-        self.logger.info('close thread for %s', self.js.get_url())
-
-
 ################################################################################
 #
 # The adaptor class
 #
 class Adaptor(a_base.Base):
     '''
     This is the actual adaptor class, which gets loaded by SAGA (i.e. by the
@@ -387,19 +291,16 @@
     def init_instance(self, adaptor_state, rm_url, session):
         '''
         Service instance constructor
         '''
 
         self.rm      = rm_url
         self.session = session
-        self.jobs    = dict()
-
-        self.mt = _job_state_monitor(job_service=self)
-        self.mt.start()
 
+        self.jobs = {}
         self._open()
 
         return self.get_api()
 
 
     # --------------------------------------------------------------------------
     #
@@ -458,15 +359,15 @@
                 message = "Error finding SLURM tool %s on remote server %s!\n" \
                           "Locations searched:\n%s\n" \
                           "Is SLURM installed on that machine? " \
                           "If so, is your remote SLURM environment "\
                           "configured properly? " % (cmd, self.rm, out)
                 raise rse.NoSuccess._log(self._logger, message)
 
-            self._logger.debug("got cmd prompt (%s)(%s)", ret, out)
+        self._logger.debug("got cmd prompt (%s)(%s)" % (ret, out))
 
         self.rm.detected_username = self.rm.username
         # figure out username if it wasn't made explicit
         # important if .ssh/config info read+connected with
         # a different username than what we expect
         if not self.rm.username:
             self._logger.debug("No username provided in URL %s, so we are"
@@ -569,67 +470,46 @@
                     self._logger.info("Transferring out %s to %s", source, target)
                     self.shell.stage_from_remote(source, target)
 
 
     # --------------------------------------------------------------------------
     #
     #
-    def _job_run(self, job_obj):
+    def _job_run(self, jd):
         '''
         runs a job on the wrapper via pty, and returns the job id
         '''
 
-        jd = job_obj.get_description()
-
         # define a bunch of default args
         exe                 = jd.executable
         pre                 = jd.as_dict().get(c.PRE_EXEC)
         post                = jd.as_dict().get(c.POST_EXEC)
         args                = jd.as_dict().get(c.ARGUMENTS, [])
         env                 = jd.as_dict().get(c.ENVIRONMENT, dict())
         cwd                 = jd.as_dict().get(c.WORKING_DIRECTORY)
         job_name            = jd.as_dict().get(c.NAME)
         spmd_variation      = jd.as_dict().get(c.SPMD_VARIATION)
         cpu_count           = jd.as_dict().get(c.TOTAL_CPU_COUNT)
         gpu_count           = jd.as_dict().get(c.TOTAL_GPU_COUNT)
         n_procs             = jd.as_dict().get(c.NUMBER_OF_PROCESSES)
-        procs_per_host      = jd.as_dict().get(c.PROCESSES_PER_HOST)
+        processes_per_host  = jd.as_dict().get(c.PROCESSES_PER_HOST)
         output              = jd.as_dict().get(c.OUTPUT, "radical.saga.stdout")
         error               = jd.as_dict().get(c.ERROR,  "radical.saga.stderr")
         file_transfer       = jd.as_dict().get(c.FILE_TRANSFER)
         wall_time           = jd.as_dict().get(c.WALL_TIME_LIMIT)
         queue               = jd.as_dict().get(c.QUEUE)
         project             = jd.as_dict().get(c.PROJECT)
         total_memory        = jd.as_dict().get(c.TOTAL_PHYSICAL_MEMORY)
         sys_arch            = jd.as_dict().get(c.SYSTEM_ARCHITECTURE)
         job_contact         = jd.as_dict().get(c.JOB_CONTACT)
         c_hosts             = jd.as_dict().get(c.CANDIDATE_HOSTS)
 
         cpu_arch            = sys_arch.get('cpu')
         gpu_arch            = sys_arch.get('gpu')
 
-        # default: only nodes with all of specified features will be used
-        constraints = []
-        for opt in sys_arch.get('options', []):
-            constraints.append(opt.lower())
-
-        threads_per_core = None
-        # check that target machine requires SMT to be set
-        if 'smt' in sys_arch:
-            threads_per_core = int(env.get('RADICAL_SMT') or
-                                   sys_arch.get('smt') or
-                                   SMT_DEFAULT)
-
-        core_spec = None
-        if 'blocked_cores' in sys_arch:
-            core_spec = len(sys_arch['blocked_cores']) // \
-                        (threads_per_core or 1)
-
-        is_exclusive = sys_arch.get('exclusive', False)
-
         # check to see what's available in our job description
         # to override defaults
 
         # try to create the working directory (if defined)
         # NOTE: this assumes a shared filesystem between login node and
         #       compute nodes.
         if cwd:
@@ -649,48 +529,38 @@
             job_contact = job_contact[0]
 
         if project and ':' in project:
             account, reservation = project.split(':', 1)
         else:
             account, reservation = project, None
 
-        if queue and ':' in queue:
-            partition, qos = queue.split(':', 1)
-        else:
-            if 'perlmutter' in self.rm.host.lower():
-                partition, qos = None, queue
-            else:
-                partition, qos = queue, None
-
         script = "#!/bin/sh\n\n"
 
         # make sure we have something for cpu_count
         if not cpu_count:
             cpu_count = 1
 
         # make sure we have something for n_procs
         if not n_procs:
             n_procs = cpu_count
 
-        # get mem_per_node from total_memory and make sure it is not None
-        mem_per_node = total_memory or 0
+        # get memory_per_node from total_memory and make sure it is not None
+        memory_per_node = total_memory or 0
 
-        resource = self.rm.host.split('.', 1)[0].lower()
-        # check user provided value first, then check discovered value
-        procs_per_host = procs_per_host or \
-                         PPN_PER_QUEUE.get(resource, {}).\
-                                       get(partition.lower()) or \
-                         self._ppn
-
-        # define n_nodes and recalculate mem_per_node
+        # define n_nodes and recalculate memory_per_node (if self._ppn is set)
         n_nodes = None
-        if procs_per_host:
+        if self._ppn:
+
+            # exception(s) for earlier defined `self._ppn`
+            if 'frontera' in self.rm.host.lower() and \
+                    queue and 'rtx' in queue.lower():
+                self._ppn = 16  # other option is to use: processes_per_host
 
-            n_nodes      = int(math.ceil(float(cpu_count) / procs_per_host))
-            mem_per_node = int(mem_per_node / float(n_nodes))
+            n_nodes = int(math.ceil(float(cpu_count) / self._ppn))
+            memory_per_node = int(memory_per_node / float(n_nodes))
 
         elif total_memory:
             raise rse.NotImplemented(
                 'cannot allocate memory, node number unknown')
 
         if spmd_variation:
             if spmd_variation.lower() not in 'mpi':
@@ -699,70 +569,50 @@
             mpi_cmd = 'mpirun -n %d ' % n_procs
 
         else:
             # we start N independent processes
             mpi_cmd = ''
 
             if  'stampede2' in self.rm.host.lower() or \
-                'longhorn'  in self.rm.host.lower() or \
-                'expanse'   in self.rm.host.lower() or \
-                'traverse'  in self.rm.host.lower():
+                'longhorn'  in self.rm.host.lower():
 
                 assert(n_nodes), 'need unique number of cores per node'
                 script += "#SBATCH -N %d\n" % n_nodes
                 script += "#SBATCH -n %s\n" % n_procs
 
-            elif 'frontera'   in self.rm.host.lower() or \
-                 'andes'      in self.rm.host.lower() or \
-                 'spock'      in self.rm.host.lower() or \
-                 'crusher'    in self.rm.host.lower() or \
-                 'frontier'   in self.rm.host.lower() or \
-                 'perlmutter' in self.rm.host.lower() or \
-                 'rivanna'    in self.rm.host.lower():
+            elif 'frontera'  in self.rm.host.lower() or \
+                 'andes'      in self.rm.host.lower():
 
                 assert(n_nodes), 'need unique number of cores per node'
                 script += "#SBATCH -N %d\n" % n_nodes
 
             elif self._version in ['17.11.5', '18.08.0', '18.08.3']:
 
                 assert(n_nodes), 'need unique number of cores per node'
                 script += "#SBATCH -N %d\n" % n_nodes
                 script += "#SBATCH --ntasks=%s\n" % n_procs
 
             else:
                 script += "#SBATCH --ntasks=%s\n" % n_procs
 
-            if 'traverse' in self.rm.host.lower():
-                # NOTE: this hardcodes the job for a specific application layout
-                script += '#SBATCH --cpus-per-task=4\n'
-                script += '#SBATCH --ntasks-per-core=1\n'
-
-            elif not procs_per_host or procs_per_host == 1:
-                # batch nodes (ppn=1) are not considered for `ntasks-per-node`
-                script += '#SBATCH --cpus-per-task=%s\n' \
+            if not processes_per_host:
+                script += "#SBATCH --cpus-per-task=%s\n" \
                         % (int(cpu_count / n_procs))
 
-            elif not threads_per_core:
-                # https://slurm.schedmd.com/sbatch.html#OPT_threads-per-core
-                # "threads" refers to the number of processing units on each
-                # core rather than the number of application tasks to be
-                # launched per core.
-                #
-                # Options `--threads-per-core` and `--ntasks-per-node` are
-                # treated as mutually exclusive.
-                script += '#SBATCH --ntasks-per-node=%s\n' % procs_per_host
+            else:
+                script += "#SBATCH --ntasks-per-node=%s\n" % processes_per_host
 
-        # target host specification
+        # target host specifica
         # FIXME: these should be moved into resource config files
         self._logger.debug ("submit SLURM script to %s", self.rm)
         if 'bridges2' in self.rm.host.lower():
-            if gpu_count:
-                # gres resources are specified *per node*
-                assert(n_nodes), 'need unique number of cores per node'
-                script += "#SBATCH --gres=gpu:%s:8\n" % (gpu_arch)
+             if gpu_count:
+                 # gres resources are specified *per node*
+                 assert(n_nodes), 'need unique number of cores per node'
+                 script += "#SBATCH --gres=gpu:%s:8\n" % (gpu_arch)
 
         elif 'comet' in self.rm.host.lower():
 
             if gpu_count:
                 # gres resources are specified *per node*
                 assert(n_nodes), 'need unique number of cores per node'
 
@@ -770,90 +620,65 @@
                 # gpu types are "p100" and "k80"
                 if gpu_arch: gpu_arch_str = ':%s' % gpu_arch.lower()
                 else       : gpu_arch_str = ''
                 count = 4
                 # Make sure we take a full GPU node
                 script += "#SBATCH --gres=gpu%s:%d\n" % (gpu_arch_str, count)
 
-        elif 'tiger'  in self.rm.host.lower() or \
-             'amarel' in self.rm.host.lower():
+        elif 'tiger' in self.rm.host.lower():
 
             if gpu_count:
                 # gres resources are specified *per node*
                 assert(n_nodes), 'need unique number of cores per node'
-                count = math.ceil(gpu_count / n_nodes)
+                count = int(gpu_count / n_nodes)
 
                 if count:
                     script += "#SBATCH --gres=gpu:%s\n" % count
 
         elif 'cori' in self.rm.host.lower():
 
             # Set to "haswell" for Haswell nodes, to "knl,quad,cache" (or other
             # modes) for KNL, etc.
-            if cpu_arch : constraints.append(cpu_arch)
+            if cpu_arch : script += "#SBATCH -C %s\n"     % cpu_arch
             if gpu_count: script += "#SBATCH --gpus=%s\n" % gpu_count
 
         elif 'longhorn' in self.rm.host.lower():
             self._logger.debug("SLURM GRES is not set (longhorn exception)\n")
 
-        elif 'traverse' in self.rm.host.lower():
-            if gpu_count:
-                script += "#SBATCH --gpus-per-task=1\n"
-                script += "#SBATCH --gres=gpu:4\n"
+        elif queue == 'tmp3':
+
+            # this is a special queue, which is associated with SuperMUC-NG,
+            # but since there is no machine name in config data we only track
+            # this queue name to set SLURM QoS option
+            script += "#SBATCH --qos=nolimit\n"
+            self._logger.debug("SLURM QoS is set (SuperMUC-NG only)\n")
 
         else:
 
-            if gpu_count and not threads_per_core:
-                # https://slurm.schedmd.com/sbatch.html#OPT_threads-per-core
-                # "threads" refers to the number of processing units on each
-                # core rather than the number of application tasks to be
-                # launched per core.
-                #
-                # Options `--threads-per-core` and `--gpus` are treated
-                # as mutually exclusive.
-                script += '#SBATCH --gpus=%s\n' % gpu_count
-
-        if job_name    : script += '#SBATCH -J "%s"\n'            % job_name
-        if cwd         : script += '#SBATCH -D "%s"\n'            % cwd
-        if output      : script += '#SBATCH --output "%s"\n'      % output
-        if error       : script += '#SBATCH --error "%s"\n'       % error
-        if job_contact : script += '#SBATCH --mail-user="%s"\n'   % job_contact
-        if account     : script += '#SBATCH --account "%s"\n'     % account
-        if partition   : script += '#SBATCH --partition "%s"\n'   % partition
-        if qos         : script += '#SBATCH --qos "%s"\n'         % qos
-        if reservation : script += '#SBATCH --reservation "%s"\n' % reservation
-        if c_hosts     : script += '#SBATCH --nodelist="%s"\n'    % c_hosts
-        if constraints : script += '#SBATCH --constraint "%s"\n'  % \
-                                   '&'.join(constraints)
-        if wall_time   : script += '#SBATCH --time %02d:%02d:00\n'  \
-                                 % (int(wall_time / 60), wall_time % 60)
-
-        if is_exclusive: script += '#SBATCH --exclusive\n'
-        if mem_per_node: script += '#SBATCH --mem=%d\n'           % mem_per_node
-
-        if core_spec is not None:
-            # Core specialization is a feature designed to isolate system
-            # overhead (system interrupts, etc.) to designated cores
-            # on compute nodes. The count identifies the number of cores to be
-            # reserved for system overhead on each allocated compute node.
-            script += '#SBATCH --core-spec=%d\n' % core_spec
-
-        if threads_per_core:
-            # High-level (automatic mask generation): minimum number of threads
-            # in a core to dedicate to a job. In task layout, use the specified
-            # maximum number of threads per core.
-            #
-            # This option may implicitly set the number of tasks (if -n was
-            # not specified) as one task per requested thread.
-            script += '#SBATCH --threads-per-core=%d\n' % threads_per_core
+            if gpu_count:
+                script += "#SBATCH --gpus=%s\n" % gpu_count
+
+
+        if job_name       : script += '#SBATCH -J "%s"\n'            % job_name
+        if cwd            : script += '#SBATCH -D "%s"\n'            % cwd
+        if output         : script += '#SBATCH --output "%s"\n'      % output
+        if error          : script += '#SBATCH --error "%s"\n'       % error
+        if queue          : script += '#SBATCH --partition "%s"\n'   % queue
+        if c_hosts        : script += '#SBATCH --nodelist="%s"\n'    % c_hosts
+        if job_contact    : script += '#SBATCH --mail-user="%s"\n'   % job_contact
+        if account        : script += '#SBATCH --account "%s"\n'     % account
+        if reservation    : script += '#SBATCH --reservation "%s"\n' % reservation
+        if memory_per_node: script += '#SBATCH --mem="%s"\n'         % memory_per_node
+        if wall_time      : script += '#SBATCH --time %02d:%02d:00\n' \
+                                         % (int(wall_time / 60), wall_time % 60)
 
         if env:
             script += "\n## ENVIRONMENT\n"
-            for key, val in env.items():
-                script += 'export %s="%s"\n' % (key, val)
+            for key,val in env.items():
+                script += 'export "%s"="%s"\n'  %  (key, val)
 
         if pre:
             script += "\n## PRE_EXEC\n" + "\n".join(pre)
             script += '\n'
 
         # create our commandline
         script += "\n## EXEC\n"
@@ -861,23 +686,23 @@
         script += '\n'
 
         if post:
             script += "\n## POST_EXEC\n" + '\n'.join(post)
             script += '\n'
 
         # write script into a tmp file for staging
+        self._logger.info("SLURM script generated:\n%s" % script)
+
         tgt = os.path.basename(tempfile.mktemp(suffix='.slurm', prefix='tmp_'))
-        if cwd:
-            tgt = os.path.join(cwd, tgt)
         self.shell.write_to_remote(src=script, tgt=tgt)
 
         # submit the job
-        ret, out, _ = self.shell.run_sync('sbatch %s' % tgt)
+        ret, out, _ = self.shell.run_sync("sbatch '%s'; echo rm -f '%s'" % (tgt,tgt))
 
-        self._logger.debug('submit SLURM script (%s) (%s)' % (tgt, ret))
+        self._logger.debug("submit SLURM script (%s) (%s)" % (tgt, ret))
 
         # find out what our job ID is
         # TODO: Could make this more efficient
         job_id = None
         for line in out.split("\n"):
             if "Submitted batch job" in line:
                 job_id = "[%s]-[%s]" % (self.rm, int(line.split()[-1:][0]))
@@ -901,16 +726,14 @@
                              'exec_hosts' : None,
                              'gone'       : False,
                              'output'     : output,
                              'error'      : error,
                              'stdout'     : None,
                              'stderr'     : None,
                              'ft'         : file_transfer,
-                             'job_obj'    : job_obj,
-                             'old_state'  : None,
                              }
         return job_id
 
 
     # --------------------------------------------------------------------------
     #
     # FROM STAMPEDE'S SQUEUE MAN PAGE
@@ -958,259 +781,14 @@
         elif slurmjs in ['S'  , "SUSPENDED"    ]: return c.SUSPENDED
         elif slurmjs in ['TO' , "TIMEOUT"      ]: return c.CANCELED
         else                                    : return c.UNKNOWN
 
 
     # --------------------------------------------------------------------------
     #
-    def _job_get_info(self, job_id):
-        '''
-        use scontrol to grab job info
-        NOT CURRENTLY USED/TESTED, here for later
-        '''
-
-        # prev. info contains the info collect when _job_get_info
-        # was called the last time
-        prev_info = self.jobs.get(job_id)
-
-        # if the 'gone' flag is set, there's no need to query the job
-        # state again. it's gone forever
-        if prev_info:
-            if prev_info.get('gone', False):
-                self._logger.debug("Job is gone.")
-                return prev_info
-
-        # curr. info will contain the new job info collect. it starts off
-        # as a copy of prev_info (don't use deepcopy because there is an API
-        # object in the dict -> recursion)
-        curr_info = dict()
-
-        if prev_info:
-            curr_info['job_id'     ] = prev_info.get('job_id'     )
-            curr_info['job_name'   ] = prev_info.get('job_name'   )
-            curr_info['state'      ] = prev_info.get('state'      )
-            curr_info['create_time'] = prev_info.get('create_time')
-            curr_info['start_time' ] = prev_info.get('start_time' )
-            curr_info['end_time'   ] = prev_info.get('end_time'   )
-            curr_info['comp_time'  ] = prev_info.get('comp_time'  )
-            curr_info['exec_hosts' ] = prev_info.get('exec_hosts' )
-            curr_info['gone'       ] = prev_info.get('gone'       )
-            curr_info['output'     ] = prev_info.get('output'     )
-            curr_info['error'      ] = prev_info.get('error'      )
-            curr_info['stdout'     ] = prev_info.get('stdout'     )
-            curr_info['stderr'     ] = prev_info.get('stderr'     )
-            curr_info['ft'         ] = prev_info.get('ft'         )
-            curr_info['job_obj'    ] = prev_info.get('job_obj'    )
-            curr_info['old_state'  ] = prev_info.get('old_state'  )
-        else:
-            curr_info['job_id'     ] = None
-            curr_info['job_name'   ] = None
-            curr_info['state'      ] = None
-            curr_info['create_time'] = None
-            curr_info['start_time' ] = None
-            curr_info['end_time'   ] = None
-            curr_info['comp_time'  ] = None
-            curr_info['exec_hosts' ] = None
-            curr_info['gone'       ] = None
-            curr_info['output'     ] = None
-            curr_info['error'      ] = None
-            curr_info['stdout'     ] = None
-            curr_info['stderr'     ] = None
-            curr_info['ft'         ] = None
-            curr_info['job_obj'    ] = None
-            curr_info['old_state'  ] = None
-
-        rm, pid = self._adaptor.parse_id(job_id)
-
-        # update current info with scontrol
-        ret, out, _ = self.shell.run_sync('scontrol show job %s' % pid)
-
-        # out is comprised of a set of space-limited words like this:
-        #
-        # ----------------------------------------------------------------------
-        # $ scontrol show job 8101313
-        #    JobId=8101313 JobName=pilot.0000 UserId=tg803521(803521)
-        #    GroupId=G-81625(81625) Priority=1701 Nice=0 Account=TG-MCB090174
-        #    QOS=normal JobState=RUNNING Reason=None Dependency=(null) Requeue=0
-        #    Restarts=0 BatchFlag=1 Reboot=0 ExitCode=0:0 RunTime=00:00:25
-        #    TimeLimit=00:15:00 TimeMin=N/A SubmitTime=2017-01-11T15:47:19
-        #    EligibleTime=2017-01-11T15:47:19 StartTime=2017-01-11T15:47:19
-        #    EndTime=2017-01-11T16:02:19 PreemptTime=None SuspendTime=None
-        #    SecsPreSuspend=0 Partition=development AllocNode:Sid=login3:2886
-        #    ReqNodeList=(null) ExcNodeList=(null) NodeList=c557-[901-904]
-        #    BatchHost=c557-901 NumNodes=4 NumCPUs=64 CPUs/Task=1
-        #    ReqB:S:C:T=0:0:*:* TRES=cpu=64,node=4 Socks/Node=*
-        #    NtasksPerN:B:S:C=0:0:*:* CoreSpec=* MinCPUsNode=1 MinMemoryNode=0
-        #    MinTmpDiskNode=0 Features=(null) Gres=(null) Reservation=(null)
-        #    Shared=0 Contiguous=0 Licenses=(null) Network=(null)
-        #    Command=/home1/01083/tg803521/tmp_egGk1n.slurm
-        #    WorkDir=/work/01083/
-        #    StdIn=/dev/null
-        #    StdOut=/work/01083/bootstrap_1.out
-        #    StdErr=/work/01083/bootstrap_1.err
-        #    Power= SICP=0
-        # ----------------------------------------------------------------------
-        #
-        # so we split on spaces and newlines, and then on '=' to get
-        # key-value-pairs.
-
-        elems = out.split()
-        data  = dict()
-        for elem in sorted(elems):
-
-            parts = elem.split('=', 1)
-
-            if len(parts) == 1:
-                # default if no '=' is found
-                parts.append(None)
-
-            # ignore non-splittable ones
-            key, val = parts
-            if val in ['', '(null)']:
-                val = None
-            self._logger.info('%-20s := %s', key, val)
-            data[key] = val
-
-        if data.get('JobState'):
-            curr_info['state'] = self._slurm_to_saga_state(data['JobState'])
-        else:
-            curr_info['state'] = self._job_get_state(job_id)
-
-        # update exit code
-        if data.get('ExitCode'):
-            curr_info['exit_code'] = data['ExitCode'].split(':')[0]
-        else:
-            curr_info['exit_code'] = self._job_get_state(job_id)
-
-        curr_info['job_name'   ] = data.get('JobName')
-      # curr_info['create_time'] = data.get('SubmitTime')
-      # curr_info['start_time' ] = data.get('StartTime')
-      # curr_info['end_time'   ] = data.get('EndTime')
-        curr_info['comp_time'  ] = data.get('RunTime')
-        curr_info['exec_hosts' ] = data.get('NodeList')
-
-        # Alas, time stamps are not in EPOCH, and do not contain time zone info,
-        # so we set approximate values here
-        now = time.time()
-        if not curr_info['create_time']: curr_info['create_time'] = now
-
-        if curr_info['state'] in [c.RUNNING] + c.FINAL:
-            if not curr_info['start_time' ]: curr_info['start_time' ] = now
-
-        if curr_info['state'] in c.FINAL:
-
-            if not curr_info['end_time' ]: curr_info['end_time' ] = now
-
-            if curr_info['stdout'] is None:
-
-                if curr_info['output'] is None:
-                    curr_info['output'] = data.get('StdOut')
-
-                ret, out, err = self.shell.run_sync(
-                                                 'cat %s' % curr_info['output'])
-                if ret: curr_info['stdout'] = None
-                else  : curr_info['stdout'] = out
-
-            if curr_info['stderr'] is None:
-
-                if curr_info['error'] is None:
-                    curr_info['error'] = data.get('StdErr')
-
-                ret, out, err = self.shell.run_sync(
-                                                  'cat %s' % curr_info['error'])
-                if ret: curr_info['stderr'] = None
-                else  : curr_info['stderr'] = out
-
-            self._handle_file_transfers(curr_info['ft'], mode='out')
-
-            curr_info['gone'] = True
-
-        self.jobs[job_id] = curr_info
-
-        return curr_info
-
-
-    # --------------------------------------------------------------------------
-    #
-    def _job_get_state(self, job_id):
-        '''
-        get the job state from the wrapper shell
-        '''
-
-      # # if the state is NEW and we haven't sent out a run command, keep
-      # # it listed as NEW
-      # if self._state == c.NEW and not self._started:
-      #     return c.NEW
-
-      # # if the state is DONE, CANCELED or FAILED, it is considered
-      # # final and we don't need to query the backend again
-      # if self._state in c.FINAL:
-      #     return self._state
-
-        rm, pid = self._adaptor.parse_id(job_id)
-
-        try:
-            ret, out, _ = self.shell.run_sync('scontrol show job %s' % pid)
-            match       = self.scontrol_jobstate_re.search(str(out))
-
-            if match:
-                slurm_state = match.group(1)
-            else:
-                # no jobstate found from scontrol
-                # the job may have finished a while back, use sacct to
-                # look at the full slurm history
-                slurm_state = self._sacct_jobstate_match(pid)
-                if not slurm_state:
-                    # no jobstate found in slurm
-                    return c.UNKNOWN
-
-            return self._slurm_to_saga_state(slurm_state)
-
-        except Exception as e:
-            self._logger.exception('failed to get job state')
-            raise rse.NoSuccess("Error getting the job state for "
-                                "job %s:\n%s" % (pid, e)) from e
-
-        raise rse.NoSuccess._log(self._logger, "Internal SLURM adaptor error"
-                                 " in _job_get_state")
-
-
-    # --------------------------------------------------------------------------
-    #
-    def _sacct_jobstate_match(self, pid):
-        '''
-        get the job state from the slurm accounting data
-        '''
-
-        ret, sacct_out, _ = self.shell.run_sync(
-            "sacct --format=JobID,State --parsable2 --noheader --jobs=%s" % pid)
-
-        # output will look like:
-        # 500723|COMPLETED
-        # 500723.batch|COMPLETED
-        # or:
-        # 500682|CANCELLED by 900369
-        # 500682.batch|CANCELLED
-
-        try:
-            for line in sacct_out.strip().split('\n'):
-
-                slurm_id, slurm_state = line.split('|', 1)
-
-                if slurm_id == pid and slurm_state:
-                    return slurm_state.split()[0].strip()
-
-        except Exception:
-            self._logger.warning('cannot parse sacct output:\n%s' % sacct_out)
-
-        return None
-
-
-    # --------------------------------------------------------------------------
-    #
     def _job_cancel(self, job):
         '''
         Given a job id, attempt to cancel it through use of commandline
         scancel.  Raises exception when unsuccessful.
         '''
 
         if job._state in c.FINAL:
@@ -1435,51 +1013,291 @@
         self._started         = None
         self._finished        = None
 
         # think "reconnect" in terms of "reloading" job id, _NOT_
         # physically creating a new network connection
         if job_info['reconnect']:
             self._id   = job_info['reconnect_jobid']
-            other_info = self.js._job_get_info(self._id)
+            other_info = self._job_get_info()
             self._name = other_info.get('job_name')
             self._started = True
         else:
             self._started = False
 
         return self.get_api()
 
 
     # --------------------------------------------------------------------------
     #
+    def _job_get_info(self):
+        '''
+        use scontrol to grab job info
+        NOT CURRENTLY USED/TESTED, here for later
+        '''
+
+        # prev. info contains the info collect when _job_get_info
+        # was called the last time
+        prev_info = self.js.jobs.get(self._id)
+
+        # if the 'gone' flag is set, there's no need to query the job
+        # state again. it's gone forever
+        if prev_info:
+            if prev_info.get('gone', False):
+                self._logger.debug("Job is gone.")
+                return prev_info
+
+        # curr. info will contain the new job info collect. it starts off
+        # as a copy of prev_info (don't use deepcopy because there is an API
+        # object in the dict -> recursion)
+        curr_info = dict()
+
+        if prev_info:
+            curr_info['job_id'     ] = prev_info.get('job_id'     )
+            curr_info['job_name'   ] = prev_info.get('job_name'   )
+            curr_info['state'      ] = prev_info.get('state'      )
+            curr_info['create_time'] = prev_info.get('create_time')
+            curr_info['start_time' ] = prev_info.get('start_time' )
+            curr_info['end_time'   ] = prev_info.get('end_time'   )
+            curr_info['comp_time'  ] = prev_info.get('comp_time'  )
+            curr_info['exec_hosts' ] = prev_info.get('exec_hosts' )
+            curr_info['gone'       ] = prev_info.get('gone'       )
+            curr_info['output'     ] = prev_info.get('output'     )
+            curr_info['error'      ] = prev_info.get('error'      )
+            curr_info['stdout'     ] = prev_info.get('stdout'     )
+            curr_info['stderr'     ] = prev_info.get('stderr'     )
+            curr_info['ft'         ] = prev_info.get('ft'         )
+        else:
+            curr_info['job_id'     ] = None
+            curr_info['job_name'   ] = None
+            curr_info['state'      ] = None
+            curr_info['create_time'] = None
+            curr_info['start_time' ] = None
+            curr_info['end_time'   ] = None
+            curr_info['comp_time'  ] = None
+            curr_info['exec_hosts' ] = None
+            curr_info['gone'       ] = None
+            curr_info['output'     ] = None
+            curr_info['error'      ] = None
+            curr_info['stdout'     ] = None
+            curr_info['stderr'     ] = None
+            curr_info['ft'         ] = None
+
+        rm, pid = self._adaptor.parse_id(self._id)
+
+        # update current info with scontrol
+        ret, out, _ = self.js.shell.run_sync('scontrol show job %s' % pid)
+
+        # out is comprised of a set of space-limited words like this:
+        #
+        # ----------------------------------------------------------------------
+        # $ scontrol show job 8101313
+        #    JobId=8101313 JobName=pilot.0000 UserId=tg803521(803521)
+        #    GroupId=G-81625(81625) Priority=1701 Nice=0 Account=TG-MCB090174
+        #    QOS=normal JobState=RUNNING Reason=None Dependency=(null) Requeue=0
+        #    Restarts=0 BatchFlag=1 Reboot=0 ExitCode=0:0 RunTime=00:00:25
+        #    TimeLimit=00:15:00 TimeMin=N/A SubmitTime=2017-01-11T15:47:19
+        #    EligibleTime=2017-01-11T15:47:19 StartTime=2017-01-11T15:47:19
+        #    EndTime=2017-01-11T16:02:19 PreemptTime=None SuspendTime=None
+        #    SecsPreSuspend=0 Partition=development AllocNode:Sid=login3:2886
+        #    ReqNodeList=(null) ExcNodeList=(null) NodeList=c557-[901-904]
+        #    BatchHost=c557-901 NumNodes=4 NumCPUs=64 CPUs/Task=1
+        #    ReqB:S:C:T=0:0:*:* TRES=cpu=64,node=4 Socks/Node=*
+        #    NtasksPerN:B:S:C=0:0:*:* CoreSpec=* MinCPUsNode=1 MinMemoryNode=0
+        #    MinTmpDiskNode=0 Features=(null) Gres=(null) Reservation=(null)
+        #    Shared=0 Contiguous=0 Licenses=(null) Network=(null)
+        #    Command=/home1/01083/tg803521/tmp_egGk1n.slurm
+        #    WorkDir=/work/01083/
+        #    StdIn=/dev/null
+        #    StdOut=/work/01083/bootstrap_1.out
+        #    StdErr=/work/01083/bootstrap_1.err
+        #    Power= SICP=0
+        # ----------------------------------------------------------------------
+        #
+        # so we split on spaces and newlines, and then on '=' to get
+        # key-value-pairs.
+
+        elems = out.split()
+        data  = dict()
+        for elem in sorted(elems):
+
+            parts = elem.split('=', 1)
+
+            if len(parts) == 1:
+                # default if no '=' is found
+                parts.append(None)
+
+            # ignore non-splittable ones
+            key, val = parts
+            if val in ['', '(null)']:
+                val = None
+            self._logger.info('%-20s := %s', key, val)
+            data[key] = val
+
+        if data.get('JobState'):
+            curr_info['state'] = self.js._slurm_to_saga_state(data['JobState'])
+        else:
+            curr_info['state'] = self._job_get_state(self._id)
+
+        # update exit code
+        if data.get('ExitCode'):
+            curr_info['exit_code'] = data['ExitCode'].split(':')[0]
+        else:
+            curr_info['exit_code'] = self._job_get_state(self._id)
+
+        curr_info['job_name'   ] = data.get('JobName')
+      # curr_info['create_time'] = data.get('SubmitTime')
+      # curr_info['start_time' ] = data.get('StartTime')
+      # curr_info['end_time'   ] = data.get('EndTime')
+        curr_info['comp_time'  ] = data.get('RunTime')
+        curr_info['exec_hosts' ] = data.get('NodeList')
+
+        # Alas, time stamps are not in EPOCH, and do not contain time zone info,
+        # so we set approximate values here
+        now = time.time()
+        if not curr_info['create_time']: curr_info['create_time'] = now
+
+        if curr_info['state'] in [c.RUNNING] + c.FINAL:
+            if not curr_info['start_time' ]: curr_info['start_time' ] = now
+
+        if curr_info['state'] in c.FINAL:
+
+            if not curr_info['end_time' ]: curr_info['end_time' ] = now
+
+            if curr_info['stdout'] is None:
+
+                if curr_info['output'] is None:
+                    curr_info['output'] = data.get('StdOut')
+
+                ret, out, err = self.js.shell.run_sync(
+                                                 'cat %s' % curr_info['output'])
+                if ret: curr_info['stdout'] = None
+                else  : curr_info['stdout'] = out
+
+            if curr_info['stderr'] is None:
+
+                if curr_info['error'] is None:
+                    curr_info['error'] = data.get('StdErr')
+
+                ret, out, err = self.js.shell.run_sync(
+                                                  'cat %s' % curr_info['error'])
+                if ret: curr_info['stderr'] = None
+                else  : curr_info['stderr'] = out
+
+            self.js._handle_file_transfers(curr_info['ft'], mode='out')
+
+            curr_info['gone'] = True
+
+        self.js.jobs[self._id] = curr_info
+
+        return curr_info
+
+
+    # --------------------------------------------------------------------------
+    #
+    def _job_get_state(self, job_id):
+        '''
+        get the job state from the wrapper shell
+        '''
+
+        # if the state is NEW and we haven't sent out a run command, keep
+        # it listed as NEW
+        if self._state == c.NEW and not self._started:
+            return c.NEW
+
+        # if the state is DONE, CANCELED or FAILED, it is considered
+        # final and we don't need to query the backend again
+        if self._state in c.FINAL:
+            return self._state
+
+        rm, pid = self._adaptor.parse_id(job_id)
+
+        try:
+            ret, out, _ = self.js.shell.run_sync('scontrol show job %s' % pid)
+            match       = self.js.scontrol_jobstate_re.search(out)
+
+            if match:
+                slurm_state = match.group(1)
+            else:
+                # no jobstate found from scontrol
+                # the job may have finished a while back, use sacct to
+                # look at the full slurm history
+                slurm_state = self._sacct_jobstate_match(pid)
+                if not slurm_state:
+                    # no jobstate found in slurm
+                    return c.UNKNOWN
+
+            return self.js._slurm_to_saga_state(slurm_state)
+
+        except Exception as e:
+            self._logger.exception('failed to get job state')
+            raise rse.NoSuccess("Error getting the job state for "
+                                "job %s:\n%s" % (pid, e)) from e
+
+        raise rse.NoSuccess._log(self._logger, "Internal SLURM adaptor error"
+                                 " in _job_get_state")
+
+
+    # --------------------------------------------------------------------------
+    #
+    def _sacct_jobstate_match(self, pid):
+        '''
+        get the job state from the slurm accounting data
+        '''
+
+        ret, sacct_out, _ = self.js.shell.run_sync(
+            "sacct --format=JobID,State --parsable2 --noheader --jobs=%s" % pid)
+
+        # output will look like:
+        # 500723|COMPLETED
+        # 500723.batch|COMPLETED
+        # or:
+        # 500682|CANCELLED by 900369
+        # 500682.batch|CANCELLED
+
+        try:
+            for line in sacct_out.strip().split('\n'):
+
+                slurm_id, slurm_state = line.split('|', 1)
+
+                if slurm_id == pid and slurm_state:
+                    return slurm_state.split()[0].strip()
+
+        except Exception:
+            self._logger.warning('cannot parse sacct output:\n%s' % sacct_out)
+
+        return None
+
+
+    # --------------------------------------------------------------------------
+    #
     @SYNC_CALL
     def get_state(self):
 
-        if self._id is not None:
-            self._state = self.js._job_get_state(self._id)
+        self._state = self._job_get_state(self._id)
         return self._state
 
 
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def get_stdout(self):
 
-        out = self.js._job_get_info(self._id)['stdout']
+        out = self._job_get_info()['stdout']
         if out is None:
             out = ''
           # raise rse.NoSuccess("Couldn't fetch stdout (js reconnected?)")
         return out
 
 
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def get_stderr(self):
 
-        err = self.js._job_get_info(self._id)['stderr']
+        err = self._job_get_info()['stderr']
         if err is None:
             err = ''
           # raise rse.NoSuccess("Couldn't fetch stderr (js reconnected?)")
         return err
 
 
     # --------------------------------------------------------------------------
@@ -1504,22 +1322,22 @@
     def wait(self, timeout):
 
         time_start = time.time()
         rm, pid    = self._adaptor.parse_id(self._id)
 
         while True:
 
-            state = self.js._job_get_state(self._id)
+            state = self._job_get_state(self._id)
             self._logger.debug("wait() for job id %s:%s" % (self._id, state))
 
             if state == c.UNKNOWN:
                 raise rse.IncorrectState("cannot get job state")
 
             if state in c.FINAL:
-                self.js._job_get_info(self._id)
+                self._job_get_info()
                 return True
 
             # check if we hit timeout
             if timeout >= 0:
                 if time.time() - time_start > timeout:
                     return False
 
@@ -1547,25 +1365,25 @@
 
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def get_name(self):
 
         if not self._name:
-            self._name = self.js._job_get_info(self._id)['job_name']
+            self._name = self._job_get_info()['job_name']
         return self._name
 
 
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def get_exit_code(self):
 
         # FIXME: use cache
-        return self.js._job_get_info(self._id)['exit_code']
+        return self._job_get_info()['exit_code']
 
 
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def suspend(self):
 
@@ -1582,44 +1400,44 @@
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def get_created(self):
 
         # FIXME: use cache
         # FIXME: convert to EOPCH
-        return self.js._job_get_info(self._id)['create_time']
+        return self._job_get_info()['create_time']
 
 
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def get_started(self):
 
         # FIXME: use cache
         # FIXME: convert to EPOCH
-        return self.js._job_get_info(self._id)['start_time']
+        return self._job_get_info()['start_time']
 
 
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def get_finished(self):
 
         # FIXME: use cache
         # FIXME: convert to EPOCH
-        return self.js._job_get_info(self._id)['end_time']
+        return self._job_get_info()['end_time']
 
 
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def get_execution_hosts(self):
 
         # FIXME: use cache
-        return self.js._job_get_info(self._id)['exec_hosts']
+        return self._job_get_info()['exec_hosts']
 
 
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def cancel(self, timeout):
 
@@ -1627,13 +1445,13 @@
 
 
     # --------------------------------------------------------------------------
     #
     @SYNC_CALL
     def run(self):
 
-        self._id      = self.js._job_run(self)
+        self._id      = self.js._job_run(self.jd)
         self._started = True
 
 
 # ------------------------------------------------------------------------------
```

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/srm/srmfile.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/srm/srmfile.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/adaptors/torque/torquejob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/torque/torquejob.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/advert/constants.py` & `radical.saga-1.8.0/src/radical/saga/advert/constants.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/advert/directory.py` & `radical.saga-1.8.0/src/radical/saga/advert/directory.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/advert/entry.py` & `radical.saga-1.8.0/src/radical/saga/advert/entry.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/attributes.py` & `radical.saga-1.8.0/src/radical/saga/attributes.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/base.py` & `radical.saga-1.8.0/src/radical/saga/base.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/configs/adaptors_globus_online_file.json` & `radical.saga-1.8.0/src/radical/saga/configs/adaptors_globus_online_file.json`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/configs/adaptors_shell_job.json` & `radical.saga-1.8.0/src/radical/saga/configs/adaptors_shell_job.json`

 * *Files 10% similar despite different names*

```diff
@@ -7,10 +7,14 @@
     # the number of available job service instances per remote host.
     "enable_notifications" : false,
 
     # Purge job information (state, stdio, ...) for all jobs which are in final
     # state when starting the job service instance. Note that this will purge
     # *all* suitable jobs, including the ones managed by another, live job
     # service instance.
-    "purge_on_start" : true
+    "purge_on_start" : true,
+
+    # The adaptor stores job state information on the filesystem on the target
+    # resource.  This parameter specified what location should be used.
+    "base_workdir" : "${HOME}/.radical/saga/adaptors/shell_job/"
 }
```

### Comparing `radical_saga-1.60.0/src/radical/saga/configs/registry_default.json` & `radical.saga-1.8.0/src/radical/saga/configs/registry_default.json`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/configs/session.json` & `radical.saga-1.8.0/src/radical/saga/configs/session.json`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/configs/utils_default.json` & `radical.saga-1.8.0/src/radical/saga/configs/utils_default.json`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/constants.py` & `radical.saga-1.8.0/src/radical/saga/constants.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/context.py` & `radical.saga-1.8.0/src/radical/saga/context.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/engine/engine.py` & `radical.saga-1.8.0/src/radical/saga/engine/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 __license__   = "MIT"
 
 
 """ Provides the SAGA runtime. """
 
 import radical.utils as ru
 
-from .. import exceptions as rse
+from ..        import exceptions as rse
+from ..version import *
 
 
 # ------------------------------------------------------------------------------
 #
 # we set the default of the pty share mode to 'no' on CentOS, as that seems to
 # consistently come with old ssh versions which can't handle sharing for sftp
 # channels.
@@ -130,14 +131,15 @@
         # get angine, adaptor and pty configs
         self._cfg      = ru.Config('radical.saga.engine')
         self._pty_cfg  = ru.Config('radical.saga.pty')
         self._registry = ru.Config('radical.saga.registry')
 
         # Initialize the logging, and log version (this is a singleton!)
         self._logger = ru.Logger('radical.saga')
+        self._logger.info('radical.saga         version: %s' % version_detail)
 
         # load adaptors
         self._load_adaptors()
 
 
     # --------------------------------------------------------------------------
     #
```

### Comparing `radical_saga-1.60.0/src/radical/saga/exceptions.py` & `radical.saga-1.8.0/src/radical/saga/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,26 @@
 
         # we can't do that earlier as _msg was not set up before
         self._messages = [self._message]
 
 
     # --------------------------------------------------------------------------
     #
+    def __str__ (self) :
+        return self.get_message ()
+
+
+    # --------------------------------------------------------------------------
+    #
+    def __repr__ (self) :
+        return "%s\n%s" % (self._message, self._traceback)
+
+
+    # --------------------------------------------------------------------------
+    #
     def _clone (self) :
         """ method is used internally -- see :func:`_get_exception_stack`."""
 
         clone = self.__class__ ("")
 
         clone._parent    = self._parent
         clone._object    = self._object
```

### Comparing `radical_saga-1.60.0/src/radical/saga/filesystem/constants.py` & `radical.saga-1.8.0/src/radical/saga/filesystem/constants.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/filesystem/directory.py` & `radical.saga-1.8.0/src/radical/saga/filesystem/directory.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/filesystem/file.py` & `radical.saga-1.8.0/src/radical/saga/filesystem/file.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/job/constants.py` & `radical.saga-1.8.0/src/radical/saga/job/constants.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/job/container.py` & `radical.saga-1.8.0/src/radical/saga/job/container.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/job/description.py` & `radical.saga-1.8.0/src/radical/saga/job/description.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/job/job.py` & `radical.saga-1.8.0/src/radical/saga/job/job.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/job/service.py` & `radical.saga-1.8.0/src/radical/saga/job/service.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/messages/message.py` & `radical.saga-1.8.0/src/radical/saga/messages/message.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/monitorable.py` & `radical.saga-1.8.0/src/radical/saga/monitorable.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/namespace/directory.py` & `radical.saga-1.8.0/src/radical/saga/namespace/directory.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/namespace/entry.py` & `radical.saga-1.8.0/src/radical/saga/namespace/entry.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/replica/constants.py` & `radical.saga-1.8.0/src/radical/saga/replica/constants.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/replica/logical_directory.py` & `radical.saga-1.8.0/src/radical/saga/replica/logical_directory.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/replica/logical_file.py` & `radical.saga-1.8.0/src/radical/saga/replica/logical_file.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/resource/constants.py` & `radical.saga-1.8.0/src/radical/saga/resource/constants.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/resource/description.py` & `radical.saga-1.8.0/src/radical/saga/resource/description.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/resource/manager.py` & `radical.saga-1.8.0/src/radical/saga/resource/manager.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/resource/resource.py` & `radical.saga-1.8.0/src/radical/saga/resource/resource.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/session.py` & `radical.saga-1.8.0/src/radical/saga/session.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/task.py` & `radical.saga-1.8.0/src/radical/saga/task.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/url.py` & `radical.saga-1.8.0/src/radical/saga/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     purposes -- it allows to manipulate individual URL elements, while
     ensuring that the resulting URL is well formatted. Example::
 
       # create a URL from a string
       location = saga.Url ("file://localhost/tmp/file.dat")
       d = saga.filesystem.Directory(location)
 
-    A URL consists of the following components (where one or more can
+    A URL consists of the following components (where one ore more can
     be 'None')::
 
       <scheme>://<user>:<pass>@<host>:<port>/<path>?<query>#<fragment>
 
     Each of these components can be accessed via its property or
     alternatively, via getter / setter methods. Example::
```

### Comparing `radical_saga-1.60.0/src/radical/saga/utils/job/transfer_directives.py` & `radical.saga-1.8.0/src/radical/saga/utils/job/transfer_directives.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/utils/misc.py` & `radical.saga-1.8.0/src/radical/saga/utils/misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 import re
 import os
 import sys
 import time
 import socket
 import traceback
 
-import radical.utils as ru
-
 from ..url import Url
 from ..    import exceptions as se
 
 
 """ Provides an assortment of utilities """
 
 _latencies = {}
@@ -37,62 +35,84 @@
         stack           = traceback.extract_stack ()
         traceback_list  = traceback.format_list (stack)
         return "".join (traceback_list[:-1])
 
 
 # --------------------------------------------------------------------
 #
-def host_is_valid (host) :
+def host_is_local (host) :
+    """ Returns True if the given host is the localhost
     """
+
+    if  not host:
+        return True
+
+    elif host == 'localhost':
+        return True
+
+    else:
+        sockhost = socket.gethostname()
+        while sockhost:
+            if host == sockhost:
+                return True
+            sockhost = '.'.join(sockhost.split('.')[1:])
+
+    return False
+
+
+# --------------------------------------------------------------------
+#
+def host_is_valid (host) :
+    """ 
     Returns True if the given hostname can be resolved.
     We also test the reverse DNS lookup -- some seriously stupid and standard
     violating internet providers implement a DNS catchall -- the reverse lookup
     can catch that case in some cases (say that quickly 3 times!)
     """
 
     # FIXME: cache results so that further lookups are quick
 
-    if ru.is_localhost(host):
+    if  host_is_local (host) :
         return True
 
     try:
         _ = socket.gethostbyname (host)
         return True
     except :
         return False
 
 
 # --------------------------------------------------------------------
 #
 def get_host_latency (host_url) :
-    """
+    """ 
     This call measures the base tcp latency for a connection to the target
     host.  Note that port 22 is used for connection tests, unless the URL
     explicitly specifies a different port.  If the used port is blocked, the
     returned latency can be wrong by orders of magnitude.
     """
 
     try :
         # FIXME see comments to #62bebc9 -- this breaks for some cases, or is at
         # least annoying.  Thus we disable latency checking for the time being,
-        # and return a constant assumed latency of 250ms (which approximately
+        # and return a constant assumed latency of 250ms (which approximately 
         # represents a random WAN link).
         return 0.25
 
         global _latencies
 
         if  host_url in _latencies :
             return _latencies[host_url]
 
         u = Url (host_url)
 
         if u.host : host = u.host
         else      : host = 'localhost'
         if u.port : port = u.port
-        else      : port = 22  # FIXME: we should guess by protocol
+        else      : port = 22  # FIXME: we should guess by protocol 
 
         # ensure host is valid
         if not host_is_valid(host):
             raise ValueError('invalid host')
 
         start = time.time ()
 
@@ -112,33 +132,33 @@
 
         raise
 
 
 # --------------------------------------------------------------------
 #
 def url_is_local (arg) :
-    """
+    """ 
     Returns True if the given url points to localhost.
 
     We consider all URLs which explicitly define a port as non-local, because it
     looks like someone wants to explicitly use some protocol --
-    `ssh://localost:2222/` is likely to point at an ssh tunnel.
+    `ssh://localost:2222/` is likely to point at an ssh tunnel.  
 
     If, however, the port matches the default port for the given protocol, we
     consider it local again -- `ssh://localhost:22/` is most likely a real local
     activity.
 
     Note that the schema set operates on substring level, so that we will accept
     port 22 for `ssh` and also for `sge+ssh` -- this may break in corner cases
     (altough I can't think of any right now).
     """
 
     u = Url (arg)
 
-    if not ru.is_localhost(u.host):
+    if  not host_is_local (u.host) :
         return False
 
     # host is local, but what does the port indicate?
     if u.port and u.port > 0 :
 
         try :
             if  socket.getservbyport (u.port) in u.schema :
@@ -159,40 +179,40 @@
     that path element does not start with '/'.
     """
 
     u1 = Url (url_1)
 
     if  str (u1) == str(u1.path) :
         if  not u1.path :
-            return True
+            return True 
         elif u1.path[0] != '/' :
             return True
 
     return False
 
 
 # --------------------------------------------------------------------
 #
 def url_get_dirname (url_1) :
-    """
+    """ 
     Extract the directory part of the given URL's path element.  We consider
     everything up to the last '/' as directory.  That also holds for relative
     paths.
     """
 
     u1 = Url (url_1)
     p1 = u1.path
 
     return re.sub (r"[^/]*$", "", p1)
 
 
 # --------------------------------------------------------------------
 #
 def url_get_filename (url_1) :
-    """
+    """ 
     Extract the directory part of the given URL's path element.  We consider
     everything up to the last '/' as directory.  That also holds for relative
     paths.
     """
 
     u1 = Url (url_1)
     p1 = u1.path
@@ -202,28 +222,28 @@
     else :
         return p1
 
 
 # --------------------------------------------------------------------
 #
 def url_normalize (url_1) :
-    """
+    """ 
     The path element of the URL is normalized
     """
 
     ret      = Url (url_1)
     ret.path = os.path.normpath (ret.path)
 
     return ret
 
 
 # --------------------------------------------------------------------
 #
 def url_make_absolute (url_1, url_2) :
-    """
+    """ 
     URL1 is expected to only have a path
     Missing elements in url_1 are copied from url_2 -- but path stays the
     same.  Unless it is a relative path in the first place: then it is
     interpreted as relative to url_2.path, and is made absolute.
     protocol/port/user etc.
     """
 
@@ -252,41 +272,41 @@
 
     return ret
 
 
 # --------------------------------------------------------------------
 #
 def url_is_compatible (url_1, url_2) :
-    """
+    """ 
     Returns True if the given urls point to the same host, using the same
     protocol/port/user etc.  If one of the URLs only contains a path, it is
     considered compatible with any other URL.
     """
 
     u1 = Url (url_1)
     u2 = Url (url_2)
 
     # if either one url only contains a path, it is compatible to anything.
     if os.path.normpath(u1.path) == os.path.normpath (str(u1)) : return True
     if os.path.normpath(u2.path) == os.path.normpath (str(u2)) : return True
 
     # more than path in both URLs -- check compatibility for all elements
-    if u1.scheme   and     u2.scheme   and u1.scheme   != u2.scheme  : return False
+    if u1.scheme   and     u2.scheme   and u1.scheme   != u2.scheme  : return False 
     if u1.host     and     u2.host     and u1.host     != u2.host    : return False
     if u1.port     and     u2.port     and u1.port     != u2.port    : return False
     if u1.username and     u2.username and u1.username != u2.username: return False
     if u1.password and     u2.password and u1.password != u2.password: return False
 
-    if u1.scheme   and not u2.scheme  : return False
+    if u1.scheme   and not u2.scheme  : return False 
     if u1.host     and not u2.host    : return False
     if u1.port     and not u2.port    : return False
     if u1.username and not u2.username: return False
     if u1.password and not u2.password: return False
 
-    if u2.scheme   and not u1.scheme  : return False
+    if u2.scheme   and not u1.scheme  : return False 
     if u2.host     and not u1.host    : return False
     if u2.port     and not u1.port    : return False
     if u2.username and not u1.username: return False
     if u2.password and not u1.password: return False
 
     # no differences detected (ignored fragments and query though)
     return True
```

### Comparing `radical_saga-1.60.0/src/radical/saga/utils/pty_exceptions.py` & `radical.saga-1.8.0/src/radical/saga/utils/pty_exceptions.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/utils/pty_process.py` & `radical.saga-1.8.0/src/radical/saga/utils/pty_process.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical/saga/utils/pty_shell.py` & `radical.saga-1.8.0/src/radical/saga/utils/pty_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
     **Asynchronous Notifications:**
 
     A third pty process will be created for asynchronous notifications.  For
     that purpose, the shell started on the first channel will create a named
     pipe, at::
 
-      $RADICAL_BASE/.radical/saga/adaptors/shell/async.$$
+      $HOME/.radical/saga/adaptors/shell/async.$$
 
     ``$$`` here represents the pid of the shell process.  It will also set the
     environment variable ``SAGA_ASYNC_PIPE`` to point to that named pipe -- any
     application running on the remote host can write event messages to that
     pipe, which will be available on the local end (see below).  `PTYShell`
     leaves it unspecified what format those messages have, but messages are
     expected to be separated by newlines.
@@ -221,20 +221,28 @@
         self.cfg = self.cfg.pty
 
         # get prompt pattern from config, or use default
         self.prompt    = self.cfg.get('prompt_pattern', DEFAULT_PROMPT)
         self.prompt_re = re.compile ("^(.*?)%s"    % self.prompt, re.DOTALL)
         self.logger.info ("PTY prompt pattern: %s" % self.prompt)
 
-        # local dir for file staging caches
-        self.base = ru.get_radical_base('saga') + 'adaptors/shell/'
+        # we need a local dir for file staging caches.  At this point we use
+        # $HOME, but should make this configurable (FIXME)
+        self.base = os.environ['HOME'] + '/.radical/saga/adaptors/shell/'
+
         try:
-            ru.rec_makedir(self.base)
+            os.makedirs (self.base)
+
         except OSError as e:
-            raise rse.NoSuccess('could not create staging dir: %s' % e) from e
+            if e.errno == errno.EEXIST and os.path.isdir (self.base):
+                pass
+            else:
+                raise rse.NoSuccess ("could not create staging dir: %s" % e) \
+                      from e
+
 
         self.factory    = supsf.PTYShellFactory   ()
         self.pty_info   = self.factory.initialize (self.url,    self.session,
                                                    self.prompt, self.logger,
                                                    self.cfg,    self.posix,
                                                    interactive=self.interactive)
         self.pty_shell  = self.factory.run_shell  (self.pty_info)
```

### Comparing `radical_saga-1.60.0/src/radical/saga/utils/pty_shell_factory.py` & `radical.saga-1.8.0/src/radical/saga/utils/pty_shell_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,15 +581,15 @@
                 info['logger'].warning("Could not contact host '%s': %s"
                                       % (url, e))
 
             if  info['shell_type'] == "sh" :
 
                 info['sh_env'] = "/usr/bin/env TERM=vt100 "  # avoid ansi escapes
 
-              # if not ru.is_localhost(url.host) :
+              # if not sumisc.host_is_local (url.host) :
               #     raise rse.BadParameter._log (self.logger,
               #             "expect local host for '%s://', not '%s'"
               #             % (url.schema, url.host))
 
                 if  'user' in info and info['user'] :
                     pass
                 else :
```

### Comparing `radical_saga-1.60.0/src/radical/saga/utils/test_config.py` & `radical.saga-1.8.0/src/radical/saga/utils/test_config.py`

 * *Files identical despite different names*

### Comparing `radical_saga-1.60.0/src/radical.saga.egg-info/SOURCES.txt` & `radical.saga-1.8.0/src/radical.saga.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 CHANGES.md
 LICENSE.md
 MANIFEST.in
 README.md
 VERSION
-pyproject.toml
-requirements-docs.txt
-requirements-tests.txt
-requirements.txt
+setup.cfg
 setup.py
 bin/radical-saga-version
 examples/context/context_ssh.py
 examples/files/go_file_copy.py
 examples/files/go_remotedir_list.py
 examples/files/http_file_copy.py
 examples/files/sftp_file_copy.py
@@ -18,14 +15,15 @@
 examples/files/srm_get_size.py
 examples/jobs/cobalt.py
 examples/jobs/condorjob.py
 examples/jobs/loadlevelerjob.py
 examples/jobs/localjob.py
 examples/jobs/localjobcontainer.py
 examples/jobs/lsfjob.py
+examples/jobs/noopjob.py
 examples/jobs/pbsgsisshjob.py
 examples/jobs/pbsjob.py
 examples/jobs/pbsprojob.py
 examples/jobs/sgejob.py
 examples/jobs/slurmjob.py
 examples/jobs/slurmjobcontainer.py
 examples/jobs/torque_gsissh_job.py
@@ -41,29 +39,32 @@
 examples/tutorial/saga_example_remote_staging.py
 examples/tutorial/mandelbrot/mandelbrot.py
 examples/tutorial/mandelbrot/saga_mandelbrot.py
 examples/tutorial/mandelbrot/saga_mandelbrot_osg.py
 src/radical.saga.egg-info/PKG-INFO
 src/radical.saga.egg-info/SOURCES.txt
 src/radical.saga.egg-info/dependency_links.txt
+src/radical.saga.egg-info/namespace_packages.txt
 src/radical.saga.egg-info/not-zip-safe
 src/radical.saga.egg-info/requires.txt
 src/radical.saga.egg-info/top_level.txt
+src/radical/saga/SDIST
 src/radical/saga/VERSION
 src/radical/saga/__init__.py
 src/radical/saga/attributes.py
 src/radical/saga/base.py
 src/radical/saga/constants.py
 src/radical/saga/context.py
 src/radical/saga/exceptions.py
 src/radical/saga/monitorable.py
 src/radical/saga/sasync.py
 src/radical/saga/session.py
 src/radical/saga/task.py
 src/radical/saga/url.py
+src/radical/saga/version.py
 src/radical/saga/adaptors/__init__.py
 src/radical/saga/adaptors/base.py
 src/radical/saga/adaptors/aws/__init__.py
 src/radical/saga/adaptors/aws/ec2_resource.py
 src/radical/saga/adaptors/cobalt/__init__.py
 src/radical/saga/adaptors/cobalt/cobaltjob.py
 src/radical/saga/adaptors/condor/__init__.py
@@ -104,14 +105,18 @@
 src/radical/saga/adaptors/http/http_file.py
 src/radical/saga/adaptors/irods/__init__.py
 src/radical/saga/adaptors/irods/irods_replica.py
 src/radical/saga/adaptors/loadl/__init__.py
 src/radical/saga/adaptors/loadl/loadljob.py
 src/radical/saga/adaptors/lsf/__init__.py
 src/radical/saga/adaptors/lsf/lsfjob.py
+src/radical/saga/adaptors/mock/__init__.py
+src/radical/saga/adaptors/mock/shell_file.py
+src/radical/saga/adaptors/mock/shell_job.py
+src/radical/saga/adaptors/mock/shell_resource.py
 src/radical/saga/adaptors/noop/__init__.py
 src/radical/saga/adaptors/noop/noop_job.py
 src/radical/saga/adaptors/pbs/__init__.py
 src/radical/saga/adaptors/pbs/pbsjob.py
 src/radical/saga/adaptors/pbspro/__init__.py
 src/radical/saga/adaptors/pbspro/pbsprojob.py
 src/radical/saga/adaptors/redis/__init__.py
@@ -143,16 +148,18 @@
 src/radical/saga/configs/adaptors_condorjob.json
 src/radical/saga/configs/adaptors_globus_online_file.json
 src/radical/saga/configs/adaptors_loadljob.json
 src/radical/saga/configs/adaptors_myproxy.json
 src/radical/saga/configs/adaptors_sgejob.json
 src/radical/saga/configs/adaptors_shell_job.json
 src/radical/saga/configs/registry_default.json
+src/radical/saga/configs/resources.json
 src/radical/saga/configs/session.json
 src/radical/saga/configs/utils_default.json
+src/radical/saga/configs/resources/stampede.json
 src/radical/saga/configs/tests/__init__.py
 src/radical/saga/configs/tests/test_advert_redis_local.json
 src/radical/saga/configs/tests/test_advert_redis_repex1.json
 src/radical/saga/configs/tests/test_condor_osg_engage.json
 src/radical/saga/configs/tests/test_condor_ssh_osg.json
 src/radical/saga/configs/tests/test_default.json
 src/radical/saga/configs/tests/test_file_localhost.json
@@ -211,9 +218,8 @@
 src/radical/saga/utils/misc.py
 src/radical/saga/utils/pty_exceptions.py
 src/radical/saga/utils/pty_process.py
 src/radical/saga/utils/pty_shell.py
 src/radical/saga/utils/pty_shell_factory.py
 src/radical/saga/utils/test_config.py
 src/radical/saga/utils/job/__init__.py
-src/radical/saga/utils/job/transfer_directives.py
-tests/test_cheyenne.py
+src/radical/saga/utils/job/transfer_directives.py
```

