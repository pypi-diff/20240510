# Comparing `tmp/erpbrasil.edoc-2.7.1.tar.gz` & `tmp/erpbrasil.edoc-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erpbrasil.edoc-2.7.1.tar", last modified: Fri Feb 23 16:02:31 2024, max compression
+gzip compressed data, was "erpbrasil.edoc-2.8.0.tar", last modified: Fri May 10 02:59:02 2024, max compression
```

## Comparing `erpbrasil.edoc-2.7.1.tar` & `erpbrasil.edoc-2.8.0.tar`

### file list

```diff
@@ -1,97 +1,100 @@
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.023473 erpbrasil.edoc-2.7.1/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1424 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/.appveyor.yml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      511 2024-02-23 16:02:01.000000 erpbrasil.edoc-2.7.1/.bumpversion.cfg
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2893 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/.cookiecutterrc
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      182 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/.coveragerc
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      215 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/.editorconfig
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      915 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/.travis.yml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       64 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/AUTHORS.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1181 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/CHANGELOG.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2753 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/CONTRIBUTING.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1105 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/LICENSE
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      359 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/MANIFEST.in
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     4536 2024-02-23 16:02:31.023473 erpbrasil.edoc-2.7.1/PKG-INFO
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3582 2024-02-23 16:02:01.000000 erpbrasil.edoc-2.7.1/README.rst
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.018473 erpbrasil.edoc-2.7.1/ci/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3995 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/ci/appveyor-bootstrap.py
--rwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3827 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/ci/appveyor-download.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      763 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/ci/appveyor-with-compiler.cmd
--rwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2097 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/ci/bootstrap.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       50 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/ci/requirements.txt
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.018473 erpbrasil.edoc-2.7.1/ci/templates/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1756 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/ci/templates/.appveyor.yml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      956 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/ci/templates/.travis.yml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1816 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/ci/templates/appveyor.yml
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.019473 erpbrasil.edoc-2.7.1/docs/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       28 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/authors.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       30 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/changelog.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1382 2024-02-23 16:02:01.000000 erpbrasil.edoc-2.7.1/docs/conf.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       33 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/contributing.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      245 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/index.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       94 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/installation.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       27 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/readme.rst
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.019473 erpbrasil.edoc-2.7.1/docs/reference/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      126 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/reference/erpbrasil.edoc.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       66 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/reference/index.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       29 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/requirements.txt
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      109 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/spelling_wordlist.txt
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       80 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/docs/usage.rst
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       98 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/requirements.txt
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      508 2024-02-23 16:02:31.024473 erpbrasil.edoc-2.7.1/setup.cfg
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3749 2024-02-23 16:02:01.000000 erpbrasil.edoc-2.7.1/setup.py
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.016473 erpbrasil.edoc-2.7.1/src/
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.019473 erpbrasil.edoc-2.7.1/src/erpbrasil/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      271 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/__init__.py
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.021473 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      481 2024-02-23 16:02:01.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/__init__.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      397 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/__main__.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6739 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/chave.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      831 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/cli.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     7176 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/edoc.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    11568 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/mde.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    10191 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/mdfe.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    14513 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/nfce.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    45505 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/nfe.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3740 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/nfse.py
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.021473 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/__init__.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     7447 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/barueri.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1127 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/cidades.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2463 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/dsf.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    10310 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/ginfes.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    12756 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/issnet.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6850 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/paulistana.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1595 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/resposta.py
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.020473 erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     4536 2024-02-23 16:02:30.000000 erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/PKG-INFO
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2648 2024-02-23 16:02:30.000000 erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/SOURCES.txt
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        1 2024-02-23 16:02:30.000000 erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/dependency_links.txt
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       59 2024-02-23 16:02:30.000000 erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/entry_points.txt
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       25 2024-02-23 16:02:30.000000 erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/namespace_packages.txt
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        1 2024-02-23 16:02:30.000000 erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/not-zip-safe
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)      281 2024-02-23 16:02:30.000000 erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/requires.txt
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)       10 2024-02-23 16:02:30.000000 erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/top_level.txt
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.022473 erpbrasil.edoc-2.7.1/tests/
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.022473 erpbrasil.edoc-2.7.1/tests/fixtures/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2597 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/dummy_cert.pfx
-drwxr-xr-x   0 ygorcarvalho  (1000) ygorcarvalho  (1000)        0 2024-02-23 16:02:31.023473 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    11491 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     9234 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3008 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_chave.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6682 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    11477 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6969 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    10324 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6744 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    16217 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_envia_documento.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)    17539 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2497 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6764 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6533 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_status_servico.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)   144902 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     2620 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/test_erpbrasil_edoc.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     3105 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/test_erpbrasil_edoc_manifestacao.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     6921 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/test_erpbrasil_edoc_nfse_ginfes.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     5431 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/test_erpbrasil_edoc_nfse_paulistana.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1261 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tests/test_erpbrasil_edoc_situacao.py
--rw-r--r--   0 ygorcarvalho  (1000) ygorcarvalho  (1000)     1989 2024-02-23 16:01:29.000000 erpbrasil.edoc-2.7.1/tox.ini
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      511 2024-05-10 02:52:49.000000 erpbrasil.edoc-2.8.0/.bumpversion.cfg
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2893 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/.cookiecutterrc
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      182 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/.coveragerc
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      215 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/.editorconfig
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.124317 erpbrasil.edoc-2.8.0/.github/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/.github/workflows/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2568 2024-05-10 00:18:43.000000 erpbrasil.edoc-2.8.0/.github/workflows/github-actions.yml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      207 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/.github/workflows/pre-commit.yml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      509 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/.pre-commit-config.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       64 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/AUTHORS.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1180 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/CHANGELOG.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2756 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/CONTRIBUTING.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1106 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/LICENSE
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      450 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/MANIFEST.in
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     4553 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/PKG-INFO
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3137 2024-05-10 02:44:10.000000 erpbrasil.edoc-2.8.0/README.rst
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/ci/
+-rwxrwxr-x   0 antonio   (1000) antonio   (1000)     2952 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/ci/bootstrap.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       54 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/ci/requirements.txt
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.124317 erpbrasil.edoc-2.8.0/ci/templates/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.124317 erpbrasil.edoc-2.8.0/ci/templates/.github/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/ci/templates/.github/workflows/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1979 2024-05-10 00:18:43.000000 erpbrasil.edoc-2.8.0/ci/templates/.github/workflows/github-actions.yml
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/docs/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       28 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/authors.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       30 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/changelog.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1302 2024-05-10 02:44:18.000000 erpbrasil.edoc-2.8.0/docs/conf.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       33 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/contributing.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      244 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/docs/index.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       94 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/installation.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       27 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/readme.rst
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/docs/reference/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      126 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/reference/erpbrasil.edoc.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       66 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/reference/index.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       29 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/requirements.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      109 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/docs/spelling_wordlist.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       83 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/docs/usage.rst
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      360 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/pyproject.toml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       99 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/requirements.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      508 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/setup.cfg
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3595 2024-05-10 02:44:13.000000 erpbrasil.edoc-2.8.0/setup.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/src/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/src/erpbrasil/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      245 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/__init__.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      455 2024-05-10 02:44:20.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/__init__.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      398 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/__main__.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6611 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/chave.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      832 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/cli.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     7386 2024-05-10 00:18:43.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/edoc.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11114 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/mde.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     9884 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/mdfe.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    14711 2024-05-10 00:18:43.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfce.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    46177 2024-05-10 02:01:41.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfe.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     3543 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfse.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        0 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/__init__.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     7047 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/barueri.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1007 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/cidades.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2239 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/dsf.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     9943 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/ginfes.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    12459 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/issnet.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6563 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/paulistana.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1545 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/resposta.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     4553 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/PKG-INFO
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2677 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       60 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/entry_points.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       25 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/namespace_packages.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        1 2024-05-10 02:44:32.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/not-zip-safe
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      281 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/requires.txt
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)       10 2024-05-10 02:59:02.000000 erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/top_level.txt
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/tests/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)        0 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/__init__.py
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.128316 erpbrasil.edoc-2.8.0/tests/fixtures/
+drwxrwxr-x   0 antonio   (1000) antonio   (1000)        0 2024-05-10 02:59:02.132316 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11491 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     9234 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     8187 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_chave.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11291 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    11477 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6969 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    10324 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6744 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    16217 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_envia_documento.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)    17539 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2497 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6764 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     6533 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_status_servico.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)   139572 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1632 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/test_certificate_mixin.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2188 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2513 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_manifestacao.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     2282 2024-05-10 00:18:43.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_nfe.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     5936 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_nfse_ginfes.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     5431 2024-05-08 22:32:06.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_nfse_paulistana.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)      823 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_situacao.py
+-rw-rw-r--   0 antonio   (1000) antonio   (1000)     1803 2024-05-09 00:55:11.000000 erpbrasil.edoc-2.8.0/tox.ini
```

### Comparing `erpbrasil.edoc-2.7.1/.cookiecutterrc` & `erpbrasil.edoc-2.8.0/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.7.1/CHANGELOG.rst` & `erpbrasil.edoc-2.8.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,7 @@
 - Manifestação do Destinatário
 - Consulta Cadastro
 
 2.2.0 (2021-05-26)
 ~~~~~~~~~~~~~~~~~~
 
 - Nota Paulistana
-
```

### Comparing `erpbrasil.edoc-2.7.1/CONTRIBUTING.rst` & `erpbrasil.edoc-2.8.0/CONTRIBUTING.rst`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 Bug reports
 ===========
 
 When `reporting a bug <https://github.com/erpbrasil/erpbrasil.edoc/issues>`_ please include:
 
     * Your operating system name and version.
-    * Any details about your local setup that might be helpful in troubleshooting.
+    * Any details about your local setup that might be helpful
+      in troubleshooting.
     * Detailed steps to reproduce the bug.
 
 Documentation improvements
 ==========================
 
 erpbrasil.edoc could always use more documentation, whether as part of the
 official erpbrasil.edoc docs, in docstrings, or even on the web in blog posts,
@@ -26,15 +27,16 @@
 
 The best way to send feedback is to file an issue at https://github.com/erpbrasil/erpbrasil.edoc/issues.
 
 If you are proposing a feature:
 
 * Explain in detail how it would work.
 * Keep the scope as narrow as possible, to make it easier to implement.
-* Remember that this is a volunteer-driven project, and that code contributions are welcome :)
+* Remember that this is a volunteer-driven project, and that code contributions
+  are welcome :)
 
 Development
 ===========
 
 To set up `erpbrasil.edoc` for local development:
 
 1. Fork `erpbrasil.edoc <https://github.com/erpbrasil/erpbrasil.edoc>`_
@@ -45,40 +47,41 @@
 
 3. Create a branch for local development::
 
     git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
-4. When you're done making changes, run all the checks, doc builder and spell checker with `tox <https://tox.readthedocs.io/en/latest/install.html>`_ one command::
+4. When you're done making changes, run all the checks, doc builder and spell checker with `tox <https://tox.wiki/en/latest/installation.html>`_ one command::
 
     tox
 
 5. Commit your changes and push your branch to GitHub::
 
     git add .
     git commit -m "Your detailed description of your changes."
     git push origin name-of-your-bugfix-or-feature
 
 6. Submit a pull request through the GitHub website.
 
 Pull Request Guidelines
 -----------------------
 
-If you need some code review or feedback while you're developing the code just make the pull request.
+If you need some code review or feedback while you're developing the code just
+make the pull request.
 
 For merging, you should:
 
 1. Include passing tests (run ``tox``) [1]_.
 2. Update documentation when there's new API, functionality etc.
 3. Add a note to ``CHANGELOG.rst`` about the changes.
 4. Add yourself to ``AUTHORS.rst``.
 
-.. [1] If you don't have all the necessary python versions available locally you can rely on Travis - it will
-       `run the tests <https://travis-ci.org/erpbrasil/erpbrasil.edoc/pull_requests>`_ for each change you add in the pull request.
+.. [1] If you don't have all the necessary python versions available locally, you can rely on GitHub Actions - it will
+       `run the tests <https://github.com/erpbrasil/erpbrasil.edoc/actions>`_ for each change you add in the pull request.
 
        It will be slower though ...
 
 Tips
 ----
 
 To run a subset of tests::
```

### Comparing `erpbrasil.edoc-2.7.1/LICENSE` & `erpbrasil.edoc-2.8.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 Copyright (c) 2019, Luis Felipe Mileo
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice (including the next paragraph) shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `erpbrasil.edoc-2.7.1/PKG-INFO` & `erpbrasil.edoc-2.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: erpbrasil.edoc
-Version: 2.7.1
+Version: 2.8.0
 Summary: Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 Home-page: https://github.com/erpbrasil/erpbrasil.edoc
 Author: Luis Felipe Mileo
 Author-email: mileo@kmee.com.br
 License: MIT
 Project-URL: Documentation, https://erpbrasiledoc.readthedocs.io/
 Project-URL: Changelog, https://erpbrasiledoc.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/erpbrasil/erpbrasil.edoc/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
@@ -20,42 +21,43 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
-Provides-Extra: nfselib.ginfes
-Provides-Extra: nfselib.paulistana
-Provides-Extra: nfselib.dsf
+Provides-Extra: mdfelib
+Provides-Extra: nfelib
 Provides-Extra: nfselib.betha
+Provides-Extra: nfselib.dsf
+Provides-Extra: nfselib.ginfes
 Provides-Extra: nfselib.issnet
-Provides-Extra: nfelib
-Provides-Extra: mdfelib
+Provides-Extra: nfselib.paulistana
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 Overview
 ========
 
 
 
-Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
+Emissão de documentos fiscais e outras obrigações
+(NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 
 
 Documentação
 ============
 
 https://erpbrasil.github.io/
 
 Créditos
 ========
 
-Esta é uma biblioteca criada atravês do esforço de das empresas:
+Esta é uma biblioteca criada através do esforço das empresas:
 
 * Akretion https://akretion.com/pt-BR/
 * KMEE https://www.kmee.com.br
 
 Favor consultar a lista de contribuidores:
 
 https://github.com/erpbrasil/erpbrasil.edoc/graphs/contributors
@@ -64,18 +66,19 @@
 ~~~~~~~
 
 * Free software: MIT license
 
 Instalação
 ==========
 
-Para permitir que a instalação do seu ERP cresça somente com a necessidade do cliente
-é possível instalar as dependências da biblioteca de forma opcional:
+Para permitir que a instalação do seu ERP cresça somente com a necessidade
+do cliente é possível instalar as dependências da biblioteca de forma opcional:
 
 ::
+
     pip install erpbrasil.edoc
 
     # Documentos do Sefaz
 
     pip install erpbrasil.edoc[nfelib] # Emissão de NF-e
     pip install erpbrasil.edoc[mdfelib] # Emissão de Manifesto de Carga - MD
     pip install erpbrasil.edoc[ctelib] # Emissão de CT-e
@@ -171,7 +174,8 @@
 - Consulta Cadastro
 
 2.2.0 (2021-05-26)
 ~~~~~~~~~~~~~~~~~~
 
 - Nota Paulistana
 
+
```

### Comparing `erpbrasil.edoc-2.7.1/README.rst` & `erpbrasil.edoc-2.8.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -4,39 +4,30 @@
 
 .. start-badges
 
 .. list-table::
     :stub-columns: 1
 
     * - tests
-      - | |travis| |appveyor|
-        | |codecov|
+      - |codecov|
     * - package
-      - | |version| |wheel| |supported-versions| |supported-implementations|
-        | |commits-since|
-
-.. |travis| image:: https://api.travis-ci.org/erpbrasil/erpbrasil.edoc.svg?branch=master
-    :alt: Travis-CI Build Status
-    :target: https://travis-ci.org/erpbrasil/erpbrasil.edoc
-
-.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/erpbrasil/erpbrasil.edoc?branch=master&svg=true
-    :alt: AppVeyor Build Status
-    :target: https://ci.appveyor.com/project/erpbrasil/erpbrasil.edoc
+      - |version| |wheel| |supported-versions| |supported-implementations|
+        |commits-since|
 
 .. |codecov| image:: https://codecov.io/github/erpbrasil/erpbrasil.edoc/coverage.svg?branch=master
     :alt: Coverage Status
     :target: https://codecov.io/github/erpbrasil/erpbrasil.edoc
 
 .. |version| image:: https://img.shields.io/pypi/v/erpbrasil.edoc.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/erpbrasil.edoc
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/erpbrasil/erpbrasil.edoc/v2.7.1.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/erpbrasil/erpbrasil.edoc/v2.8.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/erpbrasil/erpbrasil.edoc/compare/v2.7.1...master
+    :target: https://github.com/erpbrasil/erpbrasil.edoc/compare/v2.8.0...master
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/erpbrasil.edoc.svg
     :alt: PyPI Wheel
     :target: https://pypi.org/project/erpbrasil.edoc
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/erpbrasil.edoc.svg
     :alt: Supported versions
@@ -45,26 +36,27 @@
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/erpbrasil.edoc.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/erpbrasil.edoc
 
 
 .. end-badges
 
-Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
+Emissão de documentos fiscais e outras obrigações
+(NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 
 
 Documentação
 ============
 
 https://erpbrasil.github.io/
 
 Créditos
 ========
 
-Esta é uma biblioteca criada atravês do esforço de das empresas:
+Esta é uma biblioteca criada através do esforço das empresas:
 
 * Akretion https://akretion.com/pt-BR/
 * KMEE https://www.kmee.com.br
 
 Favor consultar a lista de contribuidores:
 
 https://github.com/erpbrasil/erpbrasil.edoc/graphs/contributors
@@ -73,18 +65,19 @@
 ~~~~~~~
 
 * Free software: MIT license
 
 Instalação
 ==========
 
-Para permitir que a instalação do seu ERP cresça somente com a necessidade do cliente
-é possível instalar as dependências da biblioteca de forma opcional:
+Para permitir que a instalação do seu ERP cresça somente com a necessidade
+do cliente é possível instalar as dependências da biblioteca de forma opcional:
 
 ::
+
     pip install erpbrasil.edoc
 
     # Documentos do Sefaz
 
     pip install erpbrasil.edoc[nfelib] # Emissão de NF-e
     pip install erpbrasil.edoc[mdfelib] # Emissão de Manifesto de Carga - MD
     pip install erpbrasil.edoc[ctelib] # Emissão de CT-e
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/chave.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/chave.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# coding=utf-8
 # Copyright (C) 2019  Luis Felipe Mileo - mileo at kmee com br
 
 # Python 3 compatibility hack
 try:
-    unicode('')
+    unicode("")
 except NameError:
     unicode = str
 
 import datetime
 import hashlib
 
 
-class ChaveNFSeDSF(object):
+class ChaveNFSeDSF:
     """Representa a **chave de acesso** da NFS-e-DSF conforme descrito na
     Especificação da Assinatura, pagina 9. Os campos são definidos assim:
     .. sourcecode:: text                     39
         0         11    16         28      36 40              55             70        80            94
         |         |     |                   | ||              |              |         |             |
         00000317330NF   00000003866320090905T NN000000000001686000000000000000082997990008764130000102 --> campos
         |         |     |           |       | |               |              |         |             |
@@ -25,15 +24,15 @@
         |         |     |           |       | |               Tipo de recolhimento
         |         |     |           |       | Situação da RPS ( N - Normal ou C- Canceldada)
         |         |     |           |       Tributação
         |         |     |           Data emissão
         |         |     Número RPS
         |         Serie RPS
         Inscrição Municipal
-    """
+    """  # noqa: E501
 
     IM = slice(0, 11)
 
     SERIE = slice(11, 16)
 
     NUMERO = slice(16, 28)
 
@@ -58,21 +57,21 @@
             raise Exception
         elif rps:
             self.rps(rps)
         elif chave:
             self.chave = chave
 
     def __repr__(self):
-        return '{:s}({!r})'.format(self.__class__.__name__, str(self))
+        return f"{self.__class__.__name__:s}({str(self)!r})"
 
     def __unicode__(self):
         return self._campos
 
     def __str__(self):
-        return unicode(self).encode('utf-8')
+        return unicode(self).encode("utf-8")
 
     @property
     def inscricao_municipal(self):
         return self._inscricao_municipal
 
     @inscricao_municipal.setter
     def inscricao_municipal(self, value):
@@ -92,20 +91,20 @@
 
     @numero.setter
     def numero(self, value):
         self._numero = str(value).zfill(12)
 
     @property
     def data(self):
-        return self._data.strftime('%Y%m%d')
+        return self._data.strftime("%Y%m%d")
 
     @data.setter
     def data(self, value):
-        if isinstance(value, str) or isinstance(value, unicode):
-            self._data = datetime.datetime.strptime(value, '%Y%m%d')
+        if isinstance(value, str):
+            self._data = datetime.datetime.strptime(value, "%Y%m%d")
         elif isinstance(value, datetime.datetime):
             self._data = value
 
     @property
     def tributacao(self):
         return self._tributacao
 
@@ -135,25 +134,25 @@
 
     @property
     def valor_deducao(self):
         return self._valor_deducao
 
     @valor_servico.setter
     def valor_servico(self, value):
-        if isinstance(value, str) or isinstance(value, unicode):
+        if isinstance(value, str):
             self._valor_servico = value
         elif isinstance(value, float):
-            self._valor_servico = str(value).replace('.', '')
+            self._valor_servico = str(value).replace(".", "")
 
     @valor_deducao.setter
     def valor_deducao(self, value):
-        if isinstance(value, str) or isinstance(value, unicode):
+        if isinstance(value, str):
             self._valor_deducao = value
-        elif isinstance(value, float) or isinstance(value, int):
-            self._valor_deducao = str(value).replace('.', '')
+        elif isinstance(value, (float, int)):
+            self._valor_deducao = str(value).replace(".", "")
 
     @property
     def codigo_atividade(self):
         return self._codigo_atividade
 
     @codigo_atividade.setter
     def codigo_atividade(self, value):
@@ -166,25 +165,25 @@
     @cpf_cnpj.setter
     def cpf_cnpj(self, value):
         self._cpf_cnpj = str(value).zfill(14)
 
     @property
     def chave(self):
         chave = (
-            self.inscricao_municipal +
-            self.serie +
-            self.numero +
-            self.data +
-            self.tributacao +
-            self.situacao +
-            self.tipo_recolhimento +
-            self.valor_servico +
-            self.valor_deducao +
-            self.codigo_atividade +
-            self.cpf_cnpj
+            self.inscricao_municipal
+            + self.serie
+            + self.numero
+            + self.data
+            + self.tributacao
+            + self.situacao
+            + self.tipo_recolhimento
+            + self.valor_servico
+            + self.valor_deducao
+            + self.codigo_atividade
+            + self.cpf_cnpj
         )
         return chave
 
     @chave.setter
     def chave(self, value):
         self.inscricao_municipal = value[ChaveNFSeDSF.IM]
         self.serie = value[ChaveNFSeDSF.SERIE]
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/cli.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     ``__main__.py`` as a script. That means there won't be any
     ``erpbrasil.edoc.__main__`` in ``sys.modules``.
   - When you import __main__ it will get executed again (as a module) because
     there's no ``erpbrasil.edoc.__main__`` in ``sys.modules``.
 
   Also see (1) from http://click.pocoo.org/5/setuptools/#setuptools-integration
 """
+
 import sys
 
 
 def main(argv=sys.argv):
     """
     Args:
         argv (list): List of arguments
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/edoc.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/edoc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,90 +1,80 @@
-# -*- coding: utf-8 -*-
 # Copyright (C) 2018 - TODAY Luis Felipe Mileo - KMEE INFORMATICA LTDA
 # License MIT
 
 import abc
-from datetime import datetime
-from datetime import timedelta
-from datetime import timezone
+from datetime import datetime, timedelta, timezone
 
-from erpbrasil.assinatura.assinatura import Assinatura
 from lxml import etree
 from lxml.etree import _Element
 
+from erpbrasil.assinatura.assinatura import Assinatura
+
 from .resposta import analisar_retorno_raw
 
 # Fix Python 2.x.
 try:
     UNICODE_EXISTS = bool(type(unicode))
 except NameError:
     unicode = str
 
 try:
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
-ABC = abc.ABCMeta('ABC', (object,), {})
+ABC = abc.ABCMeta("ABC", (object,), {})
 
 
 class DocumentoEletronico(ABC):
     """
     Classe abstrata responsavel por definir os metodos e logica das classes
     de transmissao com os webservices.
     """
+
     _consulta_servico_ao_enviar = False
     _consulta_documento_antes_de_enviar = False
 
-    def __init__(self, transmissao):
+    def __init__(self, transmissao, envio_sincrono=False):
         self._transmissao = transmissao
+        self.envio_sincrono = bool(envio_sincrono)
 
     def _generateds_to_string_etree(self, ds, pretty_print=False):
-
         if type(ds) == _Element:
             return etree.tostring(ds), ds
         if isinstance(ds, str):
             return ds, etree.fromstring(ds)
         # if isinstance(ds, unicode):
         #     return ds, etree.fromstring(ds)
 
         output = StringIO()
         namespace = False
         if self._namespace:
             namespace = 'xmlns="' + self._namespace + '"'
 
         if namespace:
-            ds.export(
-                output,
-                0,
-                pretty_print=pretty_print,
-                namespacedef_=namespace
-            )
+            ds.export(output, 0, pretty_print=pretty_print, namespacedef_=namespace)
         else:
             ds.export(
                 output,
                 0,
                 pretty_print=pretty_print,
             )
         contents = output.getvalue()
         output.close()
         return contents, etree.fromstring(contents)
 
     def _post(self, raiz, url, operacao, classe):
         xml_string, xml_etree = self._generateds_to_string_etree(raiz)
         with self._transmissao.cliente(url):
-            retorno = self._transmissao.enviar(
-                operacao, xml_etree
-            )
-            return analisar_retorno_raw(
-                operacao, raiz, xml_string, retorno, classe
-            )
+            retorno = self._transmissao.enviar(operacao, xml_etree)
+            return analisar_retorno_raw(operacao, raiz, xml_string, retorno, classe)
 
-    def processar_documento(self, edoc):
-        """ Processar documento executa o envio do documento fiscal de forma
+    def processar_documento(self, edoc, envio_sincrono=False):
+        """Processar documento executa o envio do documento fiscal de forma
         completa ao serviço relacionado, esta é um método padrão que
         segue o seguinte workflow:
 
         1. Consulta o serviço;
         2. Verifica se o documento não foi emitido anteriormente;
         3. Envia o documento
         4. Caso o envio seja assincrono busca o resultado do processamento
@@ -139,26 +129,27 @@
                 #
                 return
         #
         # Documento nao foi enviado, entao vamos envia-lo
         #
 
         proc_envio = self.envia_documento(edoc)
+        if self.envio_sincrono:
+            self.monta_processo(edoc, proc_envio)
         yield proc_envio
 
-        #
-        # Deu errado?
-        #
-        if not proc_envio.resposta:
-            return
-
-        if not self._verifica_resposta_envio_sucesso(proc_envio):
-            #
-            # Interrompe o processo
-            #
+        # Retorna imediatamente se alguma das condições abaixo for verdadeira:
+        # 1. A resposta do processo de envio é falsa.
+        # 2. A resposta do envio não indica sucesso.
+        # 3. O envio é síncrono (não é necessário consultar o recibo).
+        if (
+            not proc_envio.resposta
+            or not self._verifica_resposta_envio_sucesso(proc_envio)
+            or self.envio_sincrono
+        ):
             return
 
         #
         # Aguarda o tempo do processamento antes da consulta
         #
         self._aguarda_tempo_medio(proc_envio)
         #
@@ -170,16 +161,18 @@
             return
 
         #
         # Tenta receber o resultado do processamento do lote, caso ainda
         # esteja em processamento
         #
         tentativa = 0
-        while (self._edoc_situacao_em_processamento(proc_recibo) and
-               tentativa < self._maximo_tentativas_consulta_recibo):
+        while (
+            self._edoc_situacao_em_processamento(proc_recibo)
+            and tentativa < self._maximo_tentativas_consulta_recibo
+        ):
             self._aguarda_tempo_medio(proc_envio)
             tentativa += 1
             #
             # Consulta o recibo do lote, para ver o que aconteceu
             #
             proc_recibo = self.consulta_recibo(proc_envio=proc_envio)
         self.monta_processo(edoc, proc_envio, proc_recibo)
@@ -203,32 +196,33 @@
         pass
 
     @abc.abstractmethod
     def consulta_recibo(self):
         pass
 
     def _gera_numero_lote(self):
-        return datetime.now().strftime('%Y%m%d%H%M%S')
+        return datetime.now().strftime("%Y%m%d%H%M%S")
 
     def _hora_agora(self):
-        FORMAT = '%Y-%m-%dT%H:%M:%S'
+        FORMAT = "%Y-%m-%dT%H:%M:%S"
         # return datetime.today().strftime(FORMAT) + '-00:00'
-        return datetime.strftime(
-            datetime.now(tz=timezone(timedelta(hours=-3))), FORMAT
-        ) + str(timezone(timedelta(hours=-3)))[3:]
+        return (
+            datetime.strftime(datetime.now(tz=timezone(timedelta(hours=-3))), FORMAT)
+            + str(timezone(timedelta(hours=-3)))[3:]
+        )
 
     def _data_hoje(self):
         return datetime.strftime(datetime.now(), "%Y-%m-%d")
 
     def assina_raiz(self, raiz, id, getchildren=False):
         xml_string, xml_etree = self._generateds_to_string_etree(raiz)
         xml_assinado = Assinatura(self._transmissao.certificado).assina_xml2(
             xml_etree, id, getchildren
         )
-        return xml_assinado.replace('\n', '').replace('\r', '')
+        return xml_assinado.replace("\n", "").replace("\r", "")
 
     def _verifica_servico_em_operacao(self, proc_servico):
         return True
 
     def _verifica_documento_ja_enviado(self, proc_consulta):
         return False
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/mde.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/mde.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,101 +1,93 @@
-# coding=utf-8
 # Copyright (C) 2020 - KMEE
 
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
 
 import re
 
-from erpbrasil.transmissao import TransmissaoSOAP
 from lxml import etree
 
-from erpbrasil.edoc.nfe import NFe
-from erpbrasil.edoc.nfe import localizar_url
+from erpbrasil.edoc.nfe import NFe, localizar_url
 from erpbrasil.edoc.resposta import RetornoSoap
+from erpbrasil.transmissao import TransmissaoSOAP
 
 try:
     from nfelib.v4_00 import retEnvConfRecebto
-    from nfelib.v4_00.retEnvConfRecebto import TEnvEvento as TEnvEventoManifestacao  # noga
+    from nfelib.v4_00.retEnvConfRecebto import TEnvEvento as TEnvEventoManifestacao
     from nfelib.v4_00.retEnvConfRecebto import TEvento as TEventoManifestacao  # noga
-    from nfelib.v4_00.retEnvConfRecebto import descEventoType as descEventoManifestacao  # noga
-    from nfelib.v4_00.retEnvConfRecebto import detEventoType as detEventoManifestacao  # noga
-    from nfelib.v4_00.retEnvConfRecebto import infEventoType as infEventoManifestacao  # noga
-    from nfelib.v4_00.retEnvConfRecebto import tpEventoType as eventoManifestacao  # noga
+    from nfelib.v4_00.retEnvConfRecebto import descEventoType as descEventoManifestacao
+    from nfelib.v4_00.retEnvConfRecebto import detEventoType as detEventoManifestacao
+    from nfelib.v4_00.retEnvConfRecebto import infEventoType as infEventoManifestacao
+    from nfelib.v4_00.retEnvConfRecebto import tpEventoType as eventoManifestacao
 except ImportError:
     pass
 
-WS_NFE_RECEPCAO_EVENTO = 'RecepcaoEvento'
+WS_NFE_RECEPCAO_EVENTO = "RecepcaoEvento"
 
 SIGLA_ESTADO = {
-    '12': 'AC',
-    '27': 'AL',
-    '13': 'AM',
-    '16': 'AP',
-    '29': 'BA',
-    '23': 'CE',
-    '53': 'DF',
-    '32': 'ES',
-    '52': 'GO',
-    '21': 'MA',
-    '31': 'MG',
-    '50': 'MS',
-    '51': 'MT',
-    '15': 'PA',
-    '25': 'PB',
-    '26': 'PE',
-    '22': 'PI',
-    '41': 'PR',
-    '33': 'RJ',
-    '24': 'RN',
-    '11': 'RO',
-    '14': 'RR',
-    '43': 'RS',
-    '42': 'SC',
-    '28': 'SE',
-    '35': 'SP',
-    '17': 'TO',
-    '91': 'AN'
+    "12": "AC",
+    "27": "AL",
+    "13": "AM",
+    "16": "AP",
+    "29": "BA",
+    "23": "CE",
+    "53": "DF",
+    "32": "ES",
+    "52": "GO",
+    "21": "MA",
+    "31": "MG",
+    "50": "MS",
+    "51": "MT",
+    "15": "PA",
+    "25": "PB",
+    "26": "PE",
+    "22": "PI",
+    "41": "PR",
+    "33": "RJ",
+    "24": "RN",
+    "11": "RO",
+    "14": "RR",
+    "43": "RS",
+    "42": "SC",
+    "28": "SE",
+    "35": "SP",
+    "17": "TO",
+    "91": "AN",
 }
 
 
 class MDe(NFe):
-
     # ----------------------------- MANIFESTAÇÃO DO DESTINATÁRIO -----------------
 
     def nfe_recepcao_envia_lote_evento(self, lista_eventos, numero_lote=False):
         """
         Envia lote de eventos confRecebto.TEvento
         :param lista_eventos: Lista com os eventos (infEvento)
         :param numero_lote: Número do lote. Gerado caso None
         :return: retorna a resposta do _post() de envio do lote
         """
 
         if not numero_lote:
             numero_lote = self._gera_numero_lote()
 
         eventos = []
-        raiz = TEnvEventoManifestacao(
-            versao="1.00",
-            idLote=numero_lote,
-            evento=eventos
-        )
-        raiz.original_tagname_ = 'envEvento'
+        raiz = TEnvEventoManifestacao(versao="1.00", idLote=numero_lote, evento=eventos)
+        raiz.original_tagname_ = "envEvento"
         xml_envio_string, xml_envio_etree = self._generateds_to_string_etree(raiz)
 
         for raiz_evento in lista_eventos:
             evento = TEventoManifestacao(
-                versao="1.00", infEvento=raiz_evento,
+                versao="1.00",
+                infEvento=raiz_evento,
             )
-            evento.original_tagname_ = 'evento'
+            evento.original_tagname_ = "evento"
 
             # Recupera o evento do XML assinado
-            xml_assinado = self.assina_raiz(evento, evento.infEvento.Id
-                                            ).replace('\n', '').encode()
+            xml_assinado = (
+                self.assina_raiz(evento, evento.infEvento.Id).replace("\n", "").encode()
+            )
 
             xml_envio_etree.append(etree.fromstring(xml_assinado))
 
             # FIXME: Essa forma de geração foi removida no ultimo refactor
 
             # Converte o xml_assinado para um objeto pelo
             # parser do esquema leiauteConfRecebto
@@ -104,22 +96,24 @@
 
             # Adiciona o xml_object na lista de eventos. Desse modo a lista
             # de eventos terá um evento assinado corretamente
             # eventos.append(xml_object)
 
         return self._post(
             xml_envio_etree,
-            localizar_url(WS_NFE_RECEPCAO_EVENTO, str(91), self.mod,
-                          int(self.ambiente)),
-            'nfeRecepcaoEventoNF',
-            retEnvConfRecebto
+            localizar_url(
+                WS_NFE_RECEPCAO_EVENTO, str(91), self.mod, int(self.ambiente)
+            ),
+            "nfeRecepcaoEventoNF",
+            retEnvConfRecebto,
         )
 
-    def nfe_recepcao_monta_evento(self, chave, cnpj_cpf, tpEvento, descEvento,
-                                  dhEvento=None, xJust=None):
+    def nfe_recepcao_monta_evento(
+        self, chave, cnpj_cpf, tpEvento, descEvento, dhEvento=None, xJust=None
+    ):
         """
         Método para montar o evento(infEvento) da manifestação
         :param chave: chave do documento
         :param cnpj_cpf: CPF ou CNPJ
         :param tpEvento:   Código do Evento
                                 210200 – Confirmação da Operação
                                 210210 – Ciência da Operação
@@ -132,34 +126,32 @@
                                 Operacao nao Realizada
         :param dhEvento:   Data/Hora no formato AAAA-MM-DDThh:mm:ssTZD
         :param xJust:      Este campo deve ser informado somente no
                                 evento de Operação não realizada
         :return: Um objeto da classe confRecebto.infEventoType preenchido
         """
 
-        nSeqEvento = '1'
+        nSeqEvento = "1"
         raiz = infEventoManifestacao(
-            Id='ID{}{}{}'.format(tpEvento, chave, nSeqEvento.zfill(2)),
+            Id=f"ID{tpEvento}{chave}{nSeqEvento.zfill(2)}",
             cOrgao=91,
             tpAmb=self.ambiente,
             CNPJ=cnpj_cpf if len(cnpj_cpf) > 11 else None,
             CPF=cnpj_cpf if len(cnpj_cpf) <= 11 else None,
             chNFe=chave,
             dhEvento=dhEvento or self._hora_agora(),
             tpEvento=tpEvento,
             nSeqEvento=nSeqEvento,
-            verEvento='1.00',
+            verEvento="1.00",
             detEvento=detEventoManifestacao(
-                versao='1.00',
-                descEvento=descEvento,
-                xJust=xJust
-            )
+                versao="1.00", descEvento=descEvento, xJust=xJust
+            ),
         )
 
-        raiz.original_tagname_ = 'infEvento'
+        raiz.original_tagname_ = "infEvento"
 
         return raiz
 
     def nfe_recepcao_evento(self, chave, cnpj_cpf, tpEvento, descEvento, xJust=None):
         """
         Envia a manifestação do destinatário para o WS
         :param cnpj_cpf:   CPF ou CNPJ
@@ -175,22 +167,23 @@
                              Operacao nao Realizada
         :param xJust:      Este campo deve ser informado somente no
                              evento de Operação não realizada
         :return:
         """
 
         evento = self.nfe_recepcao_monta_evento(
-            chave, cnpj_cpf, tpEvento, descEvento, xJust=xJust)
+            chave, cnpj_cpf, tpEvento, descEvento, xJust=xJust
+        )
 
         # TODO: Verificar possibilidade de adaptar e utilizar código existente
         #  em self.enviar_lote_evento(lista_eventos=[evento]).
         #  A única diferença é a classe utilizada pelo evento
 
         return self.nfe_recepcao_envia_lote_evento(
-            lista_eventos=[evento], numero_lote='1'
+            lista_eventos=[evento], numero_lote="1"
         )
 
     def confirmacao_da_operacao(self, chave, cnpj_cpf):
         return self.nfe_recepcao_evento(
             chave,
             cnpj_cpf,
             eventoManifestacao._2_10200,
@@ -215,25 +208,26 @@
 
     def operacao_nao_realizada(self, chave, cnpj_cpf):
         return self.nfe_recepcao_evento(
             chave,
             cnpj_cpf,
             eventoManifestacao._2_10240,
             descEventoManifestacao.OPERACAONAO_REALIZADA,
-            xJust=''.zfill(15)
+            xJust="".zfill(15),
         )
 
     def analisar_retorno_raw(self, operacao, raiz, xml, retorno, classe):
         """
         Semelhante ao metodo generico, mas usando o primeiro filho
         do XML da resposta.
         """
         retorno.raise_for_status()
-        match = re.search('<soap:Body>(.*?)</soap:Body>',
-                          retorno.text.replace('\n', ''))
+        match = re.search(
+            "<soap:Body>(.*?)</soap:Body>", retorno.text.replace("\n", "")
+        )
         if match:
             xml_resposta = match.group(1)
             xml = etree.fromstring(xml_resposta)[0]
             if "nfeDistDFeInteresseResult" in xml.tag:
                 xml = xml[0]  # unwrapp retDistDFeInt
             resultado = etree.tostring(xml)
             classe.Validate_simpletypes_ = False
@@ -242,78 +236,70 @@
 
     def _post(self, raiz, url, operacao, classe):
         from .nfe import SIGLA_ESTADO
 
         xml_string, xml_etree = self._generateds_to_string_etree(raiz)
         with self._transmissao.cliente(url):
             # Recupera a sigla do estado
-            uf_list = [uf for nUF, uf in SIGLA_ESTADO.items() if
-                       nUF == str(getattr(raiz, 'cUFAutor', ''))]
-            if uf_list:
-                kwargs = dict(uf=uf_list and uf_list[0])
-            else:
-                kwargs = {}
-            retorno = self._transmissao.enviar(
-                operacao, xml_etree, **kwargs
-            )
+            uf_list = [
+                uf
+                for nUF, uf in SIGLA_ESTADO.items()
+                if nUF == str(getattr(raiz, "cUFAutor", ""))
+            ]
+            kwargs = {"uf": uf_list[0]} if uf_list else {}
+            retorno = self._transmissao.enviar(operacao, xml_etree, **kwargs)
             return self.analisar_retorno_raw(
                 operacao, raiz, xml_string, retorno, classe
             )
 
 
 class TransmissaoMDE(TransmissaoSOAP):
     def interpretar_mensagem(self, mensagem, **kwargs):
         # TODO: Finalizar refatoração
-        if type(mensagem) == str:
-            return etree.fromstring(mensagem, parser=etree.XMLParser(
-                remove_blank_text=True
-            ))
+        if isinstance(mensagem, str):
+            return etree.fromstring(
+                mensagem, parser=etree.XMLParser(remove_blank_text=True)
+            )
 
-        operacao = kwargs.get('operacao', '')
-        uf = kwargs.get('uf', '')
+        operacao = kwargs.get("operacao", "")
+        uf = kwargs.get("uf", "")
 
         if operacao and uf:
             _soapheaders = []
-            xmlns = 'http://www.portalfiscal.inf.br/nfe/wsdl/'
+            xmlns = "http://www.portalfiscal.inf.br/nfe/wsdl/"
 
-            if 'distDFeInt' in mensagem.tag:
-                mensagem = dict(nfeDadosMsg=mensagem)
-            elif 'TEnvEvento' in mensagem.tag:
-                xmlns += 'NFeRecepcaoEvento4'
-                mensagem = dict(nfeCabecMsg=mensagem)
-            elif operacao == 'nfeRecepcaoEvento' and 'consStatServ' in mensagem.tag:
-                xmlns += 'RecepcaoEvento'
-                mensagem = dict(mensagem=mensagem)
+            if "distDFeInt" in mensagem.tag:
+                mensagem = {"nfeDadosMsg": mensagem}
+            elif "TEnvEvento" in mensagem.tag:
+                xmlns += "NFeRecepcaoEvento4"
+                mensagem = {"nfeCabecMsg": mensagem}
+            elif operacao == "nfeRecepcaoEvento" and "consStatServ" in mensagem.tag:
+                xmlns += "RecepcaoEvento"
+                mensagem = {"mensagem": mensagem}
 
             if isinstance(mensagem, dict):
-                header_str = \
-                    '<nfeCabecMsg xmlns="{}">' \
-                    '<cUF>{}</cUF>' \
-                    '<versaoDados>{}</versaoDados>' \
-                    '</nfeCabecMsg>'.format(
-                        xmlns, uf, mensagem.get('versao', '1.00'))
+                header_str = (
+                    '<nfeCabecMsg xmlns="{}">'
+                    "<cUF>{}</cUF>"
+                    "<versaoDados>{}</versaoDados>"
+                    "</nfeCabecMsg>".format(xmlns, uf, mensagem.get("versao", "1.00"))
+                )
 
                 _soapheaders.append(etree.fromstring(header_str))
-                mensagem['_soapheaders'] = _soapheaders
+                mensagem["_soapheaders"] = _soapheaders
 
         return mensagem
 
     def enviar(self, operacao, mensagem, **kwargs):
-
-        kwargs['operacao'] = operacao
+        kwargs["operacao"] = operacao
         mensagem = self.interpretar_mensagem(mensagem, **kwargs)
         with self._cliente.settings(raw_response=self.raw_response):
             if isinstance(mensagem, dict):
                 # TODO: Remover necessidade desse IF
-                if operacao == 'nfeRecepcaoEvento' and 'consStatServ' in mensagem.tag:
+                if operacao == "nfeRecepcaoEvento" and "consStatServ" in mensagem.tag:
                     return self._cliente.service[operacao](
-                        mensagem,
-                        _soapheaders=mensagem.get('_soapheaders')
+                        mensagem, _soapheaders=mensagem.get("_soapheaders")
                     )
 
                 # TODO: Juntar dois retornos em um
-                return self._cliente.service[operacao](
-                    **mensagem
-                )
-            return self._cliente.service[operacao](
-                mensagem
-            )
+                return self._cliente.service[operacao](**mensagem)
+            return self._cliente.service[operacao](mensagem)
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/mdfe.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/mdfe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,48 @@
-# coding=utf-8
 # Copyright (C) 2019  Luis Felipe Mileo - KMEE
 
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
 
+import binascii
 import datetime
 import time
-import binascii
-import base64
 
-from erpbrasil.assinatura.assinatura import Assinatura
 from lxml import etree
 
 from erpbrasil.edoc.edoc import DocumentoEletronico
 
 try:
     # Consulta Status
-    from nfelib.mdfe.bindings.v3_0.cons_stat_serv_mdfe_v3_00 import ConsStatServMdfe
-    from nfelib.mdfe.bindings.v3_0.ret_cons_stat_serv_mdfe_v3_00 import RetConsStatServMdfe
+    # Consulta Não Encerrados
+    from nfelib.mdfe.bindings.v3_0.cons_mdfe_nao_enc_v3_00 import ConsMdfeNaoEnc
+
+    # Consulta Recibo
+    from nfelib.mdfe.bindings.v3_0.cons_reci_mdfe_v3_00 import ConsReciMdfe
 
     # Consulta Documento
     from nfelib.mdfe.bindings.v3_0.cons_sit_mdfe_v3_00 import ConsSitMdfe
-    from nfelib.mdfe.bindings.v3_0.ret_cons_sit_mdfe_v3_00 import RetConsSitMdfe
-
-    # Consulta Não Encerrados
-    from nfelib.mdfe.bindings.v3_0.cons_mdfe_nao_enc_v3_00 import ConsMdfeNaoEnc
-    from nfelib.mdfe.bindings.v3_0.ret_cons_mdfe_nao_enc_v3_00 import RetConsMdfeNaoEnc
+    from nfelib.mdfe.bindings.v3_0.cons_stat_serv_mdfe_v3_00 import ConsStatServMdfe
 
     # Envio
     from nfelib.mdfe.bindings.v3_0.envi_mdfe_v3_00 import EnviMdfe
-    from nfelib.mdfe.bindings.v3_0.ret_envi_mdfe_v3_00 import RetEnviMdfe
+    from nfelib.mdfe.bindings.v3_0.ev_canc_mdfe_v3_00 import EvCancMdfe
+    from nfelib.mdfe.bindings.v3_0.ev_enc_mdfe_v3_00 import EvEncMdfe
 
-    # Consulta Recibo
-    from nfelib.mdfe.bindings.v3_0.cons_reci_mdfe_v3_00 import ConsReciMdfe
-    from nfelib.mdfe.bindings.v3_0.ret_cons_reci_mdfe_v3_00 import RetConsReciMdfe
+    # Eventos
+    from nfelib.mdfe.bindings.v3_0.evento_mdfe_v3_00 import EventoMdfe
 
     # Processamento
     from nfelib.mdfe.bindings.v3_0.proc_mdfe_v3_00 import MdfeProc
-
-    # Eventos
-    from nfelib.mdfe.bindings.v3_0.evento_mdfe_v3_00 import EventoMdfe
+    from nfelib.mdfe.bindings.v3_0.ret_cons_mdfe_nao_enc_v3_00 import RetConsMdfeNaoEnc
+    from nfelib.mdfe.bindings.v3_0.ret_cons_reci_mdfe_v3_00 import RetConsReciMdfe
+    from nfelib.mdfe.bindings.v3_0.ret_cons_sit_mdfe_v3_00 import RetConsSitMdfe
+    from nfelib.mdfe.bindings.v3_0.ret_cons_stat_serv_mdfe_v3_00 import (
+        RetConsStatServMdfe,
+    )
+    from nfelib.mdfe.bindings.v3_0.ret_envi_mdfe_v3_00 import RetEnviMdfe
     from nfelib.mdfe.bindings.v3_0.ret_evento_mdfe_v3_00 import RetEventoMdfe
-    from nfelib.mdfe.bindings.v3_0.ev_canc_mdfe_v3_00 import EvCancMdfe
-    from nfelib.mdfe.bindings.v3_0.ev_enc_mdfe_v3_00 import EvEncMdfe
 except ImportError:
     pass
 
 WS_MDFE_CONSULTA = "MDFeConsulta"
 WS_MDFE_SITUACAO = "MDFeStatusServico"
 WS_MDFE_CONSULTA_NAO_ENCERRADOS = "MDFeConsNaoEnc"
 WS_MDFE_DISTRIBUICAO = "MDFeDistribuicaoDFe"
@@ -80,52 +75,54 @@
         WS_MDFE_RET_RECEPCAO: "ws/MDFeRetRecepcao/MDFeRetRecepcao.asmx?wsdl",
         WS_MDFE_RECEPCAO_EVENTO: "ws/MDFeRecepcaoEvento/MDFeRecepcaoEvento.asmx?wsdl",
         WS_MDFE_CONSULTA: "ws/MDFeConsulta/MDFeConsulta.asmx?wsdl",
         WS_MDFE_SITUACAO: "ws/MDFeStatusServico/MDFeStatusServico.asmx?wsdl",
         WS_MDFE_CONSULTA_NAO_ENCERRADOS: "ws/MDFeConsNaoEnc/MDFeConsNaoEnc.asmx?wsdl",
         WS_MDFE_DISTRIBUICAO: "ws/MDFeDistribuicaoDFe/MDFeDistribuicaoDFe.asmx?wsdl",
         WS_MDFE_RECEPCAO_SINC: "ws/MDFeRecepcaoSinc/MDFeRecepcaoSinc.asmx?wsdl",
-    }
+    },
 }
 
 QR_CODE_URL = "https://dfe-portal.svrs.rs.gov.br/mdfe/qrCode"
 
 NAMESPACES = {
     "mdfe": "http://www.portalfiscal.inf.br/mdfe",
     "ds": "http://www.w3.org/2000/09/xmldsig#",
 }
 
+
 def localizar_url(servico, ambiente=2):
     dominio = SVC_RS[ambiente]["servidor"]
     complemento = SVC_RS[ambiente][servico]
 
-    return "https://%s/%s" % (dominio, complemento)
+    return f"https://{dominio}/{complemento}"
 
 
 class MDFe(DocumentoEletronico):
     _namespace = "http://www.portalfiscal.inf.br/mdfe"
 
     _edoc_situacao_arquivo_recebido_com_sucesso = "103"
     _edoc_situacao_servico_em_operacao = "107"
     _edoc_situacao_ja_enviado = ("100", "101", "132")
 
     _consulta_servico_ao_enviar = True
     _maximo_tentativas_consulta_recibo = 5
 
-    def __init__(self, transmissao, uf, versao="3.00", ambiente="2",
-                 mod="58"):
-        super(MDFe, self).__init__(transmissao)
+    def __init__(self, transmissao, uf, versao="3.00", ambiente="2", mod="58"):
+        super().__init__(transmissao)
         self.versao = str(versao)
         self.ambiente = str(ambiente)
         self.uf = int(uf)
         self.mod = str(mod)
 
     def _verifica_resposta_envio_sucesso(self, proc_envio):
-        return proc_envio.resposta.cStat == \
-            self._edoc_situacao_arquivo_recebido_com_sucesso
+        return (
+            proc_envio.resposta.cStat
+            == self._edoc_situacao_arquivo_recebido_com_sucesso
+        )
 
     def _verifica_servico_em_operacao(self, proc_servico):
         return proc_servico.resposta.cStat == self._edoc_situacao_servico_em_operacao
 
     def _aguarda_tempo_medio(self, proc_envio):
         time.sleep(float(proc_envio.resposta.infRec.tMed) * 1.3)
 
@@ -137,39 +134,39 @@
 
     def monta_qrcode(self, chave):
         return f"{QR_CODE_URL}?chMDFe={chave}&tpAmb={self.ambiente}"
 
     def monta_qrcode_contingencia(self, edoc, xml_assinado):
         chave = edoc.infMDFe.Id.replace("MDFe", "")
 
-        xml = ET.fromstring(xml_assinado)
-        digest_value = xml.find('.//ds:DigestValue', namespaces=NAMESPACES).text
+        xml = etree.fromstring(xml_assinado)
+        digest_value = xml.find(".//ds:DigestValue", namespaces=NAMESPACES).text
         digest_value_hex = binascii.hexlify(digest_value.encode()).decode()
 
         return f"{self.monta_qrcode(chave)}&sign={digest_value_hex}"
 
     def status_servico(self):
         return self._post(
             ConsStatServMdfe(tpAmb=self.ambiente, versao=self.versao),
             localizar_url(WS_MDFE_SITUACAO, int(self.ambiente)),
-            "mdfeStatusServicoMDF" ,
-            RetConsStatServMdfe
+            "mdfeStatusServicoMDF",
+            RetConsStatServMdfe,
         )
 
     def consulta_documento(self, chave):
         raiz = ConsSitMdfe(
             versao=self.versao,
             tpAmb=self.ambiente,
             chMDFe=chave,
         )
         return self._post(
             raiz,
             localizar_url(WS_MDFE_CONSULTA, int(self.ambiente)),
             "mdfeConsultaMDF",
-            RetConsSitMdfe
+            RetConsSitMdfe,
         )
 
     def consulta_nao_encerrados(self, cnpj):
         raiz = ConsMdfeNaoEnc(
             versao=self.versao,
             tpAmb=self.ambiente,
             CNPJ=cnpj,
@@ -190,22 +187,22 @@
 
         :param edoc:
         :return:
         """
         raiz = EnviMdfe(
             versao=self.versao,
             idLote=datetime.datetime.now().strftime("%Y%m%d%H%M%S"),
-            MDFe=edoc
+            MDFe=edoc,
         )
         xml_assinado = self.assina_raiz(raiz, edoc.infMDFe.Id)
         return self._post(
             xml_assinado,
             localizar_url(WS_MDFE_RECEPCAO, int(self.ambiente)),
             "mdfeRecepcaoLote",
-            RetEnviMdfe
+            RetEnviMdfe,
         )
 
     def consulta_recibo(self, numero=False, proc_envio=False):
         if proc_envio:
             numero = proc_envio.resposta.infRec.nRec
 
         if not numero:
@@ -220,18 +217,18 @@
             raiz,
             localizar_url(WS_MDFE_RET_RECEPCAO, int(self.ambiente)),
             "mdfeRetRecepcao",
             RetConsReciMdfe,
         )
 
     def monta_processo(self, edoc, proc_envio, proc_recibo):
