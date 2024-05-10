# Comparing `tmp/ecuapassdocs-0.74.tar.gz` & `tmp/ecuapassdocs-0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecuapassdocs-0.74.tar", last modified: Fri Apr 26 16:00:32 2024, max compression
+gzip compressed data, was "ecuapassdocs-0.75.tar", last modified: Fri May 10 13:10:20 2024, max compression
```

## Comparing `ecuapassdocs-0.74.tar` & `ecuapassdocs-0.75.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-26 16:00:32.012024 ecuapassdocs-0.74/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-04-26 16:00:32.012024 ecuapassdocs-0.74/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)       40 2024-04-22 18:48:50.000000 ecuapassdocs-0.74/README.md
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-26 16:00:31.976023 ecuapassdocs-0.74/ecuapassdocs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-26 16:00:31.980023 ecuapassdocs-0.74/ecuapassdocs/info/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.74/ecuapassdocs/info/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     3202 2024-04-25 03:25:15.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_data.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    16144 2024-04-19 16:41:25.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_extractor.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4546 2024-04-23 23:21:48.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_feedback.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     8770 2024-04-26 15:57:00.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    22728 2024-04-19 16:44:38.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_cartaporte.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1481 2024-04-12 15:49:22.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2728 2024-04-12 15:44:03.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_declaracion.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    25562 2024-04-12 15:14:37.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_manifiesto.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1850 2024-04-12 15:43:23.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1709 2024-04-12 15:43:35.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     5488 2024-04-18 05:29:13.000000 ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_utils.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    12459 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/info/old-utils.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.74/ecuapassdocs/info/resourceloader.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-26 16:00:31.980023 ecuapassdocs-0.74/ecuapassdocs/resources/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-26 16:00:31.984023 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 20:00:30.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/documentos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/empresa.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/monedas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/out.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/sustancias.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-26 16:00:31.988023 ecuapassdocs-0.74/ecuapassdocs/resources/data_declaracion/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_declaracion/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-26 16:00:31.992023 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/sectores.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-26 16:00:32.004023 ecuapassdocs-0.74/ecuapassdocs/resources/docs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    15528 2024-04-01 17:21:22.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/declaracion_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:01:53.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/join.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    18425 2024-03-30 18:30:32.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.74/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-26 16:00:32.012024 ecuapassdocs-0.74/ecuapassdocs/resources/images/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/icon-colombia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/icon-ecuador.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/icon-white-bot.ico
--rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-cartaporte-vacia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-scroll-up.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.74/ecuapassdocs/resources/images/image-windows-WindowButtons.png
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-26 16:00:31.976023 ecuapassdocs-0.74/ecuapassdocs.egg-info/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-04-26 16:00:31.000000 ecuapassdocs-0.74/ecuapassdocs.egg-info/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)     6030 2024-04-26 16:00:31.000000 ecuapassdocs-0.74/ecuapassdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-04-26 16:00:31.000000 ecuapassdocs-0.74/ecuapassdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-04-26 16:00:31.000000 ecuapassdocs-0.74/ecuapassdocs.egg-info/requires.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-04-26 16:00:31.000000 ecuapassdocs-0.74/ecuapassdocs.egg-info/top_level.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-04-26 16:00:32.012024 ecuapassdocs-0.74/setup.cfg
--rw-rw-r--   0 lg        (1000) lg        (1000)     1356 2024-04-26 16:00:30.000000 ecuapassdocs-0.74/setup.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.507325 ecuapassdocs-0.75/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-10 13:10:20.507325 ecuapassdocs-0.75/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)       40 2024-04-22 18:48:50.000000 ecuapassdocs-0.75/README.md
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.475325 ecuapassdocs-0.75/ecuapassdocs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.479325 ecuapassdocs-0.75/ecuapassdocs/info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3202 2024-04-25 03:25:15.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_data.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18145 2024-05-06 01:21:28.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_extractor.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4490 2024-04-29 15:28:31.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_feedback.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9947 2024-05-08 05:43:09.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    20527 2024-05-08 05:40:58.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1481 2024-04-12 15:49:22.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2732 2024-05-04 03:37:00.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_declaracion.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    25562 2024-04-12 15:14:37.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1850 2024-04-12 15:43:23.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1709 2024-04-12 15:43:35.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9777 2024-05-10 05:33:15.000000 ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_utils.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    12459 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/info/old-utils.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.75/ecuapassdocs/info/resourceloader.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.479325 ecuapassdocs-0.75/ecuapassdocs/resources/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.487325 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 20:00:30.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/documentos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/empresa.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/monedas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/out.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/sustancias.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.487325 ecuapassdocs-0.75/ecuapassdocs/resources/data_declaracion/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_declaracion/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.491325 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/sectores.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.499325 ecuapassdocs-0.75/ecuapassdocs/resources/docs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    15818 2024-05-08 13:54:13.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:01:53.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/join.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18782 2024-05-08 13:57:39.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.75/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.507325 ecuapassdocs-0.75/ecuapassdocs/resources/images/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-colombia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-ecuador.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-white-bot.ico
+-rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-cartaporte-vacia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-scroll-up.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.75/ecuapassdocs/resources/images/image-windows-WindowButtons.png
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-05-10 13:10:20.475325 ecuapassdocs-0.75/ecuapassdocs.egg-info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-05-10 13:10:20.000000 ecuapassdocs-0.75/ecuapassdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6030 2024-05-10 13:10:20.000000 ecuapassdocs-0.75/ecuapassdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-05-10 13:10:20.000000 ecuapassdocs-0.75/ecuapassdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-05-10 13:10:20.000000 ecuapassdocs-0.75/ecuapassdocs.egg-info/requires.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-05-10 13:10:20.000000 ecuapassdocs-0.75/ecuapassdocs.egg-info/top_level.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-05-10 13:10:20.507325 ecuapassdocs-0.75/setup.cfg
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1424 2024-05-10 13:10:17.000000 ecuapassdocs-0.75/setup.py
```

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_data.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_data.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_extractor.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,34 +4,77 @@
 
 from .ecuapass_utils import Utils
 from ecuapassdocs.info.resourceloader import ResourceLoader 
 #--------------------------------------------------------------------
 # Class for extracting different values from document texts
 #--------------------------------------------------------------------
 class Extractor:
+	#-------------------------------------------------------------------
+	#-- Get location info: ciudad, pais, fecha -------------------------
+	#-- Boxes: Recepcion, Embarque, Entrega ----------------------------
+	#-------------------------------------------------------------------
+	def extractLocationDate (text, resourcesPath, fieldType=None):
+		location = {"ciudad":"||LOW", "pais":"||LOW", "fecha":"||LOW"}
+		try:
+			text   = text.replace ("\n", " ")
+			# Fecha
+			fecha = Extractor.getDate (text, resourcesPath)
+			location ["fecha"] = fecha if fecha else "||LOW"
+			# Pais
+			text, location = Extractor.removeSubjectCiudadPais (text, location, resourcesPath, fieldType)
+		except:
+			Utils.printException (f"Obteniendo datos de la localización: '{fieldType}' en el texto", text)
+
+		return (location)
+
 	#-----------------------------------------------------------
 	#-- Get subject (remitente, destinatario, declarante,..) info
 	#-- Info: nombre, dir, pais, ciudad, id, idNro
 	#-----------------------------------------------------------
+	def getSubjectInfoFromText (text, resourcesPath, subjectType):
+		subject = {"nombre":None, "direccion":None, "pais": None, 
+		           "ciudad":None, "tipoId":None, "numeroId": None}
+		try:
+			lines   = text.split ("\n")
+
+			if len (lines) == 3:
+				nameDirLines = lines [0:2]
+				idPaisLine   = lines [2]
+			elif len (lines) == 4:
+				nameDirLines = lines [0:3]
+				idPaisLine   = lines [3]
+			elif len (lines) < 3:
+				print (f">>> Alerta:  Pocas líneas de texto para extraer información de empresa.")
+				return subject
+
+			text, subject = Extractor.removeSubjectId (idPaisLine, subject, subjectType)
+			text, subject = Extractor.removeSubjectCiudadPais (text, subject, resourcesPath, subjectType)
+			text, subject = Extractor.removeSubjectCiudadPais (text, subject, resourcesPath, subjectType)
+			nameDirText   = "\n".join (nameDirLines)
+			text, subject = Extractor.removeSubjectNombreDireccion
+			(nameDirText, subject, subjectType)
+			subject ["numeroId"] = Utils.convertToEcuapassId (subject ["numeroId"])
+		except:
+			Utils.printException (f"Obteniendo datos del sujeto: '{subjectType}' en el texto: '{text}'")
+
+		print (subject)
+		return (subject)
 
 	#--  Extracts and replaces IdType and IdNumber from text-------
 	def getReplaceSubjectId (text, subject, replaceString, type):
 		try:
 			if not any (x in text.upper() for x in ["NIT", "RUC", "OTROS"]): 
 				return (text, subject)
 
 			reNumber = r'\d+(?:[.,]*\d*)+' # RE for extracting a float number 
 			reId     = rf"(RUC|NIT|OTROS)[\s.:]+({reNumber}(?:-\d)?)\s*"
 			result	 = re.search (reId, text, flags=re.S)
 		 
-			tipoId   = result.group (1) if result else None
-			numeroId = result.group (2) if result else None
-
-			subject ["tipoId"]   = "OTROS" if tipoId == "NIT" else tipoId
-			subject ["numeroId"] = Utils.convertToEcuapassId (numeroId)
+			subject ["tipoId"]   = result.group (1) if result else None
+			subject ["numeroId"] = result.group (2).replace (".", "") if result else None
 
 			text	 = re.sub (reId, replaceString, text, flags=re.S).strip()
 		except:
 			Utils.printException (f"Obteniendo informacion de ID de '{type}'")
 
 		return (text, subject)
 
@@ -325,20 +368,21 @@
 			reDay      = r'(?P<day>\d{1,2})'
 			reMonthNum = r'(?P<month>\d{1,2})'
 			reMonthTxt = rf'(?P<month>{monthsString})'
 			reYear     = r'(?P<year>\d[.]?\d{3})'
 			reWordSep  = r'\s+(?:DE|DEL)\s+'
 			reSep      = r'(-|/)'
 
-			reDate0 = rf'\b{reDay}\s*[-]\s*{reMonthNum}\s*[-]\s*{reYear}\b' # 31-12-2023
-			reDate1 = rf'\b{reMonthTxt}\s+{reDay}{reWordSep}{reYear}\b'     # Junio 20 del 2023
-			reDate2 = rf'\b{reDay}{reWordSep}{reMonthTxt}{reWordSep}{reYear}\b' # 20 de Junio del 2023
-			reDate3 = rf'\b{reYear}{reSep}{reMonthNum}{reSep}{reDay}\b' # 2023/12/31
-			reDate4 = rf'\b{reYear}{reSep}{reMonthTxt}{reSep}{reDay}\b' # 2023/DICIEMBRE/31
-			reDateOptions = [reDate0, reDate1, reDate2, reDate3, reDate4]
+			reDate0 = rf'\b{reDay}\s*[-]\s*{reMonthNum}\s*[-]\s*{reYear}\b'     # 31-12-2023
+			reDate1 = rf'\b{reMonthTxt}\s+{reDay}{reWordSep}{reYear}\b'         # Junio 20 del 2023
+			reDate2 = rf'\b{reMonthTxt}\s+{reDay}{reSep}{reYear}\b'             # Junio 20/2023
+			reDate3 = rf'\b{reDay}{reWordSep}{reMonthTxt}{reWordSep}{reYear}\b' # 20 de Junio del 2023
+			reDate4 = rf'\b{reYear}{reSep}{reMonthNum}{reSep}{reDay}\b'         # 2023/12/31
+			reDate5 = rf'\b{reYear}{reSep}{reMonthTxt}{reSep}{reDay}\b'         # 2023/DICIEMBRE/31
+			reDateOptions = [reDate0, reDate1, reDate2, reDate3, reDate4, reDate5]
 
 			# Evaluate all reDates and select the one with results
 			results = [re.search (x, text, re.I) for (i, x) in enumerate (reDateOptions)]
 			if results [0]:
 				result = results [0]
 				month  = result.group('month')
 			elif results [1] or results [2]:
```

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_feedback.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_feedback.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 	#----------------------------------------------------------------
 	def getBlobClient (text_blob_name):
 		# Azure Blob Storage container name
 		container_name = "blobfeedback"
 
 		# Azure Storage account connection string
 		#connection_string = os.environ.get ("AZR_BLOB_CONN_STR")
