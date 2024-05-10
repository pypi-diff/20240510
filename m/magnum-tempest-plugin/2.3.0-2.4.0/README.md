# Comparing `tmp/magnum_tempest_plugin-2.3.0.tar.gz` & `tmp/magnum_tempest_plugin-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_tempest_plugin-2.3.0.tar", last modified: Thu Mar 21 10:13:25 2024, max compression
+gzip compressed data, was "magnum_tempest_plugin-2.4.0.tar", last modified: Fri May 10 13:46:41 2024, max compression
```

## Comparing `magnum_tempest_plugin-2.3.0.tar` & `magnum_tempest_plugin-2.4.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.905722 magnum_tempest_plugin-2.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/.stestr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.897721 magnum_tempest_plugin-2.3.0/.zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/.zuul.d/base.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/.zuul.d/jobs_2023_1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2377 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/.zuul.d/jobs_2023_2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/.zuul.d/jobs_master.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/.zuul.d/jobs_zed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/.zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2694 2024-03-21 10:13:25.000000 magnum_tempest_plugin-2.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7603 2024-03-21 10:13:25.000000 magnum_tempest_plugin-2.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2024-03-21 10:13:25.905722 magnum_tempest_plugin-2.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.897721 magnum_tempest_plugin-2.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.897721 magnum_tempest_plugin-2.3.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2641 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.897721 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.897721 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4584 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2003 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6512 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11701 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/datagen.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.901722 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/templates/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13143 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/templates/cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8655 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/templates/cluster_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2798 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/templates/cluster_template_admin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4927 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3924 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.901722 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.901722 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6292 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.901722 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.901722 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1910 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/cert_client.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7138 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/cluster_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4360 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/cluster_template_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/magnum_service_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.901722 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/cert_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/cluster_id_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/cluster_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/cluster_template_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2473 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/cluster_templatepatch_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2371 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/clusterpatch_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/magnum_service_model.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.901722 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4873 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster_template_admin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/test_magnum_service.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2897 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/test_cluster.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1412 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/test_cluster_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/test_cluster_template_admin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2134 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/test_magnum_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.901722 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/contrib/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8007 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/contrib/copy_instance_logs.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1652 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/contrib/copy_pod_logs.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.897721 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2024-03-21 10:13:25.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3391 2024-03-21 10:13:25.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-21 10:13:25.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-03-21 10:13:25.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-21 10:13:25.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-21 10:13:25.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-21 10:13:25.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       22 2024-03-21 10:13:25.000000 magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.893721 magnum_tempest_plugin-2.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.901722 magnum_tempest_plugin-2.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/releasenotes/notes/drop-py-2-7-c997716906e17740.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.905722 magnum_tempest_plugin-2.3.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.905722 magnum_tempest_plugin-2.3.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:13:25.905722 magnum_tempest_plugin-2.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8804 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2024-03-21 10:13:25.905722 magnum_tempest_plugin-2.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1497 2024-03-21 10:12:44.000000 magnum_tempest_plugin-2.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.499495 magnum_tempest_plugin-2.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/.stestr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.487494 magnum_tempest_plugin-2.4.0/.zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2573 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/.zuul.d/base.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/.zuul.d/jobs_2023_1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2377 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/.zuul.d/jobs_2023_2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/.zuul.d/jobs_master.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/.zuul.d/jobs_zed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/.zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2694 2024-05-10 13:46:41.000000 magnum_tempest_plugin-2.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7656 2024-05-10 13:46:41.000000 magnum_tempest_plugin-2.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2024-05-10 13:46:41.499495 magnum_tempest_plugin-2.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.487494 magnum_tempest_plugin-2.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.487494 magnum_tempest_plugin-2.4.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2641 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.491495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.491495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4584 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2003 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6512 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11701 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/datagen.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.491495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/templates/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13143 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/templates/cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8655 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/templates/cluster_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2798 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/templates/cluster_template_admin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4927 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3924 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2165 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.491495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.495495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6292 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.495495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.495495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1035 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1910 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/cert_client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7138 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/cluster_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4360 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/cluster_template_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/magnum_service_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.495495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/cert_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/cluster_id_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1051 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/cluster_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/cluster_template_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2473 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/cluster_templatepatch_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2371 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/clusterpatch_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/magnum_service_model.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.499495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4873 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      899 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster_template_admin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/test_magnum_service.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2897 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/test_cluster.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1412 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/test_cluster_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/test_cluster_template_admin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2134 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/test_magnum_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.499495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/contrib/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8007 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/contrib/copy_instance_logs.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1826 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/contrib/copy_pod_logs.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.491495 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2024-05-10 13:46:41.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3391 2024-05-10 13:46:41.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-10 13:46:41.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-05-10 13:46:41.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-10 13:46:41.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-05-10 13:46:41.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-05-10 13:46:41.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       22 2024-05-10 13:46:41.000000 magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.483494 magnum_tempest_plugin-2.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.499495 magnum_tempest_plugin-2.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/releasenotes/notes/drop-py-2-7-c997716906e17740.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.499495 magnum_tempest_plugin-2.4.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.499495 magnum_tempest_plugin-2.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:41.499495 magnum_tempest_plugin-2.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8804 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2024-05-10 13:46:41.499495 magnum_tempest_plugin-2.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1497 2024-05-10 13:46:19.000000 magnum_tempest_plugin-2.4.0/tox.ini
```

### Comparing `magnum_tempest_plugin-2.3.0/.zuul.d/base.yaml` & `magnum_tempest_plugin-2.4.0/.zuul.d/base.yaml`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/.zuul.d/jobs_2023_1.yaml` & `magnum_tempest_plugin-2.4.0/.zuul.d/jobs_2023_1.yaml`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/.zuul.d/jobs_2023_2.yaml` & `magnum_tempest_plugin-2.4.0/.zuul.d/jobs_2023_2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/.zuul.d/jobs_master.yaml` & `magnum_tempest_plugin-2.4.0/.zuul.d/jobs_master.yaml`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/.zuul.d/jobs_zed.yaml` & `magnum_tempest_plugin-2.4.0/.zuul.d/jobs_zed.yaml`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/AUTHORS` & `magnum_tempest_plugin-2.4.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/CONTRIBUTING.rst` & `magnum_tempest_plugin-2.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/ChangeLog` & `magnum_tempest_plugin-2.4.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+2.4.0
+-----
+
+* CI: Wait before checking pods status
+
 2.3.0
 -----
 
 * CI: Rework job definitions into templates
 * Add pods description in logs
 * CI: Wait for pods to exit ContainerCreating state
 * Remove yoga job