-        mdfe = proc_envio.envio_raiz.find('{' + self._namespace + '}MDFe')
+        mdfe = proc_envio.envio_raiz.find("{" + self._namespace + "}MDFe")
         protocolos = proc_recibo.resposta.protMDFe
         if mdfe and protocolos:
-            if type(protocolos) != list:
+            if not isinstance(protocolos, list):
                 protocolos = [protocolos]
             for protocolo in protocolos:
                 mdfe_proc = MdfeProc(versao=self.versao, protMDFe=protocolo)
                 proc_recibo.processo = mdfe_proc
                 proc_recibo.processo_xml = mdfe_proc.to_xml()
                 proc_recibo.protocolo = protocolo
 
@@ -242,50 +239,43 @@
             tpAmb=self.ambiente,
             CNPJ=chave[6:20],
             chMDFe=chave,
             dhEvento=data_hora or self._hora_agora(),
             tpEvento=tipo,
             nSeqEvento=sequencia,
             detEvento=EventoMdfe.InfEvento.DetEvento(
-                versaoEvento="3.00",
-                any_element=evento
+                versaoEvento="3.00", any_element=evento
             ),
         )
         raiz = EventoMdfe(versao="3.00", infEvento=inf_evento)
         xml_assinado = etree.fromstring(self.assina_raiz(raiz, raiz.infEvento.Id))
 
         return self._post(
             xml_assinado,
             localizar_url(WS_MDFE_RECEPCAO_EVENTO, int(self.ambiente)),
             "mdfeRecepcaoEvento",
-            RetEventoMdfe
+            RetEventoMdfe,
         )
 
-    def cancela_documento(self, chave, protocolo_autorizacao, justificativa,
-                          data_hora_evento=False):
+    def cancela_documento(
+        self, chave, protocolo_autorizacao, justificativa, data_hora_evento=False
+    ):
         evento_canc = EvCancMdfe(
-            descEvento="Cancelamento",
-            nProt=protocolo_autorizacao,
-            xJust=justificativa
+            descEvento="Cancelamento", nProt=protocolo_autorizacao, xJust=justificativa
         )
         return self.envia_evento(
-            evento=evento_canc,
-            tipo="110111",
-            chave=chave,
-            data_hora=data_hora_evento
+            evento=evento_canc, tipo="110111", chave=chave, data_hora=data_hora_evento
         )
 
-    def encerra_documento(self, chave, protocolo_autorizacao, estado, municipio,
-                          data_hora_evento=False):
+    def encerra_documento(
+        self, chave, protocolo_autorizacao, estado, municipio, data_hora_evento=False
+    ):
         encerramento = EvEncMdfe(
             descEvento="Encerramento",
             dtEnc=self._data_hoje(),
             nProt=protocolo_autorizacao,
             cUF=estado,
-            cMun=municipio
+            cMun=municipio,
         )
         return self.envia_evento(
-            evento=encerramento,
-            tipo="110112",
-            chave=chave,
-            data_hora=data_hora_evento
+            evento=encerramento, tipo="110112", chave=chave, data_hora=data_hora_evento
         )
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/nfce.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfce.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-# coding=utf-8
 # Copyright (C) 2023 Ygor de Carvalho - KMEE
 
+import binascii
 import datetime
 import hashlib
 import xml.etree.ElementTree as ET
-import binascii
+from contextlib import suppress
 
 from lxml import etree
 
-from erpbrasil.edoc.nfe import SIGLA_ESTADO, NFe, localizar_url, WS_NFE_AUTORIZACAO
+from erpbrasil.edoc.nfe import SIGLA_ESTADO, WS_NFE_AUTORIZACAO, NFe, localizar_url
 
-try:
+with suppress(ImportError):
     from nfelib.v4_00 import retEnviNFe
-    from nfelib.v4_00.retEnviNFe import infNFeSuplType
-except ImportError:
-    pass
 
 
 NFCE_AMBIENTE_PRODUCAO = "1"
 NFCE_AMBIENTE_HOMOLOGACAO = "2"
 
 ESTADO_QRCODE = {
     "AC": {
@@ -245,20 +242,29 @@
 NAMESPACES = {
     "nfe": "http://www.portalfiscal.inf.br/nfe",
     "ds": "http://www.w3.org/2000/09/xmldsig#",
 }
 
 
 class NFCe(NFe):
-    _edoc_situacao_arquivo_recebido_com_sucesso = '104'
+    _edoc_situacao_arquivo_recebido_com_sucesso = "104"
 
-    def __init__(self, transmissao, uf, versao="4.00", ambiente="2", mod="65",
-                 qrcode_versao="2", csc_token=None, csc_code=None):
-        super().__init__(transmissao, uf, versao, ambiente)
-        self.mod = str(mod)
+    def __init__(
+        self,
+        transmissao,
+        uf,
+        versao="4.00",
+        ambiente="2",
+        mod="65",
+        qrcode_versao="2",
+        csc_token=None,
+        csc_code=None,
+        envio_sincrono=True,
+    ):
+        super().__init__(transmissao, uf, versao, ambiente, mod, envio_sincrono)
         self.qrcode_versao = str(qrcode_versao)
         self.csc_token = str(csc_token)
         self.csc_code = str(csc_code)
 
     def monta_qrcode(self, chave):
         pre_qrcode = self._build_pre_qrcode(chave)
         pre_qrcode_with_csc = pre_qrcode + f"{self.csc_code}"
@@ -269,29 +275,40 @@
         return f"{nfce_chave}|{self.qrcode_versao}|{self.ambiente}|{self.csc_token}"
 
     def _compute_qr_hash(self, pre_qrcode_with_csc):
         hash_object = hashlib.sha1(pre_qrcode_with_csc.encode("utf-8"))
         return hash_object.hexdigest().upper()
 
     def _build_qrcode(self, pre_qrcode, qr_hash):
-        return f"{ESTADO_QRCODE[SIGLA_ESTADO[str(self.uf)]][self.ambiente]}{pre_qrcode}|{qr_hash}"
+        return (
+            f"{ESTADO_QRCODE[SIGLA_ESTADO[str(self.uf)]][self.ambiente]}"
+            f"{pre_qrcode}|{qr_hash}"
+        )
 
     @property
     def consulta_qrcode_url(self):
         return ESTADO_CONSULTA_NFCE[SIGLA_ESTADO[str(self.uf)]][self.ambiente]
 
     def _generate_qrcode_contingency(self, edoc, xml_assinado):
         xml = ET.fromstring(xml_assinado)
         chave_nfce = edoc.infNFe.Id.replace("NFe", "")
         data_emissao = edoc.infNFe.ide.dhEmi[8:10]
-        total_nfe = xml.find(".//nfe:total/nfe:ICMSTot/nfe:vNF", namespaces=NAMESPACES).text
-        digest_value = xml.find('.//ds:DigestValue', namespaces=NAMESPACES).text
+        total_nfe = xml.find(
+            ".//nfe:total/nfe:ICMSTot/nfe:vNF", namespaces=NAMESPACES
+        ).text
+        digest_value = xml.find(".//ds:DigestValue", namespaces=NAMESPACES).text
         digest_value_hex = binascii.hexlify(digest_value.encode()).decode()
-        pre_qrcode_witouth_csc = f"{chave_nfce}|{self.qrcode_versao}|{self.ambiente}|{data_emissao}|{total_nfe}|{digest_value_hex}|{self.csc_token}"
-        pre_qrcode = f"{chave_nfce}|{self.qrcode_versao}|{self.ambiente}|{data_emissao}|{total_nfe}|{digest_value_hex}|{self.csc_token}{self.csc_code}"
+        pre_qrcode_witouth_csc = (
+            f"{chave_nfce}|{self.qrcode_versao}|{self.ambiente}|{data_emissao}"
+            f"|{total_nfe}|{digest_value_hex}|{self.csc_token}"
+        )
+        pre_qrcode = (
+            f"{chave_nfce}|{self.qrcode_versao}|{self.ambiente}|{data_emissao}"
+            f"|{total_nfe}|{digest_value_hex}|{self.csc_token}{self.csc_code}"
+        )
         qr_hash = self._compute_qr_hash(pre_qrcode)
         return self._build_qrcode(pre_qrcode_witouth_csc, qr_hash)
 
     def _update_qrcode_nfce_contingency(self, edoc, xml_assinado):
         text = self._generate_qrcode_contingency(edoc, xml_assinado)
         edoc.infNFeSupl.qrCode = text
 
@@ -303,37 +320,36 @@
         # Therefore, it is necessary that there is a change in the generation
         #   of QR COde. And, as one of the necessary values is the digestValue,
         #   calculated during the signature, it is necessary that the edoc
         #   values be updated and signed again so as not to cause a divergence
         #   in the signature with Sefaz.
 
         root = ET.fromstring(xml_assinado)
-        tp_emis = root.find('.//nfe:tpEmis', namespaces=NAMESPACES).text
+        tp_emis = root.find(".//nfe:tpEmis", namespaces=NAMESPACES).text
 
         if tp_emis != "1":
             self._update_qrcode_nfce_contingency(edoc, xml_assinado)
             xml_assinado = self.assina_raiz(edoc, edoc.infNFe.Id)
 
         raiz = retEnviNFe.TEnviNFe(
             versao=self.versao,
-            idLote=datetime.datetime.now().strftime('%Y%m%d%H%M%S'),
-            indSinc='1'
-        )
-        raiz.original_tagname_ = 'enviNFe'
-        xml_envio_string, xml_envio_etree = self._generateds_to_string_etree(
-            raiz
+            idLote=datetime.datetime.now().strftime("%Y%m%d%H%M%S"),
+            indSinc="1" if self.envio_sincrono else "0",
         )
+        raiz.original_tagname_ = "enviNFe"
+        xml_envio_string, xml_envio_etree = self._generateds_to_string_etree(raiz)
         xml_envio_etree.append(etree.fromstring(xml_assinado))
 
         return self._post(
             xml_envio_etree,
-            localizar_url(WS_NFE_AUTORIZACAO, str(self.uf), self.mod,
-                          int(self.ambiente)),
-            'nfeAutorizacaoLote',
-            retEnviNFe
+            localizar_url(
+                WS_NFE_AUTORIZACAO, str(self.uf), self.mod, int(self.ambiente)
+            ),
+            "nfeAutorizacaoLote",
+            retEnviNFe,
         )
 
     def _aguarda_tempo_medio(self, proc_envio):
         pass
 
     def consulta_recibo(self, proc_envio):
         # Since NFCe is synchronous it is not necessary to consult the receipt,
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/nfse.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/nfse.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,94 +1,87 @@
-# coding=utf-8
 # Copyright (C) 2019  Luis Felipe Mileo - KMEE
 
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
 
 import collections
 import time
 
 from erpbrasil.edoc.edoc import DocumentoEletronico
 from erpbrasil.edoc.resposta import analisar_retorno
 
 try:
     from urllib.parse import urljoin
 except ImportError:
     from urlparse import urljoin
 
 
 ServicoNFSe = collections.namedtuple(
-    'ServicoNFSe', ['operacao', 'endpoint', 'classe_retorno', 'assinar']
+    "ServicoNFSe", ["operacao", "endpoint", "classe_retorno", "assinar"]
 )
 
 
 class NFSe(DocumentoEletronico):
     _consulta_servico_ao_enviar = False
     _maximo_tentativas_consulta_recibo = 10
     _tempo_medio = 1
     _header = False
     _namespace = False
 
     _edoc_situacao_arquivo_recebido_com_sucesso = "TODO"
     _edoc_situacao_em_processamento = "TODO"
     _edoc_situacao_servico_em_operacao = "TODO"
 
-    def __init__(self, transmissao, ambiente, cidade_ibge, cnpj_prestador,
-                 im_prestador):
+    def __init__(
+        self, transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+    ):
         self.ambiente = ambiente
         self.cidade = cidade_ibge
         self.cnpj_prestador = cnpj_prestador
         self.im_prestador = im_prestador
-        super(NFSe, self).__init__(transmissao)
+        super().__init__(transmissao)
 
     def _post(self, body, servico):
         header_string = None
         if self._header:
-            header_string, header_etree = self._generateds_to_string_etree(
-                self._header
-            )
+            header_string, header_etree = self._generateds_to_string_etree(self._header)
 
         body_string, body_etree = self._generateds_to_string_etree(body)
 
         # TODO: Verificar impacto para outros provedores
         header = body_etree.find("Cabecalho")
 
         if header and header.attrib:
-            header_string = header.attrib.get('Versao')
+            header_string = header.attrib.get("Versao")
 
         if header_string:
             with self._transmissao.cliente(
-                    urljoin(self._url, servico.endpoint)) as cliente:
+                urljoin(self._url, servico.endpoint)
+            ) as cliente:
                 resposta = cliente.service[servico.operacao](
                     header_string,
                     body_string,
                 )
         else:
             with self._transmissao.cliente(
-                    urljoin(self._url, servico.endpoint)) as cliente:
+                urljoin(self._url, servico.endpoint)
+            ) as cliente:
                 resposta = cliente.service[servico.operacao](
                     body_string,
                 )
 
         return analisar_retorno(
-            servico.operacao,
-            body,
-            body_string,
-            resposta,
-            servico.classe_retorno
+            servico.operacao, body, body_string, resposta, servico.classe_retorno
         )
 
     def _aguarda_tempo_medio(self, proc_envio):
         time.sleep(self._tempo_medio)
 
     def envia_documento(self, edoc):
         return self._post(
             body=self._prepara_envia_documento(edoc),
-            servico=self._servicos[self.envia_documento.__name__]
+            servico=self._servicos[self.envia_documento.__name__],
         )
 
     def consulta_recibo(self, proc_envio):
         return self._post(
             body=self._prepara_consulta_recibo(proc_envio),
             servico=self._servicos[self.consulta_recibo.__name__],
         )
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/barueri.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/barueri.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,198 +1,198 @@
-# coding=utf-8
 # Copyright (C) 2023  Luis Felipe Mileo - KMEE
 
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
 
 import xml.etree.ElementTree as ET
