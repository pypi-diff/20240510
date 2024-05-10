# Comparing `tmp/mqtt-hass-base-4.2.6.tar.gz` & `tmp/mqtt_hass_base-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt-hass-base-4.2.6.tar", last modified: Fri Jan 26 02:26:35 2024, max compression
+gzip compressed data, was "mqtt_hass_base-4.3.0.tar", last modified: Fri May 10 03:21:51 2024, max compression
```

## Comparing `mqtt-hass-base-4.2.6.tar` & `mqtt_hass_base-4.3.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 02:26:35.390533 mqtt-hass-base-4.2.6/
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3384 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1017 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    19948 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)    11344 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1372 2024-01-26 02:26:35.390533 mqtt-hass-base-4.2.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)    34804 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt-hass-base.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 02:26:35.386532 mqtt-hass-base-4.2.6/mqtt_hass_base/
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/const.py
--rw-rw-rw-   0 root         (0) root         (0)     9696 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/daemon.py
--rw-rw-rw-   0 root         (0) root         (0)     8872 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 02:26:35.386532 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5178 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/binarysensor.py
--rw-rw-rw-   0 root         (0) root         (0)     3975 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/button.py
--rw-rw-rw-   0 root         (0) root         (0)     6978 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/common.py
--rw-rw-rw-   0 root         (0) root         (0)     6099 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/light.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/lock.py
--rw-rw-rw-   0 root         (0) root         (0)     6062 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/number.py
--rw-rw-rw-   0 root         (0) root         (0)     4362 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/sensor.py
--rw-rw-rw-   0 root         (0) root         (0)     4865 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/switch.py
--rw-rw-rw-   0 root         (0) root         (0)     7285 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/entity/vacuum.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/error.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/mqtt_hass_base/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 02:26:35.386532 mqtt-hass-base-4.2.6/mqtt_hass_base.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1372 2024-01-26 02:26:35.000000 mqtt-hass-base-4.2.6/mqtt_hass_base.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1219 2024-01-26 02:26:35.000000 mqtt-hass-base-4.2.6/mqtt_hass_base.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-26 02:26:35.000000 mqtt-hass-base-4.2.6/mqtt_hass_base.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-01-26 02:26:35.000000 mqtt-hass-base-4.2.6/mqtt_hass_base.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-01-26 02:26:35.000000 mqtt-hass-base-4.2.6/mqtt_hass_base.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1358 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2600 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/renovate.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 02:26:35.386532 mqtt-hass-base-4.2.6/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/scripts/run-mqtt-docker-for-tests.sh
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-01-26 02:26:35.390533 mqtt-hass-base-4.2.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      240 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-26 02:26:35.390533 mqtt-hass-base-4.2.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)      280 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    11438 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_daemon.py
--rw-rw-rw-   0 root         (0) root         (0)     5973 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_device.py
--rw-rw-rw-   0 root         (0) root         (0)     5103 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_entities_binsensor.py
--rw-rw-rw-   0 root         (0) root         (0)     5223 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_entities_button.py
--rw-rw-rw-   0 root         (0) root         (0)     3265 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_entities_common.py
--rw-rw-rw-   0 root         (0) root         (0)     6256 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_entities_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_entities_lock.py
--rw-rw-rw-   0 root         (0) root         (0)     3957 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_entities_number.py
--rw-rw-rw-   0 root         (0) root         (0)     4006 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_entities_sensor.py
--rw-rw-rw-   0 root         (0) root         (0)     5932 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_entities_switch.py
--rw-rw-rw-   0 root         (0) root         (0)     5010 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tests/test_entities_vacuum.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2024-01-26 02:26:28.000000 mqtt-hass-base-4.2.6/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 03:21:51.097745 mqtt_hass_base-4.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    19948 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-05-10 03:21:51.097745 mqtt_hass_base-4.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)    34804 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt-hass-base.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 03:21:51.093745 mqtt_hass_base-4.3.0/mqtt_hass_base/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/const.py
+-rw-rw-rw-   0 root         (0) root         (0)     9697 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/daemon.py
+-rw-rw-rw-   0 root         (0) root         (0)     8917 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/device.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 03:21:51.093745 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5179 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/binarysensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3976 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/button.py
+-rw-rw-rw-   0 root         (0) root         (0)     6979 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     6100 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/light.py
+-rw-rw-rw-   0 root         (0) root         (0)     5041 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     6063 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/number.py
+-rw-rw-rw-   0 root         (0) root         (0)     4363 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4866 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/switch.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/entity/vacuum.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/error.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/mqtt_hass_base/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 03:21:51.097745 mqtt_hass_base-4.3.0/mqtt_hass_base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-05-10 03:21:51.000000 mqtt_hass_base-4.3.0/mqtt_hass_base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1219 2024-05-10 03:21:51.000000 mqtt_hass_base-4.3.0/mqtt_hass_base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 03:21:51.000000 mqtt_hass_base-4.3.0/mqtt_hass_base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-10 03:21:51.000000 mqtt_hass_base-4.3.0/mqtt_hass_base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-10 03:21:51.000000 mqtt_hass_base-4.3.0/mqtt_hass_base.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     3357 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/renovate.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 03:21:51.093745 mqtt_hass_base-4.3.0/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/scripts/run-mqtt-docker-for-tests.sh
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-10 03:21:51.097745 mqtt_hass_base-4.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 03:21:51.097745 mqtt_hass_base-4.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    11457 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_daemon.py
+-rw-rw-rw-   0 root         (0) root         (0)     5981 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     5104 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_entities_binsensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5224 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_entities_button.py
+-rw-rw-rw-   0 root         (0) root         (0)     3266 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_entities_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     6257 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_entities_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4519 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_entities_lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_entities_number.py
+-rw-rw-rw-   0 root         (0) root         (0)     4007 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_entities_sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_entities_switch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5011 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tests/test_entities_vacuum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2024-05-10 03:21:41.000000 mqtt_hass_base-4.3.0/tox.ini
```

### Comparing `mqtt-hass-base-4.2.6/.gitignore` & `mqtt_hass_base-4.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.6/.gitlab-ci.yml` & `mqtt_hass_base-4.3.0/.gitlab-ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 - test
 - pypi
 
 test:
   stage: test
   tags:
   - $RUNNER_TAG
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20231211100139
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12:latest@sha256:b66812346075aabc0ee6cf452d734c28589bbe97a82c179b0a95d3a95c04ad41
   services:
     - name: eclipse-mosquitto:2.0.18
       alias: mqtt
       entrypoint:
         - "/bin/sh"
       command:
         - -c