-		connection_string ="DefaultEndpointsProtocol=https;AccountName=lgformsstorage;AccountKey=BHsWkVaWQYStRq8FOpoIl0jI39W+WFvrSJmxesr0euIEJe+qkSi0LoTM0HZfyOn2XbYfnHir7CD8+ASt6ZJnwg==;EndpointSuffix=core.windows.net"
-		Utils.printx ("Connection string:", connection_string)
+		connection_string = "DefaultEndpointsProtocol=https;AccountName=lgformsstorage;AccountKey=BHsWkVaWQYStRq8FOpoIl0jI39W+WFvrSJmxesr0euIEJe+qkSi0LoTM0HZfyOn2XbYfnHir7CD8+ASt6ZJnwg==;EndpointSuffix=core.windows.net"
 
 		# Initialize the BlobServiceClient
 		blob_service_client = BlobServiceClient.from_connection_string (connection_string)
 
 		# Create a container (if it doesn't exist)
 		container_client = blob_service_client.get_container_client (container_name)
 		blob_client = container_client.get_blob_client (text_blob_name)
```

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,34 +8,61 @@
 from .ecuapass_utils import Utils
 
 # Base class for all info document clases: CartaporteInfo (CPI), ManifiestoInfo (MCI), EcuDCL (DTAI)
 class EcuInfo:
 
 	def __init__ (self, docType, fieldsJsonFile, runningDir):
 		self.docType        = docType
+		self.inputsParametersFile = Utils.getInputsParametersFile (docType)
+
 		self.fieldsJsonFile = fieldsJsonFile
 		self.runningDir     = runningDir
 
 		self.empresa        = self.getEmpresaInfo ()   # Overwritten per 'empresa'
 		self.nombreEmpresa  = self.empresa ["id"]
 
-		if self.docType == "CARTAPORTE":
-			self.inputsParametersFile = "cartaporte_input_parameters.json"
-		elif self.docType == "MANIFIESTO":
-			self.inputsParametersFile = "manifiesto_input_parameters.json"
-		elif self.docType == "DECLARACION":
-			self.inputsParametersFile = "declaracion_input_parameters.json"
-		else:
-			Utils.printx (f"ERROR: Tipo de documento desconocido:", docType)
-
 		self.resourcesPath        = os.path.join (runningDir, "resources", "data_cartaportes") 
 		self.fields               = json.load (open (fieldsJsonFile))
 		self.fields ["jsonFile"]  = fieldsJsonFile
 		self.ecudoc               = {}
 
+#	#----------------------------------------------------------------
+#	# Obsolete: moved to utils
+#	# Return field ({...,02_Remitente:"XXXX"...} 
+#	# from params values (ej. txt00 :{....}) 
+#	# Info is embedded according to Azure format
+#	#----------------------------------------------------------------
+#	def getFieldValuesFromInputs (self, inputValues):
+#		fieldsJsonDic = {}
+#		# Load parameters from package
+#		inputParameters = ResourceLoader.loadJson ("docs", self.inputsParametersFile)
+#		for key, params in inputParameters.items():
+#			fieldName	 = params ["field"]
+#			if fieldName:
+#				value		 = inputValues [key]
+#				fieldsJsonDic [fieldName] = {"value": value, "content": value}
+#
+#		return fieldsJsonDic
+
+#	#----------------------------------------------------------------
+#	#-- Return input parameters file
+#	#----------------------------------------------------------------
+#	def getInputParametersFile (self):
+#		if self.docType == "CARTAPORTE":
+#			self.inputsParametersFile = "cartaporte_input_parameters.json"
+#		elif self.docType == "MANIFIESTO":
+#			self.inputsParametersFile = "manifiesto_input_parameters.json"
+#		elif self.docType == "DECLARACION":
+#			self.inputsParametersFile = "declaracion_input_parameters.json"
+#		else:
+#			message= f"ERROR: Tipo de documento desconocido:", docType
+#			raise Exception (message)
+#		return self.inputsParametersFile
+
+
 	#-- For all types of documents (fixed fro NTA and BYZA, check the others)
 	def getNumeroDocumento (self):
 		text   = Utils.getValue (self.fields, "00b_Numero")
 		numero = Extractor.getNumeroDocumento (text)
 
 		codigo = self.getCodigoPais (numero)
 		self.fields ["00_Pais"] = {"value":codigo, "content":codigo}
@@ -171,16 +198,16 @@
 	#-- Create CODEBIN fields from document fields using input parameters
 	#----------------------------------------------------------------
 	def getCodebinFields (self):
 		try:
 			inputsParams = ResourceLoader.loadJson ("docs", self.inputsParametersFile)
 			codebinFields = {}
 			for key in inputsParams:
-				docField   = inputsParams [key]["field"]
-				cbinField  = inputsParams [key]["fieldCodebin"]
+				docField   = inputsParams [key]["ecudocsField"]
+				cbinField  = inputsParams [key]["codebinField"]
 				#print ("-- key:", key, " dfield:", docField, "cfield: ", cbinField)
 				if cbinField:
 					value = self.getDocumentFieldValue (docField, "CODEBIN")
 					codebinFields [cbinField] = value
 
 			return codebinFields
 		except Exception as e:
@@ -191,15 +218,15 @@
 	#-- Create ECUAPASSDOCS fields from document fields using input parameters
 	#----------------------------------------------------------------
 	def getEcuapassdocsFields (self):
 		try:
 			inputsParams = ResourceLoader.loadJson ("docs", self.inputsParametersFile)
 			docFieldsAll = {}
 			for key in inputsParams:
-				docField   = inputsParams [key]["field"]
+				docField   = inputsParams [key]["ecudocsField"]
 				if docField == "" or "OriginalCopia" in docField:
 					continue
 				else:
 					value = self.getDocumentFieldValue (docField)
 					docFieldsAll [key] = value
 
 			return docFieldsAll
@@ -215,20 +242,22 @@
 			paises     = {"CO":"CO", "EC":"EC"}
 			if appName == "CODEBIN":
 				paises     = {"CO":"colombia", "EC":"ecuador"}
 
 			codigoPais = self.fields [docField]["value"]
 			value      =  paises [codigoPais]
 
-		elif "Gastos" in docField and self.docType == "CARTAPORTE" :
-			fieldName	= docField.split (":")[0]
-			rowName		= docField.split (":")[1].split (",")[0]
-			colName		= docField.split (":")[1].split (",")[1]
-			tablaGastos = self.fields [fieldName]["value"]
-			value		= self.getValueTablaGastos (tablaGastos, rowName, colName)
+		#elif "Gastos" in docField and self.docType == "CARTAPORTE" :
+			#value = self.fields [docField]["content"]
+			#value = value if value == "" else None
+			#fieldName	= docField.split (":")[0]
+			#rowName		= docField.split (":")[1].split (",")[0]
+			#colName		= docField.split (":")[1].split (",")[1]
+			#tablaGastos = self.fields [fieldName]["value"]
+			#value		= self.getValueTablaGastos (tablaGastos, rowName, colName)
 
 		elif "Carga_Tipo" in docField and not "Descripcion" in docField and self.docType == "MANIFIESTO":
 			fieldValue = self.fields [docField]["value"]
 			value = 1 if "x" in fieldValue or "X" in fieldValue else 0
 
 		else:
 			value = self.fields [docField]["content"]
```

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_cartaporte.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 			# print ("\n>>>>>> Datos Generales de la CPIC: Condiciones <<<<<<<<")
 			#--------------------------------------------------------------
 			condiciones                              = Utils.checkLow (self.getCondiciones ())
 			self.ecudoc ["38_CondicionesTransporte"] = condiciones ["transporte"]
 			self.ecudoc ["39_CondicionesPago"]       = condiciones ["pago"]
 
 			unidades                       = self.getUnidadesMedidaInfo ()
-			bultosInfo                         = self.getBultosInfo ()
+			bultosInfo                     = self.getBultosInfo ()
 			self.ecudoc ["40_PesoNeto"]	   = unidades ["pesoNeto"]
 			self.ecudoc ["41_PesoBruto"]   = unidades ["pesoBruto"]
 			self.ecudoc ["42_TotalBultos"] = bultosInfo ["cantidad"]
 			self.ecudoc ["43_Volumen"]	   = unidades ["volumen"]
 			self.ecudoc ["44_OtraUnidad"]  = unidades ["otraUnidad"]
 
 			# Incoterm
@@ -204,35 +204,43 @@
 	def getMSN (self):
 		MSN = self.empresa ["MSN"]
 		return MSN if MSN else "||LOW"
 
 	def getNombreEmpresa (self):
 		return self.empresa ["nombre"]
 
+	def getDireccionEmpresa (self):
+		return self.empresa ["direccion"]
+
+	def getIdEmpresa (self):
+		id = self.empresa ["idNumero"]
+		return id
 	#------------------------------------------------------------
 	# Return the code number from the text matching a "deposito"
 	#-- BOTERO-SOTO en casilla 21 o 22, NTA en la 22 ------------
 	#------------------------------------------------------------
 	def getDepositoMercancia (self):
 		for casilla in ["21_Instrucciones", "22_Observaciones"]:
 			text = ""
 			try:
 				text        = Utils.getValue (self.fields, casilla)
 				reBodega    = r'BODEGA[S]?\s+\b(\w*)\b'
 				bodegaText  = Extractor.getValueRE (reBodega, text)
 				Utils.printx (f"Extrayendo código para el deposito '{bodegaText}'")
+				if bodegaText == None:
+					return None
 
 				depositosDic = Extractor.getDataDic ("depositos_tulcan.txt", self.resourcesPath)
 
 				for id in depositosDic:
 					if bodegaText in depositosDic [id]:
 						Utils.printx (f"...Encontrado código '{id}' para '{depositosDic [id]}'")
 						return id
 			except:
-				Utils.printException (f"EXCEPCION: Obteniendo bodega desde texto '{text}'")
+				Utils.printException (f"Obteniendo bodega desde texto '{text}'")
 		return "||LOW"
 
 	def old_getDepositoMercancia (self):
 		for casilla in ["21_Instrucciones", "22_Observaciones"]:
 			try:
 				text        = Utils.getValue (self.fields, casilla)
 				reBodega    = r'BODEGA[S]?\s+\b(\w*)\b'