-from xml.dom import minidom
-from lxml import etree
 from datetime import datetime
 
-from erpbrasil.base import misc
+from lxml import etree
 
-from base64 import b64encode
-from erpbrasil.edoc.nfse import NFSe
-from erpbrasil.edoc.nfse import ServicoNFSe
+from erpbrasil.base import misc
+from erpbrasil.edoc.nfse import NFSe, ServicoNFSe
 
 try:
-    from nfselib.barueri import NFeLoteEnviarArquivo
-    from nfselib.barueri import NFeLoteStatusArquivo
-    from nfselib.barueri import ConsultarNFeRecebidaNumero
+    from nfselib.barueri import (
+        ConsultarNFeRecebidaNumero,
+        NFeLoteEnviarArquivo,
+        NFeLoteStatusArquivo,
+    )
+
     barueri = True
 except ImportError:
     barueri = False
 
-endpoint = 'nfeservice/wsrps.asmx?WSDL'
-nsmap = {'consulta': 'http://www.barueri.sp.gov.br/nfe/ConsultaNFeRecebidaNumero'
-                             'ConsultaNFeRecebidaNumero.v1.xsd',
-                 'tipo': 'https://servicos.barueri.sp.gov.br/nfewsxml/wsgeraxml.asmx?op=ConsultaNFeRecebidaCompetencia'}
+endpoint = "nfeservice/wsrps.asmx?WSDL"
+nsmap = {
+    "consulta": "http://www.barueri.sp.gov.br/nfe/ConsultaNFeRecebidaNumero"
+    "ConsultaNFeRecebidaNumero.v1.xsd",
+    "tipo": "https://servicos.barueri.sp.gov.br/nfewsxml/wsgeraxml.asmx?op=ConsultaNFeRecebidaCompetencia",
+}
 
 if barueri:
     servicos = {
-        'envia_documento': ServicoNFSe(
-            'NFeLoteEnviarArquivo',
-            endpoint, NFeLoteEnviarArquivo, True),
-        'consulta_recibo': ServicoNFSe(
-            'NFeLoteStatusArquivo',
-            endpoint, NFeLoteStatusArquivo, True),
-        'consultar_lote_rps': ServicoNFSe(
-            'NFeLoteStatusArquivo',
-            endpoint, NFeLoteStatusArquivo, True),
-        'consulta_nfse_rps': ServicoNFSe(
-            'ConsultarNFeRecebidaNumero',
-            endpoint, ConsultarNFeRecebidaNumero, True),
+        "envia_documento": ServicoNFSe(
+            "NFeLoteEnviarArquivo", endpoint, NFeLoteEnviarArquivo, True
+        ),
+        "consulta_recibo": ServicoNFSe(
+            "NFeLoteStatusArquivo", endpoint, NFeLoteStatusArquivo, True
+        ),
+        "consultar_lote_rps": ServicoNFSe(
+            "NFeLoteStatusArquivo", endpoint, NFeLoteStatusArquivo, True
+        ),
+        "consulta_nfse_rps": ServicoNFSe(
+            "ConsultarNFeRecebidaNumero", endpoint, ConsultarNFeRecebidaNumero, True
+        ),
     }
 else:
     servicos = {}
     cabecalho = None
 
 
 class Barueri(NFSe):
-    
-    def __init__(self, transmissao, ambiente, cidade_ibge, cnpj_prestador,
-                 im_prestador):
-        
-        if ambiente == '2':
-            self._url = 'https://testeeiss.barueri.sp.gov.br/'
+    def __init__(
+        self, transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+    ):
+        if ambiente == "2":
+            self._url = "https://testeeiss.barueri.sp.gov.br/"
         else:
-            self._url = 'https://www.barueri.sp.gov.br/'
+            self._url = "https://www.barueri.sp.gov.br/"
         self._servicos = servicos
-        
-        super(Barueri, self).__init__(
-            transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador)
-        
+
+        super().__init__(
+            transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+        )
+
     def get_documento_id(self, edoc):
         # edoc.LoteRps.ListaRps.Rps[0].InfRps.Id
         return edoc.LoteRps.Id, edoc.LoteRps.NumeroLote
-        
+
     def _prepara_envia_documento(self, edoc):
         numero_lote = self._gera_numero_lote()
         xml_string, xml_etree = self._generateds_to_string_etree(edoc)
-        root = etree.Element("NFeLoteEnviarArquivo", xmlns="http://www.barueri.sp.gov.br/nfe")
+        root = etree.Element(
+            "NFeLoteEnviarArquivo", xmlns="http://www.barueri.sp.gov.br/nfe"
+        )
         versao_schema = etree.SubElement(root, "VersaoSchema")
         versao_schema.text = "1"
         mensagem_xml = etree.SubElement(root, "MensagemXML")
         mensagem_xml.text = etree.CDATA(xml_string)
-        edoc.ApenasValidaArq = 'lote' + numero_lote
+        edoc.ApenasValidaArq = "lote" + numero_lote
         return root
 
     def _prepara_consulta_recibo(self, proc_envio):
         raiz = NFeLoteStatusArquivo.ConsultarSituacaoLoteRpsEnvio(
             Prestador=NFeLoteStatusArquivo(
-                CPFCNPJContrib=self.cnpj_prestador,
-                InscricaoMunicipal=self.im_prestador
+                CPFCNPJContrib=self.cnpj_prestador, InscricaoMunicipal=self.im_prestador
             ),
-            ProtocoloRemessa=proc_envio.resposta.Protocolo
+            ProtocoloRemessa=proc_envio.resposta.Protocolo,
         )
         return self.assina_raiz(raiz, "")
-    
+
     def _prepara_consultar_lote_rps(self, protocolo):
         raiz = NFeLoteStatusArquivo(
             Prestador=NFeLoteStatusArquivo.tcIdentificacaoPrestador(
-                CPFCNPJContrib=self.cnpj_prestador,
-                InscricaoMunicipal=self.im_prestador
+                CPFCNPJContrib=self.cnpj_prestador, InscricaoMunicipal=self.im_prestador
             ),
-            ProtocoloRemessa=protocolo
+            ProtocoloRemessa=protocolo,
         )
         xml_assinado = self.assina_raiz(raiz, raiz.Id)
         return xml_assinado
-    
+
     def _verifica_resposta_envio_sucesso(self, proc_envio):
         if proc_envio.resposta.Protocolo:
             return True
         return False
 
     def _edoc_situacao_em_processamento(self, proc_recibo):
         return proc_recibo.resposta.Situacao == 2
-    
+
     def _prepara_cancelar_nfse_envio(self, doc_numero):
         pass
-    
+
     def _prepara_consultar_nfse_rps(self, **kwargs):
-        rps_numero = kwargs.get('rps_number')
+        rps_numero = kwargs.get("rps_number")
         raiz = ConsultarNFeRecebidaNumero(
             IdentificacaoRps=ConsultarNFeRecebidaNumero(
                 NumeroNota=rps_numero,
             ),
             Prestador=ConsultarNFeRecebidaNumero(
                 CPFCNPJPrestador=self.cnpj_prestador,
             ),
         )
-        
-        return self.assina_raiz(raiz, '')
 
-    def analisa_retorno_consulta(self, processo, number, company_cnpj_cpf,
-                                 company_legal_name):
+        return self.assina_raiz(raiz, "")
+
+    def analisa_retorno_consulta(
+        self, processo, number, company_cnpj_cpf, company_legal_name
+    ):
         retorno = ET.fromstring(processo.retorno)
-        mensagem = ''
-        if processo.webservice == 'NFeRecebidaNumero':
-            enviado = retorno.findall(
-                ".//consulta:CompNfse", namespaces=nsmap)
+        mensagem = ""
+        if processo.webservice == "NFeRecebidaNumero":
+            enviado = retorno.findall(".//consulta:CompNfse", namespaces=nsmap)
             nao_encontrado = retorno.findall(
-                ".//tipo:MensagemRetorno", namespaces=nsmap)
+                ".//tipo:MensagemRetorno", namespaces=nsmap
+            )
 
             if enviado:
                 # NFS-e já foi enviada
 
                 cancelada = retorno.findall(
-                    ".//tipo:NfseCancelamento", namespaces=nsmap)
+                    ".//tipo:NfseCancelamento", namespaces=nsmap
+                )
 
                 if cancelada:
                     # NFS-e enviada foi cancelada
 
-                    data = retorno.findall(
-                        ".//tipo:DataHora", namespaces=nsmap)[0].text
-                    data = datetime.strptime(data, '%Y-%m-%dT%H:%M:%S'). \
-                        strftime("%m/%d/%Y")
-                    mensagem = 'NFS-e cancelada em ' + data
+                    data = retorno.findall(".//tipo:DataHora", namespaces=nsmap)[0].text
+                    data = datetime.strptime(data, "%Y-%m-%dT%H:%M:%S").strftime(
+                        "%m/%d/%Y"
+                    )
+                    mensagem = "NFS-e cancelada em " + data
 
                 else:
-                    numero_retorno = \
-                        retorno.findall(".//tipo:InfNfse/tipo:Numero",
-                                        namespaces=nsmap)[0].text
+                    numero_retorno = retorno.findall(
+                        ".//tipo:InfNfse/tipo:Numero", namespaces=nsmap
+                    )[0].text
                     cnpj_prestador_retorno = retorno.findall(
-                        ".//tipo:IdentificacaoPrestador/tipo:Cnpj",
-                        namespaces=nsmap)[0].text
+                        ".//tipo:IdentificacaoPrestador/tipo:Cnpj", namespaces=nsmap
+                    )[0].text
                     razao_social_prestador_retorno = retorno.findall(
-                        ".//tipo:PrestadorServico/tipo:RazaoSocial",
-                        namespaces=nsmap)[0].text
+                        ".//tipo:PrestadorServico/tipo:RazaoSocial", namespaces=nsmap
+                    )[0].text
 
                     variables_error = []
 
                     if numero_retorno != number:
-                        variables_error.append('Número')
-                    if cnpj_prestador_retorno != misc.punctuation_rm(
-                            company_cnpj_cpf):
-                        variables_error.append('CNPJ do prestador')
+                        variables_error.append("Número")
+                    if cnpj_prestador_retorno != misc.punctuation_rm(company_cnpj_cpf):
+                        variables_error.append("CNPJ do prestador")
                     if razao_social_prestador_retorno != company_legal_name:
-                        variables_error.append('Razão Social de prestador')
+                        variables_error.append("Razão Social de prestador")
 
                     if variables_error:
-                        mensagem = 'Os seguintes campos não condizem com' \
-                                   ' o provedor NFS-e: \n'
-                        mensagem += '\n'.join(variables_error)
+                        mensagem = (
+                            "Os seguintes campos não condizem com"
+                            " o provedor NFS-e: \n"
+                        )
+                        mensagem += "\n".join(variables_error)
                     else:
                         mensagem = "NFS-e enviada e corresponde com o provedor"
 
             elif nao_encontrado:
                 # NFS-e não foi enviada
 
-                mensagem_erro = retorno.findall(
-                    ".//tipo:Mensagem", namespaces=nsmap)[0].text
-                correcao = retorno.findall(
-                    ".//tipo:Correcao", namespaces=nsmap)[0].text
-                codigo = retorno.findall(
-                    ".//tipo:Codigo", namespaces=nsmap)[0].text
-                mensagem = (codigo + ' - ' + mensagem_erro + ' - Correção: ' +
-                            correcao + '\n')
+                mensagem_erro = retorno.findall(".//tipo:Mensagem", namespaces=nsmap)[
+                    0
+                ].text
+                correcao = retorno.findall(".//tipo:Correcao", namespaces=nsmap)[0].text
+                codigo = retorno.findall(".//tipo:Codigo", namespaces=nsmap)[0].text
+                mensagem = (
+                    codigo + " - " + mensagem_erro + " - Correção: " + correcao + "\n"
+                )
 
             else:
-                mensagem = 'Erro desconhecido.'
+                mensagem = "Erro desconhecido."
 
         return mensagem
 
     def analisa_retorno_cancelamento(self, processo):
         pass
-
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/cidades.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/cidades.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-# coding=utf-8
 # Copyright (C) 2019  Luis Felipe Mileo - KMEE
 
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
 
+from erpbrasil.edoc.provedores.barueri import Barueri
 from erpbrasil.edoc.provedores.dsf import Dsf
 from erpbrasil.edoc.provedores.ginfes import Ginfes
 from erpbrasil.edoc.provedores.issnet import Issnet
 from erpbrasil.edoc.provedores.paulistana import Paulistana
-from erpbrasil.edoc.provedores.barueri import Barueri
 
 cidades = {
     1501402: Dsf,  # Belem-PA
     2211001: Dsf,  # Teresina - PI
     3132404: Ginfes,  # ITAJUBA - MG
     3516200: Ginfes,  # Franca - SP
     3170206: Dsf,  # Uberlândia-MG
     3303500: Dsf,  # Nova Iguaçu - RJ
     3509502: Dsf,  # Campinas - SP
     5002704: Dsf,  # Campo Grande - MS
     3550308: Paulistana,  # São Paulo - SP
-    3543402: Issnet,    # Ribeirão Preto - SP
+    3543402: Issnet,  # Ribeirão Preto - SP
     3301702: Issnet,  # Duque de Caxias - RJ
-    3505708: Barueri # Barueri - SP
+    3505708: Barueri,  # Barueri - SP
 }
 
 
 def NFSeFactory(transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador):
     """Factory"""
     return cidades[int(cidade_ibge)](
-        transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador)
+        transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+    )
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/dsf.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/dsf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,77 @@
-# coding=utf-8
 # Copyright (C) 2019  Luis Felipe Mileo - KMEE
 
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
 
 from erpbrasil.edoc.chave import ChaveNFSeDSF
-from erpbrasil.edoc.nfse import NFSe
-from erpbrasil.edoc.nfse import ServicoNFSe
+from erpbrasil.edoc.nfse import NFSe, ServicoNFSe
 
 try:
-    from nfselib.dsf import RetornoConsultaLote
-    from nfselib.dsf import RetornoConsultaNFSeRPS
-    from nfselib.dsf import RetornoEnvioLoteRPS
+    from nfselib.dsf import (
+        RetornoConsultaLote,
+        RetornoConsultaNFSeRPS,
+        RetornoEnvioLoteRPS,
+    )
+
     dsf = True
 except ImportError:
     dsf = False
 
-endpoint = 'WsNFe2/LoteRps.jws'
+endpoint = "WsNFe2/LoteRps.jws"
 
 if dsf:
     servicos_base = {
-        'consulta_recibo': ServicoNFSe(
-            'consultarLote',
-            endpoint, RetornoConsultaLote, True),
-        'consultar_lote_rps': ServicoNFSe(
-            'ConsultarNota',
-            endpoint, RetornoConsultaNFSeRPS, True),
+        "consulta_recibo": ServicoNFSe(
+            "consultarLote", endpoint, RetornoConsultaLote, True
+        ),
+        "consultar_lote_rps": ServicoNFSe(
+            "ConsultarNota", endpoint, RetornoConsultaNFSeRPS, True
+        ),
     }
 
     servicos_hml = {
-        'envia_documento': ServicoNFSe(
-            'testeEnviar',
-            endpoint, RetornoEnvioLoteRPS, True),
+        "envia_documento": ServicoNFSe(
+            "testeEnviar", endpoint, RetornoEnvioLoteRPS, True
+        ),
     }
     servicos_hml.update(servicos_base.copy())
 
     servicos_prod = {
-        'envia_documento': ServicoNFSe(
-            'enviar',
-            endpoint, RetornoEnvioLoteRPS, True),
+        "envia_documento": ServicoNFSe("enviar", endpoint, RetornoEnvioLoteRPS, True),
     }
     servicos_prod.update(servicos_base.copy())
 
     url = {
-        3509502: 'http://issdigital.campinas.sp.gov.br',  # Campinas
-        3170206: 'http://udigital.uberlandia.mg.gov.br',  # Uberlândia-MG
-        1501402: 'http://www.issdigitalbel.com.br',  # Belem-PA
-        5002704: 'http://issdigital.pmcg.ms.gov.br',  # Campo Grande - MS
-        3303500: 'http://www.issmaisfacil.com.br',  # Nova Iguaçu - RJ
-        2211001: 'http://www.issdigitalthe.com.br',  # Teresina - PI
+        3509502: "http://issdigital.campinas.sp.gov.br",  # Campinas
+        3170206: "http://udigital.uberlandia.mg.gov.br",  # Uberlândia-MG
+        1501402: "http://www.issdigitalbel.com.br",  # Belem-PA
+        5002704: "http://issdigital.pmcg.ms.gov.br",  # Campo Grande - MS
+        3303500: "http://www.issmaisfacil.com.br",  # Nova Iguaçu - RJ
+        2211001: "http://www.issdigitalthe.com.br",  # Teresina - PI
         # 2111300 : 'http://www.issdigitalslz.com.br',  # São Luiz - MA
     }
 
 
 class Dsf(NFSe):
-
-    def __init__(self, transmissao, ambiente, cidade_ibge, cnpj_prestador,
-                 im_prestador):
+    def __init__(
+        self, transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+    ):
         # DSS só tem uma URL
         self._url = url[int(cidade_ibge)]
 
         # Não tem URL de homologação mas tem métodos para testes
         # no mesmo webservice
 
-        if ambiente == '2':
+        if ambiente == "2":
             self._servicos = servicos_hml
         else:
             self._servicos = servicos_hml
 
-        super(Dsf, self).__init__(
-            transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador)
+        super().__init__(
+            transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+        )
 
     def envia_documento(self, edoc):
-
         for rps in edoc.Lote.RPS:
             chave = ChaveNFSeDSF(rps=rps)
             rps.Assinatura = chave.hash
 
-        return super(Dsf, self).envia_documento(edoc)
+        return super().envia_documento(edoc)
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/ginfes.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/ginfes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-# coding=utf-8
 # Copyright (C) 2019  Luis Felipe Mileo - KMEE
 
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
 
 import xml.etree.ElementTree as ET
 from datetime import datetime
 
 from erpbrasil.base import misc
-
-from erpbrasil.edoc.nfse import NFSe
-from erpbrasil.edoc.nfse import ServicoNFSe
+from erpbrasil.edoc.nfse import NFSe, ServicoNFSe
 
 try:
-    from nfselib.ginfes.v3_01 import servico_cancelar_nfse_envio
-    from nfselib.ginfes.v3_01 import servico_consultar_lote_rps_envio
-    from nfselib.ginfes.v3_01 import servico_consultar_lote_rps_resposta
-    from nfselib.ginfes.v3_01 import servico_consultar_nfse_rps_envio
-    from nfselib.ginfes.v3_01 import servico_consultar_situacao_lote_rps_envio
-    from nfselib.ginfes.v3_01 import servico_consultar_situacao_lote_rps_resposta
-    from nfselib.ginfes.v3_01 import servico_enviar_lote_rps_resposta
+    from nfselib.ginfes.v3_01 import (
+        servico_cancelar_nfse_envio,
+        servico_consultar_lote_rps_envio,
+        servico_consultar_lote_rps_resposta,
+        servico_consultar_nfse_rps_envio,
+        servico_consultar_situacao_lote_rps_envio,
+        servico_consultar_situacao_lote_rps_resposta,
+        servico_enviar_lote_rps_resposta,
+    )
     from nfselib.ginfes.v3_01.cabecalho import cabecalho
+
     ginfes = True
 except ImportError:
     ginfes = False
 
 
-endpoint = 'ServiceGinfesImpl?wsdl'
+endpoint = "ServiceGinfesImpl?wsdl"
 
 if ginfes:
     servicos = {
-        'envia_documento': ServicoNFSe(
-            'RecepcionarLoteRpsV3',
-            endpoint, servico_enviar_lote_rps_resposta, True),
-        'consulta_recibo': ServicoNFSe(
-            'ConsultarSituacaoLoteRpsV3',
-            endpoint, servico_consultar_situacao_lote_rps_resposta, True),
-        'consultar_lote_rps': ServicoNFSe(
-            'ConsultarLoteRpsV3',
-            endpoint, servico_consultar_lote_rps_resposta, True),
-        'cancela_documento': ServicoNFSe(
-            'CancelarNfseV3',
-            endpoint, servico_cancelar_nfse_envio, True),
-        'consulta_nfse_rps': ServicoNFSe(
-            'ConsultarNfsePorRpsV3',
-            endpoint, servico_cancelar_nfse_envio, True),
+        "envia_documento": ServicoNFSe(
+            "RecepcionarLoteRpsV3", endpoint, servico_enviar_lote_rps_resposta, True
+        ),
+        "consulta_recibo": ServicoNFSe(
+            "ConsultarSituacaoLoteRpsV3",
+            endpoint,
+            servico_consultar_situacao_lote_rps_resposta,
+            True,
+        ),
+        "consultar_lote_rps": ServicoNFSe(
+            "ConsultarLoteRpsV3", endpoint, servico_consultar_lote_rps_resposta, True
+        ),
+        "cancela_documento": ServicoNFSe(
+            "CancelarNfseV3", endpoint, servico_cancelar_nfse_envio, True
+        ),
+        "consulta_nfse_rps": ServicoNFSe(
+            "ConsultarNfsePorRpsV3", endpoint, servico_cancelar_nfse_envio, True
+        ),
     }
     cabecalho = cabecalho(versao="3", versaoDados="3")
 else:
     servicos = {}
     cabecalho = None
 
 
 class Ginfes(NFSe):
     _header = cabecalho
 