@@ -48,15 +48,15 @@
     - if: '$CI_PIPELINE_SOURCE == "merge_request_event"'
       when: never
     - if: '$CI_COMMIT_TAG'
       when: never
     - when: on_success
 
 package:
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20231211100139
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12:latest@sha256:b66812346075aabc0ee6cf452d734c28589bbe97a82c179b0a95d3a95c04ad41
   stage: pypi
   tags:
   - $RUNNER_TAG
   script:
     #- apt-get update && apt-get install -y python3.11 python3-pip python3.11-venv
     - pip install --upgrade pip
     - pip install --upgrade build setuptools_scm
@@ -64,15 +64,15 @@
     - pip install twine
     - python3 -m twine check --strict dist/*
     - TWINE_PASSWORD=${CI_JOB_TOKEN} TWINE_USERNAME=gitlab-ci-token python3 -m twine upload --repository-url ${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi dist/*
   only:
   - master
 
 promote2pypi:
-  image: registry.gitlab.com/hydroqc/hydroqc-base-container/build:20231211100139
+  image: registry.gitlab.com/hydroqc/hydroqc-base-container/3.12:latest@sha256:b66812346075aabc0ee6cf452d734c28589bbe97a82c179b0a95d3a95c04ad41
   stage: pypi
   tags:
   - $RUNNER_TAG
   script:
     # TODO: try to pull the good package from gitlab pypi repo
     #       then change the version (promote)
     #       then push it to pypi
```

### Comparing `mqtt-hass-base-4.2.6/.pre-commit-config.yaml` & `mqtt_hass_base-4.3.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-docstring-first
   - id: check-yaml
   - id: debug-statements
   - id: check-ast
 
 - repo: https://github.com/psf/black
-  rev: 23.12.1
+  rev: 24.4.2
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/PyCQA/flake8/
   rev: 7.0.0
   hooks:
@@ -30,16 +30,16 @@
 
 - repo: https://github.com/PyCQA/doc8
   rev: v1.1.1
   hooks:
   - id: doc8
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v1.8.0
+  rev: v1.10.0
   hooks:
   - id: mypy
     args: [--strict, --pretty, --show-error-codes]
     additional_dependencies:
-      - "aiomqtt==2.0.0"
-      - "pytest-asyncio==0.23.3"
-      - "types-paho-mqtt==1.6.0.20240106"
-      - "homeassistant-stubs==2024.1.5"
+      - "aiomqtt==1.2.1"
+      - "pytest-asyncio==0.23.6"
+      - "types-paho-mqtt==1.6.0.20240321"
+      - "homeassistant-stubs==2024.5.2"
```

### Comparing `mqtt-hass-base-4.2.6/.pylintrc` & `mqtt_hass_base-4.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.6/LICENSE.txt` & `mqtt_hass_base-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.6/PKG-INFO` & `mqtt_hass_base-4.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: mqtt-hass-base
-Version: 4.2.6
+Version: 4.3.0
 Summary: Bases to build mqtt daemon compatible with Home Assistant
 Home-page: https://gitlab.com/ttblt-oss/hass/mqtt-hass-base
 Author-email: Thibault Cohen <titilambert@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://gitlab.com/ttblt-oss/hass/mqtt_hass_base
 Project-URL: Bug Reports, https://gitlab.com/ttblt-oss/hass/mqtt-hass-base/-/issues
 Project-URL: Home-page, https://gitlab.com/ttblt-oss/hass/mqtt_hass_base
 Keywords: homeassistant,mqtt,lib
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11.0
+Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: homeassistant==2024.5.2
+Requires-Dist: aiomqtt==1.2.1
 
 # MQTT HASS BASE
 
 Small python lib to create quickly daemons which interact with HomeAssistant through MQTT.
 
 [![Latest Release](https://gitlab.com/ttblt-hass/mqtt-hass-base/-/badges/release.svg)](https://gitlab.com/ttblt-hass/mqtt-hass-base/-/releases)
 [![pipeline status](https://gitlab.com/ttblt-hass/mqtt-hass-base/badges/master/pipeline.svg)](https://gitlab.com/ttblt-hass/mqtt-hass-base/-/commits/master)
```

### Comparing `mqtt-hass-base-4.2.6/README.md` & `mqtt_hass_base-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.6/mqtt-hass-base.png` & `mqtt_hass_base-4.3.0/mqtt-hass-base.png`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/daemon.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT Daemon Base."""
+
 import asyncio
 import logging
 import os
 import signal
 import uuid
 from contextlib import AsyncExitStack
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/device.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT Hass Base."""
+
 import asyncio
 import logging
 from collections.abc import Callable
 from contextlib import AsyncExitStack
 from typing import Any
 
 import aiomqtt as mqtt
@@ -66,20 +67,22 @@
             entity.set_mqtt_client(mqtt_client)
 
     def add_entity(
         self,
         entity_type: "str",
         name: str,
         unique_id: str,
-        entity_settings: mqtt_entity.BinarySensorSettingsType
-        | mqtt_entity.SensorSettingsType
-        | mqtt_entity.LightSettingsType
-        | mqtt_entity.LockSettingsType
-        | mqtt_entity.SwitchSettingsType
-        | mqtt_entity.VacuumSettingsType,
+        entity_settings: (
+            mqtt_entity.BinarySensorSettingsType
+            | mqtt_entity.SensorSettingsType
+            | mqtt_entity.LightSettingsType
+            | mqtt_entity.LockSettingsType
+            | mqtt_entity.SwitchSettingsType
+            | mqtt_entity.VacuumSettingsType
+        ),
         subscriptions: dict[str, Callable[..., Any]] | None = None,
         sub_mqtt_topic: str | None = None,
     ) -> (
         mqtt_entity.MqttBinarysensor
         | mqtt_entity.MqttLight
         | mqtt_entity.MqttSensor
         | mqtt_entity.MqttSwitch
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/entity/__init__.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/entity/binarysensor.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/entity/binarysensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT Binary sensor entity module."""
+
 import asyncio
 import json
 import logging
 from collections.abc import Callable
 from contextlib import AsyncExitStack
 from typing import Any
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/entity/button.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/entity/button.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT Switch entity module."""
+
 import asyncio
 import json
 import logging
 from collections.abc import Callable
 from contextlib import AsyncExitStack
 from typing import Any
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/entity/common.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/entity/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT base entity module."""
+
 import asyncio
 import json
 import logging
 from collections.abc import AsyncGenerator, Callable
 from contextlib import AsyncExitStack
 from typing import Any, TypedDict
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/entity/light.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/entity/light.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT Light entity module."""
+
 import asyncio
 import json
 import logging
 from collections.abc import Callable
 from contextlib import AsyncExitStack
 from typing import Any
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/entity/lock.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/entity/lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT Lock entity module."""
+
 import asyncio
 import json
 import logging
 from collections.abc import Callable
 from contextlib import AsyncExitStack
 from typing import Any
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/entity/number.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/entity/number.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT Switch entity module."""
+
 import asyncio
 import json
 import logging
 from collections.abc import Callable
 from contextlib import AsyncExitStack
 from typing import Any, Literal
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/entity/sensor.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/entity/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT Sensor entity module."""
+
 import asyncio
 import json
 import logging
 from contextlib import AsyncExitStack
 from typing import Any
 
 import aiomqtt as mqtt
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/entity/switch.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/entity/switch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT Switch entity module."""
+
 import asyncio
 import json
 import logging
 from collections.abc import Callable
 from contextlib import AsyncExitStack
 from typing import Any
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base/entity/vacuum.py` & `mqtt_hass_base-4.3.0/mqtt_hass_base/entity/vacuum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MQTT Vacuum entity module."""
+
 import asyncio
 import json
 import logging
 from collections.abc import Callable
 from contextlib import AsyncExitStack
 from typing import Any
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base.egg-info/PKG-INFO` & `mqtt_hass_base-4.3.0/mqtt_hass_base.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: mqtt-hass-base
-Version: 4.2.6
+Version: 4.3.0
 Summary: Bases to build mqtt daemon compatible with Home Assistant
 Home-page: https://gitlab.com/ttblt-oss/hass/mqtt-hass-base
 Author-email: Thibault Cohen <titilambert@gmail.com>
 License: Apache-2.0
 Project-URL: Source Code, https://gitlab.com/ttblt-oss/hass/mqtt_hass_base
 Project-URL: Bug Reports, https://gitlab.com/ttblt-oss/hass/mqtt-hass-base/-/issues
 Project-URL: Home-page, https://gitlab.com/ttblt-oss/hass/mqtt_hass_base
 Keywords: homeassistant,mqtt,lib
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11.0
+Requires-Python: >=3.12.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: homeassistant==2024.5.2
+Requires-Dist: aiomqtt==1.2.1
 
 # MQTT HASS BASE
 
 Small python lib to create quickly daemons which interact with HomeAssistant through MQTT.
 
 [![Latest Release](https://gitlab.com/ttblt-hass/mqtt-hass-base/-/badges/release.svg)](https://gitlab.com/ttblt-hass/mqtt-hass-base/-/releases)
 [![pipeline status](https://gitlab.com/ttblt-hass/mqtt-hass-base/badges/master/pipeline.svg)](https://gitlab.com/ttblt-hass/mqtt-hass-base/-/commits/master)
```

### Comparing `mqtt-hass-base-4.2.6/mqtt_hass_base.egg-info/SOURCES.txt` & `mqtt_hass_base-4.3.0/mqtt_hass_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mqtt-hass-base-4.2.6/pyproject.toml` & `mqtt_hass_base-4.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
-    "setuptools==65.6.3",
-    "setuptools_scm[toml]==7.1.0",
-    "wheel==0.38.4",
+    "setuptools==69.5.1",
+    "setuptools_scm[toml]==8.1.0",
+    "wheel==0.43.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name        = "mqtt-hass-base"
 #version     = "attr: mqtt_hass_base.__version__.VERSION"
@@ -19,15 +19,15 @@
 ]
 keywords    = ["homeassistant", "mqtt", "lib"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-requires-python = ">=3.11.0"
+requires-python = ">=3.12.0"
 # https://github.com/renovatebot/renovate/issues/10187
 #dependencies    = [
 #    "homeassistant==2022.9.7",
 #    "asyncio-mqtt==0.12.1",
 #]
 
 [project.urls]
```

### Comparing `mqtt-hass-base-4.2.6/renovate.json` & `mqtt_hass_base-4.3.0/renovate.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5574452003023431%*

 * *Differences: {"'customManagers'": "[OrderedDict([('customType', 'regex'), ('fileMatch', "*

 * *                     "['.pre-commit-config.yaml']), ('matchStrings', [' *- "*

 * *                     '"(?<depName>[^\\n=]*?)==(?<currentValue>[v0-9.]*?)"\', \' *- '*

 * *                     '"(?<depName>[^\\n=]*?)==(?<currentValue>[v0-9.]*?)"\\n\']), '*

 * *                     "('datasourceTemplate', 'pypi'), ('versioningTemplate', 'pep440')])]",*

 * * "'dependencyDashboard'": 'True',*

 * * "'packageRules'": "{0: {'matchManagers': {insert: [(7, 'custom […]*

```diff
@@ -1,28 +1,43 @@
 {
     "$schema": "https://docs.renovatebot.com/renovate-schema.json",
     "branchPrefix": "renovate-",
+    "customManagers": [
+        {
+            "customType": "regex",
+            "datasourceTemplate": "pypi",
+            "fileMatch": [
+                ".pre-commit-config.yaml"
+            ],
+            "matchStrings": [
+                " *- \"(?<depName>[^\n=]*?)==(?<currentValue>[v0-9.]*?)\"",
+                " *- \"(?<depName>[^\n=]*?)==(?<currentValue>[v0-9.]*?)\"\n"
+            ],
+            "versioningTemplate": "pep440"
+        }
+    ],
+    "dependencyDashboard": true,
     "packageRules": [
         {
             "automerge": true,
             "groupName": "Python devDependencies - non-major",
             "groupSlug": "python-devdeps-nonmajor",
-            "matchFiles": [
+            "matchFileNames": [
                 "test_requirements.txt",
                 ".pre-commit-config.yaml"
             ],
             "matchManagers": [
                 "pip-compile",
                 "pip_requirements",
                 "pip_setup",
                 "pipenv",
                 "poetry",
                 "pyenv",
                 "setup-cfg",
-                "regex"
+                "custom.regex"
             ],
             "matchUpdateTypes": [
                 "minor",
                 "patch",
                 "pin",
                 "pinDigest",
                 "digest",
@@ -31,37 +46,37 @@
                 "bump"
             ]
         },
         {
             "automerge": false,
             "groupName": "Python devDependencies - major",
             "groupSlug": "python-devdeps-major",
-            "matchFiles": [
+            "matchFileNames": [
                 "test_requirements.txt",
                 ".pre-commit-config.yaml"
             ],
             "matchManagers": [
                 "pip-compile",
                 "pip_requirements",
                 "pip_setup",
                 "pipenv",
                 "poetry",
                 "pyenv",
                 "setup-cfg",
-                "regex"
+                "custom.regex"
             ],
             "matchUpdateTypes": [
                 "major"
             ]
         },
         {
             "automerge": true,
             "groupName": "Python dependencies - non-major",
             "groupSlug": "python-deps-nonmajor",
-            "matchFiles": [
+            "matchFileNames": [
                 "setup.cfg",
                 "pyproject.toml"
             ],
             "matchManagers": [
                 "pip-compile",
                 "pip_requirements",
                 "pip_setup",
@@ -81,15 +96,15 @@
                 "bump"
             ]
         },
         {
             "automerge": false,
             "groupName": "Python dependencies - major",
             "groupSlug": "python-deps-major",
-            "matchFiles": [
+            "matchFileNames": [
                 "setup.cfg",
                 "pyproject.toml"
             ],
             "matchManagers": [
                 "pip-compile",
                 "pip_requirements",
                 "pip_setup",
@@ -130,22 +145,9 @@
             "matchUpdateTypes": [
                 "major"
             ]
         }
     ],
     "pre-commit": {
         "enabled": true
-    },
-    "regexManagers": [
-        {
-            "datasourceTemplate": "pypi",
-            "fileMatch": [
-                ".pre-commit-config.yaml"
-            ],
-            "matchStrings": [
-                " *- \"(?<depName>[^\n=]*?)==(?<currentValue>[v0-9.]*?)\"",
-                " *- \"(?<depName>[^\n=]*?)==(?<currentValue>[v0-9.]*?)\"\n"
-            ],
-            "versioningTemplate": "pep440"
-        }
-    ]
+    }
 }
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_daemon.py` & `mqtt_hass_base-4.3.0/tests/test_daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for MqttClientDaemon."""
+
 import asyncio
 import copy
 import os
 import signal
 import threading
 import traceback
 from collections.abc import AsyncGenerator, Callable
@@ -47,25 +48,25 @@
     if test_step >= 3:
 
         def _read_config(  # pylint: disable=unused-argument
             self: MqttClientDaemon,
         ) -> None:
             pass
 
-        test_fake_daemon.read_config = _read_config  # type: ignore[assignment]
+        test_fake_daemon.read_config = _read_config  # type: ignore[method-assign]
 
     if test_step >= 6:
 
         async def _init_main_loop(  # pylint: disable=unused-argument,invalid-name
             self: MqttClientDaemon,
             stack: AsyncExitStack,
         ) -> None:
             await asyncio.sleep(1)
 
-        test_fake_daemon._init_main_loop = _init_main_loop  # type: ignore[assignment]
+        test_fake_daemon._init_main_loop = _init_main_loop  # type: ignore[method-assign]
     if test_step >= 7:
 
         async def on_messages(
             messages: AsyncGenerator[  # pylint: disable=unused-argument
                 paho.MQTTMessage, None
             ]
         ) -> None:
@@ -80,40 +81,40 @@
             )
 
             task = asyncio.create_task(on_messages(messages))
             self.tasks.add(task)
             await asyncio.gather(*self.tasks)
             self.must_run = False
 
-        test_fake_daemon._main_loop = _main_loop  # type: ignore[assignment]
+        test_fake_daemon._main_loop = _main_loop  # type: ignore[method-assign]
     if test_step >= 8:
 
         async def _loop_stopped(  # pylint: disable=unused-argument,invalid-name
             self: MqttClientDaemon,
         ) -> None:
             pass
 
-        test_fake_daemon._loop_stopped = _loop_stopped  # type: ignore[assignment]
+        test_fake_daemon._loop_stopped = _loop_stopped  # type: ignore[method-assign]
     if test_step >= 9:
 
         async def _on_disconnect(  # pylint: disable=unused-argument,invalid-name
             self: MqttClientDaemon,
         ) -> None:
             pass
 
-        test_fake_daemon._on_disconnect = _on_disconnect  # type: ignore[assignment]
+        test_fake_daemon._on_disconnect = _on_disconnect  # type: ignore[method-assign]
 
     if test_step >= 13:
 
         async def _signal_handler(  # pylint: disable=unused-argument,invalid-name
             self: MqttClientDaemon, sig_name: str
         ) -> None:
             pass
 
-        test_fake_daemon._signal_handler = _signal_handler  # type: ignore[assignment]
+        test_fake_daemon._signal_handler = _signal_handler  # type: ignore[method-assign]
 
     if custom_methods:
         for method_name, func in custom_methods.items():
             setattr(test_fake_daemon, method_name, func)
 
     return test_fake_daemon(*args, **kwargs)
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_device.py` & `mqtt_hass_base-4.3.0/tests/test_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for MqttClientDevice."""
+
 import asyncio
 import logging
 from contextlib import AsyncExitStack
 from typing import cast
 
 import aiomqtt as mqtt
 import paho.mqtt.client as paho
@@ -20,15 +21,15 @@
 class TestBase:
     """Base test class."""
 
     @pytest.mark.asyncio
     async def test_1_main_test(self) -> None:
         """Main test for mqttDevice."""
         async with AsyncExitStack() as stack:
-            mqtt_client = mqtt.Client(
+            mqtt_client = mqtt.client.Client(
                 hostname="127.0.0.1",
                 port=1883,
                 # logger==
                 keepalive=60,
                 client_id="fake_client",
                 username="hass",
                 password="hass",
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_entities_binsensor.py` & `mqtt_hass_base-4.3.0/tests/test_entities_binsensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for binary sensor."""
+
 import json
 import logging
 from contextlib import AsyncExitStack
 from typing import Any
 from unittest.mock import MagicMock
 
 import pytest
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_entities_button.py` & `mqtt_hass_base-4.3.0/tests/test_entities_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for button."""
+
 import json
 import logging
 from contextlib import AsyncExitStack
 from typing import Any
 from unittest.mock import MagicMock
 
 import paho.mqtt.client as paho
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_entities_common.py` & `mqtt_hass_base-4.3.0/tests/test_entities_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for binary sensor."""
+
 import logging
 from contextlib import AsyncExitStack
 from unittest.mock import MagicMock
 
 import pytest
 
 import mqtt_hass_base.error
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_entities_light.py` & `mqtt_hass_base-4.3.0/tests/test_entities_light.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test for light."""
+
 import json
 import logging
 from contextlib import AsyncExitStack
 from typing import Any
 from unittest.mock import MagicMock
 
 import pytest
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_entities_lock.py` & `mqtt_hass_base-4.3.0/tests/test_entities_lock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for lock."""
+
 import json
 import logging
 from contextlib import AsyncExitStack
 from typing import Any
 from unittest.mock import MagicMock
 
 import pytest
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_entities_number.py` & `mqtt_hass_base-4.3.0/tests/test_entities_number.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for number."""
+
 import json
 import logging
 from contextlib import AsyncExitStack
 from typing import Any
 from unittest.mock import MagicMock
 
 import paho.mqtt.client as paho
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_entities_sensor.py` & `mqtt_hass_base-4.3.0/tests/test_entities_sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for sensor."""
+
 import json
 import logging
 from contextlib import AsyncExitStack
 from typing import Any
 from unittest.mock import MagicMock
 
 import pytest
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_entities_switch.py` & `mqtt_hass_base-4.3.0/tests/test_entities_switch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for switch."""
+
 import json
 import logging
 from contextlib import AsyncExitStack
 from typing import Any
 from unittest.mock import MagicMock
 
 import pytest
```

### Comparing `mqtt-hass-base-4.2.6/tests/test_entities_vacuum.py` & `mqtt_hass_base-4.3.0/tests/test_entities_vacuum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for vacuum."""
+
 import json
 import logging
 from contextlib import AsyncExitStack
 from typing import Any
 from unittest.mock import MagicMock
 
 import pytest
```

### Comparing `mqtt-hass-base-4.2.6/tox.ini` & `mqtt_hass_base-4.3.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = pylint,flake8,pydocstyle,typing,black,cov-init,py311,cov-report
+envlist = pylint,flake8,pydocstyle,typing,black,cov-init,py312,cov-report
 skip_missing_interpreters = True
 
 [testenv:pylint]
 basepython = {env:PYTHON3_PATH:python3}
 ignore_errors = True
 deps =
     -r {toxinidir}{/}test_requirements.txt
```