@@ -243,37 +251,21 @@
 					#Utils.printx (f"Bodega texto: '{bodegaText}', BodegaFullname: '{bodegaFullname}'")
 					if bodegaText in bodegaFullname:
 						return bodegaFullname
 			except:
 				Utils.printx (f"EXCEPCION: Obteniendo bodega desde texto '{text}'")
 		return "||LOW"
 
-	def getDireccionEmpresa (self):
-		return self.empresa ["direccion"]
-
-	def getIdEmpresa (self):
-		id = Utils.convertToEcuapassId (self.empresa ["idNumero"])
-		return id
 	#-------------------------------------------------------------------
 	#-- Get location info: ciudad, pais, fecha -------------------------
 	#-- Boxes: Recepcion, Embarque, Entrega ----------------------------
 	#-------------------------------------------------------------------
 	def getLocationInfo (self, key):
-		location = {"ciudad":"||LOW", "pais":"||LOW", "fecha":"||LOW"}
-		try:
-			text   = Utils.getValue (self.fields, key)
-			text   = text.replace ("\n", " ")
-			# Fecha
-			fecha = Extractor.getDate (text, self.resourcesPath)
-			location ["fecha"] = fecha if fecha else "||LOW"
-			# Pais
-			text, location = Extractor.removeSubjectCiudadPais (text, location, self.resourcesPath, key)
-		except:
-			Utils.printException (f"Obteniendo datos de lo localización: '{key}' en el texto", text)
-
+		text   = Utils.getValue (self.fields, key)
+		location = Extractor.extractLocationDate (text, self.resourcesPath, key)
 		return (location)
 
 	#-----------------------------------------------------------
 	# Get "Entrega" location and suggest a date if it is None
 	#-----------------------------------------------------------
 	def getEntregaLocation (self, key):
 		location = self.getLocationInfo (key)
@@ -415,99 +407,50 @@
 	# Get 'gastos' info: monto, moneda, otros gastos
 	#-----------------------------------------------------------
 	def getGastosInfo (self):
 		gastos = {"fleteRemi":None, "monedaRemi":None,       "fleteDest":None,       "monedaDest":None,
 			"otrosGastosRemi":None, "otrosMonedaRemi":None, "otrosGastosDest":None, "otrosMonedaDest": None,
 			"totalGastosRemi":None, "totalMonedaRemi": None, "totalGastosDest":None, "totalMonedaDest":None}
 		try:
-			tabla = self.fields ["17_Gastos"]["value"]
-
 			# DESTINATARIO:
 			USD = "USD"
-			gastos ["fleteDest"]	   = self.getValueTablaGastos (tabla, "ValorFlete", "MontoDestinatario")
+			gastos ["fleteDest"]	   = self.fields ["17_Gastos:ValorFlete,MontoDestinatario"]["value"]
 			gastos ["monedaDest"]      = USD if gastos ["fleteDest"] else None
-			gastos ["otrosGastosDest"] = self.getValueTablaGastos (tabla, "OtrosGastos", "MontoDestinatario")
+			gastos ["otrosGastosDest"] = self.fields ["17_Gastos:OtrosGastos,MontoDestinatario"]["value"]
 			gastos ["otrosMonedaDest"] = USD if gastos ["otrosGastosDest"] else None
-			gastos ["totalGastosDest"] = self.getValueTablaGastos (tabla, "Total", "MontoDestinatario")
+			gastos ["totalGastosDest"] = self.fields ["17_Gastos:Total,MontoDestinatario"]["value"]
 			gastos ["totalMonedaDest"] = USD if gastos ["totalGastosDest"] else None
 
 			# REMITENTE: 
-			gastos ["fleteRemi"]       = self.getValueTablaGastos (tabla, "ValorFlete", "MontoRemitente")
+			gastos ["fleteRemi"]       = self.fields ["17_Gastos:ValorFlete,MontoRemitente"]["value"]
 			gastos ["monedaRemi"]      = USD if gastos ["fleteRemi"] else None
-			gastos ["otrosGastosRemi"] = self.getValueTablaGastos (tabla, "OtrosGastos", "MontoRemitente")
+			gastos ["otrosGastosRemi"] = self.fields ["17_Gastos:OtrosGastos,MontoRemitente"]["value"]
 			gastos ["otrosMonedaRemi"] = USD if gastos ["otrosGastosRemi"] else None
-			gastos ["totalGastosRemi"] = self.getValueTablaGastos (tabla, "Total", "MontoRemitente")
+			gastos ["totalGastosRemi"] = self.fields ["17_Gastos:Total,MontoRemitente"]["value"]
 			gastos ["totalMonedaRemi"] = USD if gastos ["totalGastosRemi"] else None
 
 			for k in gastos.keys ():
 				if not "moneda" in k.lower ():
+					gastos [k] = None if gastos [k] == "" else gastos[k]
 					gastos [k] = Utils.convertToAmericanFormat (gastos [k])
 		except:
 			Utils.printException ("Obteniendo valores de 'gastos'")
 
 		return gastos
 
-	#-- Get value from Cartaporte Gastos table
-	def getValueTablaGastos (self, tabla, firstKey, secondKey):
-		try:
-			text = tabla [firstKey]["value"][secondKey]["value"]
-			value = Utils.getNumber (text)
-			return value
-		except:
-			#print (f"Sin valor en '{firstKey}'-'{secondKey}')")
-			#printx (traceback_format_exc())
-			return None
 	#-------------------------------------------------------------------
 	#-- For NTA and BYZA:
 	#   Get subject info: nombre, dir, pais, ciudad, id, idNro ---------
 	#-- BYZA format: <Nombre>\n<Direccion>\n<PaisCiudad><TipoID:ID> -----
 	#-------------------------------------------------------------------
 	#-- Get subject info: nombre, dir, pais, ciudad, id, idNro
-	def getSubjectInfo (self, key):
-		subject = {"nombre":None, "direccion":None, "pais": None, 
-		           "ciudad":None, "tipoId":None, "numeroId": None}
-		try:
-			text	= Utils.getValue (self.fields, key)
-			lines   = text.split ("\n")
-
-			if len (lines) == 3:
-				nameDirLines = lines [0:2]
-				idPaisLine   = lines [2]
-			elif len (lines) == 4:
-				nameDirLines = lines [0:3]
-				idPaisLine   = lines [3]
-			elif len (lines) < 3:
-				print (f">>> Alerta:  Pocas líneas de texto en '{key}' para extraer la información.")
-				return subject
-
-			text, subject        = Extractor.removeSubjectId (idPaisLine, subject, key)
-			text, subject        = Extractor.removeSubjectCiudadPais (text, subject, self.resourcesPath, key)
-			text, subject        = Extractor.removeSubjectCiudadPais (text, subject, self.resourcesPath, key)
-			nameDirText          = "\n".join (nameDirLines)
-			text, subject        = Extractor.removeSubjectNombreDireccion (nameDirText, subject, key)
-			subject ["numeroId"] = Utils.convertToEcuapassId (subject ["numeroId"])
-		except:
-			Utils.printException (f"Obteniendo datos del sujeto: '{key}' en el texto: '{text}'")
-
-		print ("--text:", text)
-		print (subject)
+	def getSubjectInfo (self, subjectType):
+		text	= Utils.getValue (self.fields, subjectType)
+		subject = Extractor.getSubjectInfoFromText (text, self.resourcesPath, subjectType)
 		return (subject)
 
-#	#-- Overwritten: Get value from document field
-#	def getDocumentFieldValue (self, docField):
-#		if "Gastos" in docField:
-#			fieldName	= docField.split (":")[0]
-#			rowName		= docField.split (":")[1].split (",")[0]
-#			colName		= docField.split (":")[1].split (",")[1]
-#			tablaGastos = self.fields [fieldName]["value"]
-#			value		= self.getValueTablaGastos (tablaGastos, rowName, colName)
-#		else:
-#			value		= super ().getDocumentFieldValue (docField)
-#			
-#		return value
-	
 #--------------------------------------------------------------------
 # Call main 
 #--------------------------------------------------------------------
 if __name__ == '__main__':
 	main ()