-    def __init__(self, transmissao, ambiente, cidade_ibge, cnpj_prestador,
-                 im_prestador):
-
-        if ambiente == '2':
-            self._url = 'https://homologacao.ginfes.com.br'
+    def __init__(
+        self, transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+    ):
+        if ambiente == "2":
+            self._url = "https://homologacao.ginfes.com.br"
         else:
-            self._url = 'https://producao.ginfes.com.br'
+            self._url = "https://producao.ginfes.com.br"
         self._servicos = servicos
 
-        super(Ginfes, self).__init__(
-            transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador)
+        super().__init__(
+            transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+        )
 
     def get_documento_id(self, edoc):
         # edoc.LoteRps.ListaRps.Rps[0].InfRps.Id
         return edoc.LoteRps.Id, edoc.LoteRps.NumeroLote
 
     def _prepara_envia_documento(self, edoc):
         numero_lote = self._gera_numero_lote()
-        edoc.LoteRps.Id = 'lote' + numero_lote
+        edoc.LoteRps.Id = "lote" + numero_lote
         edoc.LoteRps.NumeroLote = int(numero_lote)
         #
         # Assinamos todas as RPS e o Lote
         #
         xml_assinado = edoc
         # for rps in edoc.LoteRps.ListaRps.Rps:
-        #     xml_assinado = self.assin a_raiz(xml_assinado, rps.InfRps.Id, getchildren=True)
+        #     xml_assinado = self.assin a_raiz(
+        #       xml_assinado, rps.InfRps.Id, getchildren=True
+        #     )
         # Assinamos o lote
         # xml_assinado = self.assina_raiz(xml_assinado, edoc.LoteRps.Id)
 
         for rps in edoc.LoteRps.ListaRps.Rps:
             xml_assinado = self.assina_raiz(xml_assinado, rps.InfRps.Id)
         # Assinamos o lote
         # xml_assinado = self.assina_raiz(xml_assinado, edoc.LoteRps.Id)
 
         return xml_assinado
 
     def _prepara_consulta_recibo(self, proc_envio):
-
         raiz = servico_consultar_situacao_lote_rps_envio.ConsultarSituacaoLoteRpsEnvio(
             # Id=self._gera_numero_lote(),
             Prestador=servico_consultar_situacao_lote_rps_envio.tcIdentificacaoPrestador(
-                Cnpj=self.cnpj_prestador,
-                InscricaoMunicipal=self.im_prestador
+                Cnpj=self.cnpj_prestador, InscricaoMunicipal=self.im_prestador
             ),
-            Protocolo=proc_envio.resposta.Protocolo
+            Protocolo=proc_envio.resposta.Protocolo,
         )
         xml_assinado = self.assina_raiz(raiz, "")
         return xml_assinado
 
     def _prepara_consultar_lote_rps(self, protocolo):
         raiz = servico_consultar_lote_rps_envio.ConsultarLoteRpsEnvio(
             Id=self._gera_numero_lote(),
             Prestador=servico_consultar_lote_rps_envio.tcIdentificacaoPrestador(
-                Cnpj=self.cnpj_prestador,
-                InscricaoMunicipal=self.im_prestador
+                Cnpj=self.cnpj_prestador, InscricaoMunicipal=self.im_prestador
             ),
-            Protocolo=protocolo
+            Protocolo=protocolo,
         )
         xml_assinado = self.assina_raiz(raiz, raiz.Id)
         return xml_assinado
 
     def _verifica_resposta_envio_sucesso(self, proc_envio):
         if proc_envio.resposta.Protocolo:
             return True
@@ -132,132 +132,135 @@
             Pedido=servico_cancelar_nfse_envio.tcPedidoCancelamento(
                 InfPedidoCancelamento=servico_cancelar_nfse_envio.tcInfPedidoCancelamento(
                     Id=doc_numero,
                     IdentificacaoNfse=servico_cancelar_nfse_envio.tcIdentificacaoNfse(
                         Numero=doc_numero,
                         Cnpj=self.cnpj_prestador,
                         InscricaoMunicipal=self.im_prestador,
-                        CodigoMunicipio=self.cidade
+                        CodigoMunicipio=self.cidade,
                     ),
-                    CodigoCancelamento='0001'
+                    CodigoCancelamento="0001",
                 )
             )
         )
-        xml_assinado = self.assina_raiz(raiz, '')
+        xml_assinado = self.assina_raiz(raiz, "")
 
         return xml_assinado
 
     def _prepara_consultar_nfse_rps(self, **kwargs):
-        rps_numero = kwargs.get('rps_number')
-        rps_serie = kwargs.get('rps_serie')
-        rps_tipo = kwargs.get('rps_type')
+        rps_numero = kwargs.get("rps_number")
+        rps_serie = kwargs.get("rps_serie")
+        rps_tipo = kwargs.get("rps_type")
 
         raiz = servico_consultar_nfse_rps_envio.ConsultarNfseRpsEnvio(
             IdentificacaoRps=servico_consultar_nfse_rps_envio.tcIdentificacaoRps(
                 Numero=rps_numero,
                 Serie=rps_serie,
                 Tipo=rps_tipo,
             ),
             Prestador=servico_consultar_nfse_rps_envio.tcIdentificacaoPrestador(
-                Cnpj=self.cnpj_prestador,
-                InscricaoMunicipal=self.im_prestador
+                Cnpj=self.cnpj_prestador, InscricaoMunicipal=self.im_prestador
             ),
         )
-        xml_assinado = self.assina_raiz(raiz, '')
+        xml_assinado = self.assina_raiz(raiz, "")
 
         return xml_assinado
 
-    def analisa_retorno_consulta(self, processo, number, company_cnpj_cpf,
-                                 company_legal_name):
+    def analisa_retorno_consulta(
+        self, processo, number, company_cnpj_cpf, company_legal_name
+    ):
         retorno = ET.fromstring(processo.retorno)
-        nsmap = {'consulta': 'http://www.ginfes.com.br/servico_consultar_'
-                             'nfse_rps_resposta_v03.xsd',
-                 'tipo': 'http://www.ginfes.com.br/tipos_v03.xsd'}
-
-        mensagem = ''
-        if processo.webservice == 'ConsultarNfsePorRpsV3':
-            enviado = retorno.findall(
-                ".//consulta:CompNfse", namespaces=nsmap)
+        nsmap = {
+            "consulta": "http://www.ginfes.com.br/servico_consultar_"
+            "nfse_rps_resposta_v03.xsd",
+            "tipo": "http://www.ginfes.com.br/tipos_v03.xsd",
+        }
+
+        mensagem = ""
+        if processo.webservice == "ConsultarNfsePorRpsV3":
+            enviado = retorno.findall(".//consulta:CompNfse", namespaces=nsmap)
             nao_encontrado = retorno.findall(
-                ".//tipo:MensagemRetorno", namespaces=nsmap)
+                ".//tipo:MensagemRetorno", namespaces=nsmap
+            )
 
             if enviado:
                 # NFS-e já foi enviada
 
                 cancelada = retorno.findall(
-                    ".//tipo:NfseCancelamento", namespaces=nsmap)
+                    ".//tipo:NfseCancelamento", namespaces=nsmap
+                )
 
                 if cancelada:
                     # NFS-e enviada foi cancelada
 
-                    data = retorno.findall(
-                        ".//tipo:DataHora", namespaces=nsmap)[0].text
-                    data = datetime.strptime(data, '%Y-%m-%dT%H:%M:%S'). \
-                        strftime("%m/%d/%Y")
-                    mensagem = 'NFS-e cancelada em ' + data
+                    data = retorno.findall(".//tipo:DataHora", namespaces=nsmap)[0].text
+                    data = datetime.strptime(data, "%Y-%m-%dT%H:%M:%S").strftime(
+                        "%m/%d/%Y"
+                    )
+                    mensagem = "NFS-e cancelada em " + data
 
                 else:
-                    numero_retorno = \
-                        retorno.findall(".//tipo:InfNfse/tipo:Numero",
-                                        namespaces=nsmap)[0].text
+                    numero_retorno = retorno.findall(
+                        ".//tipo:InfNfse/tipo:Numero", namespaces=nsmap
+                    )[0].text
                     cnpj_prestador_retorno = retorno.findall(
-                        ".//tipo:IdentificacaoPrestador/tipo:Cnpj",
-                        namespaces=nsmap)[0].text
+                        ".//tipo:IdentificacaoPrestador/tipo:Cnpj", namespaces=nsmap
+                    )[0].text
                     razao_social_prestador_retorno = retorno.findall(
-                        ".//tipo:PrestadorServico/tipo:RazaoSocial",
-                        namespaces=nsmap)[0].text
+                        ".//tipo:PrestadorServico/tipo:RazaoSocial", namespaces=nsmap
+                    )[0].text
 
                     variables_error = []
 
                     if numero_retorno != number:
-                        variables_error.append('Número')
-                    if cnpj_prestador_retorno != misc.punctuation_rm(
-                            company_cnpj_cpf):
-                        variables_error.append('CNPJ do prestador')
+                        variables_error.append("Número")
+                    if cnpj_prestador_retorno != misc.punctuation_rm(company_cnpj_cpf):
+                        variables_error.append("CNPJ do prestador")
                     if razao_social_prestador_retorno != company_legal_name:
-                        variables_error.append('Razão Social de prestador')
+                        variables_error.append("Razão Social de prestador")
 
                     if variables_error:
-                        mensagem = 'Os seguintes campos não condizem com' \
-                                   ' o provedor NFS-e: \n'
-                        mensagem += '\n'.join(variables_error)
+                        mensagem = (
+                            "Os seguintes campos não condizem com"
+                            " o provedor NFS-e: \n"
+                        )
+                        mensagem += "\n".join(variables_error)
                     else:
                         mensagem = "NFS-e enviada e corresponde com o provedor"
 
             elif nao_encontrado:
                 # NFS-e não foi enviada
 
-                mensagem_erro = retorno.findall(
-                    ".//tipo:Mensagem", namespaces=nsmap)[0].text
-                correcao = retorno.findall(
-                    ".//tipo:Correcao", namespaces=nsmap)[0].text
-                codigo = retorno.findall(
-                    ".//tipo:Codigo", namespaces=nsmap)[0].text
-                mensagem = (codigo + ' - ' + mensagem_erro + ' - Correção: ' +
-                            correcao + '\n')
+                mensagem_erro = retorno.findall(".//tipo:Mensagem", namespaces=nsmap)[
+                    0
+                ].text
+                correcao = retorno.findall(".//tipo:Correcao", namespaces=nsmap)[0].text
+                codigo = retorno.findall(".//tipo:Codigo", namespaces=nsmap)[0].text
+                mensagem = (
+                    codigo + " - " + mensagem_erro + " - Correção: " + correcao + "\n"
+                )
 
             else:
-                mensagem = 'Erro desconhecido.'
+                mensagem = "Erro desconhecido."
 
         return mensagem
 
     def analisa_retorno_cancelamento(self, processo):
-        if processo.webservice in ['CancelarNfseV3', 'CancelarNfse']:
-            mensagem_completa = ''
+        if processo.webservice in ["CancelarNfseV3", "CancelarNfse"]:
+            mensagem_completa = ""
             situacao = True
             retorno = ET.fromstring(processo.retorno)
-            nsmap = {'tipo': 'http://www.ginfes.com.br/tipos_v03.xsd'}
+            nsmap = {"tipo": "http://www.ginfes.com.br/tipos_v03.xsd"}
 
             sucesso = retorno.findall(".//tipo:Sucesso", namespaces=nsmap)
             if not sucesso:
-                mensagem_erro = retorno.findall(
-                    ".//tipo:Mensagem", namespaces=nsmap)[0].text
-                correcao = retorno.findall(
-                    ".//tipo:Correcao", namespaces=nsmap)[0].text
-                codigo = retorno.findall(
-                    ".//tipo:Codigo", namespaces=nsmap)[0].text
+                mensagem_erro = retorno.findall(".//tipo:Mensagem", namespaces=nsmap)[
+                    0
+                ].text
+                correcao = retorno.findall(".//tipo:Correcao", namespaces=nsmap)[0].text
+                codigo = retorno.findall(".//tipo:Codigo", namespaces=nsmap)[0].text
                 mensagem_completa += (
-                    codigo + ' - ' + mensagem_erro +
-                    ' - Correção: ' + correcao + '\n')
+                    codigo + " - " + mensagem_erro + " - Correção: " + correcao + "\n"
+                )
                 situacao = False
 
             return situacao, mensagem_completa
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/issnet.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/issnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,95 +1,100 @@
-# coding=utf-8
 # Copyright (C) 2020 - TODAY, Marcel Savegnago - Escodoo
 
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
 
 import xml.etree.ElementTree as ET
 from datetime import datetime
 
 from erpbrasil.base import misc
-
-from erpbrasil.edoc.nfse import NFSe
-from erpbrasil.edoc.nfse import ServicoNFSe
+from erpbrasil.edoc.nfse import NFSe, ServicoNFSe
 
 try:
-    from nfselib.issnet.v1_00 import servico_cancelar_nfse_envio
-    from nfselib.issnet.v1_00 import servico_consultar_lote_rps_envio
-    from nfselib.issnet.v1_00 import servico_consultar_lote_rps_resposta
-    from nfselib.issnet.v1_00 import servico_consultar_nfse_rps_envio
-    from nfselib.issnet.v1_00 import servico_consultar_situacao_lote_rps_envio
-    from nfselib.issnet.v1_00 import servico_consultar_situacao_lote_rps_resposta
-    from nfselib.issnet.v1_00 import servico_enviar_lote_rps_resposta
+    from nfselib.issnet.v1_00 import (
+        servico_cancelar_nfse_envio,
+        servico_consultar_lote_rps_envio,
+        servico_consultar_lote_rps_resposta,
+        servico_consultar_nfse_rps_envio,
+        servico_consultar_situacao_lote_rps_envio,
+        servico_consultar_situacao_lote_rps_resposta,
+        servico_enviar_lote_rps_resposta,
+    )
+
     issnet = True
 except ImportError:
     issnet = False
 
 
 cidade = {
-
-    3543402: 'ribeiraopreto',  # Ribeirão Preto - SP
-    3301702: 'duquedecaxias',  # Duque de Caxias - RJ
-
+    3543402: "ribeiraopreto",  # Ribeirão Preto - SP
+    3301702: "duquedecaxias",  # Duque de Caxias - RJ
 }
 
-endpoint = 'servicos.asmx?WSDL'
+endpoint = "servicos.asmx?WSDL"
 
 if issnet:
     servicos = {
-        'envia_documento': ServicoNFSe(
-            'RecepcionarLoteRps',
-            endpoint, servico_enviar_lote_rps_resposta, True),
-        'consulta_recibo': ServicoNFSe(
-            'ConsultarSituacaoLoteRPS',
-            endpoint, servico_consultar_situacao_lote_rps_resposta, True),
-        'consultar_lote_rps': ServicoNFSe(
-            'ConsultarLoteRps',
-            endpoint, servico_consultar_lote_rps_resposta, True),
-        'cancela_documento': ServicoNFSe(
-            'CancelarNfse',
-            endpoint, servico_cancelar_nfse_envio, True),
-        'consulta_nfse_rps': ServicoNFSe(
-            'ConsultarNFSePorRPS',
-            endpoint, servico_consultar_nfse_rps_envio, True),
+        "envia_documento": ServicoNFSe(
+            "RecepcionarLoteRps", endpoint, servico_enviar_lote_rps_resposta, True
+        ),
+        "consulta_recibo": ServicoNFSe(
+            "ConsultarSituacaoLoteRPS",
+            endpoint,
+            servico_consultar_situacao_lote_rps_resposta,
+            True,
+        ),
+        "consultar_lote_rps": ServicoNFSe(
+            "ConsultarLoteRps", endpoint, servico_consultar_lote_rps_resposta, True
+        ),
+        "cancela_documento": ServicoNFSe(
+            "CancelarNfse", endpoint, servico_cancelar_nfse_envio, True
+        ),
+        "consulta_nfse_rps": ServicoNFSe(
+            "ConsultarNFSePorRPS", endpoint, servico_consultar_nfse_rps_envio, True
+        ),
     }
 else:
     servicos = ()
 
 
 class Issnet(NFSe):
     _header = None
 
-    def __init__(self, transmissao, ambiente, cidade_ibge, cnpj_prestador,
-                 im_prestador):
-
-        if ambiente == '2':
-            self._url = 'https://www.issnetonline.com.br/webserviceabrasf/homologacao/'
+    def __init__(
+        self, transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+    ):
+        if ambiente == "2":
+            self._url = "https://www.issnetonline.com.br/webserviceabrasf/homologacao/"
         else:
-            self._url = 'https://www.issnetonline.com.br/webserviceabrasf/' + cidade[int(cidade_ibge)] + '/'
+            self._url = (
+                "https://www.issnetonline.com.br/webserviceabrasf/"
+                + cidade[int(cidade_ibge)]
+                + "/"
+            )
         self._servicos = servicos
 
-        super(Issnet, self).__init__(
-            transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador)
+        super().__init__(
+            transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+        )
 
     def get_documento_id(self, edoc):
         # edoc.LoteRps.ListaRps.Rps[0].InfRps.Id
         return edoc.LoteRps.id, edoc.LoteRps.NumeroLote
 
     def _prepara_envia_documento(self, edoc):
         numero_lote = self._gera_numero_lote()
-        edoc.LoteRps.id = 'lote' + numero_lote
+        edoc.LoteRps.id = "lote" + numero_lote
         edoc.LoteRps.NumeroLote = int(numero_lote)
         #
         # Assinamos todas as RPS e o Lote
         #
         xml_assinado = edoc
         # for rps in edoc.LoteRps.ListaRps.Rps:
-        #     xml_assinado = self.assin a_raiz(xml_assinado, rps.InfRps.Id, getchildren=True)
+        #     xml_assinado = self.assin a_raiz(
+        #       xml_assinado, rps.InfRps.Id, getchildren=True
+        #     )
         # Assinamos o lote
         # xml_assinado = self.assina_raiz(xml_assinado, edoc.LoteRps.Id)
 
         # for rps in edoc.LoteRps.ListaRps.Rps:
         #     xml_assinado = self.assina_raiz(xml_assinado, rps.InfRps.Id)
         # Assinamos o lote
         xml_assinado = self.assina_raiz(xml_assinado, edoc.LoteRps.id)
@@ -100,33 +105,33 @@
     def _prepara_consulta_recibo(self, proc_envio):
         raiz = servico_consultar_situacao_lote_rps_envio.ConsultarSituacaoLoteRpsEnvio(
             # Id=self._gera_numero_lote(),
             Prestador=servico_consultar_situacao_lote_rps_envio.tcIdentificacaoPrestador(
                 CpfCnpj=servico_consultar_situacao_lote_rps_envio.tcCpfCnpj(
                     Cnpj=self.cnpj_prestador,
                 ),
-                InscricaoMunicipal=self.im_prestador
+                InscricaoMunicipal=self.im_prestador,
             ),
-            Protocolo=proc_envio.resposta.Protocolo
+            Protocolo=proc_envio.resposta.Protocolo,
         )
         # xml_assinado = self.assina_raiz(raiz,"")
         xml_string, xml_etree = self._generateds_to_string_etree(raiz)
         xml_string = '<?xml version="1.0"?>' + xml_string
         return xml_string
 
     def _prepara_consultar_lote_rps(self, protocolo):
         raiz = servico_consultar_lote_rps_envio.ConsultarLoteRpsEnvio(
             # Id=self._gera_numero_lote(),
             Prestador=servico_consultar_lote_rps_envio.tcIdentificacaoPrestador(
                 CpfCnpj=servico_consultar_lote_rps_envio.tcCpfCnpj(
                     Cnpj=self.cnpj_prestador,
                 ),
-                InscricaoMunicipal=self.im_prestador
+                InscricaoMunicipal=self.im_prestador,
             ),
-            Protocolo=protocolo
+            Protocolo=protocolo,
         )
         # xml_assinado = self.assina_raiz(raiz, raiz.Id)
         xml_string, xml_etree = self._generateds_to_string_etree(raiz)
         xml_string = '<?xml version="1.0"?>' + xml_string
         return xml_string
 
     def _verifica_resposta_envio_sucesso(self, proc_envio):
@@ -143,170 +148,179 @@
         raiz = servico_cancelar_nfse_envio.tcPedidoCancelamento(
             InfPedidoCancelamento=servico_cancelar_nfse_envio.tcInfPedidoCancelamento(
                 id=doc_numero,
                 IdentificacaoNfse=servico_cancelar_nfse_envio.tcIdentificacaoNfse(
                     Numero=doc_numero,
                     Cnpj=self.cnpj_prestador,
                     InscricaoMunicipal=self.im_prestador,
-                    CodigoMunicipio=self.cidade
-                    if self.ambiente == '1'
-                    else 999,
+                    CodigoMunicipio=self.cidade if self.ambiente == "1" else 999,
                 ),
-                CodigoCancelamento='0001'
+                CodigoCancelamento="0001",
             )
         )
 
-        # Foi codificado desta forma porque a assinatura fica dentro da tag Pedido. Acredito que de para melhorar.
-        pedido = self.assina_raiz(raiz, '')
-
-        xml_assinado = '<?xml version="1.0"?>' \
-                       '<p1:CancelarNfseEnvio ' \
-                       'xmlns:p1="http://www.issnetonline.com.br/webserviceabrasf/vsd/servico_cancelar_nfse_envio.xsd" ' \
-                       'xmlns:tc="http://www.issnetonline.com.br/webserviceabrasf/vsd/tipos_complexos.xsd" ' \
-                       'xmlns:ts="http://www.issnetonline.com.br/webserviceabrasf/vsd/tipos_simples.xsd">' \
-                       + pedido + '</p1:CancelarNfseEnvio>'
+        # Foi codificado desta forma porque a assinatura fica dentro da tag Pedido.
+        # Acredito que de para melhorar.
+        pedido = self.assina_raiz(raiz, "")
+
+        # flake8: noqa: E501
+        xml_assinado = (
+            '<?xml version="1.0"?>'
+            "<p1:CancelarNfseEnvio "
+            'xmlns:p1="http://www.issnetonline.com.br/webserviceabrasf/vsd/servico_cancelar_nfse_envio.xsd" '
+            'xmlns:tc="http://www.issnetonline.com.br/webserviceabrasf/vsd/tipos_complexos.xsd" '
+            'xmlns:ts="http://www.issnetonline.com.br/webserviceabrasf/vsd/tipos_simples.xsd">'
+            + pedido
+            + "</p1:CancelarNfseEnvio>"
+        )
 
