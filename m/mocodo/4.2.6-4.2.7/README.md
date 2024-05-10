# Comparing `tmp/mocodo-4.2.6.tar.gz` & `tmp/mocodo-4.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocodo-4.2.6.tar", max compression
+gzip compressed data, was "mocodo-4.2.7.tar", max compression
```

## Comparing `mocodo-4.2.6.tar` & `mocodo-4.2.7.tar`

### file list

```diff
@@ -1,215 +1,214 @@
--rw-r--r--   0        0        0     1073 2023-10-07 18:37:24.000000 mocodo-4.2.6/LICENSE
--rw-r--r--   0        0        0    10205 2024-01-26 15:15:52.094627 mocodo-4.2.6/README.md
--rw-r--r--   0        0        0      458 2024-03-25 12:49:36.172040 mocodo-4.2.6/mocodo/__init__.py
--rwxr-xr-x   0        0        0    16911 2024-03-06 19:02:39.000000 mocodo-4.2.6/mocodo/__main__.py
--rw-r--r--   0        0        0     1444 2024-03-25 11:56:34.944358 mocodo-4.2.6/mocodo/api.py
--rwxr-xr-x   0        0        0    18447 2024-03-06 18:35:31.000000 mocodo-4.2.6/mocodo/argument_parser.py
--rwxr-xr-x   0        0        0    19899 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/association.py
--rwxr-xr-x   0        0        0     5806 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/attribute.py
--rwxr-xr-x   0        0        0     4519 2024-01-28 18:14:34.000000 mocodo-4.2.6/mocodo/common.py
--rwxr-xr-x   0        0        0     5569 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/constraint.py
--rw-r--r--   0        0        0        0 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/convert/__init__.py
--rwxr-xr-x   0        0        0      674 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/convert/_ast.py
--rw-r--r--   0        0        0    14926 2024-03-06 18:05:26.000000 mocodo-4.2.6/mocodo/convert/_chen.py
--rw-r--r--   0        0        0     3482 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/convert/_crow.py
--rwxr-xr-x   0        0        0     4637 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/convert/_data_dict.py
--rwxr-xr-x   0        0        0      303 2023-10-11 10:17:43.000000 mocodo-4.2.6/mocodo/convert/_share.py
--rw-r--r--   0        0        0    10453 2024-03-06 18:05:26.000000 mocodo-4.2.6/mocodo/convert/_uml.py
--rw-r--r--   0        0        0     4247 2024-03-06 18:05:26.000000 mocodo-4.2.6/mocodo/convert/crow_gv.py
--rw-r--r--   0        0        0     2379 2024-03-06 18:05:26.000000 mocodo-4.2.6/mocodo/convert/crow_mmd.py
--rwxr-xr-x   0        0        0     4484 2023-12-07 16:48:27.000000 mocodo-4.2.6/mocodo/convert/read_template.py
--rwxr-xr-x   0        0        0    40403 2024-03-06 18:05:26.000000 mocodo-4.2.6/mocodo/convert/relations.py
--rw-r--r--   0        0        0     1586 2023-11-13 16:41:11.000000 mocodo-4.2.6/mocodo/dev/json_to_yaml_templates.py
--rw-r--r--   0        0        0     1392 2023-11-13 15:51:33.000000 mocodo-4.2.6/mocodo/dev/update_sql_reserved_words.py
--rw-r--r--   0        0        0     3605 2023-11-13 15:51:33.000000 mocodo-4.2.6/mocodo/dev/update_transfo_metadata.py
--rwxr-xr-x   0        0        0     4471 2023-10-22 15:13:09.000000 mocodo-4.2.6/mocodo/diagram_link.py
--rwxr-xr-x   0        0        0     9588 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/entity.py
--rwxr-xr-x   0        0        0     1119 2023-11-13 15:46:33.000000 mocodo-4.2.6/mocodo/font_metrics.py
--rwxr-xr-x   0        0        0     1957 2023-08-04 17:12:46.000000 mocodo-4.2.6/mocodo/grid.py
--rw-r--r--   0        0        0     1524 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/guess_title.py
--rw-r--r--   0        0        0     4754 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/inheritance.py
--rwxr-xr-x   0        0        0    24937 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/leg.py
--rw-r--r--   0        0        0     8003 2024-01-28 20:20:42.000000 mocodo-4.2.6/mocodo/magic.py
--rwxr-xr-x   0        0        0    31556 2024-01-26 12:23:37.901197 mocodo-4.2.6/mocodo/mcd.py
--rw-r--r--   0        0        0    11578 2024-03-06 18:05:26.000000 mocodo-4.2.6/mocodo/mcd_to_svg.py
--rwxr-xr-x   0        0        0     1109 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/mocodo_error.py
--rw-r--r--   0        0        0   257508 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/parse_mcd.py
--rwxr-xr-x   0        0        0      626 2023-10-22 15:13:09.000000 mocodo-4.2.6/mocodo/phantom.py
--rw-r--r--   0        0        0      756 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/blank.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer+1.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer+2.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer+3.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer+4.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer+5.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer+6.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer+7.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer+8.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer+9.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer-1.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer-2.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer-3.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer-4.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer-5.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer-6.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer-7.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer-8.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/brewer-9.json
--rw-r--r--   0        0        0      778 2023-10-24 12:15:51.190159 mocodo-4.2.6/mocodo/resources/colors/bw-alpha.json
--rw-r--r--   0        0        0      783 2023-10-24 12:15:32.719623 mocodo-4.2.6/mocodo/resources/colors/bw.json
--rw-r--r--   0        0        0      778 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/desert.json
--rw-r--r--   0        0        0      778 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/gray.json
--rw-r--r--   0        0        0      778 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/keepsake.json
--rw-r--r--   0        0        0      784 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/mondrian.json
--rw-r--r--   0        0        0      778 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/ocean.json
--rw-r--r--   0        0        0      778 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/pond.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/wb.json
--rw-r--r--   0        0        0      783 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/colors/xinnian.json
--rw-r--r--   0        0        0     2302 2023-11-11 08:55:08.000000 mocodo-4.2.6/mocodo/resources/default_datatypes_en.tsv
--rw-r--r--   0        0        0     2450 2023-11-11 09:00:46.000000 mocodo-4.2.6/mocodo/resources/default_datatypes_fr.tsv
--rw-r--r--   0        0        0    99839 2022-09-05 13:09:15.000000 mocodo-4.2.6/mocodo/resources/font_metrics.json
--rw-r--r--   0        0        0     2950 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/resources/grammar.lark
--rw-r--r--   0        0        0     4777 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/i18n/messages_de.mo
--rw-r--r--   0        0        0    28947 2023-11-20 18:02:12.000000 mocodo-4.2.6/mocodo/resources/i18n/messages_fr.mo
--rw-r--r--   0        0        0    35462 2023-11-20 18:01:44.000000 mocodo-4.2.6/mocodo/resources/i18n/messages_fr.po
--rw-r--r--   0        0        0     4048 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/i18n/messages_zh.mo
--rw-r--r--   0        0        0    62772 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/lorem/disparition.txt
--rw-r--r--   0        0        0     3200 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/lorem/en4.txt
--rw-r--r--   0        0        0    29421 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/lorem/fr.txt
--rw-r--r--   0        0        0     3248 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/lorem/fr5.txt
--rw-r--r--   0        0        0    53234 2023-10-23 18:09:08.000000 mocodo-4.2.6/mocodo/resources/lorem/lorem.txt
--rw-r--r--   0        0        0      615 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/pristine_sandbox.mcd
--rw-r--r--   0        0        0     6225 2024-03-25 12:49:41.747697 mocodo-4.2.6/mocodo/resources/relation_templates/_index.json
--rw-r--r--   0        0        0     3076 2023-10-28 08:53:14.772668 mocodo-4.2.6/mocodo/resources/relation_templates/d2.yaml
--rw-r--r--   0        0        0      129 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/dbml-b.yaml
--rw-r--r--   0        0        0     4535 2023-10-28 08:53:14.646859 mocodo-4.2.6/mocodo/resources/relation_templates/dbml.yaml
--rw-r--r--   0        0        0       14 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/ddl.yaml
--rw-r--r--   0        0        0     1422 2023-10-28 08:03:31.090668 mocodo-4.2.6/mocodo/resources/relation_templates/debug.yaml
--rw-r--r--   0        0        0     1254 2023-10-28 08:03:31.090954 mocodo-4.2.6/mocodo/resources/relation_templates/dependencies.yaml
--rw-r--r--   0        0        0     1011 2023-10-22 11:45:20.000000 mocodo-4.2.6/mocodo/resources/relation_templates/diagram-c.yaml
--rw-r--r--   0        0        0      471 2023-10-28 08:53:14.463589 mocodo-4.2.6/mocodo/resources/relation_templates/diagram.yaml
--rw-r--r--   0        0        0       72 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/html-b.yaml
--rw-r--r--   0        0        0      973 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/html-bc.yaml
--rw-r--r--   0        0        0      974 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/html-bce.yaml
--rw-r--r--   0        0        0       73 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/html-be.yaml
--rw-r--r--   0        0        0     3754 2023-11-20 15:48:29.000000 mocodo-4.2.6/mocodo/resources/relation_templates/html-c.yaml
--rw-r--r--   0        0        0    18345 2023-11-20 16:49:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/html-ce.yaml
--rw-r--r--   0        0        0       72 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/html-e.yaml
--rw-r--r--   0        0        0      730 2023-10-28 08:53:14.463855 mocodo-4.2.6/mocodo/resources/relation_templates/html.yaml
--rw-r--r--   0        0        0       73 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/latex-b.yaml
--rw-r--r--   0        0        0      627 2023-12-07 15:30:53.000000 mocodo-4.2.6/mocodo/resources/relation_templates/latex-bc.yaml
--rw-r--r--   0        0        0      628 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/latex-bce.yaml
--rw-r--r--   0        0        0       74 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/latex-be.yaml
--rw-r--r--   0        0        0     1140 2023-12-14 15:22:45.000000 mocodo-4.2.6/mocodo/resources/relation_templates/latex-c.yaml
--rw-r--r--   0        0        0     1761 2023-12-14 15:22:55.000000 mocodo-4.2.6/mocodo/resources/relation_templates/latex-ce.yaml
--rw-r--r--   0        0        0       73 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/latex-e.yaml
--rw-r--r--   0        0        0      739 2023-10-28 08:53:14.464010 mocodo-4.2.6/mocodo/resources/relation_templates/latex.yaml
--rw-r--r--   0        0        0       76 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/markdown-b.yaml
--rw-r--r--   0        0        0       21 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/markdown-bc.yaml
--rw-r--r--   0        0        0       22 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/markdown-bce.yaml
--rw-r--r--   0        0        0       77 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/markdown-be.yaml
--rw-r--r--   0        0        0      776 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/markdown-c.yaml
--rw-r--r--   0        0        0     1244 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/markdown-ce.yaml
--rw-r--r--   0        0        0       76 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/markdown-e.yaml
--rw-r--r--   0        0        0      673 2023-10-28 08:53:14.464177 mocodo-4.2.6/mocodo/resources/relation_templates/markdown.yaml
--rw-r--r--   0        0        0       21 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/md-b.yaml
--rw-r--r--   0        0        0       22 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/md-bc.yaml
--rw-r--r--   0        0        0       23 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/md-bce.yaml
--rw-r--r--   0        0        0       22 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/md-be.yaml
--rw-r--r--   0        0        0       21 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/md-c.yaml
--rw-r--r--   0        0        0       22 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/md-ce.yaml
--rw-r--r--   0        0        0       21 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/md-e.yaml
--rw-r--r--   0        0        0       19 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/md.yaml
--rw-r--r--   0        0        0       21 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mld-b.yaml
--rw-r--r--   0        0        0       22 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mld-bc.yaml
--rw-r--r--   0        0        0       23 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mld-bce.yaml
--rw-r--r--   0        0        0       22 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mld-be.yaml
--rw-r--r--   0        0        0       21 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mld-c.yaml
--rw-r--r--   0        0        0       22 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mld-ce.yaml
--rw-r--r--   0        0        0       21 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mld-e.yaml
--rw-r--r--   0        0        0       19 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mld.yaml
--rw-r--r--   0        0        0       18 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/ms_sql-b.yaml
--rw-r--r--   0        0        0       16 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/ms_sql.yaml
--rw-r--r--   0        0        0     1375 2023-10-21 11:08:53.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mssql-b.yaml
--rw-r--r--   0        0        0     7159 2023-12-28 15:47:39.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mssql.yaml
--rw-r--r--   0        0        0      526 2023-10-21 11:08:05.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mysql-b.yaml
--rw-r--r--   0        0        0     5631 2023-12-07 17:17:06.000000 mocodo-4.2.6/mocodo/resources/relation_templates/mysql.yaml
--rw-r--r--   0        0        0     1155 2023-10-21 11:08:53.000000 mocodo-4.2.6/mocodo/resources/relation_templates/oracle-b.yaml
--rw-r--r--   0        0        0     8714 2023-12-07 17:21:13.000000 mocodo-4.2.6/mocodo/resources/relation_templates/oracle.yaml
--rw-r--r--   0        0        0       19 2023-10-12 18:27:14.000000 mocodo-4.2.6/mocodo/resources/relation_templates/oracle_db-b.yaml
--rw-r--r--   0        0        0       17 2023-10-11 18:35:26.000000 mocodo-4.2.6/mocodo/resources/relation_templates/oracle_db.yaml
--rw-r--r--   0        0        0       23 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/postgres-b.yaml
--rw-r--r--   0        0        0       21 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/postgres.yaml
--rw-r--r--   0        0        0      610 2023-10-21 11:08:53.000000 mocodo-4.2.6/mocodo/resources/relation_templates/postgresql-b.yaml
--rw-r--r--   0        0        0     8360 2023-12-07 17:21:13.000000 mocodo-4.2.6/mocodo/resources/relation_templates/postgresql.yaml
--rw-r--r--   0        0        0     4378 2023-12-07 16:31:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/sql.yaml
--rw-r--r--   0        0        0       18 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/sql_server-b.yaml
--rw-r--r--   0        0        0       16 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/sql_server.yaml
--rw-r--r--   0        0        0      168 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/sqlite-b.yaml
--rw-r--r--   0        0        0     9296 2023-12-07 17:21:13.000000 mocodo-4.2.6/mocodo/resources/relation_templates/sqlite.yaml
--rw-r--r--   0        0        0       18 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/sqlserver-b.yaml
--rw-r--r--   0        0        0       16 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/sqlserver.yaml
--rw-r--r--   0        0        0       18 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/tex-b.yaml
--rw-r--r--   0        0        0       19 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/tex-bc.yaml
--rw-r--r--   0        0        0       20 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/tex-bce.yaml
--rw-r--r--   0        0        0       19 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/tex-be.yaml
--rw-r--r--   0        0        0       18 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/tex-c.yaml
--rw-r--r--   0        0        0       19 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/tex-ce.yaml
--rw-r--r--   0        0        0       18 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/tex-e.yaml
--rw-r--r--   0        0        0       16 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/tex.yaml
--rw-r--r--   0        0        0       71 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/text-b.yaml
--rw-r--r--   0        0        0       17 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/text-bc.yaml
--rw-r--r--   0        0        0       18 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/text-bce.yaml
--rw-r--r--   0        0        0       73 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/text-be.yaml
--rw-r--r--   0        0        0     1717 2023-11-05 16:01:33.140786 mocodo-4.2.6/mocodo/resources/relation_templates/text-c.yaml
--rw-r--r--   0        0        0     2198 2023-11-05 17:40:07.053195 mocodo-4.2.6/mocodo/resources/relation_templates/text-ce.yaml
--rw-r--r--   0        0        0       72 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/text-e.yaml
--rw-r--r--   0        0        0      642 2023-10-28 08:53:14.464345 mocodo-4.2.6/mocodo/resources/relation_templates/text.yaml
--rw-r--r--   0        0        0       17 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/txt-b.yaml
--rw-r--r--   0        0        0       18 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/txt-bc.yaml
--rw-r--r--   0        0        0       19 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/txt-bce.yaml
--rw-r--r--   0        0        0       18 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/txt-be.yaml
--rw-r--r--   0        0        0       17 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/txt-c.yaml
--rw-r--r--   0        0        0       18 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/txt-ce.yaml
--rw-r--r--   0        0        0       17 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/txt-e.yaml
--rw-r--r--   0        0        0       15 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/resources/relation_templates/txt.yaml
--rw-r--r--   0        0        0      668 2023-10-28 08:53:14.772945 mocodo-4.2.6/mocodo/resources/rendering_services.json
--rw-r--r--   0        0        0     1451 2023-06-06 10:56:21.000000 mocodo-4.2.6/mocodo/resources/shapes/arial.json
--rw-r--r--   0        0        0     1450 2023-06-06 10:56:21.000000 mocodo-4.2.6/mocodo/resources/shapes/copperplate.json
--rw-r--r--   0        0        0     1441 2023-06-06 10:56:21.000000 mocodo-4.2.6/mocodo/resources/shapes/georgia.json
--rw-r--r--   0        0        0     1599 2023-06-06 10:56:21.000000 mocodo-4.2.6/mocodo/resources/shapes/mondrian.json
--rw-r--r--   0        0        0     1506 2023-06-06 10:56:21.000000 mocodo-4.2.6/mocodo/resources/shapes/sans.json
--rw-r--r--   0        0        0     1514 2023-06-06 10:56:21.000000 mocodo-4.2.6/mocodo/resources/shapes/serif.json
--rw-r--r--   0        0        0     1481 2023-06-06 10:56:21.000000 mocodo-4.2.6/mocodo/resources/shapes/times.json
--rw-r--r--   0        0        0     1466 2023-06-06 10:56:21.000000 mocodo-4.2.6/mocodo/resources/shapes/trebuchet.json
--rw-r--r--   0        0        0     1591 2023-06-06 10:56:21.000000 mocodo-4.2.6/mocodo/resources/shapes/verdana.json
--rw-r--r--   0        0        0     1487 2023-06-06 10:56:21.000000 mocodo-4.2.6/mocodo/resources/shapes/xinnian.json
--rw-r--r--   0        0        0    13683 2023-11-11 10:30:33.000000 mocodo-4.2.6/mocodo/resources/transformations.json
--rw-r--r--   0        0        0        0 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/rewrite/__init__.py
--rwxr-xr-x   0        0        0      676 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/rewrite/_arrange.py
--rwxr-xr-x   0        0        0     2545 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/rewrite/_drain.py
--rw-r--r--   0        0        0     2088 2023-11-27 18:17:48.908069 mocodo-4.2.6/mocodo/rewrite/_drown.py
--rwxr-xr-x   0        0        0     4421 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/rewrite/_explode.py
--rwxr-xr-x   0        0        0     8456 2023-12-07 18:14:54.000000 mocodo-4.2.6/mocodo/rewrite/_grow.py
--rwxr-xr-x   0        0        0     3509 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/rewrite/_split.py
--rwxr-xr-x   0        0        0    10934 2023-11-20 13:17:10.000000 mocodo-4.2.6/mocodo/rewrite/arrange_bb.py
--rwxr-xr-x   0        0        0     6521 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/rewrite/arrange_ga.py
--rw-r--r--   0        0        0     1057 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/rewrite/arrows.py
--rwxr-xr-x   0        0        0     2227 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/rewrite/cards.py
--rw-r--r--   0        0        0     3095 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/rewrite/constraints.py
--rwxr-xr-x   0        0        0     1437 2023-11-20 13:17:10.000000 mocodo-4.2.6/mocodo/rewrite/cross.py
--rw-r--r--   0        0        0     1980 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/rewrite/damerau_levenshtein.py
--rwxr-xr-x   0        0        0     1280 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/rewrite/fitness.py
--rw-r--r--   0        0        0     1031 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/rewrite/guess_entities.py
--rwxr-xr-x   0        0        0     2214 2023-11-13 15:47:43.000000 mocodo-4.2.6/mocodo/rewrite/obfuscate.py
--rwxr-xr-x   0        0        0     5307 2023-10-14 07:19:39.000000 mocodo-4.2.6/mocodo/rewrite/op_tk.py
--rw-r--r--   0        0        0     2723 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/rewrite/types.py
--rw-r--r--   0        0        0        0 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/tools/__init__.py
--rw-r--r--   0        0        0     4567 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/tools/graphviz_tools.py
--rw-r--r--   0        0        0     1671 2023-11-13 15:47:43.000000 mocodo-4.2.6/mocodo/tools/load_mini_yaml.py
--rwxr-xr-x   0        0        0    13711 2023-12-01 15:42:09.000000 mocodo-4.2.6/mocodo/tools/parser_tools.py
--rwxr-xr-x   0        0        0     1639 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/tools/pluralize_fr.py
--rw-r--r--   0        0        0     4513 2023-10-22 17:03:59.000000 mocodo-4.2.6/mocodo/tools/string_tools.py
--rw-r--r--   0        0        0      163 2023-10-07 18:37:24.000000 mocodo-4.2.6/mocodo/tools/various.py
--rw-r--r--   0        0        0     1433 2024-03-06 18:07:02.000000 mocodo-4.2.6/pyproject.toml
--rw-r--r--   0        0        0   512771 1970-01-01 00:00:00.000000 mocodo-4.2.6/setup.py
--rw-r--r--   0        0        0    11522 1970-01-01 00:00:00.000000 mocodo-4.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-10-07 18:37:24.338257 mocodo-4.2.7/LICENSE
+-rw-r--r--   0        0        0    10205 2024-01-26 15:15:52.000000 mocodo-4.2.7/README.md
+-rw-r--r--   0        0        0      458 2024-05-09 09:26:06.682969 mocodo-4.2.7/mocodo/__init__.py
+-rwxr-xr-x   0        0        0    16911 2024-03-06 19:03:19.213387 mocodo-4.2.7/mocodo/__main__.py
+-rw-r--r--   0        0        0     1444 2024-03-25 11:56:34.000000 mocodo-4.2.7/mocodo/api.py
+-rwxr-xr-x   0        0        0    18447 2024-03-06 18:35:34.412488 mocodo-4.2.7/mocodo/argument_parser.py
+-rwxr-xr-x   0        0        0    19899 2023-12-01 15:42:09.477293 mocodo-4.2.7/mocodo/association.py
+-rwxr-xr-x   0        0        0     5806 2023-12-01 15:42:09.479385 mocodo-4.2.7/mocodo/attribute.py
+-rwxr-xr-x   0        0        0     4519 2024-01-28 18:14:34.517151 mocodo-4.2.7/mocodo/common.py
+-rwxr-xr-x   0        0        0     5569 2023-12-01 15:42:09.481296 mocodo-4.2.7/mocodo/constraint.py
+-rw-r--r--   0        0        0        0 2023-10-07 18:37:24.450430 mocodo-4.2.7/mocodo/convert/__init__.py
+-rwxr-xr-x   0        0        0      674 2023-10-07 18:37:24.450786 mocodo-4.2.7/mocodo/convert/_ast.py
+-rw-r--r--   0        0        0    14926 2024-03-06 18:05:26.054642 mocodo-4.2.7/mocodo/convert/_chen.py
+-rw-r--r--   0        0        0     3482 2023-12-01 15:42:09.484191 mocodo-4.2.7/mocodo/convert/_crow.py
+-rwxr-xr-x   0        0        0     4637 2023-12-01 15:42:09.484405 mocodo-4.2.7/mocodo/convert/_data_dict.py
+-rwxr-xr-x   0        0        0      303 2023-10-11 10:17:43.387018 mocodo-4.2.7/mocodo/convert/_share.py
+-rw-r--r--   0        0        0    10453 2024-03-06 18:05:26.054613 mocodo-4.2.7/mocodo/convert/_uml.py
+-rw-r--r--   0        0        0     4247 2024-03-06 18:05:26.054709 mocodo-4.2.7/mocodo/convert/crow_gv.py
+-rw-r--r--   0        0        0     2379 2024-03-06 18:05:26.055654 mocodo-4.2.7/mocodo/convert/crow_mmd.py
+-rwxr-xr-x   0        0        0     4484 2023-12-07 16:48:27.108132 mocodo-4.2.7/mocodo/convert/read_template.py
+-rwxr-xr-x   0        0        0    40403 2024-03-06 18:05:26.055848 mocodo-4.2.7/mocodo/convert/relations.py
+-rw-r--r--   0        0        0     1586 2023-11-13 16:41:11.707991 mocodo-4.2.7/mocodo/dev/json_to_yaml_templates.py
+-rw-r--r--   0        0        0     1392 2023-12-07 17:19:12.059246 mocodo-4.2.7/mocodo/dev/update_sql_reserved_words.py
+-rw-r--r--   0        0        0     3605 2023-11-13 15:51:33.576105 mocodo-4.2.7/mocodo/dev/update_transfo_metadata.py
+-rwxr-xr-x   0        0        0     4471 2023-10-22 15:13:09.831308 mocodo-4.2.7/mocodo/diagram_link.py
+-rwxr-xr-x   0        0        0     9588 2023-12-01 15:42:09.486235 mocodo-4.2.7/mocodo/entity.py
+-rwxr-xr-x   0        0        0     1119 2023-11-13 15:46:33.713628 mocodo-4.2.7/mocodo/font_metrics.py
+-rwxr-xr-x   0        0        0     1957 2023-08-04 17:12:46.621650 mocodo-4.2.7/mocodo/grid.py
+-rw-r--r--   0        0        0     1524 2023-12-01 15:42:09.486925 mocodo-4.2.7/mocodo/guess_title.py
+-rw-r--r--   0        0        0     4754 2023-12-01 15:42:09.488085 mocodo-4.2.7/mocodo/inheritance.py
+-rwxr-xr-x   0        0        0    24937 2023-12-01 15:42:09.488777 mocodo-4.2.7/mocodo/leg.py
+-rw-r--r--   0        0        0     8003 2024-01-28 20:20:42.380689 mocodo-4.2.7/mocodo/magic.py
+-rwxr-xr-x   0        0        0    31556 2024-01-26 12:23:37.000000 mocodo-4.2.7/mocodo/mcd.py
+-rw-r--r--   0        0        0    11578 2024-03-06 18:05:26.054571 mocodo-4.2.7/mocodo/mcd_to_svg.py
+-rwxr-xr-x   0        0        0     1109 2023-10-07 18:37:24.458690 mocodo-4.2.7/mocodo/mocodo_error.py
+-rw-r--r--   0        0        0   257508 2023-12-01 15:42:09.492208 mocodo-4.2.7/mocodo/parse_mcd.py
+-rwxr-xr-x   0        0        0      626 2023-10-22 15:13:09.833184 mocodo-4.2.7/mocodo/phantom.py
+-rw-r--r--   0        0        0      756 2023-10-07 18:37:24.462293 mocodo-4.2.7/mocodo/resources/colors/blank.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.462617 mocodo-4.2.7/mocodo/resources/colors/brewer+1.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.462816 mocodo-4.2.7/mocodo/resources/colors/brewer+2.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.463012 mocodo-4.2.7/mocodo/resources/colors/brewer+3.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.463201 mocodo-4.2.7/mocodo/resources/colors/brewer+4.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.463428 mocodo-4.2.7/mocodo/resources/colors/brewer+5.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.463636 mocodo-4.2.7/mocodo/resources/colors/brewer+6.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.463833 mocodo-4.2.7/mocodo/resources/colors/brewer+7.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.464019 mocodo-4.2.7/mocodo/resources/colors/brewer+8.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.464243 mocodo-4.2.7/mocodo/resources/colors/brewer+9.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.465195 mocodo-4.2.7/mocodo/resources/colors/brewer-1.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.465407 mocodo-4.2.7/mocodo/resources/colors/brewer-2.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.465614 mocodo-4.2.7/mocodo/resources/colors/brewer-3.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.465808 mocodo-4.2.7/mocodo/resources/colors/brewer-4.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.465991 mocodo-4.2.7/mocodo/resources/colors/brewer-5.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.466310 mocodo-4.2.7/mocodo/resources/colors/brewer-6.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.466592 mocodo-4.2.7/mocodo/resources/colors/brewer-7.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.466783 mocodo-4.2.7/mocodo/resources/colors/brewer-8.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.466968 mocodo-4.2.7/mocodo/resources/colors/brewer-9.json
+-rw-r--r--   0        0        0      778 2023-10-24 12:15:51.000000 mocodo-4.2.7/mocodo/resources/colors/bw-alpha.json
+-rw-r--r--   0        0        0      783 2023-10-24 12:15:32.000000 mocodo-4.2.7/mocodo/resources/colors/bw.json
+-rw-r--r--   0        0        0      778 2023-10-07 18:37:24.467589 mocodo-4.2.7/mocodo/resources/colors/desert.json
+-rw-r--r--   0        0        0      778 2023-10-07 18:37:24.467771 mocodo-4.2.7/mocodo/resources/colors/gray.json
+-rw-r--r--   0        0        0      778 2023-10-07 18:37:24.467954 mocodo-4.2.7/mocodo/resources/colors/keepsake.json
+-rw-r--r--   0        0        0      784 2023-10-07 18:37:24.468193 mocodo-4.2.7/mocodo/resources/colors/mondrian.json
+-rw-r--r--   0        0        0      778 2023-10-07 18:37:24.468386 mocodo-4.2.7/mocodo/resources/colors/ocean.json
+-rw-r--r--   0        0        0      778 2023-10-07 18:37:24.468589 mocodo-4.2.7/mocodo/resources/colors/pond.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.468795 mocodo-4.2.7/mocodo/resources/colors/wb.json
+-rw-r--r--   0        0        0      783 2023-10-07 18:37:24.468995 mocodo-4.2.7/mocodo/resources/colors/xinnian.json
+-rw-r--r--   0        0        0     2302 2023-11-11 08:55:08.244619 mocodo-4.2.7/mocodo/resources/default_datatypes_en.tsv
+-rw-r--r--   0        0        0     2450 2023-11-11 09:00:46.478196 mocodo-4.2.7/mocodo/resources/default_datatypes_fr.tsv
+-rw-r--r--   0        0        0    99839 2022-09-05 13:09:15.100146 mocodo-4.2.7/mocodo/resources/font_metrics.json
+-rw-r--r--   0        0        0     2950 2023-12-01 15:42:09.493511 mocodo-4.2.7/mocodo/resources/grammar.lark
+-rw-r--r--   0        0        0     4777 2023-10-07 18:37:24.470138 mocodo-4.2.7/mocodo/resources/i18n/messages_de.mo
+-rw-r--r--   0        0        0    28947 2023-11-20 18:02:12.159870 mocodo-4.2.7/mocodo/resources/i18n/messages_fr.mo
+-rw-r--r--   0        0        0    35462 2023-11-20 18:01:54.853573 mocodo-4.2.7/mocodo/resources/i18n/messages_fr.po
+-rw-r--r--   0        0        0     4048 2023-10-07 18:37:24.471174 mocodo-4.2.7/mocodo/resources/i18n/messages_zh.mo
+-rw-r--r--   0        0        0    62772 2023-10-07 18:37:24.472625 mocodo-4.2.7/mocodo/resources/lorem/disparition.txt
+-rw-r--r--   0        0        0     3200 2023-10-07 18:37:24.477686 mocodo-4.2.7/mocodo/resources/lorem/en4.txt
+-rw-r--r--   0        0        0    29421 2023-10-07 18:37:24.478181 mocodo-4.2.7/mocodo/resources/lorem/fr.txt
+-rw-r--r--   0        0        0     3248 2023-10-07 18:37:24.478438 mocodo-4.2.7/mocodo/resources/lorem/fr5.txt
+-rw-r--r--   0        0        0    53234 2023-10-23 18:09:08.846789 mocodo-4.2.7/mocodo/resources/lorem/lorem.txt
+-rw-r--r--   0        0        0      615 2023-10-07 18:37:24.478982 mocodo-4.2.7/mocodo/resources/pristine_sandbox.mcd
+-rw-r--r--   0        0        0     6225 2024-03-06 19:07:54.319934 mocodo-4.2.7/mocodo/resources/relation_templates/_index.json
+-rw-r--r--   0        0        0     3076 2023-10-28 08:35:20.000000 mocodo-4.2.7/mocodo/resources/relation_templates/d2.yaml
+-rw-r--r--   0        0        0      129 2023-10-07 18:37:24.479502 mocodo-4.2.7/mocodo/resources/relation_templates/dbml-b.yaml
+-rw-r--r--   0        0        0     4535 2023-10-28 08:29:16.000000 mocodo-4.2.7/mocodo/resources/relation_templates/dbml.yaml
+-rw-r--r--   0        0        0       14 2023-10-07 18:37:24.479977 mocodo-4.2.7/mocodo/resources/relation_templates/ddl.yaml
+-rw-r--r--   0        0        0     1422 2023-10-26 11:02:43.000000 mocodo-4.2.7/mocodo/resources/relation_templates/debug.yaml
+-rw-r--r--   0        0        0     1254 2023-10-26 11:02:51.000000 mocodo-4.2.7/mocodo/resources/relation_templates/dependencies.yaml
+-rw-r--r--   0        0        0     1011 2023-10-22 11:45:20.265541 mocodo-4.2.7/mocodo/resources/relation_templates/diagram-c.yaml
+-rw-r--r--   0        0        0      471 2023-10-26 11:27:39.000000 mocodo-4.2.7/mocodo/resources/relation_templates/diagram.yaml
+-rw-r--r--   0        0        0       72 2023-10-07 18:37:24.480957 mocodo-4.2.7/mocodo/resources/relation_templates/html-b.yaml
+-rw-r--r--   0        0        0      973 2023-10-07 18:37:24.481143 mocodo-4.2.7/mocodo/resources/relation_templates/html-bc.yaml
+-rw-r--r--   0        0        0      974 2023-10-07 18:37:24.481330 mocodo-4.2.7/mocodo/resources/relation_templates/html-bce.yaml
+-rw-r--r--   0        0        0       73 2023-10-07 18:37:24.481599 mocodo-4.2.7/mocodo/resources/relation_templates/html-be.yaml
+-rw-r--r--   0        0        0     3754 2023-11-20 15:48:29.594938 mocodo-4.2.7/mocodo/resources/relation_templates/html-c.yaml
+-rw-r--r--   0        0        0    18345 2023-11-20 16:49:24.896115 mocodo-4.2.7/mocodo/resources/relation_templates/html-ce.yaml
+-rw-r--r--   0        0        0       72 2023-10-07 18:37:24.482277 mocodo-4.2.7/mocodo/resources/relation_templates/html-e.yaml
+-rw-r--r--   0        0        0      730 2023-10-26 11:27:39.000000 mocodo-4.2.7/mocodo/resources/relation_templates/html.yaml
+-rw-r--r--   0        0        0       73 2023-10-07 18:37:24.482629 mocodo-4.2.7/mocodo/resources/relation_templates/latex-b.yaml
+-rw-r--r--   0        0        0      627 2023-12-07 15:30:53.799777 mocodo-4.2.7/mocodo/resources/relation_templates/latex-bc.yaml
+-rw-r--r--   0        0        0      628 2023-10-07 18:37:24.482998 mocodo-4.2.7/mocodo/resources/relation_templates/latex-bce.yaml
+-rw-r--r--   0        0        0       74 2023-10-07 18:37:24.483209 mocodo-4.2.7/mocodo/resources/relation_templates/latex-be.yaml
+-rw-r--r--   0        0        0     1140 2023-12-14 15:22:45.674847 mocodo-4.2.7/mocodo/resources/relation_templates/latex-c.yaml
+-rw-r--r--   0        0        0     1761 2023-12-14 15:22:55.334789 mocodo-4.2.7/mocodo/resources/relation_templates/latex-ce.yaml
+-rw-r--r--   0        0        0       73 2023-10-07 18:37:24.483799 mocodo-4.2.7/mocodo/resources/relation_templates/latex-e.yaml
+-rw-r--r--   0        0        0      739 2023-10-26 11:27:39.000000 mocodo-4.2.7/mocodo/resources/relation_templates/latex.yaml
+-rw-r--r--   0        0        0       76 2023-10-07 18:37:24.484162 mocodo-4.2.7/mocodo/resources/relation_templates/markdown-b.yaml
+-rw-r--r--   0        0        0       21 2023-10-07 18:37:24.484382 mocodo-4.2.7/mocodo/resources/relation_templates/markdown-bc.yaml
+-rw-r--r--   0        0        0       22 2023-10-07 18:37:24.484554 mocodo-4.2.7/mocodo/resources/relation_templates/markdown-bce.yaml
+-rw-r--r--   0        0        0       77 2023-10-07 18:37:24.484742 mocodo-4.2.7/mocodo/resources/relation_templates/markdown-be.yaml
+-rw-r--r--   0        0        0      776 2023-10-07 18:37:24.484983 mocodo-4.2.7/mocodo/resources/relation_templates/markdown-c.yaml
+-rw-r--r--   0        0        0     1244 2023-10-07 18:37:24.485223 mocodo-4.2.7/mocodo/resources/relation_templates/markdown-ce.yaml
+-rw-r--r--   0        0        0       76 2023-10-07 18:37:24.485437 mocodo-4.2.7/mocodo/resources/relation_templates/markdown-e.yaml
+-rw-r--r--   0        0        0      673 2023-10-26 11:27:39.000000 mocodo-4.2.7/mocodo/resources/relation_templates/markdown.yaml
+-rw-r--r--   0        0        0       21 2023-10-07 18:37:24.485816 mocodo-4.2.7/mocodo/resources/relation_templates/md-b.yaml
+-rw-r--r--   0        0        0       22 2023-10-07 18:37:24.486034 mocodo-4.2.7/mocodo/resources/relation_templates/md-bc.yaml
+-rw-r--r--   0        0        0       23 2023-10-07 18:37:24.486206 mocodo-4.2.7/mocodo/resources/relation_templates/md-bce.yaml
+-rw-r--r--   0        0        0       22 2023-10-07 18:37:24.486378 mocodo-4.2.7/mocodo/resources/relation_templates/md-be.yaml
+-rw-r--r--   0        0        0       21 2023-10-07 18:37:24.486559 mocodo-4.2.7/mocodo/resources/relation_templates/md-c.yaml
+-rw-r--r--   0        0        0       22 2023-10-07 18:37:24.486815 mocodo-4.2.7/mocodo/resources/relation_templates/md-ce.yaml
+-rw-r--r--   0        0        0       21 2023-10-07 18:37:24.487007 mocodo-4.2.7/mocodo/resources/relation_templates/md-e.yaml
+-rw-r--r--   0        0        0       19 2023-10-07 18:37:24.487190 mocodo-4.2.7/mocodo/resources/relation_templates/md.yaml
+-rw-r--r--   0        0        0       21 2023-10-07 18:37:24.487370 mocodo-4.2.7/mocodo/resources/relation_templates/mld-b.yaml
+-rw-r--r--   0        0        0       22 2023-10-07 18:37:24.487589 mocodo-4.2.7/mocodo/resources/relation_templates/mld-bc.yaml
+-rw-r--r--   0        0        0       23 2023-10-07 18:37:24.487756 mocodo-4.2.7/mocodo/resources/relation_templates/mld-bce.yaml
+-rw-r--r--   0        0        0       22 2023-10-07 18:37:24.487932 mocodo-4.2.7/mocodo/resources/relation_templates/mld-be.yaml
+-rw-r--r--   0        0        0       21 2023-10-07 18:37:24.488105 mocodo-4.2.7/mocodo/resources/relation_templates/mld-c.yaml
+-rw-r--r--   0        0        0       22 2023-10-07 18:37:24.488313 mocodo-4.2.7/mocodo/resources/relation_templates/mld-ce.yaml
+-rw-r--r--   0        0        0       21 2023-10-07 18:37:24.488511 mocodo-4.2.7/mocodo/resources/relation_templates/mld-e.yaml
+-rw-r--r--   0        0        0       19 2023-10-07 18:37:24.488677 mocodo-4.2.7/mocodo/resources/relation_templates/mld.yaml
+-rw-r--r--   0        0        0       18 2023-10-07 18:37:24.488842 mocodo-4.2.7/mocodo/resources/relation_templates/ms_sql-b.yaml
+-rw-r--r--   0        0        0       16 2023-10-07 18:37:24.489051 mocodo-4.2.7/mocodo/resources/relation_templates/ms_sql.yaml
+-rw-r--r--   0        0        0     1375 2023-10-21 11:08:56.824520 mocodo-4.2.7/mocodo/resources/relation_templates/mssql-b.yaml
+-rw-r--r--   0        0        0     7159 2023-12-28 15:47:39.283704 mocodo-4.2.7/mocodo/resources/relation_templates/mssql.yaml
+-rw-r--r--   0        0        0      526 2023-10-21 11:08:05.804660 mocodo-4.2.7/mocodo/resources/relation_templates/mysql-b.yaml
+-rw-r--r--   0        0        0     5631 2023-12-07 17:21:13.240290 mocodo-4.2.7/mocodo/resources/relation_templates/mysql.yaml
+-rw-r--r--   0        0        0     1155 2023-10-21 11:08:53.218094 mocodo-4.2.7/mocodo/resources/relation_templates/oracle-b.yaml
+-rw-r--r--   0        0        0     8714 2023-12-07 17:21:13.242683 mocodo-4.2.7/mocodo/resources/relation_templates/oracle.yaml
+-rw-r--r--   0        0        0       19 2023-10-12 18:27:14.624726 mocodo-4.2.7/mocodo/resources/relation_templates/oracle_db-b.yaml
+-rw-r--r--   0        0        0       17 2023-10-11 18:35:26.109814 mocodo-4.2.7/mocodo/resources/relation_templates/oracle_db.yaml
+-rw-r--r--   0        0        0       23 2023-10-07 18:37:24.490292 mocodo-4.2.7/mocodo/resources/relation_templates/postgres-b.yaml
+-rw-r--r--   0        0        0       21 2023-10-07 18:37:24.490492 mocodo-4.2.7/mocodo/resources/relation_templates/postgres.yaml
+-rw-r--r--   0        0        0      610 2023-10-21 11:08:53.218362 mocodo-4.2.7/mocodo/resources/relation_templates/postgresql-b.yaml
+-rw-r--r--   0        0        0     8360 2023-12-07 17:21:13.244524 mocodo-4.2.7/mocodo/resources/relation_templates/postgresql.yaml
+-rw-r--r--   0        0        0     4378 2023-12-07 16:31:24.699087 mocodo-4.2.7/mocodo/resources/relation_templates/sql.yaml
+-rw-r--r--   0        0        0       18 2023-10-07 18:37:24.491214 mocodo-4.2.7/mocodo/resources/relation_templates/sql_server-b.yaml
+-rw-r--r--   0        0        0       16 2023-10-07 18:37:24.491366 mocodo-4.2.7/mocodo/resources/relation_templates/sql_server.yaml
+-rw-r--r--   0        0        0      168 2023-10-07 18:37:24.491552 mocodo-4.2.7/mocodo/resources/relation_templates/sqlite-b.yaml
+-rw-r--r--   0        0        0     9296 2023-12-07 17:21:13.248573 mocodo-4.2.7/mocodo/resources/relation_templates/sqlite.yaml
+-rw-r--r--   0        0        0       18 2023-10-07 18:37:24.491936 mocodo-4.2.7/mocodo/resources/relation_templates/sqlserver-b.yaml
+-rw-r--r--   0        0        0       16 2023-10-07 18:37:24.492102 mocodo-4.2.7/mocodo/resources/relation_templates/sqlserver.yaml
+-rw-r--r--   0        0        0       18 2023-10-07 18:37:24.492259 mocodo-4.2.7/mocodo/resources/relation_templates/tex-b.yaml
+-rw-r--r--   0        0        0       19 2023-10-07 18:37:24.492437 mocodo-4.2.7/mocodo/resources/relation_templates/tex-bc.yaml
+-rw-r--r--   0        0        0       20 2023-10-07 18:37:24.492616 mocodo-4.2.7/mocodo/resources/relation_templates/tex-bce.yaml
+-rw-r--r--   0        0        0       19 2023-10-07 18:37:24.492851 mocodo-4.2.7/mocodo/resources/relation_templates/tex-be.yaml
+-rw-r--r--   0        0        0       18 2023-10-07 18:37:24.493025 mocodo-4.2.7/mocodo/resources/relation_templates/tex-c.yaml
+-rw-r--r--   0        0        0       19 2023-10-07 18:37:24.493198 mocodo-4.2.7/mocodo/resources/relation_templates/tex-ce.yaml
+-rw-r--r--   0        0        0       18 2023-10-07 18:37:24.493426 mocodo-4.2.7/mocodo/resources/relation_templates/tex-e.yaml
+-rw-r--r--   0        0        0       16 2023-10-07 18:37:24.493589 mocodo-4.2.7/mocodo/resources/relation_templates/tex.yaml
+-rw-r--r--   0        0        0       71 2023-10-07 18:37:24.493762 mocodo-4.2.7/mocodo/resources/relation_templates/text-b.yaml
+-rw-r--r--   0        0        0       17 2023-10-07 18:37:24.493932 mocodo-4.2.7/mocodo/resources/relation_templates/text-bc.yaml
+-rw-r--r--   0        0        0       18 2023-10-07 18:37:24.494094 mocodo-4.2.7/mocodo/resources/relation_templates/text-bce.yaml
+-rw-r--r--   0        0        0       73 2023-10-07 18:37:24.494283 mocodo-4.2.7/mocodo/resources/relation_templates/text-be.yaml
+-rw-r--r--   0        0        0     1717 2023-11-05 16:01:33.000000 mocodo-4.2.7/mocodo/resources/relation_templates/text-c.yaml
+-rw-r--r--   0        0        0     2198 2023-11-05 16:01:33.000000 mocodo-4.2.7/mocodo/resources/relation_templates/text-ce.yaml
+-rw-r--r--   0        0        0       72 2023-10-07 18:37:24.494938 mocodo-4.2.7/mocodo/resources/relation_templates/text-e.yaml
+-rw-r--r--   0        0        0      642 2023-10-26 11:27:39.000000 mocodo-4.2.7/mocodo/resources/relation_templates/text.yaml
+-rw-r--r--   0        0        0       17 2023-10-07 18:37:24.495304 mocodo-4.2.7/mocodo/resources/relation_templates/txt-b.yaml
+-rw-r--r--   0        0        0       18 2023-10-07 18:37:24.495471 mocodo-4.2.7/mocodo/resources/relation_templates/txt-bc.yaml
+-rw-r--r--   0        0        0       19 2023-10-07 18:37:24.495649 mocodo-4.2.7/mocodo/resources/relation_templates/txt-bce.yaml
+-rw-r--r--   0        0        0       18 2023-10-07 18:37:24.495827 mocodo-4.2.7/mocodo/resources/relation_templates/txt-be.yaml
+-rw-r--r--   0        0        0       17 2023-10-07 18:37:24.495992 mocodo-4.2.7/mocodo/resources/relation_templates/txt-c.yaml
+-rw-r--r--   0        0        0       18 2023-10-07 18:37:24.496155 mocodo-4.2.7/mocodo/resources/relation_templates/txt-ce.yaml
+-rw-r--r--   0        0        0       17 2023-10-07 18:37:24.496367 mocodo-4.2.7/mocodo/resources/relation_templates/txt-e.yaml
+-rw-r--r--   0        0        0       15 2023-10-07 18:37:24.496540 mocodo-4.2.7/mocodo/resources/relation_templates/txt.yaml
+-rw-r--r--   0        0        0      668 2023-10-28 08:03:42.000000 mocodo-4.2.7/mocodo/resources/rendering_services.json
+-rw-r--r--   0        0        0     1451 2023-06-06 10:56:21.555700 mocodo-4.2.7/mocodo/resources/shapes/arial.json
+-rw-r--r--   0        0        0     1450 2023-06-06 10:56:21.621120 mocodo-4.2.7/mocodo/resources/shapes/copperplate.json
+-rw-r--r--   0        0        0     1441 2023-06-06 10:56:21.555833 mocodo-4.2.7/mocodo/resources/shapes/georgia.json
+-rw-r--r--   0        0        0     1599 2023-06-06 10:56:21.555756 mocodo-4.2.7/mocodo/resources/shapes/mondrian.json
+-rw-r--r--   0        0        0     1506 2023-06-06 10:56:21.526558 mocodo-4.2.7/mocodo/resources/shapes/sans.json
+-rw-r--r--   0        0        0     1514 2023-06-06 10:56:21.555745 mocodo-4.2.7/mocodo/resources/shapes/serif.json
+-rw-r--r--   0        0        0     1481 2023-06-06 10:56:21.555870 mocodo-4.2.7/mocodo/resources/shapes/times.json
+-rw-r--r--   0        0        0     1466 2023-06-06 10:56:21.555816 mocodo-4.2.7/mocodo/resources/shapes/trebuchet.json
+-rw-r--r--   0        0        0     1591 2023-06-06 10:56:21.555794 mocodo-4.2.7/mocodo/resources/shapes/verdana.json
+-rw-r--r--   0        0        0     1487 2023-06-06 10:56:21.555731 mocodo-4.2.7/mocodo/resources/shapes/xinnian.json
+-rw-r--r--   0        0        0    13683 2023-11-11 10:30:33.999003 mocodo-4.2.7/mocodo/resources/transformations.json
+-rw-r--r--   0        0        0        0 2023-10-07 18:37:24.496816 mocodo-4.2.7/mocodo/rewrite/__init__.py
+-rwxr-xr-x   0        0        0      676 2023-10-12 16:18:10.772843 mocodo-4.2.7/mocodo/rewrite/_arrange.py
+-rwxr-xr-x   0        0        0     2545 2023-12-01 15:42:09.494163 mocodo-4.2.7/mocodo/rewrite/_drain.py
+-rw-r--r--   0        0        0     2088 2023-11-27 18:17:48.000000 mocodo-4.2.7/mocodo/rewrite/_drown.py
+-rwxr-xr-x   0        0        0     4421 2023-12-01 15:42:09.494661 mocodo-4.2.7/mocodo/rewrite/_explode.py
+-rwxr-xr-x   0        0        0     8456 2023-12-07 18:14:54.467132 mocodo-4.2.7/mocodo/rewrite/_grow.py
+-rwxr-xr-x   0        0        0     3509 2023-12-01 15:42:09.495674 mocodo-4.2.7/mocodo/rewrite/_split.py
+-rwxr-xr-x   0        0        0    10934 2023-11-20 13:17:10.497322 mocodo-4.2.7/mocodo/rewrite/arrange_bb.py
+-rwxr-xr-x   0        0        0     6521 2023-10-07 18:37:24.498605 mocodo-4.2.7/mocodo/rewrite/arrange_ga.py
+-rw-r--r--   0        0        0     1057 2023-12-01 15:42:09.496899 mocodo-4.2.7/mocodo/rewrite/arrows.py
+-rwxr-xr-x   0        0        0     2227 2023-12-01 15:42:09.497537 mocodo-4.2.7/mocodo/rewrite/cards.py
+-rw-r--r--   0        0        0     3095 2023-12-01 15:42:09.497799 mocodo-4.2.7/mocodo/rewrite/constraints.py
+-rwxr-xr-x   0        0        0     1437 2023-11-20 13:17:10.497938 mocodo-4.2.7/mocodo/rewrite/cross.py
+-rw-r--r--   0        0        0     1980 2023-10-07 18:37:24.499520 mocodo-4.2.7/mocodo/rewrite/damerau_levenshtein.py
+-rwxr-xr-x   0        0        0     1280 2023-10-07 18:37:24.499639 mocodo-4.2.7/mocodo/rewrite/fitness.py
+-rw-r--r--   0        0        0     1031 2023-12-01 15:42:09.498468 mocodo-4.2.7/mocodo/rewrite/guess_entities.py
+-rwxr-xr-x   0        0        0     2214 2023-11-13 15:47:43.816628 mocodo-4.2.7/mocodo/rewrite/obfuscate.py
+-rwxr-xr-x   0        0        0     5307 2023-10-14 07:19:39.038158 mocodo-4.2.7/mocodo/rewrite/op_tk.py
+-rw-r--r--   0        0        0     2723 2023-12-01 15:42:09.499228 mocodo-4.2.7/mocodo/rewrite/types.py
+-rw-r--r--   0        0        0        0 2023-10-07 18:37:24.500771 mocodo-4.2.7/mocodo/tools/__init__.py
+-rw-r--r--   0        0        0     4567 2023-10-07 18:37:24.500920 mocodo-4.2.7/mocodo/tools/graphviz_tools.py
+-rw-r--r--   0        0        0     1671 2023-11-13 15:47:43.816641 mocodo-4.2.7/mocodo/tools/load_mini_yaml.py
+-rwxr-xr-x   0        0        0    13711 2023-12-01 15:42:09.501752 mocodo-4.2.7/mocodo/tools/parser_tools.py
+-rwxr-xr-x   0        0        0     1639 2023-10-07 18:37:24.501453 mocodo-4.2.7/mocodo/tools/pluralize_fr.py
+-rw-r--r--   0        0        0     4513 2023-10-22 17:03:59.999142 mocodo-4.2.7/mocodo/tools/string_tools.py
+-rw-r--r--   0        0        0      163 2023-10-07 18:37:24.502029 mocodo-4.2.7/mocodo/tools/various.py
+-rw-r--r--   0        0        0     1433 2024-03-06 18:07:02.547048 mocodo-4.2.7/pyproject.toml
+-rw-r--r--   0        0        0    11525 1970-01-01 00:00:00.000000 mocodo-4.2.7/PKG-INFO
```

### Comparing `mocodo-4.2.6/LICENSE` & `mocodo-4.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/README.md` & `mocodo-4.2.7/README.md`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/__main__.py` & `mocodo-4.2.7/mocodo/__main__.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/api.py` & `mocodo-4.2.7/mocodo/api.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/argument_parser.py` & `mocodo-4.2.7/mocodo/argument_parser.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/association.py` & `mocodo-4.2.7/mocodo/association.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/attribute.py` & `mocodo-4.2.7/mocodo/attribute.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/common.py` & `mocodo-4.2.7/mocodo/common.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/constraint.py` & `mocodo-4.2.7/mocodo/constraint.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/convert/_ast.py` & `mocodo-4.2.7/mocodo/convert/_ast.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/convert/_chen.py` & `mocodo-4.2.7/mocodo/convert/_chen.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/convert/_crow.py` & `mocodo-4.2.7/mocodo/convert/_crow.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/convert/_data_dict.py` & `mocodo-4.2.7/mocodo/convert/_data_dict.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/convert/_uml.py` & `mocodo-4.2.7/mocodo/convert/_uml.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/convert/crow_gv.py` & `mocodo-4.2.7/mocodo/convert/crow_gv.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/convert/crow_mmd.py` & `mocodo-4.2.7/mocodo/convert/crow_mmd.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/convert/read_template.py` & `mocodo-4.2.7/mocodo/convert/read_template.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/convert/relations.py` & `mocodo-4.2.7/mocodo/convert/relations.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/dev/json_to_yaml_templates.py` & `mocodo-4.2.7/mocodo/dev/json_to_yaml_templates.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/dev/update_sql_reserved_words.py` & `mocodo-4.2.7/mocodo/dev/update_sql_reserved_words.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/dev/update_transfo_metadata.py` & `mocodo-4.2.7/mocodo/dev/update_transfo_metadata.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/diagram_link.py` & `mocodo-4.2.7/mocodo/diagram_link.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/entity.py` & `mocodo-4.2.7/mocodo/entity.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/font_metrics.py` & `mocodo-4.2.7/mocodo/font_metrics.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/grid.py` & `mocodo-4.2.7/mocodo/grid.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/guess_title.py` & `mocodo-4.2.7/mocodo/guess_title.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/inheritance.py` & `mocodo-4.2.7/mocodo/inheritance.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/leg.py` & `mocodo-4.2.7/mocodo/leg.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/magic.py` & `mocodo-4.2.7/mocodo/magic.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/mcd.py` & `mocodo-4.2.7/mocodo/mcd.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/mcd_to_svg.py` & `mocodo-4.2.7/mocodo/mcd_to_svg.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/mocodo_error.py` & `mocodo-4.2.7/mocodo/mocodo_error.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/parse_mcd.py` & `mocodo-4.2.7/mocodo/parse_mcd.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/phantom.py` & `mocodo-4.2.7/mocodo/phantom.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/blank.json` & `mocodo-4.2.7/mocodo/resources/colors/blank.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer+1.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer+1.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer+2.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer+2.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer+3.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer+3.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer+4.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer+4.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer+5.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer+5.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer+6.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer+6.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer+7.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer+7.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer+8.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer+8.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer+9.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer+9.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer-1.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer-1.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer-2.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer-2.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer-3.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer-3.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer-4.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer-4.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer-5.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer-5.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer-6.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer-6.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer-7.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer-7.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer-8.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer-8.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/brewer-9.json` & `mocodo-4.2.7/mocodo/resources/colors/brewer-9.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/bw-alpha.json` & `mocodo-4.2.7/mocodo/resources/colors/bw-alpha.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/bw.json` & `mocodo-4.2.7/mocodo/resources/colors/bw.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/desert.json` & `mocodo-4.2.7/mocodo/resources/colors/desert.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/gray.json` & `mocodo-4.2.7/mocodo/resources/colors/gray.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/keepsake.json` & `mocodo-4.2.7/mocodo/resources/colors/keepsake.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/mondrian.json` & `mocodo-4.2.7/mocodo/resources/colors/mondrian.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/ocean.json` & `mocodo-4.2.7/mocodo/resources/colors/ocean.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/pond.json` & `mocodo-4.2.7/mocodo/resources/colors/pond.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/wb.json` & `mocodo-4.2.7/mocodo/resources/colors/wb.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/colors/xinnian.json` & `mocodo-4.2.7/mocodo/resources/colors/xinnian.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/default_datatypes_en.tsv` & `mocodo-4.2.7/mocodo/resources/default_datatypes_en.tsv`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/default_datatypes_fr.tsv` & `mocodo-4.2.7/mocodo/resources/default_datatypes_fr.tsv`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/font_metrics.json` & `mocodo-4.2.7/mocodo/resources/font_metrics.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/grammar.lark` & `mocodo-4.2.7/mocodo/resources/grammar.lark`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/i18n/messages_de.mo` & `mocodo-4.2.7/mocodo/resources/i18n/messages_de.mo`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/i18n/messages_fr.mo` & `mocodo-4.2.7/mocodo/resources/i18n/messages_fr.mo`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/i18n/messages_fr.po` & `mocodo-4.2.7/mocodo/resources/i18n/messages_fr.po`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/i18n/messages_zh.mo` & `mocodo-4.2.7/mocodo/resources/i18n/messages_zh.mo`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/lorem/disparition.txt` & `mocodo-4.2.7/mocodo/resources/lorem/disparition.txt`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/lorem/en4.txt` & `mocodo-4.2.7/mocodo/resources/lorem/en4.txt`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/lorem/fr.txt` & `mocodo-4.2.7/mocodo/resources/lorem/fr.txt`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/lorem/fr5.txt` & `mocodo-4.2.7/mocodo/resources/lorem/fr5.txt`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/lorem/lorem.txt` & `mocodo-4.2.7/mocodo/resources/lorem/lorem.txt`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/pristine_sandbox.mcd` & `mocodo-4.2.7/mocodo/resources/pristine_sandbox.mcd`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/_index.json` & `mocodo-4.2.7/mocodo/resources/relation_templates/_index.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/d2.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/d2.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/dbml.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/dbml.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/debug.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/debug.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/dependencies.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/dependencies.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/diagram-c.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/diagram-c.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/html-bc.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/html-bc.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/html-bce.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/html-bce.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/html-c.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/html-c.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/html-ce.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/html-ce.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/html.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/html.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/latex-bc.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/latex-bc.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/latex-bce.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/latex-bce.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/latex-c.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/latex-c.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/latex-ce.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/latex-ce.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/latex.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/latex.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/markdown-c.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/markdown-c.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/markdown-ce.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/markdown-ce.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/markdown.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/markdown.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/mssql-b.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/mssql-b.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/mssql.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/mssql.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/mysql-b.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/mysql-b.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/mysql.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/mysql.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/oracle-b.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/oracle-b.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/oracle.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/oracle.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/postgresql-b.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/postgresql-b.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/postgresql.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/postgresql.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/sql.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/sql.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/sqlite.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/sqlite.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/text-c.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/text-c.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/text-ce.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/text-ce.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/relation_templates/text.yaml` & `mocodo-4.2.7/mocodo/resources/relation_templates/text.yaml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/rendering_services.json` & `mocodo-4.2.7/mocodo/resources/rendering_services.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/shapes/arial.json` & `mocodo-4.2.7/mocodo/resources/shapes/arial.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/shapes/copperplate.json` & `mocodo-4.2.7/mocodo/resources/shapes/copperplate.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/shapes/georgia.json` & `mocodo-4.2.7/mocodo/resources/shapes/georgia.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/shapes/mondrian.json` & `mocodo-4.2.7/mocodo/resources/shapes/mondrian.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/shapes/sans.json` & `mocodo-4.2.7/mocodo/resources/shapes/sans.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/shapes/serif.json` & `mocodo-4.2.7/mocodo/resources/shapes/serif.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/shapes/times.json` & `mocodo-4.2.7/mocodo/resources/shapes/times.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/shapes/trebuchet.json` & `mocodo-4.2.7/mocodo/resources/shapes/trebuchet.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/shapes/verdana.json` & `mocodo-4.2.7/mocodo/resources/shapes/verdana.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/shapes/xinnian.json` & `mocodo-4.2.7/mocodo/resources/shapes/xinnian.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/resources/transformations.json` & `mocodo-4.2.7/mocodo/resources/transformations.json`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/_arrange.py` & `mocodo-4.2.7/mocodo/rewrite/_arrange.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/_drain.py` & `mocodo-4.2.7/mocodo/rewrite/_drain.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/_drown.py` & `mocodo-4.2.7/mocodo/rewrite/_drown.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/_explode.py` & `mocodo-4.2.7/mocodo/rewrite/_explode.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/_grow.py` & `mocodo-4.2.7/mocodo/rewrite/_grow.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/_split.py` & `mocodo-4.2.7/mocodo/rewrite/_split.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/arrange_bb.py` & `mocodo-4.2.7/mocodo/rewrite/arrange_bb.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/arrange_ga.py` & `mocodo-4.2.7/mocodo/rewrite/arrange_ga.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/arrows.py` & `mocodo-4.2.7/mocodo/rewrite/arrows.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/cards.py` & `mocodo-4.2.7/mocodo/rewrite/cards.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/constraints.py` & `mocodo-4.2.7/mocodo/rewrite/constraints.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/cross.py` & `mocodo-4.2.7/mocodo/rewrite/cross.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/damerau_levenshtein.py` & `mocodo-4.2.7/mocodo/rewrite/damerau_levenshtein.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/fitness.py` & `mocodo-4.2.7/mocodo/rewrite/fitness.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/guess_entities.py` & `mocodo-4.2.7/mocodo/rewrite/guess_entities.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/obfuscate.py` & `mocodo-4.2.7/mocodo/rewrite/obfuscate.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/op_tk.py` & `mocodo-4.2.7/mocodo/rewrite/op_tk.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/rewrite/types.py` & `mocodo-4.2.7/mocodo/rewrite/types.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/tools/graphviz_tools.py` & `mocodo-4.2.7/mocodo/tools/graphviz_tools.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/tools/load_mini_yaml.py` & `mocodo-4.2.7/mocodo/tools/load_mini_yaml.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/tools/parser_tools.py` & `mocodo-4.2.7/mocodo/tools/parser_tools.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/tools/pluralize_fr.py` & `mocodo-4.2.7/mocodo/tools/pluralize_fr.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/mocodo/tools/string_tools.py` & `mocodo-4.2.7/mocodo/tools/string_tools.py`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/pyproject.toml` & `mocodo-4.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mocodo-4.2.6/PKG-INFO` & `mocodo-4.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocodo
-Version: 4.2.6
+Version: 4.2.7
 Summary: Modélisation Conceptuelle de Données. Nickel. Ni souris.
 Home-page: https://www.mocodo.net/
 License: MIT
 Keywords: education,relational,database,drawing,ERD,SVG,Merise
 Author: Aristide Grange
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Database
 Classifier: Topic :: Education
 Requires-Dist: requests (>=2.22.0,<3.0.0)
 Project-URL: Repository, https://github.com/laowantong/mocodo/
 Project-URL: issues, https://github.com/laowantong/mocodo/issues
 Description-Content-Type: text/markdown
```

