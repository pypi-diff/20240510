# Comparing `tmp/fake_py-0.6.8.tar.gz` & `tmp/fake_py-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fake_py-0.6.8.tar", last modified: Mon May  6 22:26:42 2024, max compression
+gzip compressed data, was "fake_py-0.6.9.tar", last modified: Thu May  9 23:03:41 2024, max compression
```

## Comparing `fake_py-0.6.8.tar` & `fake_py-0.6.9.tar`

### file list

```diff
@@ -1,189 +1,190 @@
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.474301 fake_py-0.6.8/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-17 15:38:13.000000 fake_py-0.6.8/.coveralls.yml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-17 15:38:13.000000 fake_py-0.6.8/.env
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/.github/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.450301 fake_py-0.6.8/.github/workflows/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    11430 2023-12-11 23:32:41.000000 fake_py-0.6.8/.github/workflows/test.yml
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      625 2024-05-06 22:26:08.000000 fake_py-0.6.8/.gitignore
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1422 2023-11-24 22:03:33.000000 fake_py-0.6.8/.pre-commit-config.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      361 2022-12-27 21:29:13.000000 fake_py-0.6.8/.pre-commit-hooks.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1020 2023-11-24 23:49:27.000000 fake_py-0.6.8/.readthedocs.yaml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2588 2024-05-06 22:26:08.000000 fake_py-0.6.8/.secrets.baseline
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2588 2024-05-06 22:26:08.000000 fake_py-0.6.8/CHANGELOG.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5397 2023-12-01 00:01:18.000000 fake_py-0.6.8/CODE_OF_CONDUCT.md
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5397 2023-12-01 00:01:18.000000 fake_py-0.6.8/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4070 2023-12-11 23:32:41.000000 fake_py-0.6.8/CONTRIBUTING.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1073 2023-11-01 19:30:30.000000 fake_py-0.6.8/LICENSE
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4495 2024-05-06 22:26:08.000000 fake_py-0.6.8/Makefile
--rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    13524 2024-05-06 22:26:42.474301 fake_py-0.6.8/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    11443 2024-05-06 22:26:08.000000 fake_py-0.6.8/README.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1378 2023-12-09 00:44:20.000000 fake_py-0.6.8/SECURITY.md
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1378 2023-12-09 00:44:20.000000 fake_py-0.6.8/SECURITY.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)   146229 2024-05-06 22:26:08.000000 fake_py-0.6.8/__copy_fake.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.454301 fake_py-0.6.8/docs/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      634 2023-11-25 21:31:30.000000 fake_py-0.6.8/docs/Makefile
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.454301 fake_py-0.6.8/docs/_static/examples/creating_docx/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       50 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_bytes_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       87 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_bytes_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       62 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_bytes_3.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       54 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_file_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       91 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_file_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       66 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_docx/docx_file_3.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.454301 fake_py-0.6.8/docs/_static/examples/creating_images/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       48 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_images/png_bytes_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       86 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_images/png_bytes_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       52 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_images/png_file_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       90 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_images/png_file_2.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/creating_pdf/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       98 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/graphic_pdf_bytes_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      112 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/graphic_pdf_bytes_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      102 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/graphic_pdf_file_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      116 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/graphic_pdf_file_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       92 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_bytes_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      131 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_bytes_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      106 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_bytes_3.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       96 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_file_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      135 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_file_2.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      110 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_file_3.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      241 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_file_django_1.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      308 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/_static/examples/creating_pdf/text_pdf_file_pydantic_1.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/factories/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/factories/dataclasses/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/dataclasses/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2907 2023-12-17 23:22:17.000000 fake_py-0.6.8/docs/_static/examples/factories/dataclasses/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1273 2023-12-17 23:21:49.000000 fake_py-0.6.8/docs/_static/examples/factories/dataclasses/article/models.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/factories/django/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/django/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4517 2023-12-17 23:22:17.000000 fake_py-0.6.8/docs/_static/examples/factories/django/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      835 2024-01-10 21:32:55.000000 fake_py-0.6.8/docs/_static/examples/factories/django/article/models.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/factories/pydantic/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/pydantic/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2651 2023-12-17 23:22:17.000000 fake_py-0.6.8/docs/_static/examples/factories/pydantic/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1926 2023-12-17 23:21:49.000000 fake_py-0.6.8/docs/_static/examples/factories/pydantic/article/models.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3652 2023-12-21 20:14:56.000000 fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2636 2023-12-17 23:21:49.000000 fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      425 2023-12-11 23:32:41.000000 fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/config.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.442301 fake_py-0.6.8/docs/_static/examples/factories/tortoise/
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/docs/_static/examples/factories/tortoise/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2792 2023-12-17 23:22:17.000000 fake_py-0.6.8/docs/_static/examples/factories/tortoise/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1895 2023-12-17 23:21:49.000000 fake_py-0.6.8/docs/_static/examples/factories/tortoise/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-17 15:38:13.000000 fake_py-0.6.8/docs/changelog.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       36 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/code_of_conduct.rst
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2728 2024-05-06 22:26:08.000000 fake_py-0.6.8/docs/conf.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     9004 2023-11-25 21:22:55.000000 fake_py-0.6.8/docs/conf.py.distrib
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       33 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/contributor_guidelines.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2377 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/creating_docx.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2151 2023-12-04 20:42:03.000000 fake_py-0.6.8/docs/creating_images.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4102 2023-12-03 00:58:59.000000 fake_py-0.6.8/docs/creating_pdf.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6175 2024-05-06 22:26:08.000000 fake_py-0.6.8/docs/customization.rst
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      302 2023-12-07 00:03:15.000000 fake_py-0.6.8/docs/documentation.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5816 2023-12-17 23:22:17.000000 fake_py-0.6.8/docs/factories.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      100 2023-11-25 00:03:04.000000 fake_py-0.6.8/docs/fake.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2023-11-25 21:31:30.000000 fake_py-0.6.8/docs/index.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-17 15:38:13.000000 fake_py-0.6.8/docs/index.rst.distrib
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      800 2023-11-25 21:31:30.000000 fake_py-0.6.8/docs/make.bat
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      149 2023-11-25 21:27:34.000000 fake_py-0.6.8/docs/package.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    14518 2024-01-15 21:54:25.000000 fake_py-0.6.8/docs/recipes.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5380 2024-05-06 22:26:08.000000 fake_py-0.6.8/docs/requirements.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2023-12-01 00:01:18.000000 fake_py-0.6.8/docs/security.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/examples/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      357 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.458301 fake_py-0.6.8/examples/customization/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      219 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/customization/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/customization/address/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/customization/address/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1469 2023-12-09 22:54:37.000000 fake_py-0.6.8/examples/customization/address/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      590 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/customization/address/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1592 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/address/tests.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/customization/band/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/band/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      402 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/band/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      291 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/band/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      725 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/band/tests.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4291 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/customization/data.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1529 2023-12-09 22:54:37.000000 fake_py-0.6.8/examples/customization/fake_address.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1145 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/fake_band.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      955 2023-12-09 00:44:20.000000 fake_py-0.6.8/examples/customization/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      719 2023-12-09 22:54:37.000000 fake_py-0.6.8/examples/customization/override_default_data.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/dataclasses/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      131 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/dataclasses/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/dataclasses/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-03 00:58:59.000000 fake_py-0.6.8/examples/dataclasses/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2907 2023-12-17 23:22:17.000000 fake_py-0.6.8/examples/dataclasses/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1273 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/dataclasses/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1925 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/dataclasses/article/tests.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-06 00:04:22.000000 fake_py-0.6.8/examples/dataclasses/manage.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/django/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       87 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/django/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/django/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      303 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/article/admin.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      146 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/article/apps.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4517 2023-12-17 23:22:17.000000 fake_py-0.6.8/examples/django/article/factories.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.462301 fake_py-0.6.8/examples/django/article/migrations/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1725 2023-12-17 23:22:17.000000 fake_py-0.6.8/examples/django/article/migrations/0001_initial.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/article/migrations/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      835 2024-01-10 21:32:55.000000 fake_py-0.6.8/examples/django/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3312 2023-12-16 00:28:30.000000 fake_py-0.6.8/examples/django/article/tests.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/django/blog/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/blog/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      385 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/blog/asgi.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3389 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/blog/settings.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      914 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/blog/urls.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      385 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/django/blog/wsgi.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      726 2023-12-06 00:04:22.000000 fake_py-0.6.8/examples/django/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       14 2023-12-11 23:32:41.000000 fake_py-0.6.8/examples/django/requirements.in
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/hypothesis/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       96 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/hypothesis/README.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      948 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/hypothesis/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/hypothesis/requirements.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     8548 2023-12-08 00:35:23.000000 fake_py-0.6.8/examples/hypothesis/tests.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/lazyfuzzy/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      199 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/lazyfuzzy/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/lazyfuzzy/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-13 00:06:45.000000 fake_py-0.6.8/examples/lazyfuzzy/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2507 2023-12-13 00:47:49.000000 fake_py-0.6.8/examples/lazyfuzzy/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      976 2023-12-13 00:47:49.000000 fake_py-0.6.8/examples/lazyfuzzy/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1674 2023-12-13 00:47:49.000000 fake_py-0.6.8/examples/lazyfuzzy/article/tests.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-13 00:06:45.000000 fake_py-0.6.8/examples/lazyfuzzy/manage.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/pydantic/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/pydantic/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/pydantic/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/pydantic/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2651 2023-12-17 23:22:17.000000 fake_py-0.6.8/examples/pydantic/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1926 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/pydantic/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1925 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/pydantic/article/tests.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-06 00:04:22.000000 fake_py-0.6.8/examples/pydantic/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        9 2023-12-07 00:03:15.000000 fake_py-0.6.8/examples/pydantic/requirements.in
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.466301 fake_py-0.6.8/examples/sqlalchemy/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      100 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/sqlalchemy/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.470301 fake_py-0.6.8/examples/sqlalchemy/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-11 23:32:41.000000 fake_py-0.6.8/examples/sqlalchemy/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3652 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/sqlalchemy/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2636 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/sqlalchemy/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1299 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/sqlalchemy/article/tests.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      425 2023-12-11 23:32:41.000000 fake_py-0.6.8/examples/sqlalchemy/config.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1070 2023-12-11 23:32:41.000000 fake_py-0.6.8/examples/sqlalchemy/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2023-12-11 23:32:41.000000 fake_py-0.6.8/examples/sqlalchemy/requirements.in
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.470301 fake_py-0.6.8/examples/tortoise/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      107 2023-12-21 20:14:56.000000 fake_py-0.6.8/examples/tortoise/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.470301 fake_py-0.6.8/examples/tortoise/article/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.8/examples/tortoise/article/__init__.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2792 2023-12-17 23:22:17.000000 fake_py-0.6.8/examples/tortoise/article/factories.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1895 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/tortoise/article/models.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4082 2023-12-17 23:21:49.000000 fake_py-0.6.8/examples/tortoise/article/tests.py
--rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1350 2023-12-06 00:04:22.000000 fake_py-0.6.8/examples/tortoise/manage.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       13 2023-12-07 00:03:15.000000 fake_py-0.6.8/examples/tortoise/requirements.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)   146229 2024-05-06 22:26:08.000000 fake_py-0.6.8/fake.py
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-06 22:26:42.470301 fake_py-0.6.8/fake.py.egg-info/
--rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    13524 2024-05-06 22:26:42.000000 fake_py-0.6.8/fake.py.egg-info/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5145 2024-05-06 22:26:42.000000 fake_py-0.6.8/fake.py.egg-info/SOURCES.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2024-05-06 22:26:42.000000 fake_py-0.6.8/fake.py.egg-info/dependency_links.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      200 2024-05-06 22:26:42.000000 fake_py-0.6.8/fake.py.egg-info/requires.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        5 2024-05-06 22:26:42.000000 fake_py-0.6.8/fake.py.egg-info/top_level.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3957 2024-05-06 22:26:08.000000 fake_py-0.6.8/pyproject.toml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       38 2024-05-06 22:26:42.474301 fake_py-0.6.8/setup.cfg
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.045862 fake_py-0.6.9/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2022-12-17 15:38:13.000000 fake_py-0.6.9/.coveralls.yml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       34 2022-12-17 15:38:13.000000 fake_py-0.6.9/.env
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.009862 fake_py-0.6.9/.github/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.021862 fake_py-0.6.9/.github/workflows/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    11430 2023-12-11 23:32:41.000000 fake_py-0.6.9/.github/workflows/test.yml
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      625 2024-05-06 22:26:08.000000 fake_py-0.6.9/.gitignore
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1422 2023-11-24 22:03:33.000000 fake_py-0.6.9/.pre-commit-config.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      361 2022-12-27 21:29:13.000000 fake_py-0.6.9/.pre-commit-hooks.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1020 2023-11-24 23:49:27.000000 fake_py-0.6.9/.readthedocs.yaml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2588 2024-05-06 22:26:08.000000 fake_py-0.6.9/.secrets.baseline
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2695 2024-05-09 23:02:30.000000 fake_py-0.6.9/CHANGELOG.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5397 2023-12-01 00:01:18.000000 fake_py-0.6.9/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5397 2023-12-01 00:01:18.000000 fake_py-0.6.9/CODE_OF_CONDUCT.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4070 2023-12-11 23:32:41.000000 fake_py-0.6.9/CONTRIBUTING.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1073 2023-11-01 19:30:30.000000 fake_py-0.6.9/LICENSE
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4497 2024-05-09 23:02:30.000000 fake_py-0.6.9/Makefile
+-rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    13669 2024-05-09 23:03:41.045862 fake_py-0.6.9/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    11503 2024-05-09 23:02:30.000000 fake_py-0.6.9/README.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1378 2023-12-09 00:44:20.000000 fake_py-0.6.9/SECURITY.md
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1378 2023-12-09 00:44:20.000000 fake_py-0.6.9/SECURITY.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)   146377 2024-05-09 23:02:30.000000 fake_py-0.6.9/__copy_fake.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1407 2024-05-09 23:02:30.000000 fake_py-0.6.9/conftest.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.025862 fake_py-0.6.9/docs/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      634 2023-11-25 21:31:30.000000 fake_py-0.6.9/docs/Makefile
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.009862 fake_py-0.6.9/docs/_static/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.009862 fake_py-0.6.9/docs/_static/examples/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.025862 fake_py-0.6.9/docs/_static/examples/creating_docx/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       50 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_docx/docx_bytes_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       87 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_docx/docx_bytes_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       62 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_docx/docx_bytes_3.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       54 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_docx/docx_file_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       91 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_docx/docx_file_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       66 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_docx/docx_file_3.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.025862 fake_py-0.6.9/docs/_static/examples/creating_images/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       48 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_images/png_bytes_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       86 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_images/png_bytes_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       52 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_images/png_file_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       90 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_images/png_file_2.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.029862 fake_py-0.6.9/docs/_static/examples/creating_pdf/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       98 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/graphic_pdf_bytes_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      112 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/graphic_pdf_bytes_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      102 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/graphic_pdf_file_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      116 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/graphic_pdf_file_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       92 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/text_pdf_bytes_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      131 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/text_pdf_bytes_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      106 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/text_pdf_bytes_3.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       96 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/text_pdf_file_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      135 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/text_pdf_file_2.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      110 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/text_pdf_file_3.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      241 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/text_pdf_file_django_1.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      308 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/_static/examples/creating_pdf/text_pdf_file_pydantic_1.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.009862 fake_py-0.6.9/docs/_static/examples/factories/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.009862 fake_py-0.6.9/docs/_static/examples/factories/dataclasses/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.029862 fake_py-0.6.9/docs/_static/examples/factories/dataclasses/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2907 2023-12-17 23:22:17.000000 fake_py-0.6.9/docs/_static/examples/factories/dataclasses/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1273 2023-12-17 23:21:49.000000 fake_py-0.6.9/docs/_static/examples/factories/dataclasses/article/models.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.009862 fake_py-0.6.9/docs/_static/examples/factories/django/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.029862 fake_py-0.6.9/docs/_static/examples/factories/django/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4517 2023-12-17 23:22:17.000000 fake_py-0.6.9/docs/_static/examples/factories/django/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      835 2024-01-10 21:32:55.000000 fake_py-0.6.9/docs/_static/examples/factories/django/article/models.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.009862 fake_py-0.6.9/docs/_static/examples/factories/pydantic/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.029862 fake_py-0.6.9/docs/_static/examples/factories/pydantic/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2651 2023-12-17 23:22:17.000000 fake_py-0.6.9/docs/_static/examples/factories/pydantic/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1926 2023-12-17 23:21:49.000000 fake_py-0.6.9/docs/_static/examples/factories/pydantic/article/models.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.029862 fake_py-0.6.9/docs/_static/examples/factories/sqlalchemy/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.029862 fake_py-0.6.9/docs/_static/examples/factories/sqlalchemy/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3652 2023-12-21 20:14:56.000000 fake_py-0.6.9/docs/_static/examples/factories/sqlalchemy/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2636 2023-12-17 23:21:49.000000 fake_py-0.6.9/docs/_static/examples/factories/sqlalchemy/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      425 2023-12-11 23:32:41.000000 fake_py-0.6.9/docs/_static/examples/factories/sqlalchemy/config.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.009862 fake_py-0.6.9/docs/_static/examples/factories/tortoise/
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.029862 fake_py-0.6.9/docs/_static/examples/factories/tortoise/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2792 2023-12-17 23:22:17.000000 fake_py-0.6.9/docs/_static/examples/factories/tortoise/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1895 2023-12-17 23:21:49.000000 fake_py-0.6.9/docs/_static/examples/factories/tortoise/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       30 2022-12-17 15:38:13.000000 fake_py-0.6.9/docs/changelog.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       36 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/code_of_conduct.rst
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2728 2024-05-06 22:26:08.000000 fake_py-0.6.9/docs/conf.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     9004 2023-11-25 21:22:55.000000 fake_py-0.6.9/docs/conf.py.distrib
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       33 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/contributor_guidelines.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2377 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/creating_docx.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2151 2023-12-04 20:42:03.000000 fake_py-0.6.9/docs/creating_images.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4102 2023-12-03 00:58:59.000000 fake_py-0.6.9/docs/creating_pdf.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6175 2024-05-06 22:26:08.000000 fake_py-0.6.9/docs/customization.rst
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      302 2023-12-07 00:03:15.000000 fake_py-0.6.9/docs/documentation.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5816 2023-12-17 23:22:17.000000 fake_py-0.6.9/docs/factories.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      100 2023-11-25 00:03:04.000000 fake_py-0.6.9/docs/fake.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2023-11-25 21:31:30.000000 fake_py-0.6.9/docs/index.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       58 2022-12-17 15:38:13.000000 fake_py-0.6.9/docs/index.rst.distrib
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      800 2023-11-25 21:31:30.000000 fake_py-0.6.9/docs/make.bat
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      149 2023-11-25 21:27:34.000000 fake_py-0.6.9/docs/package.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    23619 2024-05-09 23:02:30.000000 fake_py-0.6.9/docs/recipes.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4935 2024-05-09 23:02:30.000000 fake_py-0.6.9/docs/requirements.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       29 2023-12-01 00:01:18.000000 fake_py-0.6.9/docs/security.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.029862 fake_py-0.6.9/examples/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      357 2023-12-21 20:14:56.000000 fake_py-0.6.9/examples/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.033862 fake_py-0.6.9/examples/customization/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      219 2023-12-21 20:14:56.000000 fake_py-0.6.9/examples/customization/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.033862 fake_py-0.6.9/examples/customization/address/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-08 00:35:23.000000 fake_py-0.6.9/examples/customization/address/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1469 2023-12-09 22:54:37.000000 fake_py-0.6.9/examples/customization/address/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      590 2023-12-08 00:35:23.000000 fake_py-0.6.9/examples/customization/address/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1592 2023-12-09 00:44:20.000000 fake_py-0.6.9/examples/customization/address/tests.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.033862 fake_py-0.6.9/examples/customization/band/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-09 00:44:20.000000 fake_py-0.6.9/examples/customization/band/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      402 2023-12-09 00:44:20.000000 fake_py-0.6.9/examples/customization/band/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      291 2023-12-09 00:44:20.000000 fake_py-0.6.9/examples/customization/band/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      725 2023-12-09 00:44:20.000000 fake_py-0.6.9/examples/customization/band/tests.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4291 2023-12-08 00:35:23.000000 fake_py-0.6.9/examples/customization/data.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1529 2023-12-09 22:54:37.000000 fake_py-0.6.9/examples/customization/fake_address.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1145 2023-12-09 00:44:20.000000 fake_py-0.6.9/examples/customization/fake_band.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      955 2023-12-09 00:44:20.000000 fake_py-0.6.9/examples/customization/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      719 2023-12-09 22:54:37.000000 fake_py-0.6.9/examples/customization/override_default_data.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.033862 fake_py-0.6.9/examples/dataclasses/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      131 2023-12-21 20:14:56.000000 fake_py-0.6.9/examples/dataclasses/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.033862 fake_py-0.6.9/examples/dataclasses/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-03 00:58:59.000000 fake_py-0.6.9/examples/dataclasses/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2907 2023-12-17 23:22:17.000000 fake_py-0.6.9/examples/dataclasses/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1273 2023-12-17 23:21:49.000000 fake_py-0.6.9/examples/dataclasses/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1925 2023-12-17 23:21:49.000000 fake_py-0.6.9/examples/dataclasses/article/tests.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-06 00:04:22.000000 fake_py-0.6.9/examples/dataclasses/manage.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.033862 fake_py-0.6.9/examples/django/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       87 2023-12-21 20:14:56.000000 fake_py-0.6.9/examples/django/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.037862 fake_py-0.6.9/examples/django/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/django/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      303 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/django/article/admin.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      146 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/django/article/apps.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4517 2023-12-17 23:22:17.000000 fake_py-0.6.9/examples/django/article/factories.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.037862 fake_py-0.6.9/examples/django/article/migrations/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1725 2023-12-17 23:22:17.000000 fake_py-0.6.9/examples/django/article/migrations/0001_initial.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/django/article/migrations/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      835 2024-01-10 21:32:55.000000 fake_py-0.6.9/examples/django/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3312 2023-12-16 00:28:30.000000 fake_py-0.6.9/examples/django/article/tests.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.037862 fake_py-0.6.9/examples/django/blog/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/django/blog/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      385 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/django/blog/asgi.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3389 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/django/blog/settings.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      914 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/django/blog/urls.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      385 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/django/blog/wsgi.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      726 2023-12-06 00:04:22.000000 fake_py-0.6.9/examples/django/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       14 2023-12-11 23:32:41.000000 fake_py-0.6.9/examples/django/requirements.in
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.037862 fake_py-0.6.9/examples/hypothesis/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       96 2023-12-21 20:14:56.000000 fake_py-0.6.9/examples/hypothesis/README.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      948 2023-12-08 00:35:23.000000 fake_py-0.6.9/examples/hypothesis/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2023-12-08 00:35:23.000000 fake_py-0.6.9/examples/hypothesis/requirements.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     8548 2023-12-08 00:35:23.000000 fake_py-0.6.9/examples/hypothesis/tests.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.037862 fake_py-0.6.9/examples/lazyfuzzy/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      199 2023-12-21 20:14:56.000000 fake_py-0.6.9/examples/lazyfuzzy/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.037862 fake_py-0.6.9/examples/lazyfuzzy/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-13 00:06:45.000000 fake_py-0.6.9/examples/lazyfuzzy/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2507 2023-12-13 00:47:49.000000 fake_py-0.6.9/examples/lazyfuzzy/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      976 2023-12-13 00:47:49.000000 fake_py-0.6.9/examples/lazyfuzzy/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1674 2023-12-13 00:47:49.000000 fake_py-0.6.9/examples/lazyfuzzy/article/tests.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-13 00:06:45.000000 fake_py-0.6.9/examples/lazyfuzzy/manage.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.037862 fake_py-0.6.9/examples/pydantic/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       97 2023-12-21 20:14:56.000000 fake_py-0.6.9/examples/pydantic/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.041862 fake_py-0.6.9/examples/pydantic/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/pydantic/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2651 2023-12-17 23:22:17.000000 fake_py-0.6.9/examples/pydantic/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1926 2023-12-17 23:21:49.000000 fake_py-0.6.9/examples/pydantic/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1925 2023-12-17 23:21:49.000000 fake_py-0.6.9/examples/pydantic/article/tests.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      956 2023-12-06 00:04:22.000000 fake_py-0.6.9/examples/pydantic/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        9 2023-12-07 00:03:15.000000 fake_py-0.6.9/examples/pydantic/requirements.in
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.041862 fake_py-0.6.9/examples/sqlalchemy/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      100 2023-12-21 20:14:56.000000 fake_py-0.6.9/examples/sqlalchemy/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.041862 fake_py-0.6.9/examples/sqlalchemy/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-11 23:32:41.000000 fake_py-0.6.9/examples/sqlalchemy/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     3652 2023-12-21 20:14:56.000000 fake_py-0.6.9/examples/sqlalchemy/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2636 2023-12-17 23:21:49.000000 fake_py-0.6.9/examples/sqlalchemy/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1299 2023-12-17 23:21:49.000000 fake_py-0.6.9/examples/sqlalchemy/article/tests.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      425 2023-12-11 23:32:41.000000 fake_py-0.6.9/examples/sqlalchemy/config.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1070 2023-12-11 23:32:41.000000 fake_py-0.6.9/examples/sqlalchemy/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       11 2023-12-11 23:32:41.000000 fake_py-0.6.9/examples/sqlalchemy/requirements.in
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.041862 fake_py-0.6.9/examples/tortoise/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      107 2023-12-21 20:14:56.000000 fake_py-0.6.9/examples/tortoise/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.041862 fake_py-0.6.9/examples/tortoise/article/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-12-01 00:01:18.000000 fake_py-0.6.9/examples/tortoise/article/__init__.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2792 2023-12-17 23:22:17.000000 fake_py-0.6.9/examples/tortoise/article/factories.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1895 2023-12-17 23:21:49.000000 fake_py-0.6.9/examples/tortoise/article/models.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4082 2023-12-17 23:21:49.000000 fake_py-0.6.9/examples/tortoise/article/tests.py
+-rwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1350 2023-12-06 00:04:22.000000 fake_py-0.6.9/examples/tortoise/manage.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       13 2023-12-07 00:03:15.000000 fake_py-0.6.9/examples/tortoise/requirements.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)   146377 2024-05-09 23:02:30.000000 fake_py-0.6.9/fake.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2024-05-09 23:03:41.041862 fake_py-0.6.9/fake.py.egg-info/
+-rw-r--r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    13669 2024-05-09 23:03:40.000000 fake_py-0.6.9/fake.py.egg-info/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     5157 2024-05-09 23:03:41.000000 fake_py-0.6.9/fake.py.egg-info/SOURCES.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2024-05-09 23:03:40.000000 fake_py-0.6.9/fake.py.egg-info/dependency_links.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      221 2024-05-09 23:03:40.000000 fake_py-0.6.9/fake.py.egg-info/requires.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        5 2024-05-09 23:03:40.000000 fake_py-0.6.9/fake.py.egg-info/top_level.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4072 2024-05-09 23:02:30.000000 fake_py-0.6.9/pyproject.toml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       38 2024-05-09 23:03:41.045862 fake_py-0.6.9/setup.cfg
```

### Comparing `fake_py-0.6.8/.github/workflows/test.yml` & `fake_py-0.6.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/.gitignore` & `fake_py-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/.pre-commit-config.yaml` & `fake_py-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/.readthedocs.yaml` & `fake_py-0.6.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/.secrets.baseline` & `fake_py-0.6.9/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/CHANGELOG.rst` & `fake_py-0.6.9/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 - It's always safe to upgrade within the same minor version (for example, from
   0.3 to 0.3.4).
 - Minor version changes might be backwards incompatible. Read the
   release notes carefully before upgrading (for example, when upgrading from
   0.3.4 to 0.4).
 - All backwards incompatible changes are mentioned in this document.
 