-        xml_assinado = xml_assinado.replace('tcPedidoCancelamento', 'Pedido')
+        xml_assinado = xml_assinado.replace("tcPedidoCancelamento", "Pedido")
 
         return xml_assinado
 
     def _prepara_consultar_nfse_rps(self, **kwargs):
-        rps_numero = kwargs.get('rps_number')
-        rps_serie = kwargs.get('rps_serie')
-        rps_tipo = kwargs.get('rps_type')
+        rps_numero = kwargs.get("rps_number")
+        rps_serie = kwargs.get("rps_serie")
+        rps_tipo = kwargs.get("rps_type")
 
         raiz = servico_consultar_nfse_rps_envio.ConsultarNfseRpsEnvio(
             IdentificacaoRps=servico_consultar_nfse_rps_envio.tcIdentificacaoRps(
                 Numero=rps_numero,
                 Serie=rps_serie,
                 Tipo=rps_tipo,
             ),
             Prestador=servico_consultar_nfse_rps_envio.tcIdentificacaoPrestador(
                 CpfCnpj=servico_consultar_nfse_rps_envio.tcCpfCnpj(
                     Cnpj=self.cnpj_prestador,
                 ),
-                InscricaoMunicipal=self.im_prestador
+                InscricaoMunicipal=self.im_prestador,
             ),
         )
         xml_string, xml_etree = self._generateds_to_string_etree(raiz)
         xml_string = '<?xml version="1.0"?>' + xml_string
 
         return xml_string
 
-    def analisa_retorno_consulta(self, processo, number, company_cnpj_cpf,
-                                 company_legal_name):
-        mensagem = ''
+    def analisa_retorno_consulta(
+        self, processo, number, company_cnpj_cpf, company_legal_name
+    ):
+        mensagem = ""
         res = {}
         retorno = ET.fromstring(processo.retorno)
-        nsmap = {'consulta': 'http://www.issnetonline.com.br/webserviceabrasf/vsd/'
-                             'servico_consultar_nfse_rps_resposta.xsd',
-                 'tc': 'http://www.issnetonline.com.br/webserviceabrasf/vsd/'
-                       'tipos_complexos.xsd'}
-
-        if processo.webservice == 'ConsultarNFSePorRPS':
-            enviado = retorno.findall(
-                ".//consulta:CompNfse", namespaces=nsmap)
+        nsmap = {
+            "consulta": "http://www.issnetonline.com.br/webserviceabrasf/vsd/"
+            "servico_consultar_nfse_rps_resposta.xsd",
+            "tc": "http://www.issnetonline.com.br/webserviceabrasf/vsd/"
+            "tipos_complexos.xsd",
+        }
+
+        if processo.webservice == "ConsultarNFSePorRPS":
+            enviado = retorno.findall(".//consulta:CompNfse", namespaces=nsmap)
             nao_encontrado = retorno.findall(
-                ".//consulta:MensagemRetorno", namespaces=nsmap)
+                ".//consulta:MensagemRetorno", namespaces=nsmap
+            )
 
             if enviado:
                 # NFS-e já foi enviada
 
                 cancelada = retorno.findall(
-                    ".//consulta:NfseCancelamento", namespaces=nsmap)
+                    ".//consulta:NfseCancelamento", namespaces=nsmap
+                )
 
                 if cancelada:
                     # NFS-e enviada foi cancelada
 
-                    data = retorno.findall(
-                        ".//consulta:DataHora", namespaces=nsmap)[0].text
-                    data = datetime.strptime(data, '%Y-%m-%dT%H:%M:%S'). \
-                        strftime("%m/%d/%Y")
-                    mensagem = 'NFS-e cancelada em ' + data
+                    data = retorno.findall(".//consulta:DataHora", namespaces=nsmap)[
+                        0
+                    ].text
+                    data = datetime.strptime(data, "%Y-%m-%dT%H:%M:%S").strftime(
+                        "%m/%d/%Y"
+                    )
+                    mensagem = "NFS-e cancelada em " + data
 
                 else:
-                    numero_retorno = \
-                        retorno.findall(".//tc:InfNfse/tc:Numero",
-                                        namespaces=nsmap)[0].text
+                    numero_retorno = retorno.findall(
+                        ".//tc:InfNfse/tc:Numero", namespaces=nsmap
+                    )[0].text
                     cnpj_prestador_retorno = retorno.findall(
                         ".//tc:IdentificacaoPrestador/tc:CpfCnpj/tc:Cnpj",
-                        namespaces=nsmap)[0].text
+                        namespaces=nsmap,
+                    )[0].text
                     razao_social_prestador_retorno = retorno.findall(
-                        ".//tc:PrestadorServico/tc:RazaoSocial",
-                        namespaces=nsmap)[0].text
-                    verify_code = \
-                        retorno.findall(".//tc:InfNfse/tc:CodigoVerificacao",
-                                        namespaces=nsmap)[0].text
-                    authorization_date = \
-                        retorno.findall(".//tc:InfNfse/tc:DataEmissao",
-                                        namespaces=nsmap)[0].text
+                        ".//tc:PrestadorServico/tc:RazaoSocial", namespaces=nsmap
+                    )[0].text
+                    verify_code = retorno.findall(
+                        ".//tc:InfNfse/tc:CodigoVerificacao", namespaces=nsmap
+                    )[0].text
+                    authorization_date = retorno.findall(
+                        ".//tc:InfNfse/tc:DataEmissao", namespaces=nsmap
+                    )[0].text
                     variables_error = []
 
                     if number and numero_retorno != number:
-                        variables_error.append('Número')
-                    if cnpj_prestador_retorno != misc.punctuation_rm(
-                            company_cnpj_cpf):
-                        variables_error.append('CNPJ do prestador')
+                        variables_error.append("Número")
+                    if cnpj_prestador_retorno != misc.punctuation_rm(company_cnpj_cpf):
+                        variables_error.append("CNPJ do prestador")
                     if razao_social_prestador_retorno != company_legal_name:
-                        variables_error.append('Razão Social de prestador')
+                        variables_error.append("Razão Social de prestador")
 
                     if variables_error:
-                        mensagem = 'Os seguintes campos não condizem com' \
-                                   ' o provedor NFS-e: \n'
-                        mensagem += '\n'.join(variables_error)
+                        mensagem = (
+                            "Os seguintes campos não condizem com"
+                            " o provedor NFS-e: \n"
+                        )
+                        mensagem += "\n".join(variables_error)
                     else:
                         mensagem = "NFS-e enviada e corresponde com o provedor"
 
-                    res['codigo_verificacao'] = verify_code
-                    res['numero'] = numero_retorno
-                    res['data_emissao'] = authorization_date
+                    res["codigo_verificacao"] = verify_code
+                    res["numero"] = numero_retorno
+                    res["data_emissao"] = authorization_date
                     return mensagem, res
 
             elif nao_encontrado:
                 # NFS-e não foi enviada
 
-                mensagem_erro = retorno.findall(
-                    ".//tc:Mensagem", namespaces=nsmap)[0].text
-                correcao = retorno.findall(
-                    ".//tc:Correcao", namespaces=nsmap)[0].text
-                codigo = retorno.findall(
-                    ".//tc:Codigo", namespaces=nsmap)[0].text
-                mensagem = (codigo + ' - ' + mensagem_erro + ' - Correção: ' +
-                            correcao + '\n')
+                mensagem_erro = retorno.findall(".//tc:Mensagem", namespaces=nsmap)[
+                    0
+                ].text
+                correcao = retorno.findall(".//tc:Correcao", namespaces=nsmap)[0].text
+                codigo = retorno.findall(".//tc:Codigo", namespaces=nsmap)[0].text
+                mensagem = (
+                    codigo + " - " + mensagem_erro + " - Correção: " + correcao + "\n"
+                )
 
             else:
-                mensagem = 'Erro desconhecido.'
+                mensagem = "Erro desconhecido."
 
         return mensagem
 
     def analisa_retorno_cancelamento(self, processo):
-        if processo.webservice in ['CancelarNfse']:
-            mensagem_completa = ''
+        if processo.webservice in ["CancelarNfse"]:
+            mensagem_completa = ""
             situacao = True
             retorno = ET.fromstring(processo.retorno)
 
             sucesso = retorno.findall(
                 ".//{http://www.issnetonline.com.br/webserviceabrasf/vsd/"
-                "tipos_complexos.xsd}Sucesso")
+                "tipos_complexos.xsd}Sucesso"
+            )
             if not sucesso:
                 mensagem_erro = retorno.findall(
                     ".//{http://www.issnetonline.com.br/webserviceabrasf/vsd/"
-                    "tipos_complexos.xsd}Mensagem")[
-                    0].text
+                    "tipos_complexos.xsd}Mensagem"
+                )[0].text
                 correcao = retorno.findall(
                     ".//{http://www.issnetonline.com.br/webserviceabrasf/vsd/"
-                    "tipos_complexos.xsd}Correcao")[
-                    0].text
+                    "tipos_complexos.xsd}Correcao"
+                )[0].text
                 codigo = retorno.findall(
                     ".//{http://www.issnetonline.com.br/webserviceabrasf/vsd/"
-                    "tipos_complexos.xsd}Codigo")[
-                    0].text
-                mensagem_completa += (
-                    codigo + ' - ' +
-                    mensagem_erro
-                )
+                    "tipos_complexos.xsd}Codigo"
+                )[0].text
+                mensagem_completa += codigo + " - " + mensagem_erro
                 if correcao:
-                    mensagem_completa += (' - Correção: ' + correcao + '\n')
+                    mensagem_completa += " - Correção: " + correcao + "\n"
 
                 situacao = False
 
             return situacao, mensagem_completa
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/provedores/paulistana.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/provedores/paulistana.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,197 +1,191 @@
-# coding=utf-8
 # Copyright (C) 2020 KMEE
 
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
 
 import xml.etree.ElementTree as ET
-
 from base64 import b64encode
-from erpbrasil.edoc.nfse import NFSe
-from erpbrasil.edoc.nfse import ServicoNFSe
+
+from erpbrasil.edoc.nfse import NFSe, ServicoNFSe
 
 try:
+    from nfselib.paulistana.v02 import (
+        PedidoCancelamentoNFe,
+        PedidoConsultaLote,
+        PedidoConsultaNFe,
+        RetornoCancelamentoNFe,
+        RetornoConsulta,
+        RetornoEnvioLoteRPS,
+    )
+
     from erpbrasil.assinatura.assinatura import Assinatura
-    from nfselib.paulistana.v02 import PedidoCancelamentoNFe
-    from nfselib.paulistana.v02 import PedidoConsultaLote
-    from nfselib.paulistana.v02 import PedidoConsultaNFe
-    from nfselib.paulistana.v02 import RetornoCancelamentoNFe
-    from nfselib.paulistana.v02 import RetornoConsulta
-    from nfselib.paulistana.v02 import RetornoEnvioLoteRPS
+
     paulistana = True
 except ImportError:
     paulistana = False
 
-endpoint = 'ws/lotenfe.asmx?WSDL'
+endpoint = "ws/lotenfe.asmx?WSDL"
 
 if paulistana:
     servicos_base = {
-        'consulta_recibo': ServicoNFSe(
-            'ConsultaLote',
-            endpoint, RetornoConsulta, True),
-
-        'consulta_nfse_rps': ServicoNFSe(
-            'ConsultaNFe',
-            endpoint, RetornoConsulta, True),
-
-        'cancela_documento': ServicoNFSe(
-            'CancelamentoNFe',
-            endpoint, RetornoCancelamentoNFe, True),
+        "consulta_recibo": ServicoNFSe("ConsultaLote", endpoint, RetornoConsulta, True),
+        "consulta_nfse_rps": ServicoNFSe(
+            "ConsultaNFe", endpoint, RetornoConsulta, True
+        ),
+        "cancela_documento": ServicoNFSe(
+            "CancelamentoNFe", endpoint, RetornoCancelamentoNFe, True
+        ),
     }
 
     servicos_hml = {
-        'envia_documento': ServicoNFSe(
-            'TesteEnvioLoteRPS',
-            endpoint, RetornoEnvioLoteRPS, True),
+        "envia_documento": ServicoNFSe(
+            "TesteEnvioLoteRPS", endpoint, RetornoEnvioLoteRPS, True
+        ),
     }
     servicos_hml.update(servicos_base.copy())
 
     servicos_prod = {
-        'envia_documento': ServicoNFSe(
-            'EnvioLoteRPS',
-            endpoint, RetornoEnvioLoteRPS, True),
+        "envia_documento": ServicoNFSe(
+            "EnvioLoteRPS", endpoint, RetornoEnvioLoteRPS, True
+        ),
     }
     servicos_prod.update(servicos_base.copy())
 
 
 class Paulistana(NFSe):
-
-    def __init__(self, transmissao, ambiente, cidade_ibge, cnpj_prestador,
-                 im_prestador):
-
-        self._url = 'https://nfe.prefeitura.sp.gov.br'
+    def __init__(
+        self, transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+    ):
+        self._url = "https://nfe.prefeitura.sp.gov.br"
 
         # Não tem URL de homologação mas tem métodos para testes
         # no mesmo webservice
 
-        if ambiente == '2':
+        if ambiente == "2":
             self._servicos = servicos_hml
         else:
             self._servicos = servicos_prod
 
-        super(Paulistana, self).__init__(
-            transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador)
+        super().__init__(
+            transmissao, ambiente, cidade_ibge, cnpj_prestador, im_prestador
+        )
 
     def _prepara_envia_documento(self, edoc):
         assinador = Assinatura(self._transmissao.certificado)
         for rps in edoc.RPS:
             data = rps.Assinatura
-            data_bytes = data.encode('ascii')
+            data_bytes = data.encode("ascii")
             assinatura = assinador.sign_pkcs1v15_sha1(data_bytes)
             rps.Assinatura = b64encode(assinatura).decode()
-        xml_assinado = self.assina_raiz(edoc, '')
+        xml_assinado = self.assina_raiz(edoc, "")
         return xml_assinado
 
     def _verifica_resposta_envio_sucesso(self, proc_envio):
         return proc_envio.resposta.Cabecalho.Sucesso
 
     def _edoc_situacao_em_processamento(self, proc_recibo):
         # if proc_recibo.resposta.Situacao == 2:
         #     return True
         # return False
         pass
 
     def _prepara_consulta_recibo(self, proc_envio):
-
         retorno = ET.fromstring(proc_envio.retorno)
-        numero_lote = int(retorno.find('.//NumeroLote').text)
-        cnpj = retorno.find('.//CNPJ').text
+        numero_lote = int(retorno.find(".//NumeroLote").text)
+        cnpj = retorno.find(".//CNPJ").text
 
         edoc = PedidoConsultaLote.PedidoConsultaLote(
             Cabecalho=PedidoConsultaLote.CabecalhoType(
                 Versao=1,
                 CPFCNPJRemetente=PedidoConsultaNFe.tpCPFCNPJ(CNPJ=cnpj),
-                NumeroLote=numero_lote
+                NumeroLote=numero_lote,
             )
         )
 
-        xml_assinado = self.assina_raiz(edoc, '')
+        xml_assinado = self.assina_raiz(edoc, "")
 
         return xml_assinado
 
     def _prepara_consultar_nfse_rps(self, **kwargs):
         cnpj_prestador = kwargs.get("cnpj_prest")
         inscricao_prestador = kwargs.get("insc_prest")
         rps_serie = kwargs.get("serie_rps")
         rps_numero = kwargs.get("numero_rps")
 
         raiz = PedidoConsultaNFe.PedidoConsultaNFe(
             Cabecalho=PedidoConsultaNFe.CabecalhoType(
                 Versao=1,
-                CPFCNPJRemetente=PedidoConsultaNFe.tpCPFCNPJ(CNPJ=cnpj_prestador)
+                CPFCNPJRemetente=PedidoConsultaNFe.tpCPFCNPJ(CNPJ=cnpj_prestador),
             ),
-            Detalhe=[PedidoConsultaNFe.DetalheType(
-                ChaveRPS=PedidoConsultaNFe.tpChaveRPS(
-                    InscricaoPrestador=int(inscricao_prestador),
-                    SerieRPS=rps_serie,
-                    NumeroRPS=int(rps_numero),
-                ),
-            )],
+            Detalhe=[
+                PedidoConsultaNFe.DetalheType(
+                    ChaveRPS=PedidoConsultaNFe.tpChaveRPS(
+                        InscricaoPrestador=int(inscricao_prestador),
+                        SerieRPS=rps_serie,
+                        NumeroRPS=int(rps_numero),
+                    ),
+                )
+            ],
         )
 
-        xml_assinado = self.assina_raiz(raiz, '')
+        xml_assinado = self.assina_raiz(raiz, "")
 
         return xml_assinado
 
     def analisa_retorno_consulta(self, processo):
-        retorno_mensagem = ''
+        retorno_mensagem = ""
         res = {}
         if processo.resposta.Cabecalho.Sucesso:
             retorno = ET.fromstring(processo.retorno)
-            res['codigo_verificacao'] = \
-                retorno.find('.//CodigoVerificacao').text
-            res['numero'] = retorno.find('.//NumeroNFe').text
-            res['data_emissao'] = retorno.find('.//DataEmissaoNFe').text
+            res["codigo_verificacao"] = retorno.find(".//CodigoVerificacao").text
+            res["numero"] = retorno.find(".//NumeroNFe").text
+            res["data_emissao"] = retorno.find(".//DataEmissaoNFe").text
             return res
         else:
-            retorno_mensagem = 'Error communicating with the webservice'
+            retorno_mensagem = "Error communicating with the webservice"
             return retorno_mensagem
 
     def _prepara_cancelar_nfse_envio(self, doc_numero):
-        numero_nfse = doc_numero.get('numero_nfse')
-        codigo_verificacao = doc_numero.get('codigo_verificacao') or ''
+        numero_nfse = doc_numero.get("numero_nfse")
+        codigo_verificacao = doc_numero.get("codigo_verificacao") or ""
 
         assinatura = self.im_prestador.zfill(8)
         assinatura += numero_nfse.zfill(12)
 
         raiz = PedidoCancelamentoNFe.PedidoCancelamentoNFe(
             Cabecalho=PedidoCancelamentoNFe.CabecalhoType(
                 Versao=1,
                 CPFCNPJRemetente=PedidoConsultaNFe.tpCPFCNPJ(CNPJ=self.cnpj_prestador),
             ),
-            Detalhe=[PedidoCancelamentoNFe.DetalheType(
-                ChaveNFe=PedidoCancelamentoNFe.tpChaveNFe(
-                    InscricaoPrestador=int(self.im_prestador),
-                    NumeroNFe=int(numero_nfse),
-                    CodigoVerificacao=codigo_verificacao.zfill(8),
-                ),
-                AssinaturaCancelamento=assinatura,
-            )],
+            Detalhe=[
+                PedidoCancelamentoNFe.DetalheType(
+                    ChaveNFe=PedidoCancelamentoNFe.tpChaveNFe(
+                        InscricaoPrestador=int(self.im_prestador),
+                        NumeroNFe=int(numero_nfse),
+                        CodigoVerificacao=codigo_verificacao.zfill(8),
+                    ),
+                    AssinaturaCancelamento=assinatura,
+                )
+            ],
         )
 
         assinador = Assinatura(self._transmissao.certificado)
         for detalhe in raiz.Detalhe:
             data = detalhe.AssinaturaCancelamento
-            data_bytes = data.encode('ascii')
+            data_bytes = data.encode("ascii")
             assinatura = assinador.sign_pkcs1v15_sha1(data_bytes)
             detalhe.AssinaturaCancelamento = b64encode(assinatura).decode()
-        xml_assinado = self.assina_raiz(raiz, '')
+        xml_assinado = self.assina_raiz(raiz, "")
         return xml_assinado
 
     def analisa_retorno_cancelamento_paulistana(self, processo):
-        retorno_mensagem = ''
+        retorno_mensagem = ""
         status = True
         if not processo.resposta.Cabecalho.Sucesso:
             status = False
             for erro in processo.resposta.Erro:
-                retorno_mensagem = \
-                    str(erro.Codigo) + ' - ' + erro.Descricao + '\n'
+                retorno_mensagem = str(erro.Codigo) + " - " + erro.Descricao + "\n"
         return status, retorno_mensagem
 
     def assina_raiz(self, raiz, id, getchildren=False):
         xml_string, xml_etree = self._generateds_to_string_etree(raiz)
-        xml_assinado = Assinatura(self._transmissao.certificado).assina_nfse(
-            xml_etree
-        )
+        xml_assinado = Assinatura(self._transmissao.certificado).assina_nfse(xml_etree)
         return xml_assinado
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil/edoc/resposta.py` & `erpbrasil.edoc-2.8.0/src/erpbrasil/edoc/resposta.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,47 @@
-# -*- coding: utf-8 -*-
 # Copyright (C) 2018 - TODAY Luis Felipe Mileo - KMEE INFORMATICA LTDA
 # License MIT
 
 import re
 
 from lxml import etree
 
 
-class RetornoSoap(object):
-
+class RetornoSoap:
     def __init__(self, webservice, raiz, xml, retorno, resposta):
         self.webservice = webservice
         self.envio_raiz = raiz
         self.envio_xml = xml
         self.resposta = resposta
         self.retorno = retorno
 
 
 def analisar_retorno_raw(operacao, raiz, xml, retorno, classe):
     retorno.raise_for_status()
-    match = re.search('<soap:Body>(.*?)</soap:Body>',
-                      retorno.text.replace('\n', ''))
+    match = re.search("<soap:Body>(.*?)</soap:Body>", retorno.text.replace("\n", ""))
     if match:
         xml_resposta = match.group(1)
         xml_etree = etree.fromstring(xml_resposta)
         resultado = xml_etree[0]
 
         nome_classe = classe.__name__.split(".")[-1]
-        xml_classe_tags = list(filter(
-            lambda children: nome_classe in children.tag,
-            xml_etree.findall(".//")
-        ))
+        xml_classe_tags = list(
+            filter(
+                lambda children: nome_classe in children.tag, xml_etree.findall(".//")
+            )
+        )
         if xml_classe_tags:
             resultado = xml_classe_tags[0]
 
         resultado = etree.tostring(resultado)
         classe.Validate_simpletypes_ = False
         resposta = classe.parseString(resultado, silence=True)
         return RetornoSoap(operacao, raiz, xml, retorno, resposta)
 
 
 def analisar_retorno(operacao, raiz, xml, retorno, classe):
     resposta = False
     if retorno:
         classe.Validate_simpletypes_ = False
