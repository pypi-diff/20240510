# Comparing `tmp/amazon-textract-textractor-1.7.8.tar.gz` & `tmp/amazon-textract-textractor-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-textract-textractor-1.7.8.tar", last modified: Thu Mar 21 12:22:38 2024, max compression
+gzip compressed data, was "amazon-textract-textractor-1.7.9.tar", last modified: Fri Mar 22 14:55:55 2024, max compression
```

## Comparing `amazon-textract-textractor-1.7.8.tar` & `amazon-textract-textractor-1.7.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:38.861400 amazon-textract-textractor-1.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-03-21 12:22:38.861400 amazon-textract-textractor-1.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:38.853400 amazon-textract-textractor-1.7.8/amazon_textract_textractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-03-21 12:22:38.000000 amazon-textract-textractor-1.7.8/amazon_textract_textractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-21 12:22:38.000000 amazon-textract-textractor-1.7.8/amazon_textract_textractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 12:22:38.000000 amazon-textract-textractor-1.7.8/amazon_textract_textractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-21 12:22:38.000000 amazon-textract-textractor-1.7.8/amazon_textract_textractor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-21 12:22:38.000000 amazon-textract-textractor-1.7.8/amazon_textract_textractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-21 12:22:38.000000 amazon-textract-textractor-1.7.8/amazon_textract_textractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:38.853400 amazon-textract-textractor-1.7.8/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/extras/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/extras/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/extras/pandas.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/extras/pdf.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/extras/torch.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-21 12:22:38.861400 amazon-textract-textractor-1.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:38.853400 amazon-textract-textractor-1.7.8/textractor/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:38.853400 amazon-textract-textractor-1.7.8/textractor/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:38.853400 amazon-textract-textractor-1.7.8/textractor/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/data/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/data/html_linearization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/data/markdown_linearization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/data/text_linearization_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:38.857400 amazon-textract-textractor-1.7.8/textractor/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    31720 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/document_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/expense_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/expense_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/identity_document.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/identity_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     9777 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/key_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/lazy_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/linearizable.py
--rw-r--r--   0 runner    (1001) docker     (127)    39915 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/page_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/selection_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)    45610 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/table_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/table_footer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/table_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/entities/word.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:38.857400 amazon-textract-textractor-1.7.8/textractor/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57291 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/parsers/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    37557 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/textractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:38.857400 amazon-textract-textractor-1.7.8/textractor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/utils/geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/utils/results_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/utils/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/utils/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 12:22:38.861400 amazon-textract-textractor-1.7.8/textractor/visualizers/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/visualizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   367112 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/visualizers/arial.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    46312 2024-03-21 12:22:25.000000 amazon-textract-textractor-1.7.8/textractor/visualizers/entitylist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:55.715124 amazon-textract-textractor-1.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-03-22 14:55:45.000000 amazon-textract-textractor-1.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-22 14:55:45.000000 amazon-textract-textractor-1.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-22 14:55:45.000000 amazon-textract-textractor-1.7.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-03-22 14:55:55.715124 amazon-textract-textractor-1.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-03-22 14:55:45.000000 amazon-textract-textractor-1.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:55.707124 amazon-textract-textractor-1.7.9/amazon_textract_textractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-03-22 14:55:55.000000 amazon-textract-textractor-1.7.9/amazon_textract_textractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-22 14:55:55.000000 amazon-textract-textractor-1.7.9/amazon_textract_textractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:55:55.000000 amazon-textract-textractor-1.7.9/amazon_textract_textractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 14:55:55.000000 amazon-textract-textractor-1.7.9/amazon_textract_textractor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-22 14:55:55.000000 amazon-textract-textractor-1.7.9/amazon_textract_textractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 14:55:55.000000 amazon-textract-textractor-1.7.9/amazon_textract_textractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:55.707124 amazon-textract-textractor-1.7.9/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/extras/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/extras/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/extras/pandas.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/extras/pdf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/extras/torch.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-22 14:55:55.715124 amazon-textract-textractor-1.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:55.707124 amazon-textract-textractor-1.7.9/textractor/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:55.707124 amazon-textract-textractor-1.7.9/textractor/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:55.707124 amazon-textract-textractor-1.7.9/textractor/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/data/html_linearization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/data/markdown_linearization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/data/text_linearization_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:55.711124 amazon-textract-textractor-1.7.9/textractor/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31720 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/document_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/expense_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/expense_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/identity_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/identity_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9777 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/key_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11576 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/lazy_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/linearizable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39915 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/page_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/selection_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45610 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11767 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/table_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/table_footer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/table_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/entities/word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:55.711124 amazon-textract-textractor-1.7.9/textractor/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57291 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/parsers/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37684 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/textractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:55.711124 amazon-textract-textractor-1.7.9/textractor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/utils/geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/utils/results_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/utils/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:55:55.715124 amazon-textract-textractor-1.7.9/textractor/visualizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/visualizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   367112 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/visualizers/arial.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    46312 2024-03-22 14:55:46.000000 amazon-textract-textractor-1.7.9/textractor/visualizers/entitylist.py
```

### Comparing `amazon-textract-textractor-1.7.8/LICENSE` & `amazon-textract-textractor-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/PKG-INFO` & `amazon-textract-textractor-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-textractor
-Version: 1.7.8
+Version: 1.7.9
 Summary: A package to use AWS Textract services.
 Home-page: https://github.com/aws-samples/amazon-textract-textractor
 License: Apache 2.0
 Keywords: amazon textract aws ocr document
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `amazon-textract-textractor-1.7.8/README.md` & `amazon-textract-textractor-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/amazon_textract_textractor.egg-info/PKG-INFO` & `amazon-textract-textractor-1.7.9/amazon_textract_textractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-textractor
-Version: 1.7.8
+Version: 1.7.9
 Summary: A package to use AWS Textract services.
 Home-page: https://github.com/aws-samples/amazon-textract-textractor
 License: Apache 2.0
 Keywords: amazon textract aws ocr document
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `amazon-textract-textractor-1.7.8/amazon_textract_textractor.egg-info/SOURCES.txt` & `amazon-textract-textractor-1.7.9/amazon_textract_textractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/amazon_textract_textractor.egg-info/requires.txt` & `amazon-textract-textractor-1.7.9/amazon_textract_textractor.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/setup.py` & `amazon-textract-textractor-1.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         except subprocess.CalledProcessError as error:
             print('Command failed with exit code', error.returncode)
             sys.exit(error.returncode)
 
 setup(
     # include data files
     name="amazon-textract-textractor",
-    version="1.7.8",
+    version="1.7.9",
     license="Apache 2.0",
     description="A package to use AWS Textract services.",
     url="https://github.com/aws-samples/amazon-textract-textractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `amazon-textract-textractor-1.7.8/textractor/cli/cli.py` & `amazon-textract-textractor-1.7.9/textractor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/data/constants.py` & `amazon-textract-textractor-1.7.9/textractor/data/constants.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/data/html_linearization_config.py` & `amazon-textract-textractor-1.7.9/textractor/data/html_linearization_config.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/data/markdown_linearization_config.py` & `amazon-textract-textractor-1.7.9/textractor/data/markdown_linearization_config.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/data/text_linearization_config.py` & `amazon-textract-textractor-1.7.9/textractor/data/text_linearization_config.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/bbox.py` & `amazon-textract-textractor-1.7.9/textractor/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/document.py` & `amazon-textract-textractor-1.7.9/textractor/entities/document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/document_entity.py` & `amazon-textract-textractor-1.7.9/textractor/entities/document_entity.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/expense_document.py` & `amazon-textract-textractor-1.7.9/textractor/entities/expense_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/expense_field.py` & `amazon-textract-textractor-1.7.9/textractor/entities/expense_field.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/identity_document.py` & `amazon-textract-textractor-1.7.9/textractor/entities/identity_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/key_value.py` & `amazon-textract-textractor-1.7.9/textractor/entities/key_value.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/layout.py` & `amazon-textract-textractor-1.7.9/textractor/entities/layout.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/lazy_document.py` & `amazon-textract-textractor-1.7.9/textractor/entities/lazy_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/line.py` & `amazon-textract-textractor-1.7.9/textractor/entities/line.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/linearizable.py` & `amazon-textract-textractor-1.7.9/textractor/entities/linearizable.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/page.py` & `amazon-textract-textractor-1.7.9/textractor/entities/page.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/page_layout.py` & `amazon-textract-textractor-1.7.9/textractor/entities/page_layout.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/query.py` & `amazon-textract-textractor-1.7.9/textractor/entities/query.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/query_result.py` & `amazon-textract-textractor-1.7.9/textractor/entities/query_result.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/selection_element.py` & `amazon-textract-textractor-1.7.9/textractor/entities/selection_element.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/signature.py` & `amazon-textract-textractor-1.7.9/textractor/entities/signature.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/table.py` & `amazon-textract-textractor-1.7.9/textractor/entities/table.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/table_cell.py` & `amazon-textract-textractor-1.7.9/textractor/entities/table_cell.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/table_footer.py` & `amazon-textract-textractor-1.7.9/textractor/entities/table_footer.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/table_title.py` & `amazon-textract-textractor-1.7.9/textractor/entities/table_title.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/value.py` & `amazon-textract-textractor-1.7.9/textractor/entities/value.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/entities/word.py` & `amazon-textract-textractor-1.7.9/textractor/entities/word.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/exceptions.py` & `amazon-textract-textractor-1.7.9/textractor/exceptions.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/parsers/response_parser.py` & `amazon-textract-textractor-1.7.9/textractor/parsers/response_parser.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/textractor.py` & `amazon-textract-textractor-1.7.9/textractor/textractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -838,10 +838,11 @@
     Function to convert PIL.Image to bytearray for processing Document using Textract service.
     :param image: Image to be converted to bytearray
     :type image: PIL.Image, required
     :return: Returns a bytearray of the input image
     :rtype: bytes
     """
     img_byte_arr = io.BytesIO()
-    image.convert("RGB").save(img_byte_arr, format="JPEG")
+    # We set quality to 95 and subsampling to 0 because the pillow defaults are very low resolution
+    image.convert("RGB").save(img_byte_arr, format="JPEG", quality=95, subsampling=0)
     img_byte_arr = img_byte_arr.getvalue()
     return img_byte_arr
```

### Comparing `amazon-textract-textractor-1.7.8/textractor/utils/geometry_util.py` & `amazon-textract-textractor-1.7.9/textractor/utils/geometry_util.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/utils/results_utils.py` & `amazon-textract-textractor-1.7.9/textractor/utils/results_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/utils/s3_utils.py` & `amazon-textract-textractor-1.7.9/textractor/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/utils/search_utils.py` & `amazon-textract-textractor-1.7.9/textractor/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/utils/text_utils.py` & `amazon-textract-textractor-1.7.9/textractor/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/visualizers/arial.ttf` & `amazon-textract-textractor-1.7.9/textractor/visualizers/arial.ttf`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.7.8/textractor/visualizers/entitylist.py` & `amazon-textract-textractor-1.7.9/textractor/visualizers/entitylist.py`

 * *Files identical despite different names*