```

### Comparing `magnum_tempest_plugin-2.3.0/LICENSE` & `magnum_tempest_plugin-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/PKG-INFO` & `magnum_tempest_plugin-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: magnum_tempest_plugin
-Version: 2.3.0
+Version: 2.4.0
 Summary: Tempest plugin for Magnum Project
 Home-page: https://opendev.org/openstack/magnum-tempest-plugin
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===============================
         openstack Magnum Tempest Plugin
```

### Comparing `magnum_tempest_plugin-2.3.0/doc/source/conf.py` & `magnum_tempest_plugin-2.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/doc/source/index.rst` & `magnum_tempest_plugin-2.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/base.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/base.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/client.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/client.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/config.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/config.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/datagen.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/datagen.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/manager.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/manager.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/models.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/models.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/templates/cluster.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/templates/cluster.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/templates/cluster_template.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/templates/cluster_template.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/templates/cluster_template_admin.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/templates/cluster_template_admin.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/common/utils.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/common/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/config.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/config.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/plugin.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/base.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/base.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/__init__.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/cert_client.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/cert_client.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/cluster_client.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/cluster_client.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/cluster_template_client.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/cluster_template_client.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/clients/magnum_service_client.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/clients/magnum_service_client.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/cert_model.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/cert_model.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/cluster_id_model.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/cluster_id_model.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/cluster_model.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/cluster_model.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/cluster_template_model.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/cluster_template_model.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/cluster_templatepatch_model.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/cluster_templatepatch_model.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/clusterpatch_model.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/clusterpatch_model.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/models/magnum_service_model.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/models/magnum_service_model.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/base.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/base.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster_template.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster_template.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster_template_admin.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/test_cluster_template_admin.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/rbac/test_magnum_service.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/rbac/test_magnum_service.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/test_cluster.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/test_cluster.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/test_cluster_template.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/test_cluster_template.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/test_cluster_template_admin.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/test_cluster_template_admin.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/api/v1/test_magnum_service.py` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/api/v1/test_magnum_service.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/contrib/copy_instance_logs.sh` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/contrib/copy_instance_logs.sh`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin/tests/contrib/copy_pod_logs.sh` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin/tests/contrib/copy_pod_logs.sh`

 * *Files 19% similar despite different names*

```diff
@@ -12,36 +12,45 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 set -o xtrace
 
 LOG_DIR="/tmp/magnum-nodes/kubernetes/"
 KUBECTL="/opt/stack/bin/kubectl --kubeconfig /tmp/magnum-nodes/kube.conf"