-        resultado = etree.tostring(
-            etree.fromstring(retorno.encode('utf-8')))
+        resultado = etree.tostring(etree.fromstring(retorno.encode("utf-8")))
         resposta = classe.parseString(resultado, silence=True)
     return RetornoSoap(operacao, raiz, xml, retorno, resposta)
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/PKG-INFO` & `erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: erpbrasil.edoc
-Version: 2.7.1
+Version: 2.8.0
 Summary: Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 Home-page: https://github.com/erpbrasil/erpbrasil.edoc
 Author: Luis Felipe Mileo
 Author-email: mileo@kmee.com.br
 License: MIT
 Project-URL: Documentation, https://erpbrasiledoc.readthedocs.io/
 Project-URL: Changelog, https://erpbrasiledoc.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/erpbrasil/erpbrasil.edoc/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
@@ -20,42 +21,43 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
-Provides-Extra: nfselib.ginfes
-Provides-Extra: nfselib.paulistana
-Provides-Extra: nfselib.dsf
+Provides-Extra: mdfelib
+Provides-Extra: nfelib
 Provides-Extra: nfselib.betha
+Provides-Extra: nfselib.dsf
+Provides-Extra: nfselib.ginfes
 Provides-Extra: nfselib.issnet
-Provides-Extra: nfelib
-Provides-Extra: mdfelib
+Provides-Extra: nfselib.paulistana
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 Overview
 ========
 
 
 