+0.6.9
+-----
+2024-05-10
+
+- Minor fixes in ``pdf_file`` and ``docx_file`` providers.
+- Minor fixes in docs.
+
 0.6.8
 -----
 2024-05-06
 
 - Minor fixes in docs.
 
 0.6.7
```

### Comparing `fake_py-0.6.8/CODE_OF_CONDUCT.md` & `fake_py-0.6.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/CODE_OF_CONDUCT.rst` & `fake_py-0.6.9/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/CONTRIBUTING.rst` & `fake_py-0.6.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/LICENSE` & `fake_py-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/Makefile` & `fake_py-0.6.9/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -138,18 +138,18 @@
 	rm -rf .coverage
 	rm -rf .pytest_cache/
 	rm -rf .mypy_cache/
 	rm -rf .ruff_cache/
 	rm -rf dist/
 
 compile-requirements:
-	source $(VENV) && python -m piptools compile --extra all -o docs/requirements.txt pyproject.toml
+	source $(VENV) && python -m piptools compile --all-extras -o docs/requirements.txt pyproject.toml
 
 compile-requirements-upgrade:
-	source $(VENV) && python -m piptools compile --extra all -o docs/requirements.txt pyproject.toml --upgrade
+	source $(VENV) && python -m piptools compile --all-extras -o docs/requirements.txt pyproject.toml --upgrade
 
 update-version:
 	#sed -i 's/"version": "[0-9.]\+"/"version": "$(VERSION)"/' package.json
 	sed -i 's/version = "[0-9.]\+"/version = "$(VERSION)"/' pyproject.toml
 	sed -i 's/__version__ = "[0-9.]\+"/__version__ = "$(VERSION)"/' fake.py
 #	find src/ -type f -name '*.css' -exec sed -i 's/@version [0-9.]\+/@version $(VERSION)/' {} \;
 #	find src/ -type f -name '*.js' -exec sed -i 's/@version [0-9.]\+/@version $(VERSION)/' {} \;