```

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 		text	= Utils.getValue (self.fields, key)
 		try:
 			text    = re.sub ("\s*//\s*", "", text)   # For SILOG "//" separator cartaportes
 			text, subject = Extractor.removeSubjectId (text, subject, key)
 			text, subject = Extractor.removeSubjectCiudadPais (text, subject, self.resourcesPath, key)
 			text, subject = Extractor.removeSubjectNombreDireccion (text, subject, key)
 		except:
-			Utils.printException (f"Obteniendo datos del sujeto: '{key}' en el texto", text)
+			Utils.printException (f"Obteniendo datos del sujeto: '{key}' en el texto: '{text}'")
 
 		return (subject)
 
 #--------------------------------------------------------------------
 # Call main 
 #--------------------------------------------------------------------
 if __name__ == '__main__':
```

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_declaracion.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_declaracion.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_manifiesto.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py` & `ecuapassdocs-0.75/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/old-utils.py` & `ecuapassdocs-0.75/ecuapassdocs/info/old-utils.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/info/resourceloader.py` & `ecuapassdocs-0.75/ecuapassdocs/info/resourceloader.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/out.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/out.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/paises_todos.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/paises_todos.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/sustancias.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/sustancias.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/cartaporte_input_parameters.json` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto_input_parameters.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2643568840579709%*

 * *Differences: {"'id'": "{'x': 400, 'ecudocsField': '', 'codebinField': '', delete: ['field', 'fieldCodebin']}",*

 * * "'numero'": "{'x': 200, 'ecudocsField': '', 'codebinField': '', delete: ['field', "*

 * *             "'fieldCodebin']}",*

 * * "'txt00'": "{'maxChars': 12, 'width': 203, 'x': 847, 'y': 94, 'ecudocsField': '00b_Numero', "*

 * *            "'codebinField': '', delete: ['field', 'fieldCodebin']}",*

 * * "'txt01'": "{'fontSize': '28px', 'height': 150, 'maxChars': 100, 'maxLines': 5, 'width': 503, "*

 * *            "'x': 52, 'y': 172, 'e […]*

```diff
@@ -1,652 +1,790 @@
 {
     "id": {
         "align": "left",
         "class": "input_numero",
-        "field": "",
-        "fieldCodebin": "",
+        "codebinField": "",
+        "ecudocsField": "",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
         "maxChars": 10,
         "maxLines": 1,
         "restrictions": [
             "hidden",
             "readonly",
             "color=red"
         ],
         "value": "",
         "width": 233,
-        "x": 300,
+        "x": 400,
         "y": 88
     },
     "numero": {
         "align": "left",
         "class": "input_numero",
-        "field": "",
-        "fieldCodebin": "",
+        "codebinField": "",
+        "ecudocsField": "",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
         "maxChars": 10,
         "maxLines": 1,
         "restrictions": [
             "hidden",
             "readonly",
             "color=red"
         ],
         "value": "",
         "width": 233,
-        "x": 300,
+        "x": 200,
         "y": 88
     },
     "txt00": {
         "align": "left",
         "class": "input_numero",
-        "field": "00b_Numero",
-        "fieldCodebin": "nocpic",
+        "codebinField": "",
+        "ecudocsField": "00b_Numero",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
-        "maxChars": 10,
+        "maxChars": 12,
         "maxLines": 1,
         "restrictions": [
             "color=red"
         ],
         "value": "",
-        "width": 233,
-        "x": 797,
-        "y": 88
+        "width": 203,
+        "x": 847,
+        "y": 94
     },
     "txt01": {
         "align": "left",
         "class": "input_numero",
-        "field": "01_Transportista",
-        "fieldCodebin": "",
+        "codebinField": "",
+        "ecudocsField": "01_Transportista",
         "font": "hidden",
-        "fontSize": "26px",
-        "height": 103,
-        "maxChars": 10,
-        "maxLines": 1,
+        "fontSize": "28px",
+        "height": 150,
+        "maxChars": 100,
+        "maxLines": 5,
         "restrictions": [
             "hidden"
         ],
         "value": "",
-        "width": 501,
-        "x": 40,
-        "y": 162
+        "width": 503,
+        "x": 52,
+        "y": 172
     },
     "txt02": {
-        "align": "left",
-        "class": "input_empresa",
-        "field": "02_Remitente",
-        "fieldCodebin": "nremitente",
-        "font": "normal",
-        "fontSize": "14px",
-        "height": 70,
-        "maxChars": 50,
-        "maxLines": 4,
+        "align": "center",
+        "class": "input_permiso",
+        "codebinField": "",
+        "ecudocsField": "02_Permiso_Originario",
+        "font": "large",
+        "fontSize": "28px",
+        "height": 58,
+        "maxChars": 28,
+        "maxLines": 2,
         "value": "",
-        "width": 501,
-        "x": 40,
-        "y": 302
+        "width": 485,
+        "x": 572,
+        "y": 172
     },
     "txt03": {
-        "align": "left",
-        "class": "input_empresa",
-        "field": "03_Destinatario",
-        "fieldCodebin": "ndestinatario",
-        "font": "normal",
-        "fontSize": "14px",
-        "height": 70,
-        "maxChars": 50,
-        "maxLines": 4,
+        "align": "center",
+        "class": "input_permiso",
+        "codebinField": "",
+        "ecudocsField": "03_Permiso_Servicios",
+        "font": "large",
+        "fontSize": "28px",
+        "height": 58,
+        "maxChars": 28,
+        "maxLines": 2,
         "value": "",
-        "width": 501,
-        "x": 40,
-        "y": 397
+        "width": 485,
+        "x": 572,
+        "y": 264
     },
     "txt04": {
         "align": "left",
-        "class": "input_empresa",
-        "field": "04_Consignatario",
-        "fieldCodebin": "consignatario",
+        "class": "input_general",
+        "codebinField": "a4",
+        "ecudocsField": "04_Camion_Marca",
         "font": "normal",
         "fontSize": "14px",
-        "height": 70,
-        "maxChars": 50,
-        "maxLines": 4,
+        "height": 25,
+        "maxChars": 25,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 40,
-        "y": 492
+        "width": 251,
+        "x": 52,
+        "y": 372
     },
     "txt05": {
         "align": "left",
-        "class": "input_empresa",
-        "field": "05_Notificado",
-        "fieldCodebin": "notificar",
+        "class": "input_fecha",
+        "codebinField": "a5",
+        "ecudocsField": "05_Camion_AnoFabricacion",
         "font": "normal",
         "fontSize": "14px",
-        "height": 70,
-        "maxChars": 50,
-        "maxLines": 4,
+        "height": 25,
+        "maxChars": 15,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 555,
-        "y": 140
+        "width": 135,
+        "x": 316,
+        "y": 372
     },
     "txt06": {
         "align": "left",
-        "class": "input-lugar-fecha",
-        "field": "06_Recepcion",
-        "fieldCodebin": "lugar1",
+        "class": "input_placaPais",
+        "codebinField": "a6",
+        "ecudocsField": "06_Camion_PlacaPais",
         "font": "normal",
         "fontSize": "14px",
-        "height": 40,
-        "maxChars": 50,
-        "maxLines": 2,
+        "height": 25,
+        "maxChars": 30,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 555,
-        "y": 235
+        "width": 279,
+        "x": 463,
+        "y": 372
     },
     "txt07": {
         "align": "left",
-        "class": "input-lugar-fecha",
-        "field": "07_Embarque",
-        "fieldCodebin": "lugar2",
+        "class": "input_general",
+        "codebinField": "a7",
+        "ecudocsField": "07_Camion_Chasis",
         "font": "normal",
         "fontSize": "14px",
-        "height": 40,
-        "maxChars": 50,
-        "maxLines": 2,
+        "height": 25,
+        "maxChars": 30,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 555,
-        "y": 312
+        "width": 304,
+        "x": 753,
+        "y": 372
     },
     "txt08": {
         "align": "left",
-        "class": "input_lugar",
-        "field": "08_Entrega",
-        "fieldCodebin": "lugar3",
+        "class": "input_certificado",
+        "codebinField": "a8",
+        "ecudocsField": "08_Certificado_Habilitacion",
         "font": "normal",
         "fontSize": "14px",
-        "height": 40,
-        "maxChars": 50,
-        "maxLines": 2,
+        "height": 20,
+        "maxChars": 80,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 555,
-        "y": 405
+        "width": 700,
+        "x": 277,
+        "y": 403
     },
     "txt09": {
         "align": "left",
-        "class": "input_condiciones",
-        "field": "09_Condiciones",
-        "fieldCodebin": "condiciones",
+        "class": "input_general",
+        "codebinField": "a9",
+        "ecudocsField": "09_Remolque_Marca",
         "font": "normal",
         "fontSize": "14px",
-        "height": 70,
-        "maxChars": 50,
-        "maxLines": 4,
+        "height": 25,
+        "maxChars": 25,
+        "maxLines": 1,
         "value": "",
-        "width": 501,
-        "x": 555,
-        "y": 492
+        "width": 251,
+        "x": 52,
+        "y": 464
     },
     "txt0a": {
         "align": "left",
         "class": "input_numero",
-        "field": "00_Pais",
-        "fieldCodebin": "pais",
+        "codebinField": "pais",
+        "ecudocsField": "00_Pais",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
         "maxChars": 2,
         "maxLines": 1,
         "restrictions": [
             "readonly",
             "color=red"
         ],
         "value": "",
         "width": 40,
-        "x": 696,
-        "y": 88
+        "x": 760,
+        "y": 94
     },
     "txt10": {
         "align": "left",
-        "class": "input_bultos",
-        "field": "10_CantidadClase_Bultos",
-        "fieldCodebin": "a10",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 302,
-        "maxChars": 13,
-        "maxLines": 22,
+        "class": "input_general",
+        "codebinField": "a10",
+        "ecudocsField": "10_Remolque_AnoFabricacion",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 25,
+        "maxChars": 15,
+        "maxLines": 1,
         "value": "",
-        "width": 130,
-        "x": 43,
-        "y": 643
+        "width": 135,
+        "x": 316,
+        "y": 464
     },
     "txt11": {
         "align": "left",
-        "class": "input_bultos",
-        "field": "11_MarcasNumeros_Bultos",
-        "fieldCodebin": "a11",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 302,
-        "maxChars": 13,
-        "maxLines": 22,
+        "class": "input_placaPais",
+        "codebinField": "a11",
+        "ecudocsField": "11_Remolque_PlacaPais",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 25,
+        "maxChars": 30,
+        "maxLines": 1,
         "value": "",
-        "width": 122,
-        "x": 183,
-        "y": 643
+        "width": 277,
+        "x": 464,
+        "y": 464
     },
     "txt12": {
         "align": "left",
-        "class": "input_descripcion",
-        "field": "12_Descripcion_Bultos",
-        "fieldCodebin": "detalle",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 302,
-        "maxChars": 50,
-        "maxLines": 22,
-        "value": "",
-        "width": 472,
-        "x": 315,
-        "y": 643
-    },
-    "txt13_1": {
-        "align": "right",
-        "class": "input_valor",
-        "field": "13a_Peso_Neto",
-        "fieldCodebin": "neto1",
+        "class": "input_general",
+        "codebinField": "a12",
+        "ecudocsField": "12_Remolque_Otro",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 10,
+        "height": 25,
+        "maxChars": 30,
         "maxLines": 1,
         "value": "",
-        "width": 121,
-        "x": 797,
-        "y": 677
+        "width": 303,
+        "x": 754,
+        "y": 464
     },
-    "txt13_2": {
-        "align": "right",
-        "class": "input_valor",
-        "field": "13b_Peso_Bruto",
-        "fieldCodebin": "bruto1",
+    "txt13": {
+        "align": "left",
+        "class": "input_conductor",
+        "codebinField": "a13",
+        "ecudocsField": "13_Conductor_Nombre",
         "font": "normal",
         "fontSize": "14px",
         "height": 22,
-        "maxChars": 10,
+        "maxChars": 50,
         "maxLines": 1,
         "value": "",
-        "width": 121,
-        "x": 935,
-        "y": 677
+        "width": 470,
+        "x": 52,
+        "y": 526
     },
     "txt14": {
-        "align": "right",
-        "class": "input_valor",
-        "field": "14_Volumen",
-        "fieldCodebin": "volumen",
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a14",
+        "ecudocsField": "14_Conductor_Id",
         "font": "normal",
         "fontSize": "14px",
         "height": 22,
-        "maxChars": 10,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 121,
-        "x": 797,
-        "y": 777
+        "width": 210,
+        "x": 52,
+        "y": 571
     },
     "txt15": {
-        "align": "right",
-        "class": "input_valor",
-        "field": "15_Otras_Unidades",
-        "fieldCodebin": "omedidas",
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a15",
+        "ecudocsField": "15_Conductor_Nacionalidad",
         "font": "normal",
         "fontSize": "14px",
         "height": 22,
-        "maxChars": 10,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 121,
-        "x": 935,
-        "y": 777
+        "width": 247,
+        "x": 276,
+        "y": 571
     },
     "txt16": {
         "align": "left",
-        "class": "input_incoterm",
-        "field": "16_Incoterms",
-        "fieldCodebin": "precio",
+        "class": "input_general",
+        "codebinField": "a16",
+        "ecudocsField": "16_Conductor_Licencia",
         "font": "normal",
         "fontSize": "14px",
-        "height": 67,
-        "maxChars": 22,
-        "maxLines": 3,
+        "height": 22,
+        "maxChars": 20,
+        "maxLines": 1,
         "value": "",
-        "width": 263,
-        "x": 795,
-        "y": 869
+        "width": 210,
+        "x": 52,
+        "y": 615
     },
-    "txt17_11": {
-        "align": "right",
-        "class": "input_valor",
-        "field": "17_Gastos:ValorFlete,MontoRemitente",
-        "fieldCodebin": "montor",
+    "txt17": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a17",
+        "ecudocsField": "17_Conductor_Libreta",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 114,
-        "x": 112,
-        "y": 997
+        "width": 245,
+        "x": 277,
+        "y": 615
     },
-    "txt17_12": {
-        "align": "right",
-        "class": "input_valor",
-        "field": "17_Gastos:Seguro,MontoRemitente",
-        "fieldCodebin": "montoor",
+    "txt18": {
+        "align": "left",
+        "class": "input_conductor",
+        "codebinField": "a18",
+        "ecudocsField": "18_Auxiliar_Nombre",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 50,
         "maxLines": 1,
         "value": "",
-        "width": 114,
-        "x": 112,
-        "y": 1018
+        "width": 522,
+        "x": 535,
+        "y": 526
     },
-    "txt17_13": {
-        "align": "right",
-        "class": "input_valor",
-        "field": "17_Gastos:OtrosGastos,MontoRemitente",
-        "fieldCodebin": "montor1",
+    "txt19": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a19",
+        "ecudocsField": "19_Auxiliar_Id",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 114,
-        "x": 112,
-        "y": 1039
+        "width": 252,
+        "x": 535,
+        "y": 571
     },
-    "txt17_14": {
-        "align": "right",
-        "class": "input_valor",
-        "field": "17_Gastos:Total,MontoRemitente",
-        "fieldCodebin": "totalmr",
+    "txt20": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a20",
+        "ecudocsField": "20_Auxiliar_Nacionalidad",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 114,
-        "x": 112,
-        "y": 1061
+        "width": 257,
+        "x": 800,
+        "y": 571
     },
-    "txt17_21": {
+    "txt21": {
         "align": "left",
         "class": "input_general",
-        "field": "17_Gastos:ValorFlete,MonedaRemitente",
-        "fieldCodebin": "moneda1",
+        "codebinField": "a21",
+        "ecudocsField": "21_Auxiliar_Licencia",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 80,
-        "x": 240,
-        "y": 997
+        "width": 252,
+        "x": 535,
+        "y": 615
     },
-    "txt17_22": {
+    "txt22": {
         "align": "left",
         "class": "input_general",
-        "field": "17_Gastos:Seguro,MonedaRemitente",
-        "fieldCodebin": "moneda5",
+        "codebinField": "a22",
+        "ecudocsField": "22_Auxiliar_Libreta",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 20,
         "maxLines": 1,
         "value": "",
-        "width": 80,
-        "x": 240,
-        "y": 1018
+        "width": 257,
+        "x": 800,
+        "y": 615
     },
-    "txt17_23": {
+    "txt23": {
         "align": "left",
-        "class": "input_general",
-        "field": "17_Gastos:OtrosGastos,MonedaRemitente",
-        "fieldCodebin": "moneda3",
+        "class": "input_lugar",
+        "codebinField": "23",
+        "ecudocsField": "23_Carga_CiudadPais",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 50,
         "maxLines": 1,
         "value": "",
-        "width": 80,
-        "x": 240,
-        "y": 1039
+        "width": 470,
+        "x": 52,
+        "y": 676
     },
-    "txt17_24": {
+    "txt24": {
+        "align": "left",
+        "class": "input_lugar",
+        "codebinField": "24",
+        "ecudocsField": "24_Descarga_CiudadPais",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 22,
+        "maxChars": 55,
+        "maxLines": 1,
+        "value": "",
+        "width": 522,
+        "x": 535,
+        "y": 676
+    },
+    "txt25_1": {
+        "align": "left",
+        "class": "input_tipocarga",
+        "codebinField": "radio-1-set",
+        "ecudocsField": "25a_Carga_TipoPeligrosa",
+        "font": "normal",
+        "fontSize": "18px",
+        "height": 22,
+        "maxChars": 2,
+        "maxLines": 1,
+        "value": "",
+        "width": 18,
+        "x": 152,
+        "y": 724
+    },
+    "txt25_2": {
+        "align": "left",
+        "class": "input_tipocarga",
+        "codebinField": "radio-3-set",
+        "ecudocsField": "25b_Carga_TipoSustancias",
+        "font": "normal",
+        "fontSize": "18px",
+        "height": 22,
+        "maxChars": 2,
+        "maxLines": 1,
+        "value": "",
+        "width": 18,
+        "x": 432,
+        "y": 724
+    },
+    "txt25_3": {
+        "align": "left",
+        "class": "input_tipocarga",
+        "codebinField": "radio-2-set",
+        "ecudocsField": "25c_Carga_TipoPerecible",
+        "font": "normal",
+        "fontSize": "18px",
+        "height": 22,
+        "maxChars": 2,
+        "maxLines": 1,
+        "value": "",
+        "width": 18,
+        "x": 575,
+        "y": 724
+    },
+    "txt25_4": {
+        "align": "left",
+        "class": "input_tipocarga",
+        "codebinField": "radio-4-set",
+        "ecudocsField": "25d_Carga_TipoOtra",
+        "font": "normal",
+        "fontSize": "18px",
+        "height": 22,
+        "maxChars": 2,
+        "maxLines": 1,
+        "value": "",
+        "width": 18,
+        "x": 700,
+        "y": 724
+    },
+    "txt25_5": {
         "align": "left",
         "class": "input_general",
-        "field": "17_Gastos:Total,MonedaRemitente",
-        "fieldCodebin": "monedat",
+        "codebinField": "25d",
+        "ecudocsField": "25e_Carga_TipoDescripcion",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 48,
+        "maxChars": 20,
+        "maxLines": 2,
+        "value": "",
+        "width": 258,
+        "x": 799,
+        "y": 710
+    },
+    "txt26": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "26",
+        "ecudocsField": "26_Carga_Contenedores",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 22,
+        "maxChars": 50,
         "maxLines": 1,
         "value": "",
-        "width": 80,
-        "x": 240,
-        "y": 1061
+        "width": 470,
+        "x": 52,
+        "y": 798
     },
-    "txt17_31": {
-        "align": "right",
-        "class": "input_valor",
-        "field": "17_Gastos:ValorFlete,MontoDestinatario",
-        "fieldCodebin": "montod",
+    "txt27": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "27",
+        "ecudocsField": "27_Carga_Precintos",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 55,
         "maxLines": 1,
         "value": "",
-        "width": 100,
-        "x": 334,
-        "y": 997
+        "width": 522,
+        "x": 535,
+        "y": 798
     },
-    "txt17_32": {
+    "txt28": {
+        "align": "left",
+        "class": "input_cartaporte",
+        "codebinField": "a28",
+        "ecudocsField": "28_Mercancia_Cartaporte",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 341,
+        "maxChars": 13,
+        "maxLines": 20,
+        "value": "",
+        "width": 95,
+        "x": 52,
+        "y": 857
+    },
+    "txt29": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a29",
+        "ecudocsField": "29_Mercancia_Descripcion",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 341,
+        "maxChars": 52,
+        "maxLines": 20,
+        "value": "",
+        "width": 380,
+        "x": 155,
+        "y": 857
+    },
+    "txt30": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a30",
+        "ecudocsField": "30_Mercancia_Bultos",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 341,
+        "maxChars": 14,
+        "maxLines": 20,
+        "value": "",
+        "width": 105,
+        "x": 540,
+        "y": 857
+    },
+    "txt31": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "a31",
+        "ecudocsField": "31_Mercancia_Embalaje",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 341,
+        "maxChars": 17,
+        "maxLines": 20,
+        "value": "",
+        "width": 130,
+        "x": 651,
+        "y": 857
+    },
+    "txt32_1": {
         "align": "right",
         "class": "input_valor",
-        "field": "17_Gastos:Seguro,MontoDestinatario",
-        "fieldCodebin": "montod2",
+        "codebinField": "a32a",
+        "ecudocsField": "32a_Peso_Bruto",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
-        "maxLines": 1,
+        "height": 341,
+        "maxChars": 9,
+        "maxLines": 20,
         "value": "",
-        "width": 100,
-        "x": 334,
-        "y": 1018
+        "width": 82,
+        "x": 795,
+        "y": 857
     },
-    "txt17_33": {
+    "txt32_2": {
         "align": "right",
         "class": "input_valor",
-        "field": "17_Gastos:OtrosGastos,MontoDestinatario",
-        "fieldCodebin": "montod1",
+        "codebinField": "a34b",
+        "ecudocsField": "32a_Peso_BrutoTotal",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
+        "height": 22,
+        "maxChars": 9,
         "maxLines": 1,
         "value": "",
-        "width": 100,
-        "x": 334,
-        "y": 1039
+        "width": 82,
+        "x": 795,
+        "y": 1223
     },
-    "txt17_34": {
+    "txt32_3": {
         "align": "right",
         "class": "input_valor",
-        "field": "17_Gastos:Total,MontoDestinatario",
-        "fieldCodebin": "totalmd",
+        "codebinField": "a32b",
+        "ecudocsField": "32b_Peso_Neto",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 10,
-        "maxLines": 1,
+        "height": 341,
+        "maxChars": 9,
+        "maxLines": 20,
         "value": "",
-        "width": 100,
-        "x": 334,
-        "y": 1061
+        "width": 82,
+        "x": 887,
+        "y": 857
     },
-    "txt17_41": {
-        "align": "left",
-        "class": "input_general",
-        "field": "17_Gastos:ValorFlete,MonedaDestinatario",
-        "fieldCodebin": "moneda2",
+    "txt32_4": {
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "a34c",
+        "ecudocsField": "32b_Peso_NetoTotal",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 9,
         "maxLines": 1,
         "value": "",
-        "width": 94,
-        "x": 447,
-        "y": 997
+        "width": 82,
+        "x": 887,
+        "y": 1223
     },
-    "txt17_42": {
+    "txt33_1": {
         "align": "left",
-        "class": "input_general",
-        "field": "17_Gastos:Seguro,MonedaDestinatario",
-        "fieldCodebin": "moneda6",
+        "class": "input_valor",
+        "codebinField": "a33",
+        "ecudocsField": "33_Otra_Medida",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
-        "maxLines": 1,
+        "height": 341,
+        "maxChars": 9,
+        "maxLines": 20,
         "value": "",
-        "width": 94,
-        "x": 447,
-        "y": 1018
+        "width": 82,
+        "x": 979,
+        "y": 857
     },
-    "txt17_43": {
+    "txt33_2": {
         "align": "left",
-        "class": "input_general",
-        "field": "17_Gastos:OtrosGastos,MonedaDestinatario",
-        "fieldCodebin": "moneda4",
+        "class": "input_valor",
+        "codebinField": "a34d",
+        "ecudocsField": "33_Otra_MedidaTotal",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 9,
         "maxLines": 1,
         "value": "",
-        "width": 94,
-        "x": 447,
-        "y": 1039
+        "width": 82,
+        "x": 979,
+        "y": 1223
     },
-    "txt17_44": {
+    "txt34": {
         "align": "left",
-        "class": "input_general",
-        "field": "17_Gastos:Total,MonedaDestinatario",
-        "fieldCodebin": "monedat2",
+        "class": "input_incoterm",
+        "codebinField": "a34a",
+        "ecudocsField": "34_Precio_Incoterm_Moneda",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 8,
+        "height": 22,
+        "maxChars": 70,
         "maxLines": 1,
         "value": "",
-        "width": 94,
-        "x": 447,
-        "y": 1061
+        "width": 653,
+        "x": 52,
+        "y": 1223
     },
-    "txt18": {
+    "txt35": {
         "align": "left",
-        "class": "input_documento",
-        "field": "18_Documentos",
-        "fieldCodebin": "documentosr",
+        "class": "input_general",
+        "codebinField": "35",
+        "ecudocsField": "35_Observaciones",
         "font": "normal",
         "fontSize": "14px",
         "height": 36,
         "maxChars": 50,
         "maxLines": 2,
         "value": "",
-        "width": 503,
-        "x": 40,
-        "y": 1103
+        "width": 470,
+        "x": 52,
+        "y": 1262
     },
-    "txt19": {
+    "txt37": {
         "align": "left",
-        "class": "input-lugar-fecha",
-        "field": "19_Emision",
-        "fieldCodebin": "lugaremision",
+        "class": "input_general",
+        "codebinField": "37",
+        "ecudocsField": "37_Aduana_Cruce",
         "font": "normal",
         "fontSize": "14px",
-        "height": 40,
-        "maxChars": 50,
-        "maxLines": 2,
+        "height": 22,
+        "maxChars": 27,
+        "maxLines": 1,
         "value": "",
-        "width": 503,
-        "x": 40,
-        "y": 1171
+        "width": 253,
+        "x": 535,
+        "y": 1262
     },
-    "txt21": {
+    "txt38": {
         "align": "left",
         "class": "input_general",
-        "field": "21_Instrucciones",
-        "fieldCodebin": "instrucciones",
+        "codebinField": "38",
+        "ecudocsField": "38_Aduana_Destino",
         "font": "normal",
         "fontSize": "14px",
-        "height": 85,
-        "maxChars": 50,
-        "maxLines": 5,
+        "height": 22,
+        "maxChars": 27,
+        "maxLines": 1,
         "value": "",
-        "width": 503,
-        "x": 560,
-        "y": 963
+        "width": 257,
+        "x": 800,
+        "y": 1262
     },
-    "txt22": {
+    "txt40": {
         "align": "left",
-        "class": "input_general",
-        "field": "22_Observaciones",
-        "fieldCodebin": "observaciones",
-        "font": "normal",
-        "fontSize": "14px",
-        "height": 85,
-        "maxChars": 53,
-        "maxLines": 5,
+        "class": "input_fecha",
+        "codebinField": "a40",
+        "ecudocsField": "40_Fecha_Emision",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 22,
+        "maxChars": 50,
+        "maxLines": 1,
         "value": "",
-        "width": 503,
-        "x": 560,
-        "y": 1070
+        "width": 350,
+        "x": 180,
+        "y": 1366
     },
-    "txt24": {
+    "txt41": {
         "align": "center",
         "class": "input_tipo",
-        "field": "24_OriginalCopia",
-        "fieldCodebin": "",
+        "codebinField": "",
+        "ecudocsField": "41_OriginalCopia",
         "font": "large",
-        "fontSize": "26px",
+        "fontSize": "18px",
         "height": 30,
-        "maxChars": 10,
-        "maxLines": 1,
+        "nChars": 10,
+        "nlines": 1,
+        "restrictions": [
+            "readonly"
+        ],
         "value": "",
         "width": 173,
         "x": 477,
-        "y": 1357
+        "y": 1394
     }
 }
```

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/declaracion_input_parameters.json` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/declaracion_input_parameters.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/join.pdf` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/join.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/manifiesto_input_parameters.json` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/cartaporte_input_parameters.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2643568840579709%*

 * *Differences: {"'id'": "{'x': 300, 'ecudocsField': '', 'codebinField': '', delete: ['field', 'fieldCodebin']}",*

 * * "'numero'": "{'x': 300, 'ecudocsField': '', 'codebinField': '', delete: ['field', "*

 * *             "'fieldCodebin']}",*

 * * "'txt00'": "{'maxChars': 10, 'width': 233, 'x': 797, 'y': 88, 'ecudocsField': '00b_Numero', "*

 * *            "'codebinField': 'nocpic', delete: ['field', 'fieldCodebin']}",*

 * * "'txt01'": "{'fontSize': '26px', 'height': 103, 'maxChars': 10, 'maxLines': 1, 'width': 501, 'x': "*

 * *            "40, 'y': 16 […]*

```diff
@@ -1,790 +1,652 @@
 {
     "id": {
         "align": "left",
         "class": "input_numero",
-        "field": "",
-        "fieldCodebin": "",
+        "codebinField": "",
+        "ecudocsField": "",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
         "maxChars": 10,
         "maxLines": 1,
         "restrictions": [
             "hidden",
             "readonly",
             "color=red"
         ],
         "value": "",
         "width": 233,
-        "x": 400,
+        "x": 300,
         "y": 88
     },
     "numero": {
         "align": "left",
         "class": "input_numero",
-        "field": "",
-        "fieldCodebin": "",
+        "codebinField": "",
+        "ecudocsField": "",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
         "maxChars": 10,
         "maxLines": 1,
         "restrictions": [
             "hidden",
             "readonly",
             "color=red"
         ],
         "value": "",
         "width": 233,
-        "x": 200,
+        "x": 300,
         "y": 88
     },
     "txt00": {
         "align": "left",
         "class": "input_numero",
-        "field": "00b_Numero",
-        "fieldCodebin": "",
+        "codebinField": "nocpic",
+        "ecudocsField": "00b_Numero",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
-        "maxChars": 12,
+        "maxChars": 10,
         "maxLines": 1,
         "restrictions": [
             "color=red"
         ],
         "value": "",
-        "width": 203,
-        "x": 847,
-        "y": 94
+        "width": 233,
+        "x": 797,
+        "y": 88
     },
     "txt01": {
         "align": "left",
         "class": "input_numero",
-        "field": "01_Transportista",
-        "fieldCodebin": "",
+        "codebinField": "",
+        "ecudocsField": "01_Transportista",
         "font": "hidden",
-        "fontSize": "28px",
-        "height": 150,
-        "maxChars": 100,
-        "maxLines": 5,
+        "fontSize": "26px",
+        "height": 103,
+        "maxChars": 10,
+        "maxLines": 1,
         "restrictions": [
             "hidden"
         ],
         "value": "",
-        "width": 503,
-        "x": 52,
-        "y": 172
+        "width": 501,
+        "x": 40,
+        "y": 162
     },
     "txt02": {
-        "align": "center",
-        "class": "input_permiso",
-        "field": "02_Permiso_Originario",
-        "fieldCodebin": "",
-        "font": "large",
-        "fontSize": "28px",
-        "height": 58,
-        "maxChars": 28,
-        "maxLines": 2,
+        "align": "left",
+        "class": "input_empresa",
+        "codebinField": "nremitente",
+        "ecudocsField": "02_Remitente",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 70,
+        "maxChars": 50,
+        "maxLines": 4,
         "value": "",
-        "width": 485,
-        "x": 572,
-        "y": 172
+        "width": 501,
+        "x": 40,
+        "y": 302
     },
     "txt03": {
-        "align": "center",
-        "class": "input_permiso",
-        "field": "03_Permiso_Servicios",
-        "fieldCodebin": "",
-        "font": "large",
-        "fontSize": "28px",
-        "height": 58,
-        "maxChars": 28,
-        "maxLines": 2,
+        "align": "left",
+        "class": "input_empresa",
+        "codebinField": "ndestinatario",
+        "ecudocsField": "03_Destinatario",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 70,
+        "maxChars": 50,
+        "maxLines": 4,
         "value": "",
-        "width": 485,
-        "x": 572,
-        "y": 264
+        "width": 501,
+        "x": 40,
+        "y": 397
     },
     "txt04": {
         "align": "left",
-        "class": "input_general",
-        "field": "04_Camion_Marca",
-        "fieldCodebin": "a4",
+        "class": "input_empresa",
+        "codebinField": "consignatario",
+        "ecudocsField": "04_Consignatario",
         "font": "normal",
         "fontSize": "14px",
-        "height": 25,
-        "maxChars": 25,
-        "maxLines": 1,
+        "height": 70,
+        "maxChars": 50,
+        "maxLines": 4,
         "value": "",
-        "width": 251,
-        "x": 52,
-        "y": 372
+        "width": 501,
+        "x": 40,
+        "y": 492
     },
     "txt05": {
         "align": "left",
-        "class": "input_fecha",
-        "field": "05_Camion_AnoFabricacion",
-        "fieldCodebin": "a5",
+        "class": "input_empresa",
+        "codebinField": "notificar",
+        "ecudocsField": "05_Notificado",
         "font": "normal",
         "fontSize": "14px",
-        "height": 25,
-        "maxChars": 15,
-        "maxLines": 1,
+        "height": 70,
+        "maxChars": 50,
+        "maxLines": 4,
         "value": "",
-        "width": 135,
-        "x": 316,
-        "y": 372
+        "width": 501,
+        "x": 555,
+        "y": 140
     },
     "txt06": {
         "align": "left",
-        "class": "input_placaPais",
-        "field": "06_Camion_PlacaPais",
-        "fieldCodebin": "a6",
+        "class": "input-lugar-fecha",
+        "codebinField": "lugar1",
+        "ecudocsField": "06_Recepcion",
         "font": "normal",
         "fontSize": "14px",
-        "height": 25,
-        "maxChars": 30,
-        "maxLines": 1,
+        "height": 40,
+        "maxChars": 50,
+        "maxLines": 2,
         "value": "",
-        "width": 279,
-        "x": 463,
-        "y": 372
+        "width": 501,
+        "x": 555,
+        "y": 235
     },
     "txt07": {
         "align": "left",
-        "class": "input_general",
-        "field": "07_Camion_Chasis",
-        "fieldCodebin": "a7",
+        "class": "input-lugar-fecha",
+        "codebinField": "lugar2",
+        "ecudocsField": "07_Embarque",
         "font": "normal",
         "fontSize": "14px",
-        "height": 25,
-        "maxChars": 30,
-        "maxLines": 1,
+        "height": 40,
+        "maxChars": 50,
+        "maxLines": 2,
         "value": "",
-        "width": 304,
-        "x": 753,
-        "y": 372
+        "width": 501,
+        "x": 555,
+        "y": 312
     },
     "txt08": {
         "align": "left",
-        "class": "input_certificado",
-        "field": "08_Certificado_Habilitacion",
-        "fieldCodebin": "a8",
+        "class": "input_lugar",
+        "codebinField": "lugar3",
+        "ecudocsField": "08_Entrega",
         "font": "normal",
         "fontSize": "14px",
-        "height": 20,
-        "maxChars": 80,
-        "maxLines": 1,
+        "height": 40,
+        "maxChars": 50,
+        "maxLines": 2,
         "value": "",
-        "width": 700,
-        "x": 277,
-        "y": 403
+        "width": 501,
+        "x": 555,
+        "y": 405
     },
     "txt09": {
         "align": "left",
-        "class": "input_general",
-        "field": "09_Remolque_Marca",
-        "fieldCodebin": "a9",
+        "class": "input_condiciones",
+        "codebinField": "condiciones",
+        "ecudocsField": "09_Condiciones",
         "font": "normal",
         "fontSize": "14px",
-        "height": 25,
-        "maxChars": 25,
-        "maxLines": 1,
+        "height": 70,
+        "maxChars": 50,
+        "maxLines": 4,
         "value": "",
-        "width": 251,
-        "x": 52,
-        "y": 464
+        "width": 501,
+        "x": 555,
+        "y": 492
     },
     "txt0a": {
         "align": "left",
         "class": "input_numero",
-        "field": "00_Pais",
-        "fieldCodebin": "pais",
+        "codebinField": "",
+        "ecudocsField": "00_Pais",
         "font": "large",
         "fontSize": "26px",
         "height": 28,
         "maxChars": 2,
         "maxLines": 1,
         "restrictions": [
             "readonly",
             "color=red"
         ],
         "value": "",
         "width": 40,
-        "x": 760,
-        "y": 94
+        "x": 696,
+        "y": 88
     },
     "txt10": {
         "align": "left",
-        "class": "input_general",
-        "field": "10_Remolque_AnoFabricacion",
-        "fieldCodebin": "a10",
-        "font": "normal",
-        "fontSize": "14px",
-        "height": 25,
-        "maxChars": 15,
-        "maxLines": 1,
+        "class": "input_bultos",
+        "codebinField": "a10",
+        "ecudocsField": "10_CantidadClase_Bultos",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 302,
+        "maxChars": 13,
+        "maxLines": 22,
         "value": "",
-        "width": 135,
-        "x": 316,
-        "y": 464
+        "width": 130,
+        "x": 43,
+        "y": 643
     },
     "txt11": {
         "align": "left",
-        "class": "input_placaPais",
-        "field": "11_Remolque_PlacaPais",
-        "fieldCodebin": "a11",
-        "font": "normal",
-        "fontSize": "14px",
-        "height": 25,
-        "maxChars": 30,
-        "maxLines": 1,
+        "class": "input_bultos",
+        "codebinField": "a11",
+        "ecudocsField": "11_MarcasNumeros_Bultos",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 302,
+        "maxChars": 13,
+        "maxLines": 22,
         "value": "",
-        "width": 277,
-        "x": 464,
-        "y": 464
+        "width": 122,
+        "x": 183,
+        "y": 643
     },
     "txt12": {
         "align": "left",
-        "class": "input_general",
-        "field": "12_Remolque_Otro",
-        "fieldCodebin": "a12",
+        "class": "input_descripcion",
+        "codebinField": "detalle",
+        "ecudocsField": "12_Descripcion_Bultos",
+        "font": "small",
+        "fontSize": "12px",
+        "height": 302,
+        "maxChars": 50,
+        "maxLines": 22,
+        "value": "",
+        "width": 472,
+        "x": 315,
+        "y": 643
+    },
+    "txt13_1": {
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "neto1",
+        "ecudocsField": "13a_Peso_Neto",
         "font": "normal",
         "fontSize": "14px",
-        "height": 25,
-        "maxChars": 30,
+        "height": 22,
+        "maxChars": 10,
         "maxLines": 1,
         "value": "",
-        "width": 303,
-        "x": 754,
-        "y": 464
+        "width": 121,
+        "x": 797,
+        "y": 677
     },
-    "txt13": {
-        "align": "left",
-        "class": "input_conductor",
-        "field": "13_Conductor_Nombre",
-        "fieldCodebin": "a13",
+    "txt13_2": {
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "bruto1",
+        "ecudocsField": "13b_Peso_Bruto",
         "font": "normal",
         "fontSize": "14px",
         "height": 22,
-        "maxChars": 50,
+        "maxChars": 10,
         "maxLines": 1,
         "value": "",
-        "width": 470,
-        "x": 52,
-        "y": 526
+        "width": 121,
+        "x": 935,
+        "y": 677
     },
     "txt14": {
-        "align": "left",
-        "class": "input_general",
-        "field": "14_Conductor_Id",
-        "fieldCodebin": "a14",
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "volumen",
+        "ecudocsField": "14_Volumen",
         "font": "normal",
         "fontSize": "14px",
         "height": 22,
-        "maxChars": 20,
+        "maxChars": 10,
         "maxLines": 1,
         "value": "",
-        "width": 210,
-        "x": 52,
-        "y": 571
+        "width": 121,
+        "x": 797,
+        "y": 777
     },
     "txt15": {
-        "align": "left",
-        "class": "input_general",
-        "field": "15_Conductor_Nacionalidad",
-        "fieldCodebin": "a15",
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "omedidas",
+        "ecudocsField": "15_Otras_Unidades",
         "font": "normal",
         "fontSize": "14px",
         "height": 22,
-        "maxChars": 20,
+        "maxChars": 10,
         "maxLines": 1,
         "value": "",
-        "width": 247,
-        "x": 276,
-        "y": 571
+        "width": 121,
+        "x": 935,
+        "y": 777
     },
     "txt16": {
         "align": "left",
-        "class": "input_general",
-        "field": "16_Conductor_Licencia",
-        "fieldCodebin": "a16",
+        "class": "input_incoterm",
+        "codebinField": "precio",
+        "ecudocsField": "16_Incoterms",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 20,
-        "maxLines": 1,
+        "height": 67,
+        "maxChars": 28,
+        "maxLines": 3,
         "value": "",
-        "width": 210,
-        "x": 52,
-        "y": 615
+        "width": 263,
+        "x": 795,
+        "y": 869
     },
-    "txt17": {
-        "align": "left",
-        "class": "input_general",
-        "field": "17_Conductor_Libreta",
-        "fieldCodebin": "a17",
+    "txt17_11": {
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "montor",
+        "ecudocsField": "17_Gastos:ValorFlete,MontoRemitente",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 20,
+        "height": 20,
+        "maxChars": 10,
         "maxLines": 1,
         "value": "",
-        "width": 245,
-        "x": 277,
-        "y": 615
+        "width": 114,
+        "x": 112,
+        "y": 997
     },
-    "txt18": {
-        "align": "left",
-        "class": "input_conductor",
-        "field": "18_Auxiliar_Nombre",
-        "fieldCodebin": "a18",
+    "txt17_12": {
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "montor1",
+        "ecudocsField": "17_Gastos:Seguro,MontoRemitente",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 50,
+        "height": 20,
+        "maxChars": 10,
         "maxLines": 1,
         "value": "",
-        "width": 522,
-        "x": 535,
-        "y": 526
+        "width": 114,
+        "x": 112,
+        "y": 1018
     },
-    "txt19": {
-        "align": "left",
-        "class": "input_general",
-        "field": "19_Auxiliar_Id",
-        "fieldCodebin": "a19",
+    "txt17_13": {
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "montoor",
+        "ecudocsField": "17_Gastos:OtrosGastos,MontoRemitente",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 20,
+        "height": 20,
+        "maxChars": 10,
         "maxLines": 1,
         "value": "",
-        "width": 252,
-        "x": 535,
-        "y": 571
+        "width": 114,
+        "x": 112,
+        "y": 1039
     },
-    "txt20": {
-        "align": "left",
-        "class": "input_general",
-        "field": "20_Auxiliar_Nacionalidad",
-        "fieldCodebin": "a20",
+    "txt17_14": {
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "totalmr",
+        "ecudocsField": "17_Gastos:Total,MontoRemitente",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 20,
+        "height": 20,
+        "maxChars": 10,
         "maxLines": 1,
         "value": "",
-        "width": 257,
-        "x": 800,
-        "y": 571
+        "width": 114,
+        "x": 112,
+        "y": 1061
     },
-    "txt21": {
+    "txt17_21": {
         "align": "left",
         "class": "input_general",
-        "field": "21_Auxiliar_Licencia",
-        "fieldCodebin": "a21",
+        "codebinField": "moneda1",
+        "ecudocsField": "17_Gastos:ValorFlete,MonedaRemitente",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 20,
+        "height": 20,
+        "maxChars": 8,
         "maxLines": 1,
         "value": "",
-        "width": 252,
-        "x": 535,
-        "y": 615
+        "width": 80,
+        "x": 240,
+        "y": 997
     },
-    "txt22": {
+    "txt17_22": {
         "align": "left",
         "class": "input_general",
-        "field": "22_Auxiliar_Libreta",
-        "fieldCodebin": "a22",
-        "font": "normal",
-        "fontSize": "14px",
-        "height": 22,
-        "maxChars": 20,
-        "maxLines": 1,
-        "value": "",
-        "width": 257,
-        "x": 800,
-        "y": 615
-    },
-    "txt23": {
-        "align": "left",
-        "class": "input_lugar",
-        "field": "23_Carga_CiudadPais",
-        "fieldCodebin": "23",
-        "font": "normal",
-        "fontSize": "14px",
-        "height": 22,
-        "maxChars": 50,
-        "maxLines": 1,
-        "value": "",
-        "width": 470,
-        "x": 52,
-        "y": 676
-    },
-    "txt24": {
-        "align": "left",
-        "class": "input_lugar",
-        "field": "24_Descarga_CiudadPais",
-        "fieldCodebin": "24",
+        "codebinField": "moneda3",
+        "ecudocsField": "17_Gastos:Seguro,MonedaRemitente",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 55,
-        "maxLines": 1,
-        "value": "",
-        "width": 522,
-        "x": 535,
-        "y": 676
-    },
-    "txt25_1": {
-        "align": "left",
-        "class": "input_tipocarga",
-        "field": "25a_Carga_TipoPeligrosa",
-        "fieldCodebin": "radio-1-set",
-        "font": "normal",
-        "fontSize": "18px",
-        "height": 22,
-        "maxChars": 2,
-        "maxLines": 1,
-        "value": "",
-        "width": 18,
-        "x": 152,
-        "y": 724
-    },
-    "txt25_2": {
-        "align": "left",
-        "class": "input_tipocarga",
-        "field": "25b_Carga_TipoSustancias",
-        "fieldCodebin": "radio-3-set",
-        "font": "normal",
-        "fontSize": "18px",
-        "height": 22,
-        "maxChars": 2,
-        "maxLines": 1,
-        "value": "",
-        "width": 18,
-        "x": 432,
-        "y": 724
-    },
-    "txt25_3": {
-        "align": "left",
-        "class": "input_tipocarga",
-        "field": "25c_Carga_TipoPerecible",
-        "fieldCodebin": "radio-2-set",
-        "font": "normal",
-        "fontSize": "18px",
-        "height": 22,
-        "maxChars": 2,
-        "maxLines": 1,
-        "value": "",
-        "width": 18,
-        "x": 575,
-        "y": 724
-    },
-    "txt25_4": {
-        "align": "left",
-        "class": "input_tipocarga",
-        "field": "25d_Carga_TipoOtra",
-        "fieldCodebin": "radio-4-set",
-        "font": "normal",
-        "fontSize": "18px",
-        "height": 22,
-        "maxChars": 2,
+        "height": 20,
+        "maxChars": 8,
         "maxLines": 1,
         "value": "",
-        "width": 18,
-        "x": 700,
-        "y": 724
+        "width": 80,
+        "x": 240,
+        "y": 1018
     },
-    "txt25_5": {
+    "txt17_23": {
         "align": "left",
         "class": "input_general",
-        "field": "25e_Carga_TipoDescripcion",
-        "fieldCodebin": "25d",
+        "codebinField": "moneda5",
+        "ecudocsField": "17_Gastos:OtrosGastos,MonedaRemitente",
         "font": "normal",
         "fontSize": "14px",
-        "height": 48,
-        "maxChars": 20,
-        "maxLines": 2,
+        "height": 20,
+        "maxChars": 8,
+        "maxLines": 1,
         "value": "",
-        "width": 258,
-        "x": 799,
-        "y": 710
+        "width": 80,
+        "x": 240,
+        "y": 1039
     },
-    "txt26": {
+    "txt17_24": {
         "align": "left",
         "class": "input_general",
-        "field": "26_Carga_Contenedores",
-        "fieldCodebin": "26",
+        "codebinField": "monedat",
+        "ecudocsField": "17_Gastos:Total,MonedaRemitente",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 50,
+        "height": 20,
+        "maxChars": 8,
         "maxLines": 1,
         "value": "",
-        "width": 470,
-        "x": 52,
-        "y": 798
+        "width": 80,
+        "x": 240,
+        "y": 1061
     },
-    "txt27": {
-        "align": "left",
-        "class": "input_general",
-        "field": "27_Carga_Precintos",
-        "fieldCodebin": "27",
+    "txt17_31": {
+        "align": "right",
+        "class": "input_valor",
+        "codebinField": "montod",
+        "ecudocsField": "17_Gastos:ValorFlete,MontoDestinatario",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 55,
+        "height": 20,
+        "maxChars": 10,
         "maxLines": 1,
         "value": "",
-        "width": 522,
-        "x": 535,
-        "y": 798
-    },
-    "txt28": {
-        "align": "left",
-        "class": "input_cartaporte",
-        "field": "28_Mercancia_Cartaporte",
-        "fieldCodebin": "a28",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 341,
-        "maxChars": 13,
-        "maxLines": 20,
-        "value": "",
-        "width": 95,
-        "x": 52,
-        "y": 857
+        "width": 100,
+        "x": 334,
+        "y": 997
     },
-    "txt29": {
-        "align": "left",
-        "class": "input_general",
-        "field": "29_Mercancia_Descripcion",
-        "fieldCodebin": "a29",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 341,
-        "maxChars": 52,
-        "maxLines": 20,
-        "value": "",
-        "width": 380,
-        "x": 155,
-        "y": 857
-    },
-    "txt30": {
-        "align": "left",
-        "class": "input_general",
-        "field": "30_Mercancia_Bultos",
-        "fieldCodebin": "a30",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 341,
-        "maxChars": 14,
-        "maxLines": 20,
-        "value": "",
-        "width": 105,
-        "x": 540,
-        "y": 857
-    },
-    "txt31": {
-        "align": "left",
-        "class": "input_general",
-        "field": "31_Mercancia_Embalaje",
-        "fieldCodebin": "a31",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 341,
-        "maxChars": 17,
-        "maxLines": 20,
-        "value": "",
-        "width": 130,
-        "x": 651,
-        "y": 857
-    },
-    "txt32_1": {
+    "txt17_32": {
         "align": "right",
         "class": "input_valor",
-        "field": "32a_Peso_Bruto",
-        "fieldCodebin": "a32a",
+        "codebinField": "montod1",
+        "ecudocsField": "17_Gastos:Seguro,MontoDestinatario",
         "font": "normal",
         "fontSize": "14px",
-        "height": 341,
-        "maxChars": 9,
-        "maxLines": 20,
+        "height": 20,
+        "maxChars": 10,
+        "maxLines": 1,
         "value": "",
-        "width": 82,
-        "x": 795,
-        "y": 857
+        "width": 100,
+        "x": 334,
+        "y": 1018
     },
-    "txt32_2": {
+    "txt17_33": {
         "align": "right",
         "class": "input_valor",
-        "field": "32a_Peso_BrutoTotal",
-        "fieldCodebin": "a34b",
+        "codebinField": "montod2",
+        "ecudocsField": "17_Gastos:OtrosGastos,MontoDestinatario",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 9,
+        "height": 20,
+        "maxChars": 10,
         "maxLines": 1,
         "value": "",
-        "width": 82,
-        "x": 795,
-        "y": 1223
+        "width": 100,
+        "x": 334,
+        "y": 1039
     },
-    "txt32_3": {
+    "txt17_34": {
         "align": "right",
         "class": "input_valor",
-        "field": "32b_Peso_Neto",
-        "fieldCodebin": "a32b",
+        "codebinField": "totalmd",
+        "ecudocsField": "17_Gastos:Total,MontoDestinatario",
         "font": "normal",
         "fontSize": "14px",
-        "height": 341,
-        "maxChars": 9,
-        "maxLines": 20,
+        "height": 20,
+        "maxChars": 10,
+        "maxLines": 1,
         "value": "",
-        "width": 82,
-        "x": 887,
-        "y": 857
+        "width": 100,
+        "x": 334,
+        "y": 1061
     },
-    "txt32_4": {
-        "align": "right",
-        "class": "input_valor",
-        "field": "32b_Peso_NetoTotal",
-        "fieldCodebin": "a34c",
+    "txt17_41": {
+        "align": "left",
+        "class": "input_general",
+        "codebinField": "moneda2",
+        "ecudocsField": "17_Gastos:ValorFlete,MonedaDestinatario",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 9,
+        "height": 20,
+        "maxChars": 8,
         "maxLines": 1,
         "value": "",
-        "width": 82,
-        "x": 887,
-        "y": 1223
+        "width": 94,
+        "x": 447,
+        "y": 997
     },
-    "txt33_1": {
+    "txt17_42": {
         "align": "left",
-        "class": "input_valor",
-        "field": "33_Otra_Medida",
-        "fieldCodebin": "a33",
+        "class": "input_general",
+        "codebinField": "moneda4",
+        "ecudocsField": "17_Gastos:Seguro,MonedaDestinatario",
         "font": "normal",
         "fontSize": "14px",
-        "height": 341,
-        "maxChars": 9,
-        "maxLines": 20,
+        "height": 20,
+        "maxChars": 8,
+        "maxLines": 1,
         "value": "",
-        "width": 82,
-        "x": 979,
-        "y": 857
+        "width": 94,
+        "x": 447,
+        "y": 1018
     },
-    "txt33_2": {
+    "txt17_43": {
         "align": "left",
-        "class": "input_valor",
-        "field": "33_Otra_MedidaTotal",
-        "fieldCodebin": "a34d",
+        "class": "input_general",
+        "codebinField": "moneda6",
+        "ecudocsField": "17_Gastos:OtrosGastos,MonedaDestinatario",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 9,
+        "height": 20,
+        "maxChars": 8,
         "maxLines": 1,
         "value": "",
-        "width": 82,
-        "x": 979,
-        "y": 1223
+        "width": 94,
+        "x": 447,
+        "y": 1039
     },
-    "txt34": {
+    "txt17_44": {
         "align": "left",
-        "class": "input_incoterm",
-        "field": "34_Precio_Incoterm_Moneda",
-        "fieldCodebin": "a34a",
+        "class": "input_general",
+        "codebinField": "monedat2",
+        "ecudocsField": "17_Gastos:Total,MonedaDestinatario",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 70,
+        "height": 20,
+        "maxChars": 8,
         "maxLines": 1,
         "value": "",
-        "width": 653,
-        "x": 52,
-        "y": 1223
+        "width": 94,
+        "x": 447,
+        "y": 1061
     },
-    "txt35": {
+    "txt18": {
         "align": "left",
-        "class": "input_general",
-        "field": "35_Observaciones",
-        "fieldCodebin": "35",
+        "class": "input_documento",
+        "codebinField": "documentosr",
+        "ecudocsField": "18_Documentos",
         "font": "normal",
         "fontSize": "14px",
         "height": 36,
         "maxChars": 50,
         "maxLines": 2,
         "value": "",
-        "width": 470,
-        "x": 52,
-        "y": 1262
+        "width": 503,
+        "x": 40,
+        "y": 1103
     },
-    "txt37": {
+    "txt19": {
         "align": "left",
-        "class": "input_general",
-        "field": "37_Aduana_Cruce",
-        "fieldCodebin": "37",
+        "class": "input-lugar-fecha",
+        "codebinField": "lugaremision",
+        "ecudocsField": "19_Emision",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 27,
-        "maxLines": 1,
+        "height": 40,
+        "maxChars": 50,
+        "maxLines": 2,
         "value": "",
-        "width": 253,
-        "x": 535,
-        "y": 1262
+        "width": 503,
+        "x": 40,
+        "y": 1171
     },
-    "txt38": {
+    "txt21": {
         "align": "left",
         "class": "input_general",
-        "field": "38_Aduana_Destino",
-        "fieldCodebin": "38",
+        "codebinField": "instrucciones",
+        "ecudocsField": "21_Instrucciones",
         "font": "normal",
         "fontSize": "14px",
-        "height": 22,
-        "maxChars": 27,
-        "maxLines": 1,
+        "height": 85,
+        "maxChars": 50,
+        "maxLines": 5,
         "value": "",
-        "width": 257,
-        "x": 800,
-        "y": 1262
+        "width": 503,
+        "x": 560,
+        "y": 963
     },
-    "txt40": {
+    "txt22": {
         "align": "left",
-        "class": "input_fecha",
-        "field": "40_Fecha_Emision",
-        "fieldCodebin": "a40",
-        "font": "small",
-        "fontSize": "12px",
-        "height": 22,
-        "maxChars": 50,
-        "maxLines": 1,
+        "class": "input_general",
+        "codebinField": "observaciones",
+        "ecudocsField": "22_Observaciones",
+        "font": "normal",
+        "fontSize": "14px",
+        "height": 85,
+        "maxChars": 53,
+        "maxLines": 5,
         "value": "",
-        "width": 350,
-        "x": 180,
-        "y": 1366
+        "width": 503,
+        "x": 560,
+        "y": 1070
     },
-    "txt41": {
+    "txt24": {
         "align": "center",
         "class": "input_tipo",
-        "field": "41_OriginalCopia",
-        "fieldCodebin": "",
+        "codebinField": "",
+        "ecudocsField": "24_OriginalCopia",
         "font": "large",
-        "fontSize": "18px",
+        "fontSize": "26px",
         "height": 30,
-        "nChars": 10,
-        "nlines": 1,
-        "restrictions": [
-            "readonly"
-        ],
+        "maxChars": 10,
+        "maxLines": 1,
         "value": "",
         "width": 173,
         "x": 477,
-        "y": 1394
+        "y": 1357
     }
 }
```

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.75/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/icon-colombia.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-colombia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/icon-ecuador.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-ecuador.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/icon-white-bot.ico` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/icon-white-bot.ico`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/image-cartaporte-vacia.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-cartaporte-vacia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/image-declaracion-ecuapass.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-declaracion-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png` & `ecuapassdocs-0.75/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/ecuapassdocs.egg-info/SOURCES.txt` & `ecuapassdocs-0.75/ecuapassdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.74/setup.py` & `ecuapassdocs-0.75/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ecuapassdocs',  # Package name
-    version='0.74',  # Package version
+    version='0.75',  # Package version
     url="https://github.com/lgarreta/ecuapassdocs",
     author='Luis Garreta',
     author_email='lgarreta@gmail.com',
     description='Utils for creating PDFs, loading resources and extracting info from fields in ECUAPASS docs: cartaportes, manifiestos, declaraciones',
     packages=find_packages(),  # Automatically finds packages within the directory
 	include_package_data=True, 
 	package_data={"ecuapassdocs": ["resources/images/*", 
@@ -17,14 +17,15 @@
 	# List any dependencies here
     install_requires = [
 		"PyPDF2==3.0.1",
 		"reportlab==4.0.8",
 		"Pillow==10.1.0"
 	], 
 	logs = {
+		"0.75"   : "Simplified info classes (e.g. removed Gastos table)",
 		"0.74"   : "Changed tipoProc (Byza === NTA)",
 		"0.73"   : "Improved Byza's clean watermarks",
 		"0.72"   : "Improved infos: embalaje",
 		"0.71"   : "Improved assignation of vehicle type in Manifiestos",
 		"0.70"   : "Added creation of ECUAPASSDOCS fields. Added numero to parameters",
 		"0.63"   : "Added creation of CODEBIN fields",
 		"0.60"   : "Changed resource names from 'data-XXX' to data_XXX'"
```