+
+function gather_kube_logs {
+    ${KUBECTL} get all -A -o wide > ${LOG_DIR}/kubectl_get_all
+
+    for ns in $(${KUBECTL} get -o name namespace); do
+        mkdir -p ${LOG_DIR}/pods/${ns#*/}
+        for pod in $(${KUBECTL} get -n ${ns#*/} -o name pod); do
+            ${KUBECTL} -n ${ns#*/} describe pod ${pod#*/} > ${LOG_DIR}/pods/${ns#*/}/${pod#*/}_describe
+            ${KUBECTL} -n ${ns#*/} logs ${pod#*/} > ${LOG_DIR}/pods/${ns#*/}/${pod#*/}
+        done
+    done
+}
+    
 mkdir -p ${LOG_DIR}
 
+echo "INFO: Waiting 5 minutes for Pods to start up"
+sleep 300
+
 while ${KUBECTL} get pods -A -o wide | grep -q "ContainerCreating";
 do
     count=$(( $count+1 ))
-    if [ "$count" = "10" ]; then
+    if [ "$count" = "100" ]; then
         echo "ERROR: Waiting for pods to exit ContainerCreating state timed out"
+        gather_kube_logs
         exit 1
     else
         sleep 60
     fi
 done
 
-${KUBECTL} get all -A -o wide > ${LOG_DIR}/kubectl_get_all
-
-for ns in $(${KUBECTL} get -o name namespace); do
-    mkdir -p ${LOG_DIR}/pods/${ns#*/}
-    for pod in $(${KUBECTL} get -n ${ns#*/} -o name pod); do
-        ${KUBECTL} -n ${ns#*/} describe pod ${pod#*/} > ${LOG_DIR}/pods/${ns#*/}/${pod#*/}_describe
-        ${KUBECTL} -n ${ns#*/} logs ${pod#*/} > ${LOG_DIR}/pods/${ns#*/}/${pod#*/}
-    done
-done
+gather_kube_logs
 
 # NOTE(mnasiadka): Fail if any pod is not Running
 FAILED_PODS=$(${KUBECTL} get pods -A --field-selector=status.phase!=Running)
 
 if [ ! -z "${FAILED_PODS}" ]; then
     echo "ERROR: Detected pods in state other than Running"
     echo ${FAILED_PODS}
```

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/PKG-INFO` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: magnum-tempest-plugin
-Version: 2.3.0
+Version: 2.4.0
 Summary: Tempest plugin for Magnum Project
 Home-page: https://opendev.org/openstack/magnum-tempest-plugin
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===============================
         openstack Magnum Tempest Plugin
```

### Comparing `magnum_tempest_plugin-2.3.0/magnum_tempest_plugin.egg-info/SOURCES.txt` & `magnum_tempest_plugin-2.4.0/magnum_tempest_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/releasenotes/source/conf.py` & `magnum_tempest_plugin-2.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/setup.cfg` & `magnum_tempest_plugin-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/setup.py` & `magnum_tempest_plugin-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `magnum_tempest_plugin-2.3.0/tox.ini` & `magnum_tempest_plugin-2.4.0/tox.ini`

 * *Files identical despite different names*

