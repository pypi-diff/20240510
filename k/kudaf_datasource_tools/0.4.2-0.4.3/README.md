# Comparing `tmp/kudaf_datasource_tools-0.4.2.tar.gz` & `tmp/kudaf_datasource_tools-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kudaf_datasource_tools-0.4.2.tar", max compression
+gzip compressed data, was "kudaf_datasource_tools-0.4.3.tar", max compression
```

## Comparing `kudaf_datasource_tools-0.4.2.tar` & `kudaf_datasource_tools-0.4.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1061 2023-12-05 11:39:42.511263 kudaf_datasource_tools-0.4.2/LICENSE.md
--rw-r--r--   0        0        0    18529 2024-03-01 11:23:42.414319 kudaf_datasource_tools-0.4.2/README.md
--rw-r--r--   0        0        0        0 2023-12-05 11:40:29.231315 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 09:03:29.767302 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/config/__init__.py
--rw-r--r--   0        0        0     5062 2024-03-01 11:11:48.733091 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/config/config_example.yaml
--rw-r--r--   0        0        0      387 2024-03-01 11:11:44.601082 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/config/cookiecutter.json
--rw-r--r--   0        0        0      459 2024-03-01 11:21:05.930077 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/config/logger.py
--rw-r--r--   0        0        0        0 2023-11-08 07:56:49.495243 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/__init__.py
--rw-r--r--   0        0        0      679 2023-11-08 07:22:32.796809 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/exceptions.py
--rw-r--r--   0        0        0     7760 2024-03-01 11:12:14.653144 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/models.py
--rw-r--r--   0        0        0    20257 2024-03-01 11:12:48.913212 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/process.py
--rw-r--r--   0        0        0     6383 2024-02-28 10:01:52.874002 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/temporal_attributes.py
--rw-r--r--   0        0        0     2091 2024-02-15 13:55:46.633777 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/FAMILIE.json
--rw-r--r--   0        0        0     1555 2023-12-05 11:45:11.263629 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/FORETAK.json
--rw-r--r--   0        0        0     4202 2023-11-08 07:48:02.359119 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/FYLKE.json
--rw-r--r--   0        0        0     4382 2024-02-15 13:55:46.645777 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/FYLKESKOMMUNE.json
--rw-r--r--   0        0        0     2124 2024-02-15 13:55:46.665777 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/HUSHOLDNING.json
--rw-r--r--   0        0        0     1429 2024-02-15 13:55:46.677777 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/JOBB.json
--rw-r--r--   0        0        0     1378 2024-02-15 13:55:46.693777 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/KJORETOY.json
--rw-r--r--   0        0        0   232459 2023-11-08 07:48:02.363119 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/KOMMUNE.json
--rw-r--r--   0        0        0     1242 2024-02-15 13:55:46.701777 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/KURS.json
--rw-r--r--   0        0        0     1204 2023-11-08 07:48:02.363119 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/PERSON.json
--rw-r--r--   0        0        0     1565 2023-12-05 11:45:55.947678 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/VIRKSOMHET.json
--rw-r--r--   0        0        0     1786 2024-02-15 14:09:00.948286 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/__init__.py
--rw-r--r--   0        0        0     8514 2024-02-28 10:03:02.182068 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/utils.py
--rw-r--r--   0        0        0     6341 2024-03-01 11:27:00.438613 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/main.py
--rw-r--r--   0        0        0        0 2023-12-04 12:27:46.546902 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/__init__.py
--rw-r--r--   0        0        0      387 2024-03-01 11:15:21.941500 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/cookiecutter.json
--rw-r--r--   0        0        0     1324 2022-11-16 11:05:47.019196 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/.gitignore
--rw-r--r--   0        0        0     1249 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/.gitlab-ci.yml
--rw-r--r--   0        0        0      475 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/Dockerfile
--rw-r--r--   0        0        0     2657 2024-03-01 08:31:30.686086 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/README.md
--rw-r--r--   0        0        0        0 2022-11-16 11:05:46.963196 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/__init__.py
--rw-r--r--   0        0        0        0 2022-11-16 11:05:46.975196 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/__init__.py
--rw-r--r--   0        0        0      282 2023-11-29 09:37:11.708321 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/api.py
--rw-r--r--   0        0        0        0 2022-11-16 11:05:46.979196 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/endpoints/__init__.py
--rw-r--r--   0        0        0      863 2023-11-29 09:34:05.136657 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/endpoints/metadata.py
--rw-r--r--   0        0        0     3898 2024-02-26 12:13:42.944339 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/endpoints/variables.py
--rw-r--r--   0        0        0        0 2022-11-16 11:05:46.987196 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/core/__init__.py
--rw-r--r--   0        0        0     1425 2024-03-01 08:36:49.445328 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/core/config.py
--rw-r--r--   0        0        0     5290 2024-02-26 07:29:01.580635 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/core/security.py
--rw-r--r--   0        0        0        0 2023-03-04 11:24:04.394271 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/logic/__init__.py
--rw-r--r--   0        0        0     6822 2024-03-01 10:13:55.910760 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/logic/data.py
--rw-r--r--   0        0        0      487 2023-11-29 09:07:21.739537 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/main.py
--rw-r--r--   0        0        0        0 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/tests/__init__.py
--rw-r--r--   0        0        0      212 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/tests/conftest.py
--rw-r--r--   0        0        0      482 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/tests/test_main.py
--rw-r--r--   0        0        0     3200 2024-02-27 07:56:34.271377 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/utils/utils.py
--rw-r--r--   0        0        0     1784 2023-12-28 12:09:54.558599 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/deployment.yaml
--rw-r--r--   0        0        0       70 2024-02-06 10:33:17.720756 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/files/.gitignore
--rw-r--r--   0        0        0       70 2024-02-06 10:33:35.308697 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/metadata/.gitignore
--rw-r--r--   0        0        0     2442 2024-03-01 08:57:05.132635 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/requirements.txt
--rw-r--r--   0        0        0        0 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/scripts/__init__.py
--rw-r--r--   0        0        0      210 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/scripts/make_test.sh
--rw-r--r--   0        0        0     1550 2024-03-01 11:38:10.893469 kudaf_datasource_tools-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    19963 1970-01-01 00:00:00.000000 kudaf_datasource_tools-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-12-05 11:39:42.511263 kudaf_datasource_tools-0.4.3/LICENSE.md
+-rw-r--r--   0        0        0    18529 2024-03-01 11:23:42.414319 kudaf_datasource_tools-0.4.3/README.md
+-rw-r--r--   0        0        0        0 2023-12-05 11:40:29.231315 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-28 09:03:29.767302 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/config/__init__.py
+-rw-r--r--   0        0        0     5062 2024-03-01 11:11:48.733091 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/config/config_example.yaml
+-rw-r--r--   0        0        0      387 2024-03-01 11:11:44.601082 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/config/cookiecutter.json
+-rw-r--r--   0        0        0      459 2024-03-01 11:21:05.930077 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/config/logger.py
+-rw-r--r--   0        0        0        0 2023-11-08 07:56:49.495243 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/__init__.py
+-rw-r--r--   0        0        0      679 2023-11-08 07:22:32.796809 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/exceptions.py
+-rw-r--r--   0        0        0     7760 2024-03-01 11:12:14.653144 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/models.py
+-rw-r--r--   0        0        0    20555 2024-05-10 13:40:30.616464 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/process.py
+-rw-r--r--   0        0        0     6383 2024-02-28 10:01:52.874002 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/temporal_attributes.py
+-rw-r--r--   0        0        0     2091 2024-02-15 13:55:46.633777 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/FAMILIE.json
+-rw-r--r--   0        0        0     1555 2023-12-05 11:45:11.263629 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/FORETAK.json
+-rw-r--r--   0        0        0     4202 2023-11-08 07:48:02.359119 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/FYLKE.json
+-rw-r--r--   0        0        0     4382 2024-02-15 13:55:46.645777 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/FYLKESKOMMUNE.json
+-rw-r--r--   0        0        0     2124 2024-02-15 13:55:46.665777 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/HUSHOLDNING.json
+-rw-r--r--   0        0        0     1429 2024-02-15 13:55:46.677777 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/JOBB.json
+-rw-r--r--   0        0        0     1378 2024-02-15 13:55:46.693777 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/KJORETOY.json
+-rw-r--r--   0        0        0   232459 2023-11-08 07:48:02.363119 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/KOMMUNE.json
+-rw-r--r--   0        0        0     1242 2024-02-15 13:55:46.701777 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/KURS.json
+-rw-r--r--   0        0        0     1204 2023-11-08 07:48:02.363119 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/PERSON.json
+-rw-r--r--   0        0        0     1565 2023-12-05 11:45:55.947678 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/VIRKSOMHET.json
+-rw-r--r--   0        0        0     1786 2024-02-15 14:09:00.948286 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/__init__.py
+-rw-r--r--   0        0        0     8514 2024-02-28 10:03:02.182068 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/utils.py
+-rw-r--r--   0        0        0     6341 2024-03-01 11:27:00.438613 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/main.py
+-rw-r--r--   0        0        0        0 2023-12-04 12:27:46.546902 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/__init__.py
+-rw-r--r--   0        0        0      387 2024-03-01 11:15:21.941500 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/cookiecutter.json
+-rw-r--r--   0        0        0     1324 2022-11-16 11:05:47.019196 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/.gitignore
+-rw-r--r--   0        0        0     1249 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/.gitlab-ci.yml
+-rw-r--r--   0        0        0      475 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/Dockerfile
+-rw-r--r--   0        0        0     2657 2024-03-01 08:31:30.686086 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/README.md
+-rw-r--r--   0        0        0        0 2022-11-16 11:05:46.963196 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-16 11:05:46.975196 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/__init__.py
+-rw-r--r--   0        0        0      282 2023-11-29 09:37:11.708321 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/api.py
+-rw-r--r--   0        0        0        0 2022-11-16 11:05:46.979196 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/endpoints/__init__.py
+-rw-r--r--   0        0        0      863 2023-11-29 09:34:05.136657 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/endpoints/metadata.py
+-rw-r--r--   0        0        0     3898 2024-02-26 12:13:42.944339 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/endpoints/variables.py
+-rw-r--r--   0        0        0        0 2022-11-16 11:05:46.987196 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/core/__init__.py
+-rw-r--r--   0        0        0     1425 2024-03-01 08:36:49.445328 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/core/config.py
+-rw-r--r--   0        0        0     5290 2024-02-26 07:29:01.580635 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/core/security.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:24:04.394271 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/logic/__init__.py
+-rw-r--r--   0        0        0     6822 2024-03-01 10:13:55.910760 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/logic/data.py
+-rw-r--r--   0        0        0      487 2023-11-29 09:07:21.739537 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/main.py
+-rw-r--r--   0        0        0        0 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/tests/__init__.py
+-rw-r--r--   0        0        0      212 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/tests/conftest.py
+-rw-r--r--   0        0        0      482 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/tests/test_main.py
+-rw-r--r--   0        0        0     3200 2024-02-27 07:56:34.271377 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/utils/utils.py
+-rw-r--r--   0        0        0     1784 2023-12-28 12:09:54.558599 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/deployment.yaml
+-rw-r--r--   0        0        0       70 2024-02-06 10:33:17.720756 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/files/.gitignore
+-rw-r--r--   0        0        0       70 2024-02-06 10:33:35.308697 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/metadata/.gitignore
+-rw-r--r--   0        0        0     2442 2024-03-01 08:57:05.132635 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/requirements.txt
+-rw-r--r--   0        0        0        0 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/scripts/__init__.py
+-rw-r--r--   0        0        0      210 2024-02-14 17:48:58.034907 kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/scripts/make_test.sh
+-rw-r--r--   0        0        0     1550 2024-05-10 13:48:10.084613 kudaf_datasource_tools-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    19963 1970-01-01 00:00:00.000000 kudaf_datasource_tools-0.4.3/PKG-INFO
```

### Comparing `kudaf_datasource_tools-0.4.2/LICENSE.md` & `kudaf_datasource_tools-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/README.md` & `kudaf_datasource_tools-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/config/config_example.yaml` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/config/config_example.yaml`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/exceptions.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/exceptions.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/models.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/models.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/process.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,17 +196,20 @@
         """
         # Identifier Variables: 
         # Could come from pre-defined Global Unit Types or from provided Datasource-specific Unit Types
         ivars = []
         ds_units = []
         for _iv in metadata_input.identifierVariables:
             _utype = _iv.unitType
-            if isinstance(_utype, UnitTypeGlobal) and _utype in unit_type_variables.UNIT_TYPE_VARIABLES:
-                 _ivmodel = self.convert_unit_type_to_identifier(unit_type_variables.get(_utype))
-                 ivars.append(replace_enums(input_dict=_ivmodel.dict(exclude_unset=True)))
+            if not isinstance(_utype, UnitTypeMetadataInput) and \
+                hasattr(_utype, 'value') and \
+                _utype.value in UnitTypeGlobal._member_names_ and \
+                _utype in unit_type_variables.UNIT_TYPE_VARIABLES:
+                _ivmodel = self.convert_unit_type_to_identifier(unit_type_variables.get(_utype))
+                ivars.append(replace_enums(input_dict=_ivmodel.dict(exclude_unset=True)))
             elif isinstance(_utype, UnitTypeMetadataInput):
                 # This is a datasource-specific UnitType
                 # First create an Identifier Variable out of it (an InstanceVariable)
                 if isinstance(_iv.unitType.name, str):
                     # Extract if string before converting to dicts
                     _label = _iv.unitType.name
                 else:
@@ -261,15 +264,18 @@
             insert_measure["label"] = _mvdict["label"]
             insert_measure["description"] = _mvdict["description"] if isinstance(_mvdict["description"], list) else [
                             convert_to_multilingual_dict(input_str=_mvdict["description"], default_lang="no")
                         ]
             insert_measure["variableRole"] = "Measure"
 
             if _utype:
-                if isinstance(_utype, UnitTypeGlobal) and _utype in unit_type_variables.UNIT_TYPE_VARIABLES:
+                if not isinstance(_utype, UnitTypeMetadataInput) and \
+                    hasattr(_utype, 'value') and \
+                    _utype.value in UnitTypeGlobal._member_names_ and \
+                    _utype in unit_type_variables.UNIT_TYPE_VARIABLES:
                     utmodel = UnitTypeMetadataInput(**unit_type_variables.get(_utype))
                 elif isinstance(_utype, dict):
                     utmodel = UnitTypeMetadataInput(**_utype)
                     utmodel = unittype_to_multilingual(utype=utmodel, default_lang="no")
                 elif type(_utype) not in [str, UnitTypeMetadataInput]:
                     log_console.log(f"UNIT TYPE: {_utype} NOT FOUND")
                     raise UnregisteredUnitTypeError
```

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/temporal_attributes.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/temporal_attributes.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/FAMILIE.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/FAMILIE.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/FORETAK.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/FORETAK.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/FYLKE.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/FYLKE.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/FYLKESKOMMUNE.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/FYLKESKOMMUNE.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/HUSHOLDNING.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/HUSHOLDNING.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/JOBB.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/JOBB.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/KJORETOY.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/KJORETOY.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/KOMMUNE.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/KOMMUNE.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/KURS.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/KURS.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/PERSON.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/PERSON.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/VIRKSOMHET.json` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/VIRKSOMHET.json`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/unit_type_variables/__init__.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/unit_type_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/logic/utils.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/logic/utils.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/main.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/main.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/.gitignore` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/.gitignore`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/.gitlab-ci.yml` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/README.md` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/README.md`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/endpoints/metadata.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/endpoints/metadata.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/endpoints/variables.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/api/endpoints/variables.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/core/config.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/core/config.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/core/security.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/core/security.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/logic/data.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/logic/data.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/utils/utils.py` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/app/utils/utils.py`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/deployment.yaml` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/requirements.txt` & `kudaf_datasource_tools-0.4.3/kudaf_datasource_tools/template_api/{{cookiecutter.module_name}}/requirements.txt`

 * *Files identical despite different names*

### Comparing `kudaf_datasource_tools-0.4.2/pyproject.toml` & `kudaf_datasource_tools-0.4.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kudaf_datasource_tools"
-version = "0.4.2"
+version = "0.4.3"
 description = "CLI tools for the creation of Kudaf Data Source components: 1) Variables Metadata, and 2) REST API Datasource back-end"
 authors = ["Daniel Díguele,  Sikt - Kunnskapssektorens tjenesteleverandør  <daniel.diguele@sikt.no>"]
 maintainers = ["Daniel Díguele,  Sikt - Kunnskapssektorens tjenesteleverandør  <daniel.diguele@sikt.no>"]
 repository = "https://gitlab.sikt.no/kudaf/kudaf-datasource-tools"
 license = "MIT License"
 readme = "README.md"
 classifiers = [
```

### Comparing `kudaf_datasource_tools-0.4.2/PKG-INFO` & `kudaf_datasource_tools-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kudaf_datasource_tools
-Version: 0.4.2
+Version: 0.4.3
 Summary: CLI tools for the creation of Kudaf Data Source components: 1) Variables Metadata, and 2) REST API Datasource back-end
 Home-page: https://gitlab.sikt.no/kudaf/kudaf-datasource-tools
 License: MIT
 Author: Daniel Díguele,  Sikt - Kunnskapssektorens tjenesteleverandør 
 Author-email: daniel.diguele@sikt.no
 Maintainer: Daniel Díguele,  Sikt - Kunnskapssektorens tjenesteleverandør 
 Maintainer-email: daniel.diguele@sikt.no
```