-Emissão de documentos fiscais e outras obrigações (NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
+Emissão de documentos fiscais e outras obrigações
+(NF-E, NFS-E, MDF-E, CT-E, REINF, E-SOCIAL)
 
 
 Documentação
 ============
 
 https://erpbrasil.github.io/
 
 Créditos
 ========
 
-Esta é uma biblioteca criada atravês do esforço de das empresas:
+Esta é uma biblioteca criada através do esforço das empresas:
 
 * Akretion https://akretion.com/pt-BR/
 * KMEE https://www.kmee.com.br
 
 Favor consultar a lista de contribuidores:
 
 https://github.com/erpbrasil/erpbrasil.edoc/graphs/contributors
@@ -64,18 +66,19 @@
 ~~~~~~~
 
 * Free software: MIT license
 
 Instalação
 ==========
 
-Para permitir que a instalação do seu ERP cresça somente com a necessidade do cliente
-é possível instalar as dependências da biblioteca de forma opcional:
+Para permitir que a instalação do seu ERP cresça somente com a necessidade
+do cliente é possível instalar as dependências da biblioteca de forma opcional:
 
 ::
+
     pip install erpbrasil.edoc
 
     # Documentos do Sefaz
 
     pip install erpbrasil.edoc[nfelib] # Emissão de NF-e
     pip install erpbrasil.edoc[mdfelib] # Emissão de Manifesto de Carga - MD
     pip install erpbrasil.edoc[ctelib] # Emissão de CT-e
@@ -171,7 +174,8 @@
 - Consulta Cadastro
 
 2.2.0 (2021-05-26)
 ~~~~~~~~~~~~~~~~~~
 
 - Nota Paulistana
 
+
```

### Comparing `erpbrasil.edoc-2.7.1/src/erpbrasil.edoc.egg-info/SOURCES.txt` & `erpbrasil.edoc-2.8.0/src/erpbrasil.edoc.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-.appveyor.yml
 .bumpversion.cfg
 .cookiecutterrc
 .coveragerc
 .editorconfig
-.travis.yml
+.pre-commit-config.yaml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
-ci/appveyor-bootstrap.py
-ci/appveyor-download.py
-ci/appveyor-with-compiler.cmd
+.github/workflows/github-actions.yml
+.github/workflows/pre-commit.yml
 ci/bootstrap.py
 ci/requirements.txt
-ci/templates/.appveyor.yml
-ci/templates/.travis.yml
-ci/templates/appveyor.yml
+ci/templates/.github/workflows/github-actions.yml
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/readme.rst
@@ -57,20 +54,22 @@
 src/erpbrasil/edoc/provedores/__init__.py
 src/erpbrasil/edoc/provedores/barueri.py
 src/erpbrasil/edoc/provedores/cidades.py
 src/erpbrasil/edoc/provedores/dsf.py
 src/erpbrasil/edoc/provedores/ginfes.py
 src/erpbrasil/edoc/provedores/issnet.py
 src/erpbrasil/edoc/provedores/paulistana.py
+tests/__init__.py
+tests/test_certificate_mixin.py
 tests/test_erpbrasil_edoc.py
 tests/test_erpbrasil_edoc_manifestacao.py
+tests/test_erpbrasil_edoc_nfe.py
 tests/test_erpbrasil_edoc_nfse_ginfes.py
 tests/test_erpbrasil_edoc_nfse_paulistana.py
 tests/test_erpbrasil_edoc_situacao.py
-tests/fixtures/dummy_cert.pfx
 tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml
 tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml
 tests/fixtures/vcr_cassettes/test_chave.yaml
 tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml
 tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml
 tests/fixtures/vcr_cassettes/test_consulta_documento.yaml
 tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml
```

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_cancelar_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_cancelar_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_chave.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 interactions:
 - request:
     body: '<?xml version=''1.0'' encoding=''utf-8''?>
 
       <soap-env:Envelope xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/"><soap-env:Header><nfeCabecMsg
       xmlns="http://www.portalfiscal.inf.br/nfe/wsdl/"><cUF>SP</cUF><versaoDados>1.00</versaoDados></nfeCabecMsg></soap-env:Header><soap-env:Body><ns0:nfeDistDFeInteresse
       xmlns:ns0="http://www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe"><ns0:nfeDadosMsg><distDFeInt
-      xmlns="http://www.portalfiscal.inf.br/nfe" versao="1.01"><tpAmb>1</tpAmb><cUFAutor>35</cUFAutor><CNPJ>23765766000162</CNPJ><consChNFe><chNFe>35200309091076000144550010001807401003642343</chNFe></consChNFe></distDFeInt></ns0:nfeDadosMsg></ns0:nfeDistDFeInteresse></soap-env:Body></soap-env:Envelope>'
+      xmlns="http://www.portalfiscal.inf.br/nfe" versao="1.01"><tpAmb>1</tpAmb><cUFAutor>35</cUFAutor><CNPJ>23765766000162</CNPJ><consNSU><NSU>000000000000001</NSU></consNSU></distDFeInt></ns0:nfeDadosMsg></ns0:nfeDistDFeInteresse></soap-env:Body></soap-env:Envelope>'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '710'
+      - '673'
       Content-Type:
       - text/xml; charset=utf-8
       SOAPAction:
       - '"http://www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe/nfeDistDFeInteresse"'
       User-Agent:
       - Zeep/3.4.0 (www.python-zeep.org)
     method: POST
     uri: https://www1.nfe.fazenda.gov.br/NFeDistribuicaoDFe/NFeDistribuicaoDFe.asmx
   response:
     body:
       string: <?xml version="1.0" encoding="utf-8"?><soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
-        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"><soap:Header><WSCorIDSOAPHeader
-        CorID="E54B8CD1C8C6EFB5033F1B4700000000,1:1,0,0,SPCDSRVV4733|.NET Process|NFeDistribuicaoDFe|WebServices|Server|http_//www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe|nfeDistDFeInteresse,1,AgAAALNIQgAAAAFGAAAAAQAAABFqYXZhLnV0aWwuSGFzaE1hcAAAAAJIQgAAAAJGAAAAAgAAABBqYXZhLmxhbmcuU3RyaW5nAA9DYWxsZXJUaW1lc3RhbXBIQgAAAANFAAAAAgANMTYwNTg2OTczNTEyMUhCAAAABEUAAAACAApUeG5UcmFjZUlkSEIAAAAFRQAAAAIAIUU1NEI4QzQ0QzhDNkVGQjUwMzNGMUI0NzAwMDAwMDAwMA=="
-        xmlns="http://www.ca.com/apm" /></soap:Header><soap:Body><nfeDistDFeInteresseResponse
+        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"><soap:Body><nfeDistDFeInteresseResponse
         xmlns="http://www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe"><nfeDistDFeInteresseResult><retDistDFeInt
         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         versao="1.01" xmlns="http://www.portalfiscal.inf.br/nfe"><tpAmb>1</tpAmb><verAplic>1.2.1</verAplic><cStat>137</cStat><xMotivo>Nenhum
-        documento localizado</xMotivo><dhResp>2020-11-20T07:55:35-03:00</dhResp></retDistDFeInt></nfeDistDFeInteresseResult></nfeDistDFeInteresseResponse></soap:Body></soap:Envelope>
+        documento localizado</xMotivo><dhResp>2020-11-20T07:55:35-03:00</dhResp><ultNSU>000000000000051</ultNSU><maxNSU>000000000020175</maxNSU></retDistDFeInt></nfeDistDFeInteresseResult></nfeDistDFeInteresseResponse></soap:Body></soap:Envelope>
     headers:
       Cache-Control:
       - private, max-age=0
       Content-Length:
-      - '1283'
+      - '826'
       Content-Type:
       - text/xml; charset=utf-8
       Date:
-      - Fri, 20 Nov 2020 10:55:34 GMT
+      - Fri, 20 Nov 2020 10:55:33 GMT
       Server:
       - Microsoft-IIS/8.5
       X-AspNet-Version:
       - 4.0.30319
       X-Powered-By:
       - ASP.NET
     status:
```

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 interactions:
 - request:
     body: '<?xml version=''1.0'' encoding=''utf-8''?>
 
       <soap-env:Envelope xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/"><soap-env:Body><ns0:nfeDadosMsg
       xmlns:ns0="http://www.portalfiscal.inf.br/nfe/wsdl/NFeRecepcaoEvento4"><envEvento
       xmlns="http://www.portalfiscal.inf.br/nfe" versao="1.00"><idLote>1</idLote><evento
-      versao="1.00"><infEvento Id="ID2102103520030909107600014455001000180740100364234301"><cOrgao>91</cOrgao><tpAmb>1</tpAmb><CNPJ>23765766000162</CNPJ><chNFe>35200309091076000144550010001807401003642343</chNFe><dhEvento>2020-11-20T07:55:59-03:00</dhEvento><tpEvento>210210</tpEvento><nSeqEvento>1</nSeqEvento><verEvento>1.00</verEvento><detEvento
-      versao="1.00"><descEvento>Ciencia da Operacao</descEvento></detEvento></infEvento><Signature
+      versao="1.00"><infEvento Id="ID2102203520030909107600014455001000180740100364234301"><cOrgao>91</cOrgao><tpAmb>1</tpAmb><CNPJ>23765766000162</CNPJ><chNFe>35200309091076000144550010001807401003642343</chNFe><dhEvento>2020-11-20T07:55:59-03:00</dhEvento><tpEvento>210220</tpEvento><nSeqEvento>1</nSeqEvento><verEvento>1.00</verEvento><detEvento
+      versao="1.00"><descEvento>Desconhecimento da Operacao</descEvento></detEvento></infEvento><Signature
       xmlns="http://www.w3.org/2000/09/xmldsig#"><SignedInfo><CanonicalizationMethod
       Algorithm="http://www.w3.org/TR/2001/REC-xml-c14n-20010315"/><SignatureMethod
-      Algorithm="http://www.w3.org/2000/09/xmldsig#rsa-sha1"/><Reference URI="#ID2102103520030909107600014455001000180740100364234301"><Transforms><Transform
+      Algorithm="http://www.w3.org/2000/09/xmldsig#rsa-sha1"/><Reference URI="#ID2102203520030909107600014455001000180740100364234301"><Transforms><Transform
       Algorithm="http://www.w3.org/2000/09/xmldsig#enveloped-signature"/><Transform
       Algorithm="http://www.w3.org/TR/2001/REC-xml-c14n-20010315"/></Transforms><DigestMethod
-      Algorithm="http://www.w3.org/2000/09/xmldsig#sha1"/><DigestValue>ssry1MKF1mBOhCecq3qq35hQvBo=</DigestValue></Reference></SignedInfo><SignatureValue>ck3TXbcgr/XNSyuxMW2qH8BQ0Cr8TydckROI+uUZTit76waa2Sc8e/69nrzQt3q0WQ3Jng+ogViIa5kqzwqbOq85sK6CXONqWGWJWIbLfhA0dBpSyHrBYfXMU9uCwZ4kKNKQypclrM4mRjl5XdwqdBe1lwquW231hs9udzm6FaakjPbM/Ba+9z2XGbhQWpv4Iv71eCWI6iFbQwG33HGmzR8QzzaCPgTkHIHj772OP/a4zbdlW2Gq6npcdpziZCeHM4jLrQzyNRKULKV7vRN2rnFCjBPW1ivOo+NtubmcIxHVftZcdXMRM0tKzrlP0y4I5fOnkHvJdIso33DbgmRvPA==</SignatureValue><KeyInfo><X509Data><X509Certificate>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</X509Certificate></X509Data></KeyInfo></Signature></evento></envEvento></ns0:nfeDadosMsg></soap-env:Body></soap-env:Envelope>'
+      Algorithm="http://www.w3.org/2000/09/xmldsig#sha1"/><DigestValue>naXg5SQRX5a96qvzrEpV5MEmZQ8=</DigestValue></Reference></SignedInfo><SignatureValue>TSKMLK9pN/AbQwXhFrhAl5k6AD7FVurxDH6vjEI6aH3b9DehNfWU/41N8IBsY4++zGJyJkUzb+TaZbcKxi+cUMG58RLNgN70ODu4eD2u2V6qiGxpPBMCdVg2iqDOHLPmro3H7dSyUJTL30GVQzeFY+j39tcRquVPO49RMxDT9XmMAD+kL8f5v1QiUNO9SrrFsUlF7fIC6oELmSskmQRNlnN8niv4dd//uMd/1dsCcHD+k2BurTcsArp7X7Wl7W+PDQ9pgk+pIg93iXULmPrdcZkAmZvYO6UWYLRRGVNtWnDVV3PNxpgBEZYuFGBG1xgf95Rp8y6JVBFYejlMK3c7ng==</SignatureValue><KeyInfo><X509Data><X509Certificate>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</X509Certificate></X509Data></KeyInfo></Signature></evento></envEvento></ns0:nfeDadosMsg></soap-env:Body></soap-env:Envelope>'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '4640'
+      - '4648'
       Content-Type:
       - text/xml; charset=utf-8
       SOAPAction:
       - '"http://www.portalfiscal.inf.br/nfe/wsdl/NFeRecepcaoEvento4/nfeRecepcaoEventoNF"'
       User-Agent:
       - Zeep/3.4.0 (www.python-zeep.org)
     method: POST
     uri: https://www.nfe.fazenda.gov.br/NFeRecepcaoEvento4/NFeRecepcaoEvento4.asmx
   response:
     body:
       string: '<?xml version="1.0" encoding="utf-8"?><soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"><soap:Body><nfeRecepcaoEventoNFResult
         xmlns="http://www.portalfiscal.inf.br/nfe/wsdl/NFeRecepcaoEvento4"><retEnvEvento
         versao="1.00" xmlns="http://www.portalfiscal.inf.br/nfe"><idLote>1</idLote><tpAmb>1</tpAmb><verAplic>AN_1.1.3</verAplic><cOrgao>91</cOrgao><cStat>128</cStat><xMotivo>Lote
-        de evento processado</xMotivo><retEvento versao="1.00"><infEvento><tpAmb>1</tpAmb><verAplic>AN_1.1.3</verAplic><cOrgao>91</cOrgao><cStat>573</cStat><xMotivo>Rejeicao:
-        Duplicidade de evento</xMotivo><chNFe>35200309091076000144550010001807401003642343</chNFe><tpEvento>210210</tpEvento><xEvento>Ciencia
+        de evento processado</xMotivo><retEvento versao="1.00"><infEvento><tpAmb>1</tpAmb><verAplic>AN_1.1.3</verAplic><cOrgao>91</cOrgao><cStat>596</cStat><xMotivo>Rejeicao:
+        Evento apresentado apos o prazo permitido para o evento: [6 meses]</xMotivo><chNFe>35200309091076000144550010001807401003642343</chNFe><tpEvento>210220</tpEvento><xEvento>Desconhecimento
         da Operacao</xEvento><nSeqEvento>1</nSeqEvento><dhRegEvento>2020-11-20T07:55:59-03:00</dhRegEvento></infEvento></retEvento></retEnvEvento></nfeRecepcaoEventoNFResult></soap:Body></soap:Envelope>'
     headers:
       Cache-Control:
       - private, max-age=0
       Content-Length:
-      - '992'
+      - '1045'
       Content-Type:
       - text/xml; charset=utf-8
       Date:
       - Fri, 20 Nov 2020 10:55:59 GMT
       Server:
       - Microsoft-IIS/8.5
       X-AspNet-Version:
```

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_consulta_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_consulta_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 interactions:
 - request:
     body: '<?xml version=''1.0'' encoding=''utf-8''?>
 
       <soap-env:Envelope xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/"><soap-env:Body><ns0:nfeDadosMsg
       xmlns:ns0="http://www.portalfiscal.inf.br/nfe/wsdl/NFeRecepcaoEvento4"><envEvento
       xmlns="http://www.portalfiscal.inf.br/nfe" versao="1.00"><idLote>1</idLote><evento
-      versao="1.00"><infEvento Id="ID2102203520030909107600014455001000180740100364234301"><cOrgao>91</cOrgao><tpAmb>1</tpAmb><CNPJ>23765766000162</CNPJ><chNFe>35200309091076000144550010001807401003642343</chNFe><dhEvento>2020-11-20T07:55:59-03:00</dhEvento><tpEvento>210220</tpEvento><nSeqEvento>1</nSeqEvento><verEvento>1.00</verEvento><detEvento
-      versao="1.00"><descEvento>Desconhecimento da Operacao</descEvento></detEvento></infEvento><Signature
+      versao="1.00"><infEvento Id="ID2102403520030909107600014455001000180740100364234301"><cOrgao>91</cOrgao><tpAmb>1</tpAmb><CNPJ>23765766000162</CNPJ><chNFe>35200309091076000144550010001807401003642343</chNFe><dhEvento>2020-11-20T07:55:59-03:00</dhEvento><tpEvento>210240</tpEvento><nSeqEvento>1</nSeqEvento><verEvento>1.00</verEvento><detEvento
+      versao="1.00"><descEvento>Operacao nao Realizada</descEvento><xJust>000000000000000</xJust></detEvento></infEvento><Signature
       xmlns="http://www.w3.org/2000/09/xmldsig#"><SignedInfo><CanonicalizationMethod
       Algorithm="http://www.w3.org/TR/2001/REC-xml-c14n-20010315"/><SignatureMethod
-      Algorithm="http://www.w3.org/2000/09/xmldsig#rsa-sha1"/><Reference URI="#ID2102203520030909107600014455001000180740100364234301"><Transforms><Transform
+      Algorithm="http://www.w3.org/2000/09/xmldsig#rsa-sha1"/><Reference URI="#ID2102403520030909107600014455001000180740100364234301"><Transforms><Transform
       Algorithm="http://www.w3.org/2000/09/xmldsig#enveloped-signature"/><Transform
       Algorithm="http://www.w3.org/TR/2001/REC-xml-c14n-20010315"/></Transforms><DigestMethod
-      Algorithm="http://www.w3.org/2000/09/xmldsig#sha1"/><DigestValue>naXg5SQRX5a96qvzrEpV5MEmZQ8=</DigestValue></Reference></SignedInfo><SignatureValue>TSKMLK9pN/AbQwXhFrhAl5k6AD7FVurxDH6vjEI6aH3b9DehNfWU/41N8IBsY4++zGJyJkUzb+TaZbcKxi+cUMG58RLNgN70ODu4eD2u2V6qiGxpPBMCdVg2iqDOHLPmro3H7dSyUJTL30GVQzeFY+j39tcRquVPO49RMxDT9XmMAD+kL8f5v1QiUNO9SrrFsUlF7fIC6oELmSskmQRNlnN8niv4dd//uMd/1dsCcHD+k2BurTcsArp7X7Wl7W+PDQ9pgk+pIg93iXULmPrdcZkAmZvYO6UWYLRRGVNtWnDVV3PNxpgBEZYuFGBG1xgf95Rp8y6JVBFYejlMK3c7ng==</SignatureValue><KeyInfo><X509Data><X509Certificate>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</X509Certificate></X509Data></KeyInfo></Signature></evento></envEvento></ns0:nfeDadosMsg></soap-env:Body></soap-env:Envelope>'
+      Algorithm="http://www.w3.org/2000/09/xmldsig#sha1"/><DigestValue>M9Hmp7S2Bmi7D/eUme0nCkmcJfo=</DigestValue></Reference></SignedInfo><SignatureValue>Skq1VfIPR0af0nVfQmGWl8JBR6cWKxvsryNFObfHwfUycaewje4tID+t5R6xLcFwsRfRBiLHd4timwR36t53OgjV+s962uppkuBJWx27Hg+9kMijxFgWM/8kOiBKdfC0+cm2LIVpWMmkc2zLwrcxhIQi2Bz2XJz1V035oovlEYxirYxxpBUJJQt2TcgFDaPCBr7xsCeinInZ9Mw6g+L8XIThKLTwrtd2SFji7uZ+dsRnLS82uZE20y94xlOlt1pCVdDuKPOgPgaALCArDJn5W83L8HdB2Wclq/YuT9yf2ho91IujtY5mzIJDPCBV7Y7UIu8DhGsJ5LeUcGIyLQIALA==</SignatureValue><KeyInfo><X509Data><X509Certificate>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</X509Certificate></X509Data></KeyInfo></Signature></evento></envEvento></ns0:nfeDadosMsg></soap-env:Body></soap-env:Envelope>'
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       Content-Length:
-      - '4648'
+      - '4673'
       Content-Type:
       - text/xml; charset=utf-8
       SOAPAction:
       - '"http://www.portalfiscal.inf.br/nfe/wsdl/NFeRecepcaoEvento4/nfeRecepcaoEventoNF"'
       User-Agent:
       - Zeep/3.4.0 (www.python-zeep.org)
     method: POST
@@ -33,21 +33,21 @@
   response:
     body:
       string: '<?xml version="1.0" encoding="utf-8"?><soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"><soap:Body><nfeRecepcaoEventoNFResult
         xmlns="http://www.portalfiscal.inf.br/nfe/wsdl/NFeRecepcaoEvento4"><retEnvEvento
         versao="1.00" xmlns="http://www.portalfiscal.inf.br/nfe"><idLote>1</idLote><tpAmb>1</tpAmb><verAplic>AN_1.1.3</verAplic><cOrgao>91</cOrgao><cStat>128</cStat><xMotivo>Lote
         de evento processado</xMotivo><retEvento versao="1.00"><infEvento><tpAmb>1</tpAmb><verAplic>AN_1.1.3</verAplic><cOrgao>91</cOrgao><cStat>596</cStat><xMotivo>Rejeicao:
-        Evento apresentado apos o prazo permitido para o evento: [6 meses]</xMotivo><chNFe>35200309091076000144550010001807401003642343</chNFe><tpEvento>210220</tpEvento><xEvento>Desconhecimento
-        da Operacao</xEvento><nSeqEvento>1</nSeqEvento><dhRegEvento>2020-11-20T07:55:59-03:00</dhRegEvento></infEvento></retEvento></retEnvEvento></nfeRecepcaoEventoNFResult></soap:Body></soap:Envelope>'
+        Evento apresentado apos o prazo permitido para o evento: [6 meses]</xMotivo><chNFe>35200309091076000144550010001807401003642343</chNFe><tpEvento>210240</tpEvento><xEvento>Operacao
+        nao Realizada</xEvento><nSeqEvento>1</nSeqEvento><dhRegEvento>2020-11-20T07:55:59-03:00</dhRegEvento></infEvento></retEvento></retEnvEvento></nfeRecepcaoEventoNFResult></soap:Body></soap:Envelope>'
     headers:
       Cache-Control:
       - private, max-age=0
       Content-Length:
-      - '1045'
+      - '1040'
       Content-Type:
       - text/xml; charset=utf-8
       Date:
       - Fri, 20 Nov 2020 10:55:59 GMT
       Server:
       - Microsoft-IIS/8.5
       X-AspNet-Version:
```

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_envia_documento.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_envia_documento.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_envia_documento_ginfes.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_status_servico.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_status_servico.yaml`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.7.1/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml` & `erpbrasil.edoc-2.8.0/tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,92 +1,9 @@
 interactions:
 - request:
-    body: null
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      User-Agent:
-      - Zeep/3.4.0 (www.python-zeep.org)
-    method: GET
-    uri: https://www1.nfe.fazenda.gov.br/NFeDistribuicaoDFe/NFeDistribuicaoDFe.asmx?wsdl
-  response:
-    body:
-      string: "<?xml version=\"1.0\" encoding=\"utf-8\"?>\r\n<wsdl:definitions xmlns:s=\"\
-        http://www.w3.org/2001/XMLSchema\" xmlns:soap12=\"http://schemas.xmlsoap.org/wsdl/soap12/\"\
-        \ xmlns:http=\"http://schemas.xmlsoap.org/wsdl/http/\" xmlns:mime=\"http://schemas.xmlsoap.org/wsdl/mime/\"\
-        \ xmlns:tns=\"http://www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe\"\
-        \ xmlns:soap=\"http://schemas.xmlsoap.org/wsdl/soap/\" xmlns:tm=\"http://microsoft.com/wsdl/mime/textMatching/\"\
-        \ xmlns:soapenc=\"http://schemas.xmlsoap.org/soap/encoding/\" targetNamespace=\"\
-        http://www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe\" xmlns:wsdl=\"\
-        http://schemas.xmlsoap.org/wsdl/\">\r\n  <wsdl:types>\r\n    <s:schema elementFormDefault=\"\
-        qualified\" targetNamespace=\"http://www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe\"\
-        >\r\n      <s:element name=\"nfeDistDFeInteresse\">\r\n        <s:complexType>\r\
-        \n          <s:sequence>\r\n            <s:element minOccurs=\"0\" maxOccurs=\"\
-        1\" name=\"nfeDadosMsg\">\r\n              <s:complexType mixed=\"true\">\r\
-        \n                <s:sequence>\r\n                  <s:any />\r\n        \
-        \        </s:sequence>\r\n              </s:complexType>\r\n            </s:element>\r\
-        \n          </s:sequence>\r\n        </s:complexType>\r\n      </s:element>\r\
-        \n      <s:element name=\"nfeDistDFeInteresseResponse\">\r\n        <s:complexType>\r\
-        \n          <s:sequence>\r\n            <s:element minOccurs=\"0\" maxOccurs=\"\
-        1\" name=\"nfeDistDFeInteresseResult\">\r\n              <s:complexType mixed=\"\
-        true\">\r\n                <s:sequence>\r\n                  <s:any />\r\n\
-        \                </s:sequence>\r\n              </s:complexType>\r\n     \
-        \       </s:element>\r\n          </s:sequence>\r\n        </s:complexType>\r\
-        \n      </s:element>\r\n    </s:schema>\r\n  </wsdl:types>\r\n  <wsdl:message\
-        \ name=\"nfeDistDFeInteresseSoapIn\">\r\n    <wsdl:part name=\"parameters\"\
-        \ element=\"tns:nfeDistDFeInteresse\" />\r\n  </wsdl:message>\r\n  <wsdl:message\
-        \ name=\"nfeDistDFeInteresseSoapOut\">\r\n    <wsdl:part name=\"parameters\"\
-        \ element=\"tns:nfeDistDFeInteresseResponse\" />\r\n  </wsdl:message>\r\n\
-        \  <wsdl:portType name=\"NFeDistribuicaoDFeSoap\">\r\n    <wsdl:operation\
-        \ name=\"nfeDistDFeInteresse\">\r\n      <wsdl:input message=\"tns:nfeDistDFeInteresseSoapIn\"\
-        \ />\r\n      <wsdl:output message=\"tns:nfeDistDFeInteresseSoapOut\" />\r\
-        \n    </wsdl:operation>\r\n  </wsdl:portType>\r\n  <wsdl:binding name=\"NFeDistribuicaoDFeSoap\"\
-        \ type=\"tns:NFeDistribuicaoDFeSoap\">\r\n    <soap:binding transport=\"http://schemas.xmlsoap.org/soap/http\"\
-        \ />\r\n    <wsdl:operation name=\"nfeDistDFeInteresse\">\r\n      <soap:operation\
-        \ soapAction=\"http://www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe/nfeDistDFeInteresse\"\
-        \ style=\"document\" />\r\n      <wsdl:input>\r\n        <soap:body use=\"\
-        literal\" />\r\n      </wsdl:input>\r\n      <wsdl:output>\r\n        <soap:body\
-        \ use=\"literal\" />\r\n      </wsdl:output>\r\n    </wsdl:operation>\r\n\
-        \  </wsdl:binding>\r\n  <wsdl:binding name=\"NFeDistribuicaoDFeSoap12\" type=\"\
-        tns:NFeDistribuicaoDFeSoap\">\r\n    <soap12:binding transport=\"http://schemas.xmlsoap.org/soap/http\"\
-        \ />\r\n    <wsdl:operation name=\"nfeDistDFeInteresse\">\r\n      <soap12:operation\
-        \ soapAction=\"http://www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe/nfeDistDFeInteresse\"\
-        \ style=\"document\" />\r\n      <wsdl:input>\r\n        <soap12:body use=\"\
-        literal\" />\r\n      </wsdl:input>\r\n      <wsdl:output>\r\n        <soap12:body\
-        \ use=\"literal\" />\r\n      </wsdl:output>\r\n    </wsdl:operation>\r\n\
-        \  </wsdl:binding>\r\n  <wsdl:service name=\"NFeDistribuicaoDFe\">\r\n   \
-        \ <wsdl:port name=\"NFeDistribuicaoDFeSoap\" binding=\"tns:NFeDistribuicaoDFeSoap\"\
-        >\r\n      <soap:address location=\"https://www1.nfe.fazenda.gov.br/NFeDistribuicaoDFe/NFeDistribuicaoDFe.asmx\"\
-        \ />\r\n    </wsdl:port>\r\n    <wsdl:port name=\"NFeDistribuicaoDFeSoap12\"\
-        \ binding=\"tns:NFeDistribuicaoDFeSoap12\">\r\n      <soap12:address location=\"\
-        https://www1.nfe.fazenda.gov.br/NFeDistribuicaoDFe/NFeDistribuicaoDFe.asmx\"\
-        \ />\r\n    </wsdl:port>\r\n  </wsdl:service>\r\n</wsdl:definitions>"
-    headers:
-      Cache-Control:
-      - private, max-age=0
-      Content-Length:
-      - '3829'
-      Content-Type:
-      - text/xml; charset=utf-8
-      Date:
-      - Fri, 20 Nov 2020 10:55:33 GMT
-      Server:
-      - Microsoft-IIS/8.5
-      X-AspNet-Version:
-      - 4.0.30319
-      X-Powered-By:
-      - ASP.NET
-    status:
-      code: 200
-      message: OK
-- request:
     body: '<?xml version=''1.0'' encoding=''utf-8''?>
 
       <soap-env:Envelope xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/"><soap-env:Header><nfeCabecMsg
       xmlns="http://www.portalfiscal.inf.br/nfe/wsdl/"><cUF>SP</cUF><versaoDados>1.00</versaoDados></nfeCabecMsg></soap-env:Header><soap-env:Body><ns0:nfeDistDFeInteresse
       xmlns:ns0="http://www.portalfiscal.inf.br/nfe/wsdl/NFeDistribuicaoDFe"><ns0:nfeDadosMsg><distDFeInt
       xmlns="http://www.portalfiscal.inf.br/nfe" versao="1.01"><tpAmb>1</tpAmb><cUFAutor>35</cUFAutor><CNPJ>23765766000162</CNPJ><distNSU><ultNSU>000000000000001</ultNSU></distNSU></distDFeInt></ns0:nfeDadosMsg></ns0:nfeDistDFeInteresse></soap-env:Body></soap-env:Envelope>'
     headers:
```

### Comparing `erpbrasil.edoc-2.7.1/tests/test_erpbrasil_edoc.py` & `erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,103 +1,77 @@
-# coding=utf-8
 import logging.config
 import os
 from unittest import TestCase
 
 import vcr
-from erpbrasil.assinatura.certificado import Certificado
+from erpbrasil.edoc.mde import MDe, TransmissaoMDE
 from requests import Session
 
-from erpbrasil.edoc.mde import MDe
-from erpbrasil.edoc.mde import TransmissaoMDE
+from .test_certificate_mixin import TestCertificateMixin
 
-logging.config.dictConfig({
-    'version': 1,
-    'formatters': {
-        'verbose': {
-            'format': '%(name)s: %(message)s'
-        }
-    },
-    'handlers': {
-        'console': {
-            'level': 'DEBUG',
-            'class': 'logging.StreamHandler',
-            'formatter': 'verbose',
+logging.config.dictConfig(
+    {
+        "version": 1,
+        "formatters": {"verbose": {"format": "%(name)s: %(message)s"}},
+        "handlers": {
+            "console": {
+                "level": "DEBUG",
+                "class": "logging.StreamHandler",
+                "formatter": "verbose",
+            },
         },
-    },
-    'loggers': {
-        'zeep.transports': {
-            'level': 'DEBUG',
-            'propagate': True,
-            'handlers': ['console'],
+        "loggers": {
+            "zeep.transports": {
+                "level": "DEBUG",
+                "propagate": True,
+                "handlers": ["console"],
+            },
         },
     }
-})
+)
 
-VALID_CSTAT_LIST = ['137', '138']
+VALID_CSTAT_LIST = ["137", "138"]
 
 
-class Tests(TestCase):
-    """ Rodar este teste muitas vezes pode bloquear o seu IP"""
+class Tests(TestCertificateMixin, TestCase):
+    """Rodar este teste muitas vezes pode bloquear o seu IP"""
 
     def setUp(self):
-        certificado_nfe_caminho = os.environ.get(
-            'certificado_nfe_caminho',
-            'test/fixtures/dummy_cert.pfx'
-        )
-        certificado_nfe_senha = os.environ.get(
-            'certificado_nfe_senha', 'dummy_password'
-        )
-        self.certificado = Certificado(
-            certificado_nfe_caminho,
-            certificado_nfe_senha
-        )
-
+        super().setUp()
         self.chave = os.environ.get(
-            'chNFe', '35200309091076000144550010001807401003642343'
+            "CHAVE_NFE", "35200309091076000144550010001807401003642343"
         )
-
         session = Session()
         session.verify = False
 
-        transmissao = TransmissaoMDE(self.certificado, session)
-        self.mde = MDe(
-            transmissao, '35',
-            versao='1.01', ambiente='1'
-        )
-
-    @vcr.use_cassette('tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml')
-    def test_ultimo_nsu(self):
+        transmissao = TransmissaoMDE(self.certificate, session)
+        self.mde = MDe(transmissao, "35", versao="1.01", ambiente="1")
 
+    @vcr.use_cassette(
+        "tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml",
+    )
+    def test_nsu_especifico(self):
         ret = self.mde.consultar_distribuicao(
-            cnpj_cpf=self.certificado.cnpj_cpf,
-            ultimo_nsu='1'.zfill(15),
+            cnpj_cpf=self.certificate.cnpj_cpf,
+            nsu_especifico="16172".zfill(15),
         )
 
         self.assertIn(ret.resposta.cStat, VALID_CSTAT_LIST)
 
-    @vcr.use_cassette('tests/fixtures/vcr_cassettes/test_nsu_especifico.yaml')
-    def test_nsu_especifico(self):
-
+    @vcr.use_cassette(
+        "tests/fixtures/vcr_cassettes/test_ultimo_nsu.yaml",
+    )
+    def test_ultimo_nsu(self):
         ret = self.mde.consultar_distribuicao(
-            cnpj_cpf=self.certificado.cnpj_cpf,
-            nsu_especifico='1'.zfill(15),
+            cnpj_cpf=self.certificate.cnpj_cpf,
+            ultimo_nsu="0".zfill(15),
         )
 
         self.assertIn(ret.resposta.cStat, VALID_CSTAT_LIST)
 
-    @vcr.use_cassette('tests/fixtures/vcr_cassettes/test_chave.yaml')
+    @vcr.use_cassette("tests/fixtures/vcr_cassettes/test_chave.yaml")
     def test_chave(self):
-
         ret = self.mde.consultar_distribuicao(
-            cnpj_cpf=self.certificado.cnpj_cpf,
-            chave=self.chave
+            cnpj_cpf=self.certificate.cnpj_cpf, chave=self.chave
         )
 
         self.assertIn(ret.resposta.cStat, VALID_CSTAT_LIST)
-
-
-t = Tests()
-t.setUp()
-t.test_ultimo_nsu()
-t.test_nsu_especifico()
-t.test_chave()
```

### Comparing `erpbrasil.edoc-2.7.1/tests/test_erpbrasil_edoc_manifestacao.py` & `erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_manifestacao.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,82 @@
-# coding=utf-8
-
 import logging.config
 import os
 from unittest import TestCase
 
 import vcr
-from erpbrasil.assinatura.certificado import Certificado
+from erpbrasil.edoc.mde import MDe, TransmissaoMDE
 from requests import Session
 
-from erpbrasil.edoc.mde import MDe
-from erpbrasil.edoc.mde import TransmissaoMDE
+from .test_certificate_mixin import TestCertificateMixin
 
-logging.config.dictConfig({
-    'version': 1,
-    'formatters': {
-        'verbose': {
-            'format': '%(name)s: %(message)s'
-        }
-    },
-    'handlers': {
-        'console': {
-            'level': 'DEBUG',
-            'class': 'logging.StreamHandler',
-            'formatter': 'verbose',
+logging.config.dictConfig(
+    {
+        "version": 1,
+        "formatters": {"verbose": {"format": "%(name)s: %(message)s"}},
+        "handlers": {
+            "console": {
+                "level": "DEBUG",
+                "class": "logging.StreamHandler",
+                "formatter": "verbose",
+            },
         },
-    },
-    'loggers': {
-        'zeep.transports': {
-            'level': 'DEBUG',
-            'propagate': True,
-            'handlers': ['console'],
+        "loggers": {
+            "zeep.transports": {
+                "level": "DEBUG",
+                "propagate": True,
+                "handlers": ["console"],
+            },
         },
     }
-})
+)
 
-VALID_CSTAT_LIST = ['128']
+VALID_CSTAT_LIST = ["128"]
 
 
-class Tests(TestCase):
-    """ Rodar este teste muitas vezes pode bloquear o seu IP"""
+class Tests(TestCertificateMixin, TestCase):
+    """Rodar este teste muitas vezes pode bloquear o seu IP"""
 
     def setUp(self):
-        certificado_nfe_caminho = os.environ.get(
-            'certificado_nfe_caminho',
-            'test/fixtures/dummy_cert.pfx'
-        )
-        certificado_nfe_senha = os.environ.get(
-            'certificado_nfe_senha', 'dummy_password'
-        )
-        self.certificado = Certificado(
-            certificado_nfe_caminho,
-            certificado_nfe_senha
-        )
+        super().setUp()
         session = Session()
         session.verify = False
 
-        transmissao = TransmissaoMDE(self.certificado, session)
-        self.mde = MDe(
-            transmissao, '35',
-            versao='1.00', ambiente='1'
-        )
+        transmissao = TransmissaoMDE(self.certificate, session)
+        self.mde = MDe(transmissao, "35", versao="1.00", ambiente="1")
 
         self.chave = os.environ.get(
-            'chNFe', '35200309091076000144550010001807401003642343'
+            "CHAVE_NFE", "35200309091076000144550010001807401003642343"
         )
 
-    @vcr.use_cassette(
-        'tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml')
+    @vcr.use_cassette("tests/fixtures/vcr_cassettes/test_confirmacao_da_operacao.yaml")
     def test_confirmacao_da_operacao(self):
         ret = self.mde.confirmacao_da_operacao(
-            chave=self.chave,
-            cnpj_cpf=self.certificado.cnpj_cpf
+            chave=self.chave, cnpj_cpf=self.certificate.cnpj_cpf
         )
 
         self.assertIn(ret.resposta.cStat, VALID_CSTAT_LIST)
 
-    @vcr.use_cassette(
-        'tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml')
+    @vcr.use_cassette("tests/fixtures/vcr_cassettes/test_ciencia_da_operacao.yaml")
     def test_ciencia_da_operacao(self):
         ret = self.mde.ciencia_da_operacao(
-            chave=self.chave,
-            cnpj_cpf=self.certificado.cnpj_cpf
+            chave=self.chave, cnpj_cpf=self.certificate.cnpj_cpf
         )
 
         self.assertIn(ret.resposta.cStat, VALID_CSTAT_LIST)
 
     @vcr.use_cassette(
-        'tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml')
+        "tests/fixtures/vcr_cassettes/test_desconhecimento_da_operacao.yaml"
+    )
     def test_desconhecimento_da_operacao(self):
         ret = self.mde.desconhecimento_da_operacao(
-            chave=self.chave,
-            cnpj_cpf=self.certificado.cnpj_cpf
+            chave=self.chave, cnpj_cpf=self.certificate.cnpj_cpf
         )
 
         self.assertIn(ret.resposta.cStat, VALID_CSTAT_LIST)
 
-    @vcr.use_cassette(
-        'tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml')
+    @vcr.use_cassette("tests/fixtures/vcr_cassettes/test_operacao_nao_realizada.yaml")
     def test_operacao_nao_realizada(self):
         ret = self.mde.operacao_nao_realizada(
-            chave=self.chave,
-            cnpj_cpf=self.certificado.cnpj_cpf
+            chave=self.chave, cnpj_cpf=self.certificate.cnpj_cpf
         )
 
         self.assertIn(ret.resposta.cStat, VALID_CSTAT_LIST)
-
-
-t = Tests()
-t.setUp()
-t.test_confirmacao_da_operacao()
-t.test_ciencia_da_operacao()
-t.test_desconhecimento_da_operacao()
-t.test_operacao_nao_realizada()
```

### Comparing `erpbrasil.edoc-2.7.1/tests/test_erpbrasil_edoc_nfse_paulistana.py` & `erpbrasil.edoc-2.8.0/tests/test_erpbrasil_edoc_nfse_paulistana.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.edoc-2.7.1/tox.ini` & `erpbrasil.edoc-2.8.0/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,59 @@
-[testenv:bootstrap]
-deps =
-    jinja2
-    matrix
-    tox
-skip_install = true
-commands =
-    python ci/bootstrap.py
-passenv =
-    *
 ; a generative tox configuration, see: https://tox.readthedocs.io/en/latest/config.html#generative-envlist
 
 [tox]
 envlist =
     clean,
     check,
     docs,
-    {py36,py37,py38,pypy,pypy3},
+    {py37,py38,py39,py310},
     report
 ignore_basepython_conflict = true
 
 [testenv]
 basepython =
-    pypy: {env:TOXPYTHON:pypy}
-    pypy3: {env:TOXPYTHON:pypy3}
-    py36: {env:TOXPYTHON:python3.6}
-    {py38,docs,spell}: {env:TOXPYTHON:python3.8}
+    {py39,docs,spell}: {env:TOXPYTHON:python3.9}
     py37: {env:TOXPYTHON:python3.7}
     py38: {env:TOXPYTHON:python3.8}
+    py39: {env:TOXPYTHON:python3.9}
+    py310: {env:TOXPYTHON:python3.10}
     {bootstrap,clean,check,report,codecov}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
-    certificado_nfe_caminho=tests/fixtures/dummy_cert.pfx
 passenv =
     *
 usedevelop = false
 deps =
     pytest
-    pytest-travis-fold
     pytest-cov
-    vcrpy
+    vcrpy==4.1.1
+    urllib3==1.26.0
     -rrequirements.txt
 commands =
     {posargs:pytest --cov --cov-report=term-missing -vv tests}
 
+[testenv:bootstrap]
+deps =
+    jinja2
+    matrix
+    tox
+skip_install = true
+commands =
+    python ci/bootstrap.py
+
 [testenv:check]
 deps =
-    docutils
     check-manifest
-    flake8
     readme-renderer
     pygments
-    isort
 skip_install = true
 commands =
-    python setup.py check --strict --metadata --restructuredtext
+    python setup.py check --strict --metadata --restructuredtext -vv
     check-manifest {toxinidir}
-    flake8 src tests setup.py
-    isort --verbose --check-only --diff src tests setup.py
 
 [testenv:spell]
 setenv =
     SPELLCHECK=1
 commands =
     sphinx-build -b spelling docs dist/docs
 skip_install = true
@@ -79,14 +71,15 @@
     sphinx-build -b linkcheck docs dist/docs
 
 [testenv:codecov]
 deps =
     codecov
 skip_install = true
 commands =
+    coverage xml --ignore-errors
     codecov []
 
 [testenv:report]
 deps = coverage
 skip_install = true
 commands =
     coverage report
```