```

### Comparing `fake_py-0.6.8/PKG-INFO` & `fake_py-0.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake.py
-Version: 0.6.8
+Version: 0.6.9
 Summary: Minimalistic, standalone alternative fake data generator with no dependencies.
 Author-email: Artur Barseghyan <artur.barseghyan@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/barseghyanartur/fake.py/
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/fake.py/issues
 Project-URL: Documentation, https://fakepy.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/fake.py/
@@ -35,16 +35,18 @@
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
+Requires-Dist: django; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-django; extra == "test"
 Requires-Dist: pytest-rst; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx<6.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "docs"
 Requires-Dist: sphinx-no-pragma; extra == "docs"
 
 =======
@@ -267,20 +269,21 @@
     FAKER.docx_file()  # str
     FAKER.png_file()  # str
     FAKER.svg_file()  # str
     FAKER.bmp_file()  # str
     FAKER.gif_file()  # str
     FAKER.txt_file()  # str
 
-Factories
----------
+Factories/dynamic fixtures
+--------------------------
 This is how you could define factories for `Django`_'s built-in ``Group``
 and ``User`` models.
 
 .. code-block:: python
+    :name: test_factories
 
     from django.contrib.auth.models import Group, User
     from fake import (
         DjangoModelFactory,
         FACTORY,
         PostSave,
         PreSave,
```

### Comparing `fake_py-0.6.8/README.rst` & `fake_py-0.6.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -218,20 +218,21 @@
     FAKER.docx_file()  # str
     FAKER.png_file()  # str
     FAKER.svg_file()  # str
     FAKER.bmp_file()  # str
     FAKER.gif_file()  # str
     FAKER.txt_file()  # str
 
-Factories
----------
+Factories/dynamic fixtures
+--------------------------
 This is how you could define factories for `Django`_'s built-in ``Group``
 and ``User`` models.
 
 .. code-block:: python
+    :name: test_factories
 
     from django.contrib.auth.models import Group, User
     from fake import (
         DjangoModelFactory,
         FACTORY,
         PostSave,
         PreSave,
```

### Comparing `fake_py-0.6.8/SECURITY.md` & `fake_py-0.6.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/SECURITY.rst` & `fake_py-0.6.9/SECURITY.rst`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/__copy_fake.py` & `fake_py-0.6.9/__copy_fake.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     get_args,
     get_origin,
     get_type_hints,
 )
 from uuid import UUID
 
 __title__ = "fake.py"
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
 __copyright__ = "2023-2024 Artur Barseghyan"
 __license__ = "MIT"
 __all__ = (
     "AuthorshipData",
     "BaseStorage",
     "DjangoModelFactory",
@@ -1529,27 +1529,29 @@
     @provider
     def pdf_file(
         self,
         nb_pages: int = 1,
         generator: Union[
             Type[TextPdfGenerator], Type[GraphicPdfGenerator]
         ] = GraphicPdfGenerator,
+        metadata: Optional[MetaData] = None,
         storage: Optional[BaseStorage] = None,
         basename: Optional[str] = None,
         prefix: Optional[str] = None,
         **kwargs,
     ) -> StringValue:
         if storage is None:
             storage = FileSystemStorage()
         filename = storage.generate_filename(
             extension="pdf",
             prefix=prefix,
             basename=basename,
         )
-        metadata = MetaData()
+        if not metadata:
+            metadata = MetaData()
         data = self.pdf(
             nb_pages=nb_pages, generator=generator, metadata=metadata, **kwargs
         )
         storage.write_bytes(filename=filename, data=data)
         file = StringValue(storage.relpath(filename))
         file.data = {
             "storage": storage,
@@ -1655,26 +1657,28 @@
         )
 
     @provider
     def docx_file(
         self,
         nb_pages: int = 1,
         texts: Optional[List[str]] = None,
+        metadata: Optional[MetaData] = None,
         storage: Optional[BaseStorage] = None,
         basename: Optional[str] = None,
         prefix: Optional[str] = None,
     ) -> StringValue:
         if storage is None:
             storage = FileSystemStorage()
         filename = storage.generate_filename(
             extension="docx",
             prefix=prefix,
             basename=basename,
         )
-        metadata = MetaData()
+        if not metadata:
+            metadata = MetaData()
         data = self.docx(texts=texts, metadata=metadata)
         storage.write_bytes(filename=filename, data=data)
         file = StringValue(storage.relpath(filename))
         file.data = {
             "storage": storage,
             "filename": filename,
             "content": metadata.content,
```

### Comparing `fake_py-0.6.8/docs/Makefile` & `fake_py-0.6.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/_static/examples/factories/dataclasses/article/factories.py` & `fake_py-0.6.9/docs/_static/examples/factories/dataclasses/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/_static/examples/factories/dataclasses/article/models.py` & `fake_py-0.6.9/docs/_static/examples/factories/dataclasses/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/_static/examples/factories/django/article/factories.py` & `fake_py-0.6.9/docs/_static/examples/factories/django/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/_static/examples/factories/django/article/models.py` & `fake_py-0.6.9/docs/_static/examples/factories/django/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/_static/examples/factories/pydantic/article/factories.py` & `fake_py-0.6.9/docs/_static/examples/factories/pydantic/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/_static/examples/factories/pydantic/article/models.py` & `fake_py-0.6.9/docs/_static/examples/factories/pydantic/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/article/factories.py` & `fake_py-0.6.9/docs/_static/examples/factories/sqlalchemy/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/_static/examples/factories/sqlalchemy/article/models.py` & `fake_py-0.6.9/docs/_static/examples/factories/sqlalchemy/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/_static/examples/factories/tortoise/article/factories.py` & `fake_py-0.6.9/docs/_static/examples/factories/tortoise/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/_static/examples/factories/tortoise/article/models.py` & `fake_py-0.6.9/docs/_static/examples/factories/tortoise/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/conf.py` & `fake_py-0.6.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/conf.py.distrib` & `fake_py-0.6.9/docs/conf.py.distrib`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/creating_docx.rst` & `fake_py-0.6.9/docs/creating_docx.rst`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/creating_images.rst` & `fake_py-0.6.9/docs/creating_images.rst`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/creating_pdf.rst` & `fake_py-0.6.9/docs/creating_pdf.rst`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/customization.rst` & `fake_py-0.6.9/docs/customization.rst`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/factories.rst` & `fake_py-0.6.9/docs/factories.rst`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/docs/make.bat` & `fake_py-0.6.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/customization/address/factories.py` & `fake_py-0.6.9/examples/customization/address/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/customization/address/models.py` & `fake_py-0.6.9/examples/customization/address/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/customization/address/tests.py` & `fake_py-0.6.9/examples/customization/address/tests.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/customization/band/tests.py` & `fake_py-0.6.9/examples/customization/band/tests.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/customization/data.py` & `fake_py-0.6.9/examples/customization/data.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/customization/fake_address.py` & `fake_py-0.6.9/examples/customization/fake_address.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/customization/fake_band.py` & `fake_py-0.6.9/examples/customization/fake_band.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/customization/manage.py` & `fake_py-0.6.9/examples/customization/manage.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/customization/override_default_data.py` & `fake_py-0.6.9/examples/customization/override_default_data.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/dataclasses/article/factories.py` & `fake_py-0.6.9/examples/dataclasses/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/dataclasses/article/models.py` & `fake_py-0.6.9/examples/dataclasses/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/dataclasses/article/tests.py` & `fake_py-0.6.9/examples/dataclasses/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/dataclasses/manage.py` & `fake_py-0.6.9/examples/dataclasses/manage.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/django/article/factories.py` & `fake_py-0.6.9/examples/django/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/django/article/migrations/0001_initial.py` & `fake_py-0.6.9/examples/django/article/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/django/article/models.py` & `fake_py-0.6.9/examples/django/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/django/article/tests.py` & `fake_py-0.6.9/examples/django/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/django/blog/settings.py` & `fake_py-0.6.9/examples/django/blog/settings.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/django/blog/urls.py` & `fake_py-0.6.9/examples/django/blog/urls.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/django/manage.py` & `fake_py-0.6.9/examples/django/manage.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/hypothesis/manage.py` & `fake_py-0.6.9/examples/hypothesis/manage.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/hypothesis/tests.py` & `fake_py-0.6.9/examples/hypothesis/tests.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/lazyfuzzy/article/factories.py` & `fake_py-0.6.9/examples/lazyfuzzy/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/lazyfuzzy/article/models.py` & `fake_py-0.6.9/examples/lazyfuzzy/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/lazyfuzzy/article/tests.py` & `fake_py-0.6.9/examples/lazyfuzzy/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/lazyfuzzy/manage.py` & `fake_py-0.6.9/examples/lazyfuzzy/manage.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/pydantic/article/factories.py` & `fake_py-0.6.9/examples/pydantic/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/pydantic/article/models.py` & `fake_py-0.6.9/examples/pydantic/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/pydantic/article/tests.py` & `fake_py-0.6.9/examples/pydantic/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/pydantic/manage.py` & `fake_py-0.6.9/examples/pydantic/manage.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/sqlalchemy/article/factories.py` & `fake_py-0.6.9/examples/sqlalchemy/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/sqlalchemy/article/models.py` & `fake_py-0.6.9/examples/sqlalchemy/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/sqlalchemy/article/tests.py` & `fake_py-0.6.9/examples/sqlalchemy/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/sqlalchemy/manage.py` & `fake_py-0.6.9/examples/sqlalchemy/manage.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/tortoise/article/factories.py` & `fake_py-0.6.9/examples/tortoise/article/factories.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/tortoise/article/models.py` & `fake_py-0.6.9/examples/tortoise/article/models.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/tortoise/article/tests.py` & `fake_py-0.6.9/examples/tortoise/article/tests.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/examples/tortoise/manage.py` & `fake_py-0.6.9/examples/tortoise/manage.py`

 * *Files identical despite different names*

### Comparing `fake_py-0.6.8/fake.py` & `fake_py-0.6.9/fake.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     get_args,
     get_origin,
     get_type_hints,
 )
 from uuid import UUID
 
 __title__ = "fake.py"
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
 __copyright__ = "2023-2024 Artur Barseghyan"
 __license__ = "MIT"
 __all__ = (
     "AuthorshipData",
     "BaseStorage",
     "DjangoModelFactory",
@@ -1529,27 +1529,29 @@
     @provider
     def pdf_file(
         self,
         nb_pages: int = 1,
         generator: Union[
             Type[TextPdfGenerator], Type[GraphicPdfGenerator]
         ] = GraphicPdfGenerator,
+        metadata: Optional[MetaData] = None,
         storage: Optional[BaseStorage] = None,
         basename: Optional[str] = None,
         prefix: Optional[str] = None,
         **kwargs,
     ) -> StringValue:
         if storage is None:
             storage = FileSystemStorage()
         filename = storage.generate_filename(
             extension="pdf",
             prefix=prefix,
             basename=basename,
         )
-        metadata = MetaData()
+        if not metadata:
+            metadata = MetaData()
         data = self.pdf(
             nb_pages=nb_pages, generator=generator, metadata=metadata, **kwargs
         )
         storage.write_bytes(filename=filename, data=data)
         file = StringValue(storage.relpath(filename))
         file.data = {
             "storage": storage,
@@ -1655,26 +1657,28 @@
         )
 
     @provider
     def docx_file(
         self,
         nb_pages: int = 1,
         texts: Optional[List[str]] = None,
+        metadata: Optional[MetaData] = None,
         storage: Optional[BaseStorage] = None,
         basename: Optional[str] = None,
         prefix: Optional[str] = None,
     ) -> StringValue:
         if storage is None:
             storage = FileSystemStorage()
         filename = storage.generate_filename(
             extension="docx",
             prefix=prefix,
             basename=basename,
         )
-        metadata = MetaData()
+        if not metadata:
+            metadata = MetaData()
         data = self.docx(texts=texts, metadata=metadata)
         storage.write_bytes(filename=filename, data=data)
         file = StringValue(storage.relpath(filename))
         file.data = {
             "storage": storage,
             "filename": filename,
             "content": metadata.content,
```

### Comparing `fake_py-0.6.8/fake.py.egg-info/PKG-INFO` & `fake_py-0.6.9/fake.py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fake.py
-Version: 0.6.8
+Version: 0.6.9
 Summary: Minimalistic, standalone alternative fake data generator with no dependencies.
 Author-email: Artur Barseghyan <artur.barseghyan@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/barseghyanartur/fake.py/
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/fake.py/issues
 Project-URL: Documentation, https://fakepy.readthedocs.io/
 Project-URL: Source Code, https://github.com/barseghyanartur/fake.py/
@@ -35,16 +35,18 @@
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
+Requires-Dist: django; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-django; extra == "test"
 Requires-Dist: pytest-rst; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx<6.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=1.3.0; extra == "docs"
 Requires-Dist: sphinx-no-pragma; extra == "docs"
 
 =======
@@ -267,20 +269,21 @@
     FAKER.docx_file()  # str
     FAKER.png_file()  # str
     FAKER.svg_file()  # str
     FAKER.bmp_file()  # str
     FAKER.gif_file()  # str
     FAKER.txt_file()  # str
 
-Factories
----------
+Factories/dynamic fixtures
+--------------------------
 This is how you could define factories for `Django`_'s built-in ``Group``
 and ``User`` models.
 
 .. code-block:: python
+    :name: test_factories
 
     from django.contrib.auth.models import Group, User
     from fake import (
         DjangoModelFactory,
         FACTORY,
         PostSave,
         PreSave,
```

### Comparing `fake_py-0.6.8/fake.py.egg-info/SOURCES.txt` & `fake_py-0.6.9/fake.py.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 CONTRIBUTING.rst
 LICENSE
 Makefile
 README.rst
 SECURITY.md
 SECURITY.rst
 __copy_fake.py
+conftest.py
 fake.py
 pyproject.toml
 .github/workflows/test.yml
 docs/Makefile
 docs/changelog.rst
 docs/code_of_conduct.rst
 docs/conf.py
```

### Comparing `fake_py-0.6.8/pyproject.toml` & `fake_py-0.6.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "fake.py"
 description = "Minimalistic, standalone alternative fake data generator with no dependencies."
 readme = "README.rst"
-version = "0.6.8"
+version = "0.6.9"
 dependencies = []
 authors = [
     {name = "Artur Barseghyan", email = "artur.barseghyan@gmail.com"},
 ]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -29,31 +29,32 @@
 [project.urls]
 "Homepage" = "https://github.com/barseghyanartur/fake.py/"
 "Bug Tracker" = "https://github.com/barseghyanartur/fake.py/issues"
 "Documentation" = "https://fakepy.readthedocs.io/"
 "Source Code" = "https://github.com/barseghyanartur/fake.py/"
 "Changelog" = "https://fakepy.readthedocs.io/en/latest/changelog.html"
 
-
 [project.optional-dependencies]
 all = ["fake.py[dev,test,docs]"]
 dev = [
     "black",
     "detect-secrets",
     "doc8",
     "ipython",
     "isort",
     "mypy",
     "pip-tools",
     "ruff",
     "twine",
 ]
 test = [
+    "django",
     "pytest",
     "pytest-cov",
+    "pytest-django",
     "pytest-rst",
 ]
 docs = [
     "sphinx<6.0",
     "sphinx-rtd-theme>=1.3.0",
     "sphinx-no-pragma",
 ]
@@ -162,14 +163,18 @@
 ]
 testpaths = [
     "fake.py",
     "__copy_fake.py",
     "*.rst",
     "**/*.rst",
 ]
+pythonpath = [
+    "examples/django",
+]
+DJANGO_SETTINGS_MODULE = "blog.settings"
 
 [tool.coverage.run]
 relative_files = true
 omit = [
     ".tox/*",
 ]
```

