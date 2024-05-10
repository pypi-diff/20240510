# Comparing `tmp/django-inapp-survey-0.2.5.tar.gz` & `tmp/django-inapp-survey-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-inapp-survey-0.2.5.tar", last modified: Thu Aug 24 07:35:28 2023, max compression
+gzip compressed data, was "django-inapp-survey-0.2.6.tar", last modified: Fri May 10 05:17:30 2024, max compression
```

## Comparing `django-inapp-survey-0.2.5.tar` & `django-inapp-survey-0.2.6.tar`

### file list

```diff
@@ -1,795 +1,796 @@
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.795254 django-inapp-survey-0.2.5/
--rw-r--r--   0 naveen     (501) staff       (20)    11357 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/LICENSE
--rw-r--r--   0 naveen     (501) staff       (20)      155 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/MANIFEST.in
--rw-r--r--   0 naveen     (501) staff       (20)     2110 2023-08-24 07:35:28.795089 django-inapp-survey-0.2.5/PKG-INFO
--rw-r--r--   0 naveen     (501) staff       (20)     1256 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/README.md
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.628351 django-inapp-survey-0.2.5/django_inapp_survey.egg-info/
--rw-r--r--   0 naveen     (501) staff       (20)     2110 2023-08-24 07:35:28.000000 django-inapp-survey-0.2.5/django_inapp_survey.egg-info/PKG-INFO
--rw-r--r--   0 naveen     (501) staff       (20)    44391 2023-08-24 07:35:28.000000 django-inapp-survey-0.2.5/django_inapp_survey.egg-info/SOURCES.txt
--rw-r--r--   0 naveen     (501) staff       (20)        1 2023-08-24 07:35:28.000000 django-inapp-survey-0.2.5/django_inapp_survey.egg-info/dependency_links.txt
--rw-r--r--   0 naveen     (501) staff       (20)       50 2023-08-24 07:35:28.000000 django-inapp-survey-0.2.5/django_inapp_survey.egg-info/requires.txt
--rw-r--r--   0 naveen     (501) staff       (20)       13 2023-08-24 07:35:28.000000 django-inapp-survey-0.2.5/django_inapp_survey.egg-info/top_level.txt
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.630386 django-inapp-survey-0.2.5/inapp_survey/
--rw-r--r--   0 naveen     (501) staff       (20)       22 2023-08-24 06:57:12.000000 django-inapp-survey-0.2.5/inapp_survey/__init__.py
--rw-r--r--   0 naveen     (501) staff       (20)     2935 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.5/inapp_survey/admin.py
--rw-r--r--   0 naveen     (501) staff       (20)      196 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.5/inapp_survey/apps.py
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.630633 django-inapp-survey-0.2.5/inapp_survey/docs/
--rw-r--r--   0 naveen     (501) staff       (20)       65 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/docs/example.md
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.631256 django-inapp-survey-0.2.5/inapp_survey/migrations/
--rw-r--r--   0 naveen     (501) staff       (20)     5640 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/migrations/0001_initial.py
--rw-r--r--   0 naveen     (501) staff       (20)     1863 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.5/inapp_survey/migrations/0002_auto_20210912_1311.py
--rw-r--r--   0 naveen     (501) staff       (20)        0 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/migrations/__init__.py
--rw-r--r--   0 naveen     (501) staff       (20)     3088 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.5/inapp_survey/models.py
--rw-r--r--   0 naveen     (501) staff       (20)     3510 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.5/inapp_survey/resources.py
--rw-r--r--   0 naveen     (501) staff       (20)     3124 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/serializers.py
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.626237 django-inapp-survey-0.2.5/inapp_survey/static/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.625933 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.632579 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/
--rw-r--r--   0 naveen     (501) staff       (20)      333 2022-11-04 12:33:27.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/.bower.json
--rwxr-xr-x   0 naveen     (501) staff       (20)     1711 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/README.md
--rw-r--r--   0 naveen     (501) staff       (20)      160 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/SECURITY.md
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.613054 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/examples/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.632903 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/examples/node/
--rw-r--r--   0 naveen     (501) staff       (20)      576 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/examples/node/index.js
--rw-r--r--   0 naveen     (501) staff       (20)     1449 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/license.txt
--rw-r--r--   0 naveen     (501) staff       (20)      223 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/manifest.json
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.636442 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/
--rw-r--r--   0 naveen     (501) staff       (20)      237 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/README.md
--rw-r--r--   0 naveen     (501) staff       (20)      741 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/british.html
--rw-r--r--   0 naveen     (501) staff       (20)      779 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/british.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.613407 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.637890 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/
--rw-r--r--   0 naveen     (501) staff       (20)    18071 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/LICENSE
--rw-r--r--   0 naveen     (501) staff       (20)    12799 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/de_DE.aff
--rw-r--r--   0 naveen     (501) staff       (20)  1185467 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/de_DE.dic
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.640430 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/
--rw-r--r--   0 naveen     (501) staff       (20)    15184 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/LICENSE
--rw-r--r--   0 naveen     (501) staff       (20)    28123 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/en_GB.aff
--rw-r--r--   0 naveen     (501) staff       (20)   706742 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/en_GB.dic
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.642434 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/fr_FR/
--rw-r--r--   0 naveen     (501) staff       (20)   311776 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/fr_FR/fr_FR.aff
--rw-r--r--   0 naveen     (501) staff       (20)   903141 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/fr_FR/fr_FR.dic
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.646425 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/
--rwxr-xr-x   0 naveen     (501) staff       (20)    18957 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/README_la.txt
--rwxr-xr-x   0 naveen     (501) staff       (20)   102451 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/la.aff
--rwxr-xr-x   0 naveen     (501) staff       (20)   131575 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/la.dic
--rw-r--r--   0 naveen     (501) staff       (20)      725 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/english.html
--rw-r--r--   0 naveen     (501) staff       (20)     6772 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/english.js
--rw-r--r--   0 naveen     (501) staff       (20)      718 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/french.html
--rw-r--r--   0 naveen     (501) staff       (20)     1992 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/french.js
--rw-r--r--   0 naveen     (501) staff       (20)      725 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/general.html
--rw-r--r--   0 naveen     (501) staff       (20)     2802 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/general.js
--rw-r--r--   0 naveen     (501) staff       (20)      722 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/german.html
--rw-r--r--   0 naveen     (501) staff       (20)     1310 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/german.js
--rw-r--r--   0 naveen     (501) staff       (20)      567 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/index.html
--rw-r--r--   0 naveen     (501) staff       (20)      719 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/latin.html
--rw-r--r--   0 naveen     (501) staff       (20)     2280 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/latin.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.647993 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/
--rw-r--r--   0 naveen     (501) staff       (20)   268381 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/jquery-1.9.1.js
--rw-r--r--   0 naveen     (501) staff       (20)     4525 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/qunit.css
--rw-r--r--   0 naveen     (501) staff       (20)    50111 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/qunit.js
--rw-r--r--   0 naveen     (501) staff       (20)       24 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/tests.css
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.648968 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/
--rw-r--r--   0 naveen     (501) staff       (20)      910 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/README.md
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.613798 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.649892 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/
--rw-r--r--   0 naveen     (501) staff       (20)      420 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/README.md
--rw-r--r--   0 naveen     (501) staff       (20)     3045 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/en_US.aff
--rw-r--r--   0 naveen     (501) staff       (20)   696131 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/en_US.dic
--rw-r--r--   0 naveen     (501) staff       (20)      704 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/package.json
--rw-r--r--   0 naveen     (501) staff       (20)    27334 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/typo.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.653093 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/
--rw-r--r--   0 naveen     (501) staff       (20)      639 2022-11-04 12:33:27.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/.bower.json
--rw-r--r--   0 naveen     (501) staff       (20)     7279 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/AUTHORS
--rw-r--r--   0 naveen     (501) staff       (20)    52656 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/CHANGELOG.md
--rw-r--r--   0 naveen     (501) staff       (20)     3689 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/CONTRIBUTING.md
--rw-r--r--   0 naveen     (501) staff       (20)     1094 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/LICENSE
--rw-r--r--   0 naveen     (501) staff       (20)     1409 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/README.md
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.614881 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.653649 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/comment/
--rw-r--r--   0 naveen     (501) staff       (20)     8446 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/comment/comment.js
--rw-r--r--   0 naveen     (501) staff       (20)     3399 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/comment/continuecomment.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.654098 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/dialog/
--rw-r--r--   0 naveen     (501) staff       (20)      507 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/dialog/dialog.css
--rw-r--r--   0 naveen     (501) staff       (20)     4938 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/dialog/dialog.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.655733 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/
--rw-r--r--   0 naveen     (501) staff       (20)     1543 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/autorefresh.js
--rw-r--r--   0 naveen     (501) staff       (20)      116 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/fullscreen.css
--rw-r--r--   0 naveen     (501) staff       (20)     1494 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/fullscreen.js
--rw-r--r--   0 naveen     (501) staff       (20)     3844 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/panel.js
--rw-r--r--   0 naveen     (501) staff       (20)     2139 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/placeholder.js
--rw-r--r--   0 naveen     (501) staff       (20)     2090 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/rulers.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.657662 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/
--rw-r--r--   0 naveen     (501) staff       (20)     6945 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/closebrackets.js
--rw-r--r--   0 naveen     (501) staff       (20)     7705 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/closetag.js
--rw-r--r--   0 naveen     (501) staff       (20)     1761 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/continuelist.js
--rw-r--r--   0 naveen     (501) staff       (20)     5254 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/matchbrackets.js
--rw-r--r--   0 naveen     (501) staff       (20)     2355 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/matchtags.js
--rw-r--r--   0 naveen     (501) staff       (20)     1003 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/trailingspace.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.659978 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/
--rw-r--r--   0 naveen     (501) staff       (20)     3904 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/brace-fold.js
--rw-r--r--   0 naveen     (501) staff       (20)     2147 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/comment-fold.js
--rw-r--r--   0 naveen     (501) staff       (20)     4693 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/foldcode.js
--rw-r--r--   0 naveen     (501) staff       (20)      435 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/foldgutter.css
--rw-r--r--   0 naveen     (501) staff       (20)     4612 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/foldgutter.js
--rw-r--r--   0 naveen     (501) staff       (20)     1627 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/indent-fold.js
--rw-r--r--   0 naveen     (501) staff       (20)     1605 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/markdown-fold.js
--rw-r--r--   0 naveen     (501) staff       (20)     6570 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/xml-fold.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.661843 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/
--rw-r--r--   0 naveen     (501) staff       (20)     1680 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/anyword-hint.js
--rw-r--r--   0 naveen     (501) staff       (20)     2165 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/css-hint.js
--rw-r--r--   0 naveen     (501) staff       (20)    11341 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/html-hint.js
--rw-r--r--   0 naveen     (501) staff       (20)     6163 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/javascript-hint.js
--rw-r--r--   0 naveen     (501) staff       (20)      662 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/show-hint.css
--rw-r--r--   0 naveen     (501) staff       (20)    16422 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/show-hint.js
--rw-r--r--   0 naveen     (501) staff       (20)     8578 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/sql-hint.js
--rw-r--r--   0 naveen     (501) staff       (20)     4735 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/xml-hint.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.663410 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/
--rw-r--r--   0 naveen     (501) staff       (20)     1270 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/coffeescript-lint.js
--rw-r--r--   0 naveen     (501) staff       (20)     1146 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/css-lint.js
--rw-r--r--   0 naveen     (501) staff       (20)     1513 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/html-lint.js
--rw-r--r--   0 naveen     (501) staff       (20)     4469 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/javascript-lint.js
--rw-r--r--   0 naveen     (501) staff       (20)      954 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/json-lint.js
--rw-r--r--   0 naveen     (501) staff       (20)     3012 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/lint.css
--rw-r--r--   0 naveen     (501) staff       (20)     8032 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/lint.js
--rw-r--r--   0 naveen     (501) staff       (20)      848 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/yaml-lint.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.663799 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/merge/
--rw-r--r--   0 naveen     (501) staff       (20)     3249 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/merge/merge.css
--rw-r--r--   0 naveen     (501) staff       (20)    28660 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/merge/merge.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.665985 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/
--rw-r--r--   0 naveen     (501) staff       (20)     2277 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/loadmode.js
--rw-r--r--   0 naveen     (501) staff       (20)     4624 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/multiplex.js
--rw-r--r--   0 naveen     (501) staff       (20)      833 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/multiplex_test.js
--rw-r--r--   0 naveen     (501) staff       (20)     3021 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/overlay.js
--rw-r--r--   0 naveen     (501) staff       (20)     7899 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/simple.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.666913 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/
--rw-r--r--   0 naveen     (501) staff       (20)     1303 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/colorize.js
--rw-r--r--   0 naveen     (501) staff       (20)     5302 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode-standalone.js
--rw-r--r--   0 naveen     (501) staff       (20)     2499 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode.js
--rw-r--r--   0 naveen     (501) staff       (20)     6528 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode.node.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.667749 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/
--rw-r--r--   0 naveen     (501) staff       (20)     4250 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/annotatescrollbar.js
--rw-r--r--   0 naveen     (501) staff       (20)     1492 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/scrollpastend.js
--rw-r--r--   0 naveen     (501) staff       (20)     1347 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/simplescrollbars.css
--rw-r--r--   0 naveen     (501) staff       (20)     5297 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/simplescrollbars.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.668681 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/
--rw-r--r--   0 naveen     (501) staff       (20)     1940 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/jump-to-line.js
--rw-r--r--   0 naveen     (501) staff       (20)     5745 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/match-highlighter.js
--rw-r--r--   0 naveen     (501) staff       (20)      188 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/matchesonscrollbar.css
--rw-r--r--   0 naveen     (501) staff       (20)     3808 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/matchesonscrollbar.js
--rw-r--r--   0 naveen     (501) staff       (20)     8957 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/search.js
--rw-r--r--   0 naveen     (501) staff       (20)     7723 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/searchcursor.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.669163 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/
--rw-r--r--   0 naveen     (501) staff       (20)     2624 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/active-line.js
--rw-r--r--   0 naveen     (501) staff       (20)     3781 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/mark-selection.js
--rw-r--r--   0 naveen     (501) staff       (20)     3292 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/selection-pointer.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.669681 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/
--rw-r--r--   0 naveen     (501) staff       (20)     1872 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/tern.css
--rw-r--r--   0 naveen     (501) staff       (20)    24561 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/tern.js
--rw-r--r--   0 naveen     (501) staff       (20)     1208 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/worker.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.669849 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/wrap/
--rw-r--r--   0 naveen     (501) staff       (20)     5414 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/wrap/hardwrap.js
--rw-r--r--   0 naveen     (501) staff       (20)      279 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/bower.json
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.670667 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/keymap/
--rw-r--r--   0 naveen     (501) staff       (20)    13338 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/keymap/emacs.js
--rw-r--r--   0 naveen     (501) staff       (20)    21589 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/keymap/sublime.js
--rw-r--r--   0 naveen     (501) staff       (20)   197901 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/keymap/vim.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.671189 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/lib/
--rw-r--r--   0 naveen     (501) staff       (20)     8137 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/lib/codemirror.css
--rw-r--r--   0 naveen     (501) staff       (20)   353548 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/lib/codemirror.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.671958 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.672343 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/apl/
--rw-r--r--   0 naveen     (501) staff       (20)     4736 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/apl/apl.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.672635 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/asciiarmor/
--rw-r--r--   0 naveen     (501) staff       (20)     2378 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/asciiarmor/asciiarmor.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.672909 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/asn.1/
--rw-r--r--   0 naveen     (501) staff       (20)     7735 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/asn.1/asn.1.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.673303 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/asterisk/
--rw-r--r--   0 naveen     (501) staff       (20)     7437 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/asterisk/asterisk.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.673641 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/brainfuck/
--rw-r--r--   0 naveen     (501) staff       (20)     2174 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/brainfuck/brainfuck.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.673890 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/clike/
--rw-r--r--   0 naveen     (501) staff       (20)    30346 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/clike/clike.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.674204 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/clojure/
--rw-r--r--   0 naveen     (501) staff       (20)    15189 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/clojure/clojure.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.674408 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/cmake/
--rw-r--r--   0 naveen     (501) staff       (20)     2600 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/cmake/cmake.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.674671 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/cobol/
--rw-r--r--   0 naveen     (501) staff       (20)    10288 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/cobol/cobol.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.674876 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/coffeescript/
--rw-r--r--   0 naveen     (501) staff       (20)     9884 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/coffeescript/coffeescript.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.675078 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/commonlisp/
--rw-r--r--   0 naveen     (501) staff       (20)     4488 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/commonlisp/commonlisp.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.675308 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/crystal/
--rw-r--r--   0 naveen     (501) staff       (20)    11339 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/crystal/crystal.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.675537 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/css/
--rw-r--r--   0 naveen     (501) staff       (20)    37156 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/css/css.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.675830 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/cypher/
--rw-r--r--   0 naveen     (501) staff       (20)     6277 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/cypher/cypher.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.676022 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/d/
--rw-r--r--   0 naveen     (501) staff       (20)     7566 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/d/d.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.676256 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dart/
--rw-r--r--   0 naveen     (501) staff       (20)     5114 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dart/dart.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.676460 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/diff/
--rw-r--r--   0 naveen     (501) staff       (20)     1138 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/diff/diff.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.676654 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/django/
--rw-r--r--   0 naveen     (501) staff       (20)    11787 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/django/django.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.676841 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dockerfile/
--rw-r--r--   0 naveen     (501) staff       (20)     2221 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dockerfile/dockerfile.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.677020 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dtd/
--rw-r--r--   0 naveen     (501) staff       (20)     4808 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dtd/dtd.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.677184 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dylan/
--rw-r--r--   0 naveen     (501) staff       (20)     9902 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dylan/dylan.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.677358 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ebnf/
--rw-r--r--   0 naveen     (501) staff       (20)     6075 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ebnf/ebnf.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.677541 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ecl/
--rw-r--r--   0 naveen     (501) staff       (20)     8843 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ecl/ecl.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.677706 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/eiffel/
--rw-r--r--   0 naveen     (501) staff       (20)     3744 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/eiffel/eiffel.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.677888 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/elm/
--rw-r--r--   0 naveen     (501) staff       (20)     5552 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/elm/elm.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.678061 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/erlang/
--rw-r--r--   0 naveen     (501) staff       (20)    18853 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/erlang/erlang.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.678277 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/factor/
--rw-r--r--   0 naveen     (501) staff       (20)     2919 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/factor/factor.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.678448 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/fcl/
--rw-r--r--   0 naveen     (501) staff       (20)     4703 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/fcl/fcl.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.678609 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/forth/
--rw-r--r--   0 naveen     (501) staff       (20)     5230 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/forth/forth.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.678769 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/fortran/
--rw-r--r--   0 naveen     (501) staff       (20)     8686 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/fortran/fortran.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.678934 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/gas/
--rw-r--r--   0 naveen     (501) staff       (20)     8886 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/gas/gas.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.679155 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/gfm/
--rw-r--r--   0 naveen     (501) staff       (20)     5137 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/gfm/gfm.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.679373 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/gherkin/
--rw-r--r--   0 naveen     (501) staff       (20)    13257 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/gherkin/gherkin.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.679555 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/go/
--rw-r--r--   0 naveen     (501) staff       (20)     5938 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/go/go.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.679764 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/groovy/
--rw-r--r--   0 naveen     (501) staff       (20)     7878 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/groovy/groovy.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.679949 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haml/
--rw-r--r--   0 naveen     (501) staff       (20)     5332 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haml/haml.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.680226 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/handlebars/
--rw-r--r--   0 naveen     (501) staff       (20)     2172 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/handlebars/handlebars.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.680390 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell/
--rw-r--r--   0 naveen     (501) staff       (20)     8101 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell/haskell.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.680568 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell-literate/
--rw-r--r--   0 naveen     (501) staff       (20)     1390 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell-literate/haskell-literate.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.680776 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haxe/
--rw-r--r--   0 naveen     (501) staff       (20)    17568 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haxe/haxe.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.681009 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlembedded/
--rw-r--r--   0 naveen     (501) staff       (20)     1417 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlembedded/htmlembedded.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.681415 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlmixed/
--rw-r--r--   0 naveen     (501) staff       (20)     5555 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlmixed/htmlmixed.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.681589 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/http/
--rw-r--r--   0 naveen     (501) staff       (20)     2795 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/http/http.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.681949 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/idl/
--rw-r--r--   0 naveen     (501) staff       (20)    14889 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/idl/idl.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.682125 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/jade/
--rw-r--r--   0 naveen     (501) staff       (20)    15972 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/jade/jade.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.682302 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/javascript/
--rw-r--r--   0 naveen     (501) staff       (20)    28078 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/javascript/javascript.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.682582 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/jinja2/
--rw-r--r--   0 naveen     (501) staff       (20)     4284 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/jinja2/jinja2.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.682753 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/jsx/
--rw-r--r--   0 naveen     (501) staff       (20)     5087 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/jsx/jsx.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.682929 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/julia/
--rw-r--r--   0 naveen     (501) staff       (20)    11430 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/julia/julia.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.683133 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/livescript/
--rw-r--r--   0 naveen     (501) staff       (20)     7635 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/livescript/livescript.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.683360 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/lua/
--rw-r--r--   0 naveen     (501) staff       (20)     5950 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/lua/lua.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.683551 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/markdown/
--rw-r--r--   0 naveen     (501) staff       (20)    25301 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/markdown/markdown.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.683782 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mathematica/
--rw-r--r--   0 naveen     (501) staff       (20)     5570 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mathematica/mathematica.js
--rw-r--r--   0 naveen     (501) staff       (20)    14057 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/meta.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.683953 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mirc/
--rw-r--r--   0 naveen     (501) staff       (20)    10082 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mirc/mirc.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.684121 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mllike/
--rw-r--r--   0 naveen     (501) staff       (20)     5018 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mllike/mllike.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.684283 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/modelica/
--rw-r--r--   0 naveen     (501) staff       (20)     6930 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/modelica/modelica.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.684438 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mscgen/
--rw-r--r--   0 naveen     (501) staff       (20)     6523 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mscgen/mscgen.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.684589 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mumps/
--rw-r--r--   0 naveen     (501) staff       (20)     5354 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mumps/mumps.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.684738 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/nginx/
--rw-r--r--   0 naveen     (501) staff       (20)    10164 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/nginx/nginx.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.684899 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/nsis/
--rw-r--r--   0 naveen     (501) staff       (20)     7632 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/nsis/nsis.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.685074 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ntriples/
--rw-r--r--   0 naveen     (501) staff       (20)     6643 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ntriples/ntriples.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.685228 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/octave/
--rw-r--r--   0 naveen     (501) staff       (20)     4463 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/octave/octave.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.685373 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/oz/
--rw-r--r--   0 naveen     (501) staff       (20)     6658 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/oz/oz.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.685543 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/pascal/
--rw-r--r--   0 naveen     (501) staff       (20)     3055 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/pascal/pascal.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.685688 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/pegjs/
--rw-r--r--   0 naveen     (501) staff       (20)     3562 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/pegjs/pegjs.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.685828 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/perl/
--rw-r--r--   0 naveen     (501) staff       (20)    56134 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/perl/perl.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.686248 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/php/
--rw-r--r--   0 naveen     (501) staff       (20)    18177 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/php/php.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.686561 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/pig/
--rw-r--r--   0 naveen     (501) staff       (20)     5810 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/pig/pig.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.686750 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/properties/
--rw-r--r--   0 naveen     (501) staff       (20)     2169 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/properties/properties.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.686960 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/protobuf/
--rw-r--r--   0 naveen     (501) staff       (20)     2113 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/protobuf/protobuf.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.687182 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/puppet/
--rw-r--r--   0 naveen     (501) staff       (20)     7574 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/puppet/puppet.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.687383 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/python/
--rw-r--r--   0 naveen     (501) staff       (20)    12627 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/python/python.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.687588 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/q/
--rw-r--r--   0 naveen     (501) staff       (20)     6617 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/q/q.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.687768 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/r/
--rw-r--r--   0 naveen     (501) staff       (20)     5677 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/r/r.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.687967 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/rpm/
--rw-r--r--   0 naveen     (501) staff       (20)     3775 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/rpm/rpm.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.688247 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/rst/
--rw-r--r--   0 naveen     (501) staff       (20)    17547 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/rst/rst.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.689025 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ruby/
--rw-r--r--   0 naveen     (501) staff       (20)    10457 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ruby/ruby.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.689202 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/rust/
--rw-r--r--   0 naveen     (501) staff       (20)     3025 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/rust/rust.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.689378 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sass/
--rw-r--r--   0 naveen     (501) staff       (20)    10059 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sass/sass.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.689661 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/scheme/
--rw-r--r--   0 naveen     (501) staff       (20)    13439 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/scheme/scheme.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.689907 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/shell/
--rw-r--r--   0 naveen     (501) staff       (20)     3792 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/shell/shell.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.690188 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sieve/
--rw-r--r--   0 naveen     (501) staff       (20)     4285 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sieve/sieve.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.690381 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/slim/
--rw-r--r--   0 naveen     (501) staff       (20)    18008 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/slim/slim.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.690824 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/smalltalk/
--rw-r--r--   0 naveen     (501) staff       (20)     4543 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/smalltalk/smalltalk.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.691061 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/smarty/
--rw-r--r--   0 naveen     (501) staff       (20)     6828 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/smarty/smarty.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.691311 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/solr/
--rw-r--r--   0 naveen     (501) staff       (20)     2678 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/solr/solr.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.691930 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/soy/
--rw-r--r--   0 naveen     (501) staff       (20)     7564 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/soy/soy.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.692107 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sparql/
--rw-r--r--   0 naveen     (501) staff       (20)     6327 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sparql/sparql.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.692286 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/spreadsheet/
--rw-r--r--   0 naveen     (501) staff       (20)     3139 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/spreadsheet/spreadsheet.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.692444 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sql/
--rw-r--r--   0 naveen     (501) staff       (20)    33831 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sql/sql.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.692674 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/stex/
--rw-r--r--   0 naveen     (501) staff       (20)     6932 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/stex/stex.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.692841 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/stylus/
--rw-r--r--   0 naveen     (501) staff       (20)    42120 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/stylus/stylus.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.693056 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/swift/
--rw-r--r--   0 naveen     (501) staff       (20)     6424 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/swift/swift.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.693618 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tcl/
--rw-r--r--   0 naveen     (501) staff       (20)     4920 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tcl/tcl.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.693765 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/textile/
--rw-r--r--   0 naveen     (501) staff       (20)    13842 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/textile/textile.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.694072 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tiddlywiki/
--rw-r--r--   0 naveen     (501) staff       (20)      220 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tiddlywiki/tiddlywiki.css
--rw-r--r--   0 naveen     (501) staff       (20)     9467 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tiddlywiki/tiddlywiki.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.694356 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tiki/
--rw-r--r--   0 naveen     (501) staff       (20)      439 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tiki/tiki.css
--rw-r--r--   0 naveen     (501) staff       (20)     8490 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tiki/tiki.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.694496 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/toml/
--rw-r--r--   0 naveen     (501) staff       (20)     2897 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/toml/toml.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.694655 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tornado/
--rw-r--r--   0 naveen     (501) staff       (20)     2496 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tornado/tornado.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.694797 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/troff/
--rw-r--r--   0 naveen     (501) staff       (20)     2392 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/troff/troff.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.694944 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn/
--rw-r--r--   0 naveen     (501) staff       (20)    10155 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn/ttcn.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.695092 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn-cfg/
--rw-r--r--   0 naveen     (501) staff       (20)     7857 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn-cfg/ttcn-cfg.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.695229 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/turtle/
--rw-r--r--   0 naveen     (501) staff       (20)     4849 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/turtle/turtle.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.695377 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/twig/
--rw-r--r--   0 naveen     (501) staff       (20)     4570 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/twig/twig.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.695537 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vb/
--rw-r--r--   0 naveen     (501) staff       (20)     8774 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vb/vb.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.695685 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vbscript/
--rw-r--r--   0 naveen     (501) staff       (20)    13793 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vbscript/vbscript.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.695828 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/velocity/
--rw-r--r--   0 naveen     (501) staff       (20)     7098 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/velocity/velocity.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.696043 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/verilog/
--rw-r--r--   0 naveen     (501) staff       (20)    19212 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/verilog/verilog.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.696282 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vhdl/
--rw-r--r--   0 naveen     (501) staff       (20)     6704 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vhdl/vhdl.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.696476 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vue/
--rw-r--r--   0 naveen     (501) staff       (20)     2507 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vue/vue.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.696703 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/xml/
--rw-r--r--   0 naveen     (501) staff       (20)    12570 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/xml/xml.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.696932 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/xquery/
--rw-r--r--   0 naveen     (501) staff       (20)    14470 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/xquery/xquery.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.697125 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml/
--rw-r--r--   0 naveen     (501) staff       (20)     3649 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml/yaml.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.697338 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml-frontmatter/
--rw-r--r--   0 naveen     (501) staff       (20)     2292 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.697521 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/z80/
--rw-r--r--   0 naveen     (501) staff       (20)     3577 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/z80/z80.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.709438 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/
--rw-r--r--   0 naveen     (501) staff       (20)     1987 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/3024-day.css
--rw-r--r--   0 naveen     (501) staff       (20)     2076 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/3024-night.css
--rw-r--r--   0 naveen     (501) staff       (20)     1942 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/abcdef.css
--rw-r--r--   0 naveen     (501) staff       (20)      103 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/ambiance-mobile.css
--rw-r--r--   0 naveen     (501) staff       (20)    26468 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/ambiance.css
--rw-r--r--   0 naveen     (501) staff       (20)     2112 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/base16-dark.css
--rw-r--r--   0 naveen     (501) staff       (20)     2114 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/base16-light.css
--rw-r--r--   0 naveen     (501) staff       (20)     1413 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/bespin.css
--rw-r--r--   0 naveen     (501) staff       (20)     1931 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/blackboard.css
--rw-r--r--   0 naveen     (501) staff       (20)     1703 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/cobalt.css
--rw-r--r--   0 naveen     (501) staff       (20)     1647 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/colorforth.css
--rw-r--r--   0 naveen     (501) staff       (20)     2086 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/dracula.css
--rw-r--r--   0 naveen     (501) staff       (20)     1159 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/eclipse.css
--rw-r--r--   0 naveen     (501) staff       (20)      781 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/elegant.css
--rw-r--r--   0 naveen     (501) staff       (20)     2254 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/erlang-dark.css
--rw-r--r--   0 naveen     (501) staff       (20)     1469 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/hopscotch.css
--rw-r--r--   0 naveen     (501) staff       (20)     2494 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/icecoder.css
--rw-r--r--   0 naveen     (501) staff       (20)     1442 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/isotope.css
--rw-r--r--   0 naveen     (501) staff       (20)     2599 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/lesser-dark.css
--rw-r--r--   0 naveen     (501) staff       (20)     3930 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/liquibyte.css
--rw-r--r--   0 naveen     (501) staff       (20)     2430 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/material.css
--rw-r--r--   0 naveen     (501) staff       (20)     2112 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/mbo.css
--rw-r--r--   0 naveen     (501) staff       (20)     5167 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/mdn-like.css
--rw-r--r--   0 naveen     (501) staff       (20)     2138 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/midnight.css
--rw-r--r--   0 naveen     (501) staff       (20)     1915 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/monokai.css
--rw-r--r--   0 naveen     (501) staff       (20)      688 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/neat.css
--rw-r--r--   0 naveen     (501) staff       (20)      947 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/neo.css
--rw-r--r--   0 naveen     (501) staff       (20)     1720 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/night.css
--rw-r--r--   0 naveen     (501) staff       (20)     2078 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/paraiso-dark.css
--rw-r--r--   0 naveen     (501) staff       (20)     2078 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/paraiso-light.css
--rw-r--r--   0 naveen     (501) staff       (20)     2468 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/pastel-on-dark.css
--rw-r--r--   0 naveen     (501) staff       (20)     1514 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/railscasts.css
--rw-r--r--   0 naveen     (501) staff       (20)     1772 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/rubyblue.css
--rw-r--r--   0 naveen     (501) staff       (20)     1984 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/seti.css
--rw-r--r--   0 naveen     (501) staff       (20)     5158 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/solarized.css
--rw-r--r--   0 naveen     (501) staff       (20)     1909 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/the-matrix.css
--rw-r--r--   0 naveen     (501) staff       (20)     1769 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/tomorrow-night-bright.css
--rw-r--r--   0 naveen     (501) staff       (20)     2439 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/tomorrow-night-eighties.css
--rw-r--r--   0 naveen     (501) staff       (20)     2419 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/ttcn.css
--rw-r--r--   0 naveen     (501) staff       (20)     2135 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/twilight.css
--rw-r--r--   0 naveen     (501) staff       (20)     2111 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/vibrant-ink.css
--rw-r--r--   0 naveen     (501) staff       (20)     3005 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/xq-dark.css
--rw-r--r--   0 naveen     (501) staff       (20)     2226 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/xq-light.css
--rw-r--r--   0 naveen     (501) staff       (20)     1859 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/yeti.css
--rw-r--r--   0 naveen     (501) staff       (20)     1990 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/zenburn.css
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.710632 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/
--rw-r--r--   0 naveen     (501) staff       (20)      759 2022-11-04 12:33:27.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/.bower.json
--rw-r--r--   0 naveen     (501) staff       (20)       50 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/.gitignore
--rw-r--r--   0 naveen     (501) staff       (20)       46 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/.npmignore
--rw-r--r--   0 naveen     (501) staff       (20)     1021 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/README.md
--rw-r--r--   0 naveen     (501) staff       (20)      399 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/bower.json
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.712155 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/css/
--rw-r--r--   0 naveen     (501) staff       (20)    37414 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.css
--rw-r--r--   0 naveen     (501) staff       (20)    21778 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.css.map
--rw-r--r--   0 naveen     (501) staff       (20)    31000 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.min.css
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.716946 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/
--rw-r--r--   0 naveen     (501) staff       (20)   134808 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0 naveen     (501) staff       (20)   165742 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0 naveen     (501) staff       (20)   444379 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0 naveen     (501) staff       (20)   165548 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 naveen     (501) staff       (20)    98024 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0 naveen     (501) staff       (20)    77160 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.720814 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/
--rw-r--r--   0 naveen     (501) staff       (20)      713 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/animated.less
--rw-r--r--   0 naveen     (501) staff       (20)      585 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/bordered-pulled.less
--rw-r--r--   0 naveen     (501) staff       (20)      452 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/core.less
--rw-r--r--   0 naveen     (501) staff       (20)      119 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/fixed-width.less
--rw-r--r--   0 naveen     (501) staff       (20)      495 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/font-awesome.less
--rw-r--r--   0 naveen     (501) staff       (20)    49712 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/icons.less
--rw-r--r--   0 naveen     (501) staff       (20)      370 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/larger.less
--rw-r--r--   0 naveen     (501) staff       (20)      377 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/list.less
--rw-r--r--   0 naveen     (501) staff       (20)     1603 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/mixins.less
--rw-r--r--   0 naveen     (501) staff       (20)      771 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/path.less
--rw-r--r--   0 naveen     (501) staff       (20)      622 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/rotated-flipped.less
--rw-r--r--   0 naveen     (501) staff       (20)      118 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/screen-reader.less
--rw-r--r--   0 naveen     (501) staff       (20)      476 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/stacked.less
--rw-r--r--   0 naveen     (501) staff       (20)    22563 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/variables.less
--rw-r--r--   0 naveen     (501) staff       (20)      332 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/package.json
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.725061 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/
--rw-r--r--   0 naveen     (501) staff       (20)      715 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_animated.scss
--rw-r--r--   0 naveen     (501) staff       (20)      592 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_bordered-pulled.scss
--rw-r--r--   0 naveen     (501) staff       (20)      459 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_core.scss
--rw-r--r--   0 naveen     (501) staff       (20)      120 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_fixed-width.scss
--rw-r--r--   0 naveen     (501) staff       (20)    50498 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_icons.scss
--rw-r--r--   0 naveen     (501) staff       (20)      375 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_larger.scss
--rw-r--r--   0 naveen     (501) staff       (20)      378 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_list.scss
--rw-r--r--   0 naveen     (501) staff       (20)     1637 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_mixins.scss
--rw-r--r--   0 naveen     (501) staff       (20)      783 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_path.scss
--rw-r--r--   0 naveen     (501) staff       (20)      672 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_rotated-flipped.scss
--rw-r--r--   0 naveen     (501) staff       (20)      134 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_screen-reader.scss
--rw-r--r--   0 naveen     (501) staff       (20)      482 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_stacked.scss
--rw-r--r--   0 naveen     (501) staff       (20)    22644 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_variables.scss
--rw-r--r--   0 naveen     (501) staff       (20)      430 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/font-awesome.scss
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.730347 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/
--rw-r--r--   0 naveen     (501) staff       (20)      404 2022-11-04 12:33:27.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/.bower.json
--rw-r--r--   0 naveen     (501) staff       (20)       26 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/.gitattributes
--rw-r--r--   0 naveen     (501) staff       (20)       98 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/.gitignore
--rw-r--r--   0 naveen     (501) staff       (20)      171 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/.gitmodules
--rw-r--r--   0 naveen     (501) staff       (20)    15099 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/GPL-LICENSE.txt
--rw-r--r--   0 naveen     (501) staff       (20)     1074 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/MIT-LICENSE.txt
--rw-r--r--   0 naveen     (501) staff       (20)     3558 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/Makefile
--rw-r--r--   0 naveen     (501) staff       (20)     6703 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/README.md
--rwxr-xr-x   0 naveen     (501) staff       (20)      117 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/bower.json
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.733029 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/
--rw-r--r--   0 naveen     (501) staff       (20)     1244 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/freq.js
--rw-r--r--   0 naveen     (501) staff       (20)      793 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/jshint-check.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.734551 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/lib/
--rw-r--r--   0 naveen     (501) staff       (20)   157207 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/lib/jshint.js
--rw-r--r--   0 naveen     (501) staff       (20)    52471 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/lib/parse-js.js
--rw-r--r--   0 naveen     (501) staff       (20)    73284 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/lib/process.js
--rw-r--r--   0 naveen     (501) staff       (20)      742 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/lib/squeeze-more.js
--rw-r--r--   0 naveen     (501) staff       (20)      651 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/post-compile.js
--rw-r--r--   0 naveen     (501) staff       (20)     1211 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/release-notes.js
--rw-r--r--   0 naveen     (501) staff       (20)     1303 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/release-notes.txt
--rw-r--r--   0 naveen     (501) staff       (20)     3950 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/release.js
--rw-r--r--   0 naveen     (501) staff       (20)      939 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/sizer.js
--rw-r--r--   0 naveen     (501) staff       (20)    10404 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/uglify.js
--rwxr-xr-x   0 naveen     (501) staff       (20)   252881 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/jquery.js
--rwxr-xr-x   0 naveen     (501) staff       (20)    94840 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/jquery.min.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.737401 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/
--rw-r--r--   0 naveen     (501) staff       (20)      452 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/benchmark.js
--rw-r--r--   0 naveen     (501) staff       (20)      864 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/benchmarker.css
--rw-r--r--   0 naveen     (501) staff       (20)     7154 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/benchmarker.js
--rw-r--r--   0 naveen     (501) staff       (20)     1044 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/closest.html
--rw-r--r--   0 naveen     (501) staff       (20)     1860 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/css.html
--rw-r--r--   0 naveen     (501) staff       (20)     1233 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/event.html
--rw-r--r--   0 naveen     (501) staff       (20)    10446 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/filter.html
--rw-r--r--   0 naveen     (501) staff       (20)    10151 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/find.html
--rw-r--r--   0 naveen     (501) staff       (20)    18353 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/index.html
--rw-r--r--   0 naveen     (501) staff       (20)   163854 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/jquery-basis.js
--rw-r--r--   0 naveen     (501) staff       (20)      868 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/slice.vs.concat.html
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.742209 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.742812 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/ajax/
--rw-r--r--   0 naveen     (501) staff       (20)     2022 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/ajax/jsonp.js
--rw-r--r--   0 naveen     (501) staff       (20)     1948 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/ajax/script.js
--rw-r--r--   0 naveen     (501) staff       (20)     6373 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/ajax/xhr.js
--rw-r--r--   0 naveen     (501) staff       (20)    27147 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/ajax.js
--rw-r--r--   0 naveen     (501) staff       (20)    17303 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/attributes.js
--rw-r--r--   0 naveen     (501) staff       (20)     5910 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/callbacks.js
--rw-r--r--   0 naveen     (501) staff       (20)    24388 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/core.js
--rw-r--r--   0 naveen     (501) staff       (20)    11687 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/css.js
--rw-r--r--   0 naveen     (501) staff       (20)     9574 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/data.js
--rw-r--r--   0 naveen     (501) staff       (20)     3905 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/deferred.js
--rw-r--r--   0 naveen     (501) staff       (20)     2201 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/dimensions.js
--rw-r--r--   0 naveen     (501) staff       (20)    18660 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/effects.js
--rw-r--r--   0 naveen     (501) staff       (20)    32354 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/event.js
--rw-r--r--   0 naveen     (501) staff       (20)     1072 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/exports.js
--rw-r--r--   0 naveen     (501) staff       (20)      542 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/intro.js
--rw-r--r--   0 naveen     (501) staff       (20)    23697 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/manipulation.js
--rw-r--r--   0 naveen     (501) staff       (20)     7055 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/offset.js
--rw-r--r--   0 naveen     (501) staff       (20)       15 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/outro.js
--rw-r--r--   0 naveen     (501) staff       (20)     4468 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/queue.js
--rw-r--r--   0 naveen     (501) staff       (20)      323 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/sizzle-jquery.js
--rw-r--r--   0 naveen     (501) staff       (20)    10423 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/support.js
--rw-r--r--   0 naveen     (501) staff       (20)     8085 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/traversing.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.744709 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/
--rw-r--r--   0 naveen     (501) staff       (20)      299 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/csp.php
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.751896 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/
--rw-r--r--   0 naveen     (501) staff       (20)      693 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/1x1.jpg
--rw-r--r--   0 naveen     (501) staff       (20)       69 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/atom+xml.php
--rw-r--r--   0 naveen     (501) staff       (20)        9 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/badjson.js
--rw-r--r--   0 naveen     (501) staff       (20)      298 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/dashboard.xml
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.752258 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/dimensions/
--rw-r--r--   0 naveen     (501) staff       (20)      446 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/dimensions/documentLarge.html
--rw-r--r--   0 naveen     (501) staff       (20)      377 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/dimensions/documentSmall.html
--rw-r--r--   0 naveen     (501) staff       (20)       48 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/echoData.php
--rw-r--r--   0 naveen     (501) staff       (20)       39 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/echoQuery.php
--rw-r--r--   0 naveen     (501) staff       (20)       70 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/errorWithText.php
--rw-r--r--   0 naveen     (501) staff       (20)      379 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/etag.php
--rw-r--r--   0 naveen     (501) staff       (20)      121 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/evalScript.php
--rw-r--r--   0 naveen     (501) staff       (20)      424 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/headers.php
--rw-r--r--   0 naveen     (501) staff       (20)      384 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/if_modified_since.php
--rw-r--r--   0 naveen     (501) staff       (20)      117 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/iframe.html
--rw-r--r--   0 naveen     (501) staff       (20)     2418 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/include_js.php
--rw-r--r--   0 naveen     (501) staff       (20)      276 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/json.php
--rw-r--r--   0 naveen     (501) staff       (20)       41 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/json_obj.js
--rw-r--r--   0 naveen     (501) staff       (20)      383 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/jsonp.php
--rw-r--r--   0 naveen     (501) staff       (20)       81 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/name.html
--rw-r--r--   0 naveen     (501) staff       (20)      493 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/name.php
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.753618 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/
--rw-r--r--   0 naveen     (501) staff       (20)     1772 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/absolute.html
--rw-r--r--   0 naveen     (501) staff       (20)      725 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/body.html
--rw-r--r--   0 naveen     (501) staff       (20)     1273 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/fixed.html
--rw-r--r--   0 naveen     (501) staff       (20)     1450 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/relative.html
--rw-r--r--   0 naveen     (501) staff       (20)     1411 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/scroll.html
--rw-r--r--   0 naveen     (501) staff       (20)     1424 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/static.html
--rw-r--r--   0 naveen     (501) staff       (20)     1233 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/table.html
--rw-r--r--   0 naveen     (501) staff       (20)      199 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/params_html.php
--rw-r--r--   0 naveen     (501) staff       (20)       35 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/readywaitasset.js
--rw-r--r--   0 naveen     (501) staff       (20)      722 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/readywaitloader.js
--rw-r--r--   0 naveen     (501) staff       (20)      248 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/script.php
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.754412 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/selector/
--rw-r--r--   0 naveen     (501) staff       (20)     1997 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/selector/html5_selector.html
--rw-r--r--   0 naveen     (501) staff       (20)      405 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/selector/sizzle_cache.html
--rw-r--r--   0 naveen     (501) staff       (20)       58 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/statusText.php
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.755241 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/support/
--rw-r--r--   0 naveen     (501) staff       (20)      671 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/support/bodyBackground.html
--rw-r--r--   0 naveen     (501) staff       (20)      300 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/support/boxModelIE.html
--rw-r--r--   0 naveen     (501) staff       (20)       93 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/support/hiddenIFrameFF.html
--rw-r--r--   0 naveen     (501) staff       (20)      501 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/support/testElementCrash.html
--rw-r--r--   0 naveen     (501) staff       (20)      204 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/test.html
--rw-r--r--   0 naveen     (501) staff       (20)       78 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/test.js
--rw-r--r--   0 naveen     (501) staff       (20)      247 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/test.php
--rw-r--r--   0 naveen     (501) staff       (20)      126 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/test2.html
--rw-r--r--   0 naveen     (501) staff       (20)      123 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/test3.html
--rw-r--r--   0 naveen     (501) staff       (20)     4466 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/testinit.js
--rw-r--r--   0 naveen     (501) staff       (20)      770 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/testrunner.js
--rw-r--r--   0 naveen     (501) staff       (20)     2720 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/testsuite.css
--rw-r--r--   0 naveen     (501) staff       (20)      287 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/text.php
--rw-r--r--   0 naveen     (501) staff       (20)    26351 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/ua.txt
--rw-r--r--   0 naveen     (501) staff       (20)      752 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/with_fries.xml
--rw-r--r--   0 naveen     (501) staff       (20)      193 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/with_fries_over_jsonp.php
--rw-r--r--   0 naveen     (501) staff       (20)     6535 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/delegatetest.html
--rw-r--r--   0 naveen     (501) staff       (20)     4073 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/hovertest.html
--rw-r--r--   0 naveen     (501) staff       (20)    12033 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/index.html
--rw-r--r--   0 naveen     (501) staff       (20)     1921 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/localfile.html
--rw-r--r--   0 naveen     (501) staff       (20)     1559 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/networkerror.html
--rw-r--r--   0 naveen     (501) staff       (20)     3100 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/polluted.php
--rw-r--r--   0 naveen     (501) staff       (20)     1803 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/readywait.html
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.759975 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/
--rw-r--r--   0 naveen     (501) staff       (20)    62936 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/ajax.js
--rw-r--r--   0 naveen     (501) staff       (20)    49839 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/attributes.js
--rw-r--r--   0 naveen     (501) staff       (20)     5218 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/callbacks.js
--rw-r--r--   0 naveen     (501) staff       (20)    45867 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/core.js
--rw-r--r--   0 naveen     (501) staff       (20)    21865 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/css.js
--rw-r--r--   0 naveen     (501) staff       (20)    22654 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/data.js
--rw-r--r--   0 naveen     (501) staff       (20)     9508 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/deferred.js
--rw-r--r--   0 naveen     (501) staff       (20)    11912 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/dimensions.js
--rw-r--r--   0 naveen     (501) staff       (20)    40568 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/effects.js
--rw-r--r--   0 naveen     (501) staff       (20)    83593 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/event.js
--rw-r--r--   0 naveen     (501) staff       (20)      171 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/exports.js
--rw-r--r--   0 naveen     (501) staff       (20)    66339 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/manipulation.js
--rw-r--r--   0 naveen     (501) staff       (20)    18807 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/offset.js
--rw-r--r--   0 naveen     (501) staff       (20)     6499 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/queue.js
--rw-r--r--   0 naveen     (501) staff       (20)     4954 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/selector.js
--rw-r--r--   0 naveen     (501) staff       (20)     9237 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/support.js
--rw-r--r--   0 naveen     (501) staff       (20)    35683 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/traversing.js
--rw-r--r--   0 naveen     (501) staff       (20)      136 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/xhtml.php
--rw-r--r--   0 naveen     (501) staff       (20)        5 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/version.txt
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.762120 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/
--rw-r--r--   0 naveen     (501) staff       (20)     1016 2022-11-04 12:33:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/.bower.json
--rw-r--r--   0 naveen     (501) staff       (20)      855 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/README.md
--rw-r--r--   0 naveen     (501) staff       (20)      702 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/bower.json
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.762310 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/demo/
--rw-r--r--   0 naveen     (501) staff       (20)      618 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/demo/index.html
--rw-r--r--   0 naveen     (501) staff       (20)     1138 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/index.html
--rw-r--r--   0 naveen     (501) staff       (20)      543 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/markdown-delight-editor-import.html
--rw-r--r--   0 naveen     (501) staff       (20)    26813 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/markdown-delight-editor.html
--rw-r--r--   0 naveen     (501) staff       (20)      115 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/spell-checker.css
--rw-r--r--   0 naveen     (501) staff       (20)     1556 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/spell-checker.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.762512 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/static/
--rw-r--r--   0 naveen     (501) staff       (20)    33467 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/static/markdown.png
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.764358 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/
--rw-r--r--   0 naveen     (501) staff       (20)     1080 2022-11-04 12:33:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/.bower.json
--rw-r--r--   0 naveen     (501) staff       (20)     1562 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/LICENSE.txt
--rw-r--r--   0 naveen     (501) staff       (20)      761 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/bower.json
--rw-r--r--   0 naveen     (501) staff       (20)    12024 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/build.log
--rw-r--r--   0 naveen     (501) staff       (20)    20816 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/polymer-micro.html
--rw-r--r--   0 naveen     (501) staff       (20)    57290 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/polymer-mini.html
--rw-r--r--   0 naveen     (501) staff       (20)   146591 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/polymer.html
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.766717 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/
--rw-r--r--   0 naveen     (501) staff       (20)     1043 2022-11-04 12:33:27.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/.bower.json
--rw-r--r--   0 naveen     (501) staff       (20)    40179 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/CHANGELOG.md
--rw-r--r--   0 naveen     (501) staff       (20)     2745 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/CONTRIBUTING.md
--rw-r--r--   0 naveen     (501) staff       (20)     1864 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/CREDITS.md
--rw-r--r--   0 naveen     (501) staff       (20)     1514 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/DONATIONS.md
--rw-r--r--   0 naveen     (501) staff       (20)    19471 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/README.md
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.767386 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/bin/
--rw-r--r--   0 naveen     (501) staff       (20)       47 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/bin/showdown.js
--rw-r--r--   0 naveen     (501) staff       (20)      812 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/bower.json
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.769404 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/dist/
--rw-r--r--   0 naveen     (501) staff       (20)   159368 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.js
--rw-r--r--   0 naveen     (501) staff       (20)   450443 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.js.map
--rw-r--r--   0 naveen     (501) staff       (20)    75674 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.min.js
--rw-r--r--   0 naveen     (501) staff       (20)    86982 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.min.js.map
--rw-r--r--   0 naveen     (501) staff       (20)     1613 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/license.txt
--rw-r--r--   0 naveen     (501) staff       (20)   173390 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/package-lock.json
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.771330 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.773193 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/cli/
--rw-r--r--   0 naveen     (501) staff       (20)      938 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/cli/cli.js
--rw-r--r--   0 naveen     (501) staff       (20)     5710 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/cli/makehtml.cmd.js
--rw-r--r--   0 naveen     (501) staff       (20)      802 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/cli/messenger.js
--rw-r--r--   0 naveen     (501) staff       (20)    15975 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/converter.js
--rw-r--r--   0 naveen     (501) staff       (20)    50830 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/helpers.js
--rw-r--r--   0 naveen     (501) staff       (20)      334 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/loader.js
--rw-r--r--   0 naveen     (501) staff       (20)     6073 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/options.js
--rw-r--r--   0 naveen     (501) staff       (20)     9659 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/showdown.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.782965 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/
--rw-r--r--   0 naveen     (501) staff       (20)     3632 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/anchors.js
--rw-r--r--   0 naveen     (501) staff       (20)     3075 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/autoLinks.js
--rw-r--r--   0 naveen     (501) staff       (20)     1299 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/blockGamut.js
--rw-r--r--   0 naveen     (501) staff       (20)     1486 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/blockQuotes.js
--rw-r--r--   0 naveen     (501) staff       (20)     1278 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/codeBlocks.js
--rw-r--r--   0 naveen     (501) staff       (20)     1498 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/codeSpans.js
--rw-r--r--   0 naveen     (501) staff       (20)     2044 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/completeHTMLDocument.js
--rw-r--r--   0 naveen     (501) staff       (20)      951 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/detab.js
--rw-r--r--   0 naveen     (501) staff       (20)      308 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/ellipsis.js
--rw-r--r--   0 naveen     (501) staff       (20)      654 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/emoji.js
--rw-r--r--   0 naveen     (501) staff       (20)      752 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeAmpsAndAngles.js
--rw-r--r--   0 naveen     (501) staff       (20)      914 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeBackslashEscapes.js
--rw-r--r--   0 naveen     (501) staff       (20)      814 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeCode.js
--rw-r--r--   0 naveen     (501) staff       (20)     1030 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/escapeSpecialCharsWithinTagAttributes.js
--rw-r--r--   0 naveen     (501) staff       (20)     1736 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/githubCodeBlocks.js
--rw-r--r--   0 naveen     (501) staff       (20)      378 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashBlock.js
--rw-r--r--   0 naveen     (501) staff       (20)      708 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashCodeTags.js
--rw-r--r--   0 naveen     (501) staff       (20)      542 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashElement.js
--rw-r--r--   0 naveen     (501) staff       (20)     3000 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashHTMLBlocks.js
--rw-r--r--   0 naveen     (501) staff       (20)     1901 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashHTMLSpans.js
--rw-r--r--   0 naveen     (501) staff       (20)      831 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashPreCodeTags.js
--rw-r--r--   0 naveen     (501) staff       (20)     4201 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/headers.js
--rw-r--r--   0 naveen     (501) staff       (20)      589 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/horizontalRule.js
--rw-r--r--   0 naveen     (501) staff       (20)     3896 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/images.js
--rw-r--r--   0 naveen     (501) staff       (20)     2908 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/italicsAndBold.js
--rw-r--r--   0 naveen     (501) staff       (20)     7633 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/lists.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.785998 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/
--rw-r--r--   0 naveen     (501) staff       (20)      531 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/blockquote.js
--rw-r--r--   0 naveen     (501) staff       (20)      246 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/codeBlock.js
--rw-r--r--   0 naveen     (501) staff       (20)      120 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/codeSpan.js
--rw-r--r--   0 naveen     (501) staff       (20)      395 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/emphasis.js
--rw-r--r--   0 naveen     (501) staff       (20)      461 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/header.js
--rw-r--r--   0 naveen     (501) staff       (20)       89 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/hr.js
--rw-r--r--   0 naveen     (501) staff       (20)      522 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/image.js
--rw-r--r--   0 naveen     (501) staff       (20)      585 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/links.js
--rw-r--r--   0 naveen     (501) staff       (20)      887 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/list.js
--rw-r--r--   0 naveen     (501) staff       (20)      670 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/listItem.js
--rw-r--r--   0 naveen     (501) staff       (20)     3186 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/node.js
--rw-r--r--   0 naveen     (501) staff       (20)      415 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/paragraph.js
--rw-r--r--   0 naveen     (501) staff       (20)      181 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/pre.js
--rw-r--r--   0 naveen     (501) staff       (20)      402 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/strikethrough.js
--rw-r--r--   0 naveen     (501) staff       (20)      395 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/strong.js
--rw-r--r--   0 naveen     (501) staff       (20)     2151 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/table.js
--rw-r--r--   0 naveen     (501) staff       (20)      384 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/tableCell.js
--rw-r--r--   0 naveen     (501) staff       (20)     1465 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/txt.js
--rw-r--r--   0 naveen     (501) staff       (20)     1329 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/metadata.js
--rw-r--r--   0 naveen     (501) staff       (20)      560 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/outdent.js
--rw-r--r--   0 naveen     (501) staff       (20)     2297 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/paragraphs.js
--rw-r--r--   0 naveen     (501) staff       (20)      460 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/runExtension.js
--rw-r--r--   0 naveen     (501) staff       (20)     2089 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/spanGamut.js
--rw-r--r--   0 naveen     (501) staff       (20)      619 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/strikethrough.js
--rw-r--r--   0 naveen     (501) staff       (20)     1909 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/stripLinkDefinitions.js
--rw-r--r--   0 naveen     (501) staff       (20)     4318 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/tables.js
--rw-r--r--   0 naveen     (501) staff       (20)     1020 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/underline.js
--rw-r--r--   0 naveen     (501) staff       (20)      529 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/unescapeSpecialChars.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.792201 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/
--rw-r--r--   0 naveen     (501) staff       (20)      719 2022-11-04 12:33:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/.bower.json
--rw-r--r--   0 naveen     (501) staff       (20)    33744 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/CustomElements.js
--rw-r--r--   0 naveen     (501) staff       (20)    16664 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/CustomElements.min.js
--rw-r--r--   0 naveen     (501) staff       (20)    38189 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/HTMLImports.js
--rw-r--r--   0 naveen     (501) staff       (20)    19924 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/HTMLImports.min.js
--rw-r--r--   0 naveen     (501) staff       (20)    12660 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/MutationObserver.js
--rw-r--r--   0 naveen     (501) staff       (20)     6000 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/MutationObserver.min.js
--rw-r--r--   0 naveen     (501) staff       (20)     9002 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/README.md
--rw-r--r--   0 naveen     (501) staff       (20)   159413 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/ShadowDOM.js
--rw-r--r--   0 naveen     (501) staff       (20)    72261 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/ShadowDOM.min.js
--rw-r--r--   0 naveen     (501) staff       (20)      423 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/bower.json
--rw-r--r--   0 naveen     (501) staff       (20)     9941 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/build.log
--rw-r--r--   0 naveen     (501) staff       (20)      737 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/package.json
--rw-r--r--   0 naveen     (501) staff       (20)    79576 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents-lite.js
--rw-r--r--   0 naveen     (501) staff       (20)    40547 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents-lite.min.js
--rw-r--r--   0 naveen     (501) staff       (20)   259853 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents.js
--rw-r--r--   0 naveen     (501) staff       (20)   118419 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents.min.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.793740 django-inapp-survey-0.2.5/inapp_survey/static/images/
--rw-r--r--   0 naveen     (501) staff       (20)      963 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/static/images/survey-finished.svg
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.793997 django-inapp-survey-0.2.5/inapp_survey/static/inapp_survey/
--rw-r--r--   0 naveen     (501) staff       (20)        0 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/static/inapp_survey/style.css
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.794367 django-inapp-survey-0.2.5/inapp_survey/static/javascript/
--rw-r--r--   0 naveen     (501) staff       (20)    13348 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/static/javascript/extended-markdown.js
--rw-r--r--   0 naveen     (501) staff       (20)    19328 2023-08-24 06:42:23.000000 django-inapp-survey-0.2.5/inapp_survey/static/javascript/script.js
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.794505 django-inapp-survey-0.2.5/inapp_survey/static/markdown-delight-editor-inapp/
--rw-r--r--   0 naveen     (501) staff       (20)     8020 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/static/markdown-delight-editor-inapp/markdown-delight-editor-extended.html
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.626537 django-inapp-survey-0.2.5/inapp_survey/templates/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.626442 django-inapp-survey-0.2.5/inapp_survey/templates/admin/
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.794682 django-inapp-survey-0.2.5/inapp_survey/templates/admin/inapp_survey/
--rw-r--r--   0 naveen     (501) staff       (20)      725 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/templates/admin/inapp_survey/change_form.html
-drwxr-xr-x   0 naveen     (501) staff       (20)        0 2023-08-24 07:35:28.794829 django-inapp-survey-0.2.5/inapp_survey/templates/inapp_survey/
--rw-r--r--   0 naveen     (501) staff       (20)     7867 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/templates/inapp_survey/index.html
--rw-r--r--   0 naveen     (501) staff       (20)       60 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.5/inapp_survey/tests.py
--rw-r--r--   0 naveen     (501) staff       (20)      928 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.5/inapp_survey/urls.py
--rw-r--r--   0 naveen     (501) staff       (20)      338 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.5/inapp_survey/views.py
--rw-r--r--   0 naveen     (501) staff       (20)       38 2023-08-24 07:35:28.795295 django-inapp-survey-0.2.5/setup.cfg
--rw-r--r--   0 naveen     (501) staff       (20)     1380 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.5/setup.py
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.860761 django-inapp-survey-0.2.6/
+-rw-r--r--   0 naveen     (501) staff       (20)    11357 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/LICENSE
+-rw-r--r--   0 naveen     (501) staff       (20)      155 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/MANIFEST.in
+-rw-r--r--   0 naveen     (501) staff       (20)     2110 2024-05-10 05:17:30.860538 django-inapp-survey-0.2.6/PKG-INFO
+-rw-r--r--   0 naveen     (501) staff       (20)     1256 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/README.md
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.643762 django-inapp-survey-0.2.6/django_inapp_survey.egg-info/
+-rw-r--r--   0 naveen     (501) staff       (20)     2110 2024-05-10 05:17:30.000000 django-inapp-survey-0.2.6/django_inapp_survey.egg-info/PKG-INFO
+-rw-r--r--   0 naveen     (501) staff       (20)    44442 2024-05-10 05:17:30.000000 django-inapp-survey-0.2.6/django_inapp_survey.egg-info/SOURCES.txt
+-rw-r--r--   0 naveen     (501) staff       (20)        1 2024-05-10 05:17:30.000000 django-inapp-survey-0.2.6/django_inapp_survey.egg-info/dependency_links.txt
+-rw-r--r--   0 naveen     (501) staff       (20)       50 2024-05-10 05:17:30.000000 django-inapp-survey-0.2.6/django_inapp_survey.egg-info/requires.txt
+-rw-r--r--   0 naveen     (501) staff       (20)       13 2024-05-10 05:17:30.000000 django-inapp-survey-0.2.6/django_inapp_survey.egg-info/top_level.txt
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.646140 django-inapp-survey-0.2.6/inapp_survey/
+-rw-r--r--   0 naveen     (501) staff       (20)       22 2024-05-10 03:50:35.000000 django-inapp-survey-0.2.6/inapp_survey/__init__.py
+-rw-r--r--   0 naveen     (501) staff       (20)     2935 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.6/inapp_survey/admin.py
+-rw-r--r--   0 naveen     (501) staff       (20)      196 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.6/inapp_survey/apps.py
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.646314 django-inapp-survey-0.2.6/inapp_survey/docs/
+-rw-r--r--   0 naveen     (501) staff       (20)       65 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/inapp_survey/docs/example.md
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.647359 django-inapp-survey-0.2.6/inapp_survey/migrations/
+-rw-r--r--   0 naveen     (501) staff       (20)     5640 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/inapp_survey/migrations/0001_initial.py
+-rw-r--r--   0 naveen     (501) staff       (20)     1863 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.6/inapp_survey/migrations/0002_auto_20210912_1311.py
+-rw-r--r--   0 naveen     (501) staff       (20)      767 2024-05-10 03:52:18.000000 django-inapp-survey-0.2.6/inapp_survey/migrations/0003_auto_20240510_0351.py
+-rw-r--r--   0 naveen     (501) staff       (20)        0 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/inapp_survey/migrations/__init__.py
+-rw-r--r--   0 naveen     (501) staff       (20)     3296 2024-05-10 03:33:40.000000 django-inapp-survey-0.2.6/inapp_survey/models.py
+-rw-r--r--   0 naveen     (501) staff       (20)     3584 2024-05-10 05:12:29.000000 django-inapp-survey-0.2.6/inapp_survey/resources.py
+-rw-r--r--   0 naveen     (501) staff       (20)     3152 2024-05-10 04:11:37.000000 django-inapp-survey-0.2.6/inapp_survey/serializers.py
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.641549 django-inapp-survey-0.2.6/inapp_survey/static/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.641118 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.648595 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/
+-rw-r--r--   0 naveen     (501) staff       (20)      333 2022-11-04 12:33:27.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/.bower.json
+-rwxr-xr-x   0 naveen     (501) staff       (20)     1711 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/README.md
+-rw-r--r--   0 naveen     (501) staff       (20)      160 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/SECURITY.md
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.625586 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/examples/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.648910 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/examples/node/
+-rw-r--r--   0 naveen     (501) staff       (20)      576 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/examples/node/index.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1449 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/license.txt
+-rw-r--r--   0 naveen     (501) staff       (20)      223 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/manifest.json
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.652855 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/
+-rw-r--r--   0 naveen     (501) staff       (20)      237 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/README.md
+-rw-r--r--   0 naveen     (501) staff       (20)      741 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/british.html
+-rw-r--r--   0 naveen     (501) staff       (20)      779 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/british.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.626051 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.654138 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/
+-rw-r--r--   0 naveen     (501) staff       (20)    18071 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/LICENSE
+-rw-r--r--   0 naveen     (501) staff       (20)    12799 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/de_DE.aff
+-rw-r--r--   0 naveen     (501) staff       (20)  1185467 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/de_DE.dic
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.656996 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/
+-rw-r--r--   0 naveen     (501) staff       (20)    15184 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/LICENSE
+-rw-r--r--   0 naveen     (501) staff       (20)    28123 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/en_GB.aff
+-rw-r--r--   0 naveen     (501) staff       (20)   706742 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/en_GB.dic
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.659515 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/fr_FR/
+-rw-r--r--   0 naveen     (501) staff       (20)   311776 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/fr_FR/fr_FR.aff
+-rw-r--r--   0 naveen     (501) staff       (20)   903141 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/fr_FR/fr_FR.dic
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.664041 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/
+-rwxr-xr-x   0 naveen     (501) staff       (20)    18957 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/README_la.txt
+-rwxr-xr-x   0 naveen     (501) staff       (20)   102451 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/la.aff
+-rwxr-xr-x   0 naveen     (501) staff       (20)   131575 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/la.dic
+-rw-r--r--   0 naveen     (501) staff       (20)      725 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/english.html
+-rw-r--r--   0 naveen     (501) staff       (20)     6772 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/english.js
+-rw-r--r--   0 naveen     (501) staff       (20)      718 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/french.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1992 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/french.js
+-rw-r--r--   0 naveen     (501) staff       (20)      725 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/general.html
+-rw-r--r--   0 naveen     (501) staff       (20)     2802 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/general.js
+-rw-r--r--   0 naveen     (501) staff       (20)      722 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/german.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1310 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/german.js
+-rw-r--r--   0 naveen     (501) staff       (20)      567 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/index.html
+-rw-r--r--   0 naveen     (501) staff       (20)      719 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/latin.html
+-rw-r--r--   0 naveen     (501) staff       (20)     2280 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/latin.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.665908 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/
+-rw-r--r--   0 naveen     (501) staff       (20)   268381 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/jquery-1.9.1.js
+-rw-r--r--   0 naveen     (501) staff       (20)     4525 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/qunit.css
+-rw-r--r--   0 naveen     (501) staff       (20)    50111 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/qunit.js
+-rw-r--r--   0 naveen     (501) staff       (20)       24 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/tests.css
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.667094 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/
+-rw-r--r--   0 naveen     (501) staff       (20)      910 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/README.md
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.626353 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.668261 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/
+-rw-r--r--   0 naveen     (501) staff       (20)      420 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/README.md
+-rw-r--r--   0 naveen     (501) staff       (20)     3045 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/en_US.aff
+-rw-r--r--   0 naveen     (501) staff       (20)   696131 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/en_US.dic
+-rw-r--r--   0 naveen     (501) staff       (20)      704 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/package.json
+-rw-r--r--   0 naveen     (501) staff       (20)    27334 2022-08-01 04:44:42.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/typo.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.671511 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/
+-rw-r--r--   0 naveen     (501) staff       (20)      639 2022-11-04 12:33:27.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/.bower.json
+-rw-r--r--   0 naveen     (501) staff       (20)     7279 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/AUTHORS
+-rw-r--r--   0 naveen     (501) staff       (20)    52656 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/CHANGELOG.md
+-rw-r--r--   0 naveen     (501) staff       (20)     3689 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/CONTRIBUTING.md
+-rw-r--r--   0 naveen     (501) staff       (20)     1094 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/LICENSE
+-rw-r--r--   0 naveen     (501) staff       (20)     1409 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/README.md
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.627727 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.672211 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/comment/
+-rw-r--r--   0 naveen     (501) staff       (20)     8446 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/comment/comment.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3399 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/comment/continuecomment.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.672738 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/dialog/
+-rw-r--r--   0 naveen     (501) staff       (20)      507 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/dialog/dialog.css
+-rw-r--r--   0 naveen     (501) staff       (20)     4938 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/dialog/dialog.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.674333 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/
+-rw-r--r--   0 naveen     (501) staff       (20)     1543 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/autorefresh.js
+-rw-r--r--   0 naveen     (501) staff       (20)      116 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/fullscreen.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1494 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/fullscreen.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3844 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/panel.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2139 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/placeholder.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2090 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/rulers.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.677736 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/
+-rw-r--r--   0 naveen     (501) staff       (20)     6945 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/closebrackets.js
+-rw-r--r--   0 naveen     (501) staff       (20)     7705 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/closetag.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1761 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/continuelist.js
+-rw-r--r--   0 naveen     (501) staff       (20)     5254 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/matchbrackets.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2355 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/matchtags.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1003 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/trailingspace.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.681186 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/
+-rw-r--r--   0 naveen     (501) staff       (20)     3904 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/brace-fold.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2147 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/comment-fold.js
+-rw-r--r--   0 naveen     (501) staff       (20)     4693 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/foldcode.js
+-rw-r--r--   0 naveen     (501) staff       (20)      435 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/foldgutter.css
+-rw-r--r--   0 naveen     (501) staff       (20)     4612 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/foldgutter.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1627 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/indent-fold.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1605 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/markdown-fold.js
+-rw-r--r--   0 naveen     (501) staff       (20)     6570 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/xml-fold.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.685180 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/
+-rw-r--r--   0 naveen     (501) staff       (20)     1680 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/anyword-hint.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2165 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/css-hint.js
+-rw-r--r--   0 naveen     (501) staff       (20)    11341 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/html-hint.js
+-rw-r--r--   0 naveen     (501) staff       (20)     6163 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/javascript-hint.js
+-rw-r--r--   0 naveen     (501) staff       (20)      662 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/show-hint.css
+-rw-r--r--   0 naveen     (501) staff       (20)    16422 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/show-hint.js
+-rw-r--r--   0 naveen     (501) staff       (20)     8578 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/sql-hint.js
+-rw-r--r--   0 naveen     (501) staff       (20)     4735 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/xml-hint.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.688858 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/
+-rw-r--r--   0 naveen     (501) staff       (20)     1270 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/coffeescript-lint.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1146 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/css-lint.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1513 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/html-lint.js
+-rw-r--r--   0 naveen     (501) staff       (20)     4469 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/javascript-lint.js
+-rw-r--r--   0 naveen     (501) staff       (20)      954 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/json-lint.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3012 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/lint.css
+-rw-r--r--   0 naveen     (501) staff       (20)     8032 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/lint.js
+-rw-r--r--   0 naveen     (501) staff       (20)      848 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/yaml-lint.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.689924 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/merge/
+-rw-r--r--   0 naveen     (501) staff       (20)     3249 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/merge/merge.css
+-rw-r--r--   0 naveen     (501) staff       (20)    28660 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/merge/merge.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.691843 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/
+-rw-r--r--   0 naveen     (501) staff       (20)     2277 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/loadmode.js
+-rw-r--r--   0 naveen     (501) staff       (20)     4624 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/multiplex.js
+-rw-r--r--   0 naveen     (501) staff       (20)      833 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/multiplex_test.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3021 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/overlay.js
+-rw-r--r--   0 naveen     (501) staff       (20)     7899 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/simple.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.693882 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/
+-rw-r--r--   0 naveen     (501) staff       (20)     1303 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/colorize.js
+-rw-r--r--   0 naveen     (501) staff       (20)     5302 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode-standalone.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2499 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode.js
+-rw-r--r--   0 naveen     (501) staff       (20)     6528 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode.node.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.696299 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/
+-rw-r--r--   0 naveen     (501) staff       (20)     4250 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/annotatescrollbar.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1492 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/scrollpastend.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1347 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/simplescrollbars.css
+-rw-r--r--   0 naveen     (501) staff       (20)     5297 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/simplescrollbars.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.699030 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/
+-rw-r--r--   0 naveen     (501) staff       (20)     1940 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/jump-to-line.js
+-rw-r--r--   0 naveen     (501) staff       (20)     5745 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/match-highlighter.js
+-rw-r--r--   0 naveen     (501) staff       (20)      188 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/matchesonscrollbar.css
+-rw-r--r--   0 naveen     (501) staff       (20)     3808 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/matchesonscrollbar.js
+-rw-r--r--   0 naveen     (501) staff       (20)     8957 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/search.js
+-rw-r--r--   0 naveen     (501) staff       (20)     7723 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/searchcursor.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.700358 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/
+-rw-r--r--   0 naveen     (501) staff       (20)     2624 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/active-line.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3781 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/mark-selection.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3292 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/selection-pointer.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.702864 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/
+-rw-r--r--   0 naveen     (501) staff       (20)     1872 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/tern.css
+-rw-r--r--   0 naveen     (501) staff       (20)    24561 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/tern.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1208 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/worker.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.703183 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/wrap/
+-rw-r--r--   0 naveen     (501) staff       (20)     5414 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/wrap/hardwrap.js
+-rw-r--r--   0 naveen     (501) staff       (20)      279 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/bower.json
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.704330 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/keymap/
+-rw-r--r--   0 naveen     (501) staff       (20)    13338 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/keymap/emacs.js
+-rw-r--r--   0 naveen     (501) staff       (20)    21589 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/keymap/sublime.js
+-rw-r--r--   0 naveen     (501) staff       (20)   197901 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/keymap/vim.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.707017 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/lib/
+-rw-r--r--   0 naveen     (501) staff       (20)     8137 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/lib/codemirror.css
+-rw-r--r--   0 naveen     (501) staff       (20)   353548 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/lib/codemirror.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.708951 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.709472 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/apl/
+-rw-r--r--   0 naveen     (501) staff       (20)     4736 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/apl/apl.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.709925 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/asciiarmor/
+-rw-r--r--   0 naveen     (501) staff       (20)     2378 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/asciiarmor/asciiarmor.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.710385 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/asn.1/
+-rw-r--r--   0 naveen     (501) staff       (20)     7735 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/asn.1/asn.1.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.710796 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/asterisk/
+-rw-r--r--   0 naveen     (501) staff       (20)     7437 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/asterisk/asterisk.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.711361 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/brainfuck/
+-rw-r--r--   0 naveen     (501) staff       (20)     2174 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/brainfuck/brainfuck.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.712255 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/clike/
+-rw-r--r--   0 naveen     (501) staff       (20)    30346 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/clike/clike.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.712688 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/clojure/
+-rw-r--r--   0 naveen     (501) staff       (20)    15189 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/clojure/clojure.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.713366 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/cmake/
+-rw-r--r--   0 naveen     (501) staff       (20)     2600 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/cmake/cmake.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.713567 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/cobol/
+-rw-r--r--   0 naveen     (501) staff       (20)    10288 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/cobol/cobol.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.713806 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/coffeescript/
+-rw-r--r--   0 naveen     (501) staff       (20)     9884 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/coffeescript/coffeescript.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.714398 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/commonlisp/
+-rw-r--r--   0 naveen     (501) staff       (20)     4488 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/commonlisp/commonlisp.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.715019 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/crystal/
+-rw-r--r--   0 naveen     (501) staff       (20)    11339 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/crystal/crystal.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.715251 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/css/
+-rw-r--r--   0 naveen     (501) staff       (20)    37156 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/css/css.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.715950 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/cypher/
+-rw-r--r--   0 naveen     (501) staff       (20)     6277 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/cypher/cypher.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.716266 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/d/
+-rw-r--r--   0 naveen     (501) staff       (20)     7566 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/d/d.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.716498 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dart/
+-rw-r--r--   0 naveen     (501) staff       (20)     5114 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dart/dart.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.716734 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/diff/
+-rw-r--r--   0 naveen     (501) staff       (20)     1138 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/diff/diff.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.717492 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/django/
+-rw-r--r--   0 naveen     (501) staff       (20)    11787 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/django/django.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.717954 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dockerfile/
+-rw-r--r--   0 naveen     (501) staff       (20)     2221 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dockerfile/dockerfile.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.718176 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dtd/
+-rw-r--r--   0 naveen     (501) staff       (20)     4808 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dtd/dtd.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.718669 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dylan/
+-rw-r--r--   0 naveen     (501) staff       (20)     9902 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dylan/dylan.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.718983 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ebnf/
+-rw-r--r--   0 naveen     (501) staff       (20)     6075 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ebnf/ebnf.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.719224 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ecl/
+-rw-r--r--   0 naveen     (501) staff       (20)     8843 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ecl/ecl.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.719450 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/eiffel/
+-rw-r--r--   0 naveen     (501) staff       (20)     3744 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/eiffel/eiffel.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.719660 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/elm/
+-rw-r--r--   0 naveen     (501) staff       (20)     5552 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/elm/elm.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.719894 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/erlang/
+-rw-r--r--   0 naveen     (501) staff       (20)    18853 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/erlang/erlang.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.720303 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/factor/
+-rw-r--r--   0 naveen     (501) staff       (20)     2919 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/factor/factor.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.721122 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/fcl/
+-rw-r--r--   0 naveen     (501) staff       (20)     4703 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/fcl/fcl.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.721736 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/forth/
+-rw-r--r--   0 naveen     (501) staff       (20)     5230 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/forth/forth.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.722173 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/fortran/
+-rw-r--r--   0 naveen     (501) staff       (20)     8686 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/fortran/fortran.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.722451 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/gas/
+-rw-r--r--   0 naveen     (501) staff       (20)     8886 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/gas/gas.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.722812 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/gfm/
+-rw-r--r--   0 naveen     (501) staff       (20)     5137 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/gfm/gfm.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.723255 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/gherkin/
+-rw-r--r--   0 naveen     (501) staff       (20)    13257 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/gherkin/gherkin.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.723685 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/go/
+-rw-r--r--   0 naveen     (501) staff       (20)     5938 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/go/go.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.723908 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/groovy/
+-rw-r--r--   0 naveen     (501) staff       (20)     7878 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/groovy/groovy.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.724129 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haml/
+-rw-r--r--   0 naveen     (501) staff       (20)     5332 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haml/haml.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.724587 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/handlebars/
+-rw-r--r--   0 naveen     (501) staff       (20)     2172 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/handlebars/handlebars.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.724948 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell/
+-rw-r--r--   0 naveen     (501) staff       (20)     8101 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell/haskell.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.725223 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell-literate/
+-rw-r--r--   0 naveen     (501) staff       (20)     1390 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell-literate/haskell-literate.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.725434 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haxe/
+-rw-r--r--   0 naveen     (501) staff       (20)    17568 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haxe/haxe.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.726093 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlembedded/
+-rw-r--r--   0 naveen     (501) staff       (20)     1417 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlembedded/htmlembedded.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.726964 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlmixed/
+-rw-r--r--   0 naveen     (501) staff       (20)     5555 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlmixed/htmlmixed.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.727324 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/http/
+-rw-r--r--   0 naveen     (501) staff       (20)     2795 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/http/http.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.727538 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/idl/
+-rw-r--r--   0 naveen     (501) staff       (20)    14889 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/idl/idl.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.728003 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/jade/
+-rw-r--r--   0 naveen     (501) staff       (20)    15972 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/jade/jade.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.728525 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/javascript/
+-rw-r--r--   0 naveen     (501) staff       (20)    28078 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/javascript/javascript.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.728852 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/jinja2/
+-rw-r--r--   0 naveen     (501) staff       (20)     4284 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/jinja2/jinja2.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.729080 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/jsx/
+-rw-r--r--   0 naveen     (501) staff       (20)     5087 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/jsx/jsx.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.729287 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/julia/
+-rw-r--r--   0 naveen     (501) staff       (20)    11430 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/julia/julia.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.729498 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/livescript/
+-rw-r--r--   0 naveen     (501) staff       (20)     7635 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/livescript/livescript.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.729710 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/lua/
+-rw-r--r--   0 naveen     (501) staff       (20)     5950 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/lua/lua.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.729947 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/markdown/
+-rw-r--r--   0 naveen     (501) staff       (20)    25301 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/markdown/markdown.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.730244 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mathematica/
+-rw-r--r--   0 naveen     (501) staff       (20)     5570 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mathematica/mathematica.js
+-rw-r--r--   0 naveen     (501) staff       (20)    14057 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/meta.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.730816 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mirc/
+-rw-r--r--   0 naveen     (501) staff       (20)    10082 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mirc/mirc.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.731057 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mllike/
+-rw-r--r--   0 naveen     (501) staff       (20)     5018 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mllike/mllike.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.731264 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/modelica/
+-rw-r--r--   0 naveen     (501) staff       (20)     6930 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/modelica/modelica.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.731496 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mscgen/
+-rw-r--r--   0 naveen     (501) staff       (20)     6523 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mscgen/mscgen.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.731717 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mumps/
+-rw-r--r--   0 naveen     (501) staff       (20)     5354 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mumps/mumps.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.732663 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/nginx/
+-rw-r--r--   0 naveen     (501) staff       (20)    10164 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/nginx/nginx.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.733561 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/nsis/
+-rw-r--r--   0 naveen     (501) staff       (20)     7632 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/nsis/nsis.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.733839 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ntriples/
+-rw-r--r--   0 naveen     (501) staff       (20)     6643 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ntriples/ntriples.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.734200 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/octave/
+-rw-r--r--   0 naveen     (501) staff       (20)     4463 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/octave/octave.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.734539 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/oz/
+-rw-r--r--   0 naveen     (501) staff       (20)     6658 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/oz/oz.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.735095 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/pascal/
+-rw-r--r--   0 naveen     (501) staff       (20)     3055 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/pascal/pascal.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.735317 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/pegjs/
+-rw-r--r--   0 naveen     (501) staff       (20)     3562 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/pegjs/pegjs.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.735661 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/perl/
+-rw-r--r--   0 naveen     (501) staff       (20)    56134 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/perl/perl.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.736032 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/php/
+-rw-r--r--   0 naveen     (501) staff       (20)    18177 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/php/php.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.736685 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/pig/
+-rw-r--r--   0 naveen     (501) staff       (20)     5810 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/pig/pig.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.737376 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/properties/
+-rw-r--r--   0 naveen     (501) staff       (20)     2169 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/properties/properties.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.737745 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/protobuf/
+-rw-r--r--   0 naveen     (501) staff       (20)     2113 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/protobuf/protobuf.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.737974 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/puppet/
+-rw-r--r--   0 naveen     (501) staff       (20)     7574 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/puppet/puppet.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.738692 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/python/
+-rw-r--r--   0 naveen     (501) staff       (20)    12627 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/python/python.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.739062 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/q/
+-rw-r--r--   0 naveen     (501) staff       (20)     6617 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/q/q.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.739302 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/r/
+-rw-r--r--   0 naveen     (501) staff       (20)     5677 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/r/r.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.739651 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/rpm/
+-rw-r--r--   0 naveen     (501) staff       (20)     3775 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/rpm/rpm.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.739904 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/rst/
+-rw-r--r--   0 naveen     (501) staff       (20)    17547 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/rst/rst.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.740674 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ruby/
+-rw-r--r--   0 naveen     (501) staff       (20)    10457 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ruby/ruby.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.740920 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/rust/
+-rw-r--r--   0 naveen     (501) staff       (20)     3025 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/rust/rust.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.741115 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sass/
+-rw-r--r--   0 naveen     (501) staff       (20)    10059 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sass/sass.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.741356 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/scheme/
+-rw-r--r--   0 naveen     (501) staff       (20)    13439 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/scheme/scheme.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.741708 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/shell/
+-rw-r--r--   0 naveen     (501) staff       (20)     3792 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/shell/shell.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.741905 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sieve/
+-rw-r--r--   0 naveen     (501) staff       (20)     4285 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sieve/sieve.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.742365 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/slim/
+-rw-r--r--   0 naveen     (501) staff       (20)    18008 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/slim/slim.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.742911 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/smalltalk/
+-rw-r--r--   0 naveen     (501) staff       (20)     4543 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/smalltalk/smalltalk.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.743178 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/smarty/
+-rw-r--r--   0 naveen     (501) staff       (20)     6828 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/smarty/smarty.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.743424 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/solr/
+-rw-r--r--   0 naveen     (501) staff       (20)     2678 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/solr/solr.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.743643 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/soy/
+-rw-r--r--   0 naveen     (501) staff       (20)     7564 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/soy/soy.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.743901 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sparql/
+-rw-r--r--   0 naveen     (501) staff       (20)     6327 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sparql/sparql.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.744149 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/spreadsheet/
+-rw-r--r--   0 naveen     (501) staff       (20)     3139 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/spreadsheet/spreadsheet.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.744352 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sql/
+-rw-r--r--   0 naveen     (501) staff       (20)    33831 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sql/sql.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.744641 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/stex/
+-rw-r--r--   0 naveen     (501) staff       (20)     6932 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/stex/stex.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.744943 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/stylus/
+-rw-r--r--   0 naveen     (501) staff       (20)    42120 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/stylus/stylus.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.745208 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/swift/
+-rw-r--r--   0 naveen     (501) staff       (20)     6424 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/swift/swift.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.745423 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tcl/
+-rw-r--r--   0 naveen     (501) staff       (20)     4920 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tcl/tcl.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.745682 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/textile/
+-rw-r--r--   0 naveen     (501) staff       (20)    13842 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/textile/textile.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.746528 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tiddlywiki/
+-rw-r--r--   0 naveen     (501) staff       (20)      220 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tiddlywiki/tiddlywiki.css
+-rw-r--r--   0 naveen     (501) staff       (20)     9467 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tiddlywiki/tiddlywiki.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.747091 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tiki/
+-rw-r--r--   0 naveen     (501) staff       (20)      439 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tiki/tiki.css
+-rw-r--r--   0 naveen     (501) staff       (20)     8490 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tiki/tiki.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.747368 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/toml/
+-rw-r--r--   0 naveen     (501) staff       (20)     2897 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/toml/toml.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.747648 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tornado/
+-rw-r--r--   0 naveen     (501) staff       (20)     2496 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tornado/tornado.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.747930 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/troff/
+-rw-r--r--   0 naveen     (501) staff       (20)     2392 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/troff/troff.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.748188 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn/
+-rw-r--r--   0 naveen     (501) staff       (20)    10155 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn/ttcn.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.748692 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn-cfg/
+-rw-r--r--   0 naveen     (501) staff       (20)     7857 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn-cfg/ttcn-cfg.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.748937 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/turtle/
+-rw-r--r--   0 naveen     (501) staff       (20)     4849 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/turtle/turtle.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.750562 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/twig/
+-rw-r--r--   0 naveen     (501) staff       (20)     4570 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/twig/twig.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.750857 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vb/
+-rw-r--r--   0 naveen     (501) staff       (20)     8774 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vb/vb.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.751344 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vbscript/
+-rw-r--r--   0 naveen     (501) staff       (20)    13793 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vbscript/vbscript.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.752801 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/velocity/
+-rw-r--r--   0 naveen     (501) staff       (20)     7098 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/velocity/velocity.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.753106 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/verilog/
+-rw-r--r--   0 naveen     (501) staff       (20)    19212 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/verilog/verilog.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.753427 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vhdl/
+-rw-r--r--   0 naveen     (501) staff       (20)     6704 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vhdl/vhdl.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.753651 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vue/
+-rw-r--r--   0 naveen     (501) staff       (20)     2507 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vue/vue.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.755435 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/xml/
+-rw-r--r--   0 naveen     (501) staff       (20)    12570 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/xml/xml.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.755921 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/xquery/
+-rw-r--r--   0 naveen     (501) staff       (20)    14470 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/xquery/xquery.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.756333 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml/
+-rw-r--r--   0 naveen     (501) staff       (20)     3649 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml/yaml.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.756553 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml-frontmatter/
+-rw-r--r--   0 naveen     (501) staff       (20)     2292 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.756782 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/z80/
+-rw-r--r--   0 naveen     (501) staff       (20)     3577 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/z80/z80.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.768082 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/
+-rw-r--r--   0 naveen     (501) staff       (20)     1987 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/3024-day.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2076 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/3024-night.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1942 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/abcdef.css
+-rw-r--r--   0 naveen     (501) staff       (20)      103 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/ambiance-mobile.css
+-rw-r--r--   0 naveen     (501) staff       (20)    26468 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/ambiance.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2112 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/base16-dark.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2114 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/base16-light.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1413 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/bespin.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1931 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/blackboard.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1703 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/cobalt.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1647 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/colorforth.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2086 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/dracula.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1159 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/eclipse.css
+-rw-r--r--   0 naveen     (501) staff       (20)      781 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/elegant.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2254 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/erlang-dark.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1469 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/hopscotch.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2494 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/icecoder.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1442 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/isotope.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2599 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/lesser-dark.css
+-rw-r--r--   0 naveen     (501) staff       (20)     3930 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/liquibyte.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2430 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/material.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2112 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/mbo.css
+-rw-r--r--   0 naveen     (501) staff       (20)     5167 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/mdn-like.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2138 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/midnight.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1915 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/monokai.css
+-rw-r--r--   0 naveen     (501) staff       (20)      688 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/neat.css
+-rw-r--r--   0 naveen     (501) staff       (20)      947 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/neo.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1720 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/night.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2078 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/paraiso-dark.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2078 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/paraiso-light.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2468 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/pastel-on-dark.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1514 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/railscasts.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1772 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/rubyblue.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1984 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/seti.css
+-rw-r--r--   0 naveen     (501) staff       (20)     5158 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/solarized.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1909 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/the-matrix.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1769 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/tomorrow-night-bright.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2439 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/tomorrow-night-eighties.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2419 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/ttcn.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2135 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/twilight.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2111 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/vibrant-ink.css
+-rw-r--r--   0 naveen     (501) staff       (20)     3005 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/xq-dark.css
+-rw-r--r--   0 naveen     (501) staff       (20)     2226 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/xq-light.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1859 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/yeti.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1990 2016-03-23 08:30:48.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/zenburn.css
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.769650 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/
+-rw-r--r--   0 naveen     (501) staff       (20)      759 2022-11-04 12:33:27.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/.bower.json
+-rw-r--r--   0 naveen     (501) staff       (20)       50 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/.gitignore
+-rw-r--r--   0 naveen     (501) staff       (20)       46 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/.npmignore
+-rw-r--r--   0 naveen     (501) staff       (20)     1021 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/README.md
+-rw-r--r--   0 naveen     (501) staff       (20)      399 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/bower.json
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.770984 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/css/
+-rw-r--r--   0 naveen     (501) staff       (20)    37414 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.css
+-rw-r--r--   0 naveen     (501) staff       (20)    21778 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.css.map
+-rw-r--r--   0 naveen     (501) staff       (20)    31000 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.min.css
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.777186 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/
+-rw-r--r--   0 naveen     (501) staff       (20)   134808 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0 naveen     (501) staff       (20)   165742 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 naveen     (501) staff       (20)   444379 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 naveen     (501) staff       (20)   165548 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 naveen     (501) staff       (20)    98024 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 naveen     (501) staff       (20)    77160 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.781332 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/
+-rw-r--r--   0 naveen     (501) staff       (20)      713 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/animated.less
+-rw-r--r--   0 naveen     (501) staff       (20)      585 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/bordered-pulled.less
+-rw-r--r--   0 naveen     (501) staff       (20)      452 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/core.less
+-rw-r--r--   0 naveen     (501) staff       (20)      119 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/fixed-width.less
+-rw-r--r--   0 naveen     (501) staff       (20)      495 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/font-awesome.less
+-rw-r--r--   0 naveen     (501) staff       (20)    49712 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/icons.less
+-rw-r--r--   0 naveen     (501) staff       (20)      370 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/larger.less
+-rw-r--r--   0 naveen     (501) staff       (20)      377 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/list.less
+-rw-r--r--   0 naveen     (501) staff       (20)     1603 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/mixins.less
+-rw-r--r--   0 naveen     (501) staff       (20)      771 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/path.less
+-rw-r--r--   0 naveen     (501) staff       (20)      622 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/rotated-flipped.less
+-rw-r--r--   0 naveen     (501) staff       (20)      118 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/screen-reader.less
+-rw-r--r--   0 naveen     (501) staff       (20)      476 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/stacked.less
+-rw-r--r--   0 naveen     (501) staff       (20)    22563 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/variables.less
+-rw-r--r--   0 naveen     (501) staff       (20)      332 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/package.json
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.785460 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/
+-rw-r--r--   0 naveen     (501) staff       (20)      715 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_animated.scss
+-rw-r--r--   0 naveen     (501) staff       (20)      592 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_bordered-pulled.scss
+-rw-r--r--   0 naveen     (501) staff       (20)      459 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_core.scss
+-rw-r--r--   0 naveen     (501) staff       (20)      120 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_fixed-width.scss
+-rw-r--r--   0 naveen     (501) staff       (20)    50498 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_icons.scss
+-rw-r--r--   0 naveen     (501) staff       (20)      375 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_larger.scss
+-rw-r--r--   0 naveen     (501) staff       (20)      378 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_list.scss
+-rw-r--r--   0 naveen     (501) staff       (20)     1637 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_mixins.scss
+-rw-r--r--   0 naveen     (501) staff       (20)      783 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_path.scss
+-rw-r--r--   0 naveen     (501) staff       (20)      672 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_rotated-flipped.scss
+-rw-r--r--   0 naveen     (501) staff       (20)      134 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_screen-reader.scss
+-rw-r--r--   0 naveen     (501) staff       (20)      482 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_stacked.scss
+-rw-r--r--   0 naveen     (501) staff       (20)    22644 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_variables.scss
+-rw-r--r--   0 naveen     (501) staff       (20)      430 2016-10-25 10:56:23.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/font-awesome.scss
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.790890 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/
+-rw-r--r--   0 naveen     (501) staff       (20)      404 2022-11-04 12:33:27.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/.bower.json
+-rw-r--r--   0 naveen     (501) staff       (20)       26 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/.gitattributes
+-rw-r--r--   0 naveen     (501) staff       (20)       98 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/.gitignore
+-rw-r--r--   0 naveen     (501) staff       (20)      171 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/.gitmodules
+-rw-r--r--   0 naveen     (501) staff       (20)    15099 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/GPL-LICENSE.txt
+-rw-r--r--   0 naveen     (501) staff       (20)     1074 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/MIT-LICENSE.txt
+-rw-r--r--   0 naveen     (501) staff       (20)     3558 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/Makefile
+-rw-r--r--   0 naveen     (501) staff       (20)     6703 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/README.md
+-rwxr-xr-x   0 naveen     (501) staff       (20)      117 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/bower.json
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.793272 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/
+-rw-r--r--   0 naveen     (501) staff       (20)     1244 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/freq.js
+-rw-r--r--   0 naveen     (501) staff       (20)      793 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/jshint-check.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.794870 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/lib/
+-rw-r--r--   0 naveen     (501) staff       (20)   157207 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/lib/jshint.js
+-rw-r--r--   0 naveen     (501) staff       (20)    52471 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/lib/parse-js.js
+-rw-r--r--   0 naveen     (501) staff       (20)    73284 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/lib/process.js
+-rw-r--r--   0 naveen     (501) staff       (20)      742 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/lib/squeeze-more.js
+-rw-r--r--   0 naveen     (501) staff       (20)      651 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/post-compile.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1211 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/release-notes.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1303 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/release-notes.txt
+-rw-r--r--   0 naveen     (501) staff       (20)     3950 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/release.js
+-rw-r--r--   0 naveen     (501) staff       (20)      939 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/sizer.js
+-rw-r--r--   0 naveen     (501) staff       (20)    10404 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/uglify.js
+-rwxr-xr-x   0 naveen     (501) staff       (20)   252881 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/jquery.js
+-rwxr-xr-x   0 naveen     (501) staff       (20)    94840 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/jquery.min.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.797803 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/
+-rw-r--r--   0 naveen     (501) staff       (20)      452 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/benchmark.js
+-rw-r--r--   0 naveen     (501) staff       (20)      864 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/benchmarker.css
+-rw-r--r--   0 naveen     (501) staff       (20)     7154 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/benchmarker.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1044 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/closest.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1860 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/css.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1233 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/event.html
+-rw-r--r--   0 naveen     (501) staff       (20)    10446 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/filter.html
+-rw-r--r--   0 naveen     (501) staff       (20)    10151 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/find.html
+-rw-r--r--   0 naveen     (501) staff       (20)    18353 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/index.html
+-rw-r--r--   0 naveen     (501) staff       (20)   163854 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/jquery-basis.js
+-rw-r--r--   0 naveen     (501) staff       (20)      868 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/slice.vs.concat.html
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.803330 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.804083 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/ajax/
+-rw-r--r--   0 naveen     (501) staff       (20)     2022 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/ajax/jsonp.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1948 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/ajax/script.js
+-rw-r--r--   0 naveen     (501) staff       (20)     6373 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/ajax/xhr.js
+-rw-r--r--   0 naveen     (501) staff       (20)    27147 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/ajax.js
+-rw-r--r--   0 naveen     (501) staff       (20)    17303 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/attributes.js
+-rw-r--r--   0 naveen     (501) staff       (20)     5910 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/callbacks.js
+-rw-r--r--   0 naveen     (501) staff       (20)    24388 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/core.js
+-rw-r--r--   0 naveen     (501) staff       (20)    11687 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/css.js
+-rw-r--r--   0 naveen     (501) staff       (20)     9574 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/data.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3905 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/deferred.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2201 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/dimensions.js
+-rw-r--r--   0 naveen     (501) staff       (20)    18660 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/effects.js
+-rw-r--r--   0 naveen     (501) staff       (20)    32354 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/event.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1072 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/exports.js
+-rw-r--r--   0 naveen     (501) staff       (20)      542 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/intro.js
+-rw-r--r--   0 naveen     (501) staff       (20)    23697 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/manipulation.js
+-rw-r--r--   0 naveen     (501) staff       (20)     7055 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/offset.js
+-rw-r--r--   0 naveen     (501) staff       (20)       15 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/outro.js
+-rw-r--r--   0 naveen     (501) staff       (20)     4468 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/queue.js
+-rw-r--r--   0 naveen     (501) staff       (20)      323 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/sizzle-jquery.js
+-rw-r--r--   0 naveen     (501) staff       (20)    10423 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/support.js
+-rw-r--r--   0 naveen     (501) staff       (20)     8085 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/traversing.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.806354 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/
+-rw-r--r--   0 naveen     (501) staff       (20)      299 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/csp.php
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.814241 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/
+-rw-r--r--   0 naveen     (501) staff       (20)      693 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/1x1.jpg
+-rw-r--r--   0 naveen     (501) staff       (20)       69 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/atom+xml.php
+-rw-r--r--   0 naveen     (501) staff       (20)        9 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/badjson.js
+-rw-r--r--   0 naveen     (501) staff       (20)      298 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/dashboard.xml
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.814636 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/dimensions/
+-rw-r--r--   0 naveen     (501) staff       (20)      446 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/dimensions/documentLarge.html
+-rw-r--r--   0 naveen     (501) staff       (20)      377 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/dimensions/documentSmall.html
+-rw-r--r--   0 naveen     (501) staff       (20)       48 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/echoData.php
+-rw-r--r--   0 naveen     (501) staff       (20)       39 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/echoQuery.php
+-rw-r--r--   0 naveen     (501) staff       (20)       70 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/errorWithText.php
+-rw-r--r--   0 naveen     (501) staff       (20)      379 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/etag.php
+-rw-r--r--   0 naveen     (501) staff       (20)      121 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/evalScript.php
+-rw-r--r--   0 naveen     (501) staff       (20)      424 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/headers.php
+-rw-r--r--   0 naveen     (501) staff       (20)      384 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/if_modified_since.php
+-rw-r--r--   0 naveen     (501) staff       (20)      117 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/iframe.html
+-rw-r--r--   0 naveen     (501) staff       (20)     2418 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/include_js.php
+-rw-r--r--   0 naveen     (501) staff       (20)      276 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/json.php
+-rw-r--r--   0 naveen     (501) staff       (20)       41 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/json_obj.js
+-rw-r--r--   0 naveen     (501) staff       (20)      383 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/jsonp.php
+-rw-r--r--   0 naveen     (501) staff       (20)       81 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/name.html
+-rw-r--r--   0 naveen     (501) staff       (20)      493 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/name.php
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.816023 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/
+-rw-r--r--   0 naveen     (501) staff       (20)     1772 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/absolute.html
+-rw-r--r--   0 naveen     (501) staff       (20)      725 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/body.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1273 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/fixed.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1450 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/relative.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1411 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/scroll.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1424 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/static.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1233 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/table.html
+-rw-r--r--   0 naveen     (501) staff       (20)      199 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/params_html.php
+-rw-r--r--   0 naveen     (501) staff       (20)       35 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/readywaitasset.js
+-rw-r--r--   0 naveen     (501) staff       (20)      722 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/readywaitloader.js
+-rw-r--r--   0 naveen     (501) staff       (20)      248 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/script.php
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.816414 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/selector/
+-rw-r--r--   0 naveen     (501) staff       (20)     1997 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/selector/html5_selector.html
+-rw-r--r--   0 naveen     (501) staff       (20)      405 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/selector/sizzle_cache.html
+-rw-r--r--   0 naveen     (501) staff       (20)       58 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/statusText.php
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.817311 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/support/
+-rw-r--r--   0 naveen     (501) staff       (20)      671 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/support/bodyBackground.html
+-rw-r--r--   0 naveen     (501) staff       (20)      300 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/support/boxModelIE.html
+-rw-r--r--   0 naveen     (501) staff       (20)       93 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/support/hiddenIFrameFF.html
+-rw-r--r--   0 naveen     (501) staff       (20)      501 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/support/testElementCrash.html
+-rw-r--r--   0 naveen     (501) staff       (20)      204 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/test.html
+-rw-r--r--   0 naveen     (501) staff       (20)       78 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/test.js
+-rw-r--r--   0 naveen     (501) staff       (20)      247 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/test.php
+-rw-r--r--   0 naveen     (501) staff       (20)      126 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/test2.html
+-rw-r--r--   0 naveen     (501) staff       (20)      123 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/test3.html
+-rw-r--r--   0 naveen     (501) staff       (20)     4466 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/testinit.js
+-rw-r--r--   0 naveen     (501) staff       (20)      770 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/testrunner.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2720 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/testsuite.css
+-rw-r--r--   0 naveen     (501) staff       (20)      287 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/text.php
+-rw-r--r--   0 naveen     (501) staff       (20)    26351 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/ua.txt
+-rw-r--r--   0 naveen     (501) staff       (20)      752 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/with_fries.xml
+-rw-r--r--   0 naveen     (501) staff       (20)      193 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/with_fries_over_jsonp.php
+-rw-r--r--   0 naveen     (501) staff       (20)     6535 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/delegatetest.html
+-rw-r--r--   0 naveen     (501) staff       (20)     4073 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/hovertest.html
+-rw-r--r--   0 naveen     (501) staff       (20)    12033 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/index.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1921 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/localfile.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1559 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/networkerror.html
+-rw-r--r--   0 naveen     (501) staff       (20)     3100 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/polluted.php
+-rw-r--r--   0 naveen     (501) staff       (20)     1803 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/readywait.html
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.823735 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/
+-rw-r--r--   0 naveen     (501) staff       (20)    62936 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/ajax.js
+-rw-r--r--   0 naveen     (501) staff       (20)    49839 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/attributes.js
+-rw-r--r--   0 naveen     (501) staff       (20)     5218 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/callbacks.js
+-rw-r--r--   0 naveen     (501) staff       (20)    45867 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/core.js
+-rw-r--r--   0 naveen     (501) staff       (20)    21865 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/css.js
+-rw-r--r--   0 naveen     (501) staff       (20)    22654 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/data.js
+-rw-r--r--   0 naveen     (501) staff       (20)     9508 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/deferred.js
+-rw-r--r--   0 naveen     (501) staff       (20)    11912 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/dimensions.js
+-rw-r--r--   0 naveen     (501) staff       (20)    40568 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/effects.js
+-rw-r--r--   0 naveen     (501) staff       (20)    83593 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/event.js
+-rw-r--r--   0 naveen     (501) staff       (20)      171 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/exports.js
+-rw-r--r--   0 naveen     (501) staff       (20)    66339 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/manipulation.js
+-rw-r--r--   0 naveen     (501) staff       (20)    18807 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/offset.js
+-rw-r--r--   0 naveen     (501) staff       (20)     6499 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/queue.js
+-rw-r--r--   0 naveen     (501) staff       (20)     4954 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/selector.js
+-rw-r--r--   0 naveen     (501) staff       (20)     9237 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/support.js
+-rw-r--r--   0 naveen     (501) staff       (20)    35683 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/traversing.js
+-rw-r--r--   0 naveen     (501) staff       (20)      136 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/xhtml.php
+-rw-r--r--   0 naveen     (501) staff       (20)        5 2012-03-21 19:46:34.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/version.txt
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.826105 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/
+-rw-r--r--   0 naveen     (501) staff       (20)     1016 2022-11-04 12:33:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/.bower.json
+-rw-r--r--   0 naveen     (501) staff       (20)      855 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/README.md
+-rw-r--r--   0 naveen     (501) staff       (20)      702 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/bower.json
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.826314 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/demo/
+-rw-r--r--   0 naveen     (501) staff       (20)      618 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/demo/index.html
+-rw-r--r--   0 naveen     (501) staff       (20)     1138 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/index.html
+-rw-r--r--   0 naveen     (501) staff       (20)      543 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/markdown-delight-editor-import.html
+-rw-r--r--   0 naveen     (501) staff       (20)    26813 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/markdown-delight-editor.html
+-rw-r--r--   0 naveen     (501) staff       (20)      115 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/spell-checker.css
+-rw-r--r--   0 naveen     (501) staff       (20)     1556 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/spell-checker.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.826496 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/static/
+-rw-r--r--   0 naveen     (501) staff       (20)    33467 2019-06-13 10:54:37.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/static/markdown.png
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.828576 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/
+-rw-r--r--   0 naveen     (501) staff       (20)     1080 2022-11-04 12:33:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/.bower.json
+-rw-r--r--   0 naveen     (501) staff       (20)     1562 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/LICENSE.txt
+-rw-r--r--   0 naveen     (501) staff       (20)      761 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/bower.json
+-rw-r--r--   0 naveen     (501) staff       (20)    12024 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/build.log
+-rw-r--r--   0 naveen     (501) staff       (20)    20816 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/polymer-micro.html
+-rw-r--r--   0 naveen     (501) staff       (20)    57290 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/polymer-mini.html
+-rw-r--r--   0 naveen     (501) staff       (20)   146591 2019-05-20 22:13:49.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/polymer.html
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.830620 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/
+-rw-r--r--   0 naveen     (501) staff       (20)     1043 2022-11-04 12:33:27.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/.bower.json
+-rw-r--r--   0 naveen     (501) staff       (20)    40179 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/CHANGELOG.md
+-rw-r--r--   0 naveen     (501) staff       (20)     2745 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/CONTRIBUTING.md
+-rw-r--r--   0 naveen     (501) staff       (20)     1864 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/CREDITS.md
+-rw-r--r--   0 naveen     (501) staff       (20)     1514 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/DONATIONS.md
+-rw-r--r--   0 naveen     (501) staff       (20)    19471 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/README.md
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.831328 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/bin/
+-rw-r--r--   0 naveen     (501) staff       (20)       47 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/bin/showdown.js
+-rw-r--r--   0 naveen     (501) staff       (20)      812 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/bower.json
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.833975 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/dist/
+-rw-r--r--   0 naveen     (501) staff       (20)   159368 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.js
+-rw-r--r--   0 naveen     (501) staff       (20)   450443 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.js.map
+-rw-r--r--   0 naveen     (501) staff       (20)    75674 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.min.js
+-rw-r--r--   0 naveen     (501) staff       (20)    86982 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.min.js.map
+-rw-r--r--   0 naveen     (501) staff       (20)     1613 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/license.txt
+-rw-r--r--   0 naveen     (501) staff       (20)   173390 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/package-lock.json
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.836628 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.837436 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/cli/
+-rw-r--r--   0 naveen     (501) staff       (20)      938 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/cli/cli.js
+-rw-r--r--   0 naveen     (501) staff       (20)     5710 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/cli/makehtml.cmd.js
+-rw-r--r--   0 naveen     (501) staff       (20)      802 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/cli/messenger.js
+-rw-r--r--   0 naveen     (501) staff       (20)    15975 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/converter.js
+-rw-r--r--   0 naveen     (501) staff       (20)    50830 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/helpers.js
+-rw-r--r--   0 naveen     (501) staff       (20)      334 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/loader.js
+-rw-r--r--   0 naveen     (501) staff       (20)     6073 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/options.js
+-rw-r--r--   0 naveen     (501) staff       (20)     9659 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/showdown.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.845567 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/
+-rw-r--r--   0 naveen     (501) staff       (20)     3632 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/anchors.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3075 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/autoLinks.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1299 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/blockGamut.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1486 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/blockQuotes.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1278 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/codeBlocks.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1498 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/codeSpans.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2044 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/completeHTMLDocument.js
+-rw-r--r--   0 naveen     (501) staff       (20)      951 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/detab.js
+-rw-r--r--   0 naveen     (501) staff       (20)      308 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/ellipsis.js
+-rw-r--r--   0 naveen     (501) staff       (20)      654 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/emoji.js
+-rw-r--r--   0 naveen     (501) staff       (20)      752 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeAmpsAndAngles.js
+-rw-r--r--   0 naveen     (501) staff       (20)      914 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeBackslashEscapes.js
+-rw-r--r--   0 naveen     (501) staff       (20)      814 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeCode.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1030 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/escapeSpecialCharsWithinTagAttributes.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1736 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/githubCodeBlocks.js
+-rw-r--r--   0 naveen     (501) staff       (20)      378 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashBlock.js
+-rw-r--r--   0 naveen     (501) staff       (20)      708 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashCodeTags.js
+-rw-r--r--   0 naveen     (501) staff       (20)      542 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashElement.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3000 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashHTMLBlocks.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1901 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashHTMLSpans.js
+-rw-r--r--   0 naveen     (501) staff       (20)      831 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashPreCodeTags.js
+-rw-r--r--   0 naveen     (501) staff       (20)     4201 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/headers.js
+-rw-r--r--   0 naveen     (501) staff       (20)      589 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/horizontalRule.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3896 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/images.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2908 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/italicsAndBold.js
+-rw-r--r--   0 naveen     (501) staff       (20)     7633 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/lists.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.849208 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/
+-rw-r--r--   0 naveen     (501) staff       (20)      531 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/blockquote.js
+-rw-r--r--   0 naveen     (501) staff       (20)      246 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/codeBlock.js
+-rw-r--r--   0 naveen     (501) staff       (20)      120 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/codeSpan.js
+-rw-r--r--   0 naveen     (501) staff       (20)      395 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/emphasis.js
+-rw-r--r--   0 naveen     (501) staff       (20)      461 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/header.js
+-rw-r--r--   0 naveen     (501) staff       (20)       89 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/hr.js
+-rw-r--r--   0 naveen     (501) staff       (20)      522 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/image.js
+-rw-r--r--   0 naveen     (501) staff       (20)      585 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/links.js
+-rw-r--r--   0 naveen     (501) staff       (20)      887 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/list.js
+-rw-r--r--   0 naveen     (501) staff       (20)      670 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/listItem.js
+-rw-r--r--   0 naveen     (501) staff       (20)     3186 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/node.js
+-rw-r--r--   0 naveen     (501) staff       (20)      415 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/paragraph.js
+-rw-r--r--   0 naveen     (501) staff       (20)      181 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/pre.js
+-rw-r--r--   0 naveen     (501) staff       (20)      402 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/strikethrough.js
+-rw-r--r--   0 naveen     (501) staff       (20)      395 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/strong.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2151 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/table.js
+-rw-r--r--   0 naveen     (501) staff       (20)      384 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/tableCell.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1465 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/txt.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1329 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/metadata.js
+-rw-r--r--   0 naveen     (501) staff       (20)      560 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/outdent.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2297 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/paragraphs.js
+-rw-r--r--   0 naveen     (501) staff       (20)      460 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/runExtension.js
+-rw-r--r--   0 naveen     (501) staff       (20)     2089 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/spanGamut.js
+-rw-r--r--   0 naveen     (501) staff       (20)      619 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/strikethrough.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1909 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/stripLinkDefinitions.js
+-rw-r--r--   0 naveen     (501) staff       (20)     4318 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/tables.js
+-rw-r--r--   0 naveen     (501) staff       (20)     1020 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/underline.js
+-rw-r--r--   0 naveen     (501) staff       (20)      529 2019-11-02 23:04:21.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/unescapeSpecialChars.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.857303 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/
+-rw-r--r--   0 naveen     (501) staff       (20)      719 2022-11-04 12:33:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/.bower.json
+-rw-r--r--   0 naveen     (501) staff       (20)    33744 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/CustomElements.js
+-rw-r--r--   0 naveen     (501) staff       (20)    16664 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/CustomElements.min.js
+-rw-r--r--   0 naveen     (501) staff       (20)    38189 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/HTMLImports.js
+-rw-r--r--   0 naveen     (501) staff       (20)    19924 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/HTMLImports.min.js
+-rw-r--r--   0 naveen     (501) staff       (20)    12660 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/MutationObserver.js
+-rw-r--r--   0 naveen     (501) staff       (20)     6000 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/MutationObserver.min.js
+-rw-r--r--   0 naveen     (501) staff       (20)     9002 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/README.md
+-rw-r--r--   0 naveen     (501) staff       (20)   159413 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/ShadowDOM.js
+-rw-r--r--   0 naveen     (501) staff       (20)    72261 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/ShadowDOM.min.js
+-rw-r--r--   0 naveen     (501) staff       (20)      423 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/bower.json
+-rw-r--r--   0 naveen     (501) staff       (20)     9941 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/build.log
+-rw-r--r--   0 naveen     (501) staff       (20)      737 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/package.json
+-rw-r--r--   0 naveen     (501) staff       (20)    79576 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents-lite.js
+-rw-r--r--   0 naveen     (501) staff       (20)    40547 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents-lite.min.js
+-rw-r--r--   0 naveen     (501) staff       (20)   259853 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents.js
+-rw-r--r--   0 naveen     (501) staff       (20)   118419 2017-02-06 23:35:26.000000 django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents.min.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.858147 django-inapp-survey-0.2.6/inapp_survey/static/images/
+-rw-r--r--   0 naveen     (501) staff       (20)      963 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/inapp_survey/static/images/survey-finished.svg
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.858420 django-inapp-survey-0.2.6/inapp_survey/static/inapp_survey/
+-rw-r--r--   0 naveen     (501) staff       (20)        0 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/inapp_survey/static/inapp_survey/style.css
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.859156 django-inapp-survey-0.2.6/inapp_survey/static/javascript/
+-rw-r--r--   0 naveen     (501) staff       (20)    13348 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/inapp_survey/static/javascript/extended-markdown.js
+-rw-r--r--   0 naveen     (501) staff       (20)    19765 2024-05-10 03:43:06.000000 django-inapp-survey-0.2.6/inapp_survey/static/javascript/script.js
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.859582 django-inapp-survey-0.2.6/inapp_survey/static/markdown-delight-editor-inapp/
+-rw-r--r--   0 naveen     (501) staff       (20)     8020 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/inapp_survey/static/markdown-delight-editor-inapp/markdown-delight-editor-extended.html
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.641877 django-inapp-survey-0.2.6/inapp_survey/templates/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.641776 django-inapp-survey-0.2.6/inapp_survey/templates/admin/
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.859855 django-inapp-survey-0.2.6/inapp_survey/templates/admin/inapp_survey/
+-rw-r--r--   0 naveen     (501) staff       (20)      725 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/inapp_survey/templates/admin/inapp_survey/change_form.html
+drwxr-xr-x   0 naveen     (501) staff       (20)        0 2024-05-10 05:17:30.860051 django-inapp-survey-0.2.6/inapp_survey/templates/inapp_survey/
+-rw-r--r--   0 naveen     (501) staff       (20)     7867 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/inapp_survey/templates/inapp_survey/index.html
+-rw-r--r--   0 naveen     (501) staff       (20)       60 2022-11-03 11:08:07.000000 django-inapp-survey-0.2.6/inapp_survey/tests.py
+-rw-r--r--   0 naveen     (501) staff       (20)      928 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.6/inapp_survey/urls.py
+-rw-r--r--   0 naveen     (501) staff       (20)      338 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.6/inapp_survey/views.py
+-rw-r--r--   0 naveen     (501) staff       (20)       38 2024-05-10 05:17:30.860823 django-inapp-survey-0.2.6/setup.cfg
+-rw-r--r--   0 naveen     (501) staff       (20)     1380 2022-11-03 11:11:54.000000 django-inapp-survey-0.2.6/setup.py
```

### Comparing `django-inapp-survey-0.2.5/LICENSE` & `django-inapp-survey-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/PKG-INFO` & `django-inapp-survey-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-inapp-survey
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple Django app to conduct Web-based survey or do announcement.
 Home-page: https://github.com/TuvaLabs/django-inapp-survey
 Author: Jaimin <jpatel@tuvalabs.com>, Naveen <nganesan@tuvalabs.com>
 Author-email: support@tuvalabs.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-inapp-survey-0.2.5/README.md` & `django-inapp-survey-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/django_inapp_survey.egg-info/PKG-INFO` & `django-inapp-survey-0.2.6/django_inapp_survey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-inapp-survey
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple Django app to conduct Web-based survey or do announcement.
 Home-page: https://github.com/TuvaLabs/django-inapp-survey
 Author: Jaimin <jpatel@tuvalabs.com>, Naveen <nganesan@tuvalabs.com>
 Author-email: support@tuvalabs.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-inapp-survey-0.2.5/django_inapp_survey.egg-info/SOURCES.txt` & `django-inapp-survey-0.2.6/django_inapp_survey.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 inapp_survey/serializers.py
 inapp_survey/tests.py
 inapp_survey/urls.py
 inapp_survey/views.py
 inapp_survey/docs/example.md
 inapp_survey/migrations/0001_initial.py
 inapp_survey/migrations/0002_auto_20210912_1311.py
+inapp_survey/migrations/0003_auto_20240510_0351.py
 inapp_survey/migrations/__init__.py
 inapp_survey/static/bower_components_inapp/Typo.js/.bower.json
 inapp_survey/static/bower_components_inapp/Typo.js/README.md
 inapp_survey/static/bower_components_inapp/Typo.js/SECURITY.md
 inapp_survey/static/bower_components_inapp/Typo.js/license.txt
 inapp_survey/static/bower_components_inapp/Typo.js/manifest.json
 inapp_survey/static/bower_components_inapp/Typo.js/examples/node/index.js
```

### Comparing `django-inapp-survey-0.2.5/inapp_survey/admin.py` & `django-inapp-survey-0.2.6/inapp_survey/admin.py`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/migrations/0001_initial.py` & `django-inapp-survey-0.2.6/inapp_survey/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/migrations/0002_auto_20210912_1311.py` & `django-inapp-survey-0.2.6/inapp_survey/migrations/0002_auto_20210912_1311.py`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/models.py` & `django-inapp-survey-0.2.6/inapp_survey/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 
 
 CAMPAIGN_TYPE = (
     ('announcement', 'Announcement'),
     ('survey', 'Survey'),
 )
 
+CAMPAIGN_PRIORITY = (
+    ('normal', 'Normal'),
+    ('high', 'High'),
+)
+
 
 class CampaignCustomParam(TimeStampedModel):
     # example
     # audience: teacher, student
     # premium_only: true
     # page: Dataset, Course
 
@@ -55,15 +60,20 @@
         "Expiry",
         blank=True,
         null=True)
     campaign_type = models.CharField(
         "Campaign Type",
         choices=CAMPAIGN_TYPE,
         max_length=500,
-        default="Request A Demo")
+        default="announcement")
+    priority = models.CharField(
+        "Priority",
+        choices=CAMPAIGN_PRIORITY,
+        max_length=10,
+        default="normal")
     custom_param = models.ManyToManyField(
         CampaignCustomParam,
         related_name="params",
         blank=True)
 
 
     def completed_count(self):
```

### Comparing `django-inapp-survey-0.2.5/inapp_survey/resources.py` & `django-inapp-survey-0.2.6/inapp_survey/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     # Only return the first one.
     permission_classes = [
         permissions.AllowAny
     ]
 
     def post(self, request, *args, **kwargs):
 
-        # If its expired, don't return
-        campaign = Campaign.objects.filter(expiry_date__gt=datetime.now()).order_by('expiry_date')
+        # If its expired, don't return and give preference to high priority campaigns/survey
+        campaign = Campaign.objects.filter(expiry_date__gte=datetime.now().date()).order_by('priority', 'expiry_date')
 
         # check for is_authenticated
         if request.user.is_authenticated:
 
             exclude_responded = []
             for item in campaign:
                 if item.usercampaign_set.filter(
```

### Comparing `django-inapp-survey-0.2.5/inapp_survey/serializers.py` & `django-inapp-survey-0.2.6/inapp_survey/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
                 'id',
                 'title',
                 'slug',
                 'description',
                 'is_authenticated',
                 'expiry_date',
                 'campaign_type',
+                'priority',
                 'steps',
                 'custom_param'
             )
 
 
 # User Campaign Responses
 class UserCampaignResponseSerializer(serializers.ModelSerializer):
```

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/README.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/README.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/examples/node/index.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/examples/node/index.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/license.txt` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/license.txt`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/british.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/british.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/british.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/british.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/LICENSE` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/LICENSE`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/de_DE.aff` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/de_DE.aff`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/de_DE.dic` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/de_DE/de_DE.dic`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/LICENSE` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/LICENSE`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/en_GB.aff` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/en_GB.aff`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/en_GB.dic` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/en_GB/en_GB.dic`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/fr_FR/fr_FR.aff` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/fr_FR/fr_FR.aff`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/fr_FR/fr_FR.dic` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/fr_FR/fr_FR.dic`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/README_la.txt` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/README_la.txt`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/la.aff` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/la.aff`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/la.dic` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/dictionaries/la/la.dic`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/english.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/english.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/english.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/english.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/french.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/french.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/french.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/french.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/general.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/general.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/general.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/general.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/german.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/german.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/german.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/german.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/index.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/index.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/latin.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/latin.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/latin.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/latin.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/jquery-1.9.1.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/jquery-1.9.1.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/qunit.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/qunit.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/qunit.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/tests/lib/qunit.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/README.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/README.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/en_US.aff` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/en_US.aff`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/en_US.dic` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/dictionaries/en_US/en_US.dic`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/package.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/package.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/Typo.js/typo/typo.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/Typo.js/typo/typo.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/.bower.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/.bower.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/AUTHORS` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/CHANGELOG.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/CONTRIBUTING.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/LICENSE` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/LICENSE`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/README.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/README.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/comment/comment.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/comment/comment.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/comment/continuecomment.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/comment/continuecomment.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/dialog/dialog.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/dialog/dialog.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/autorefresh.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/autorefresh.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/fullscreen.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/fullscreen.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/panel.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/panel.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/placeholder.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/placeholder.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/display/rulers.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/display/rulers.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/closebrackets.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/closebrackets.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/closetag.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/closetag.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/continuelist.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/continuelist.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/matchbrackets.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/matchbrackets.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/matchtags.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/matchtags.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/trailingspace.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/edit/trailingspace.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/brace-fold.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/brace-fold.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/comment-fold.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/comment-fold.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/foldcode.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/foldcode.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/foldgutter.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/foldgutter.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/indent-fold.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/indent-fold.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/markdown-fold.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/markdown-fold.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/xml-fold.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/fold/xml-fold.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/anyword-hint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/anyword-hint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/css-hint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/css-hint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/html-hint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/html-hint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/javascript-hint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/javascript-hint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/show-hint.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/show-hint.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/show-hint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/show-hint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/sql-hint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/sql-hint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/xml-hint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/hint/xml-hint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/coffeescript-lint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/coffeescript-lint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/css-lint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/css-lint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/html-lint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/html-lint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/javascript-lint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/javascript-lint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/json-lint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/json-lint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/lint.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/lint.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/lint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/lint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/yaml-lint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/lint/yaml-lint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/merge/merge.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/merge/merge.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/merge/merge.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/merge/merge.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/loadmode.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/loadmode.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/multiplex.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/multiplex.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/multiplex_test.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/multiplex_test.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/overlay.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/overlay.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/simple.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/mode/simple.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/colorize.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/colorize.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode-standalone.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode-standalone.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode.node.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/runmode/runmode.node.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/annotatescrollbar.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/annotatescrollbar.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/scrollpastend.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/scrollpastend.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/simplescrollbars.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/simplescrollbars.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/simplescrollbars.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/scroll/simplescrollbars.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/jump-to-line.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/jump-to-line.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/match-highlighter.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/match-highlighter.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/matchesonscrollbar.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/matchesonscrollbar.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/search.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/search.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/search/searchcursor.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/search/searchcursor.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/active-line.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/active-line.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/mark-selection.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/mark-selection.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/selection-pointer.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/selection/selection-pointer.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/tern.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/tern.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/tern.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/tern.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/worker.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/tern/worker.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/addon/wrap/hardwrap.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/addon/wrap/hardwrap.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/keymap/emacs.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/keymap/emacs.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/keymap/sublime.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/keymap/sublime.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/keymap/vim.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/keymap/vim.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/lib/codemirror.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/lib/codemirror.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/lib/codemirror.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/lib/codemirror.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/apl/apl.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/apl/apl.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/asciiarmor/asciiarmor.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/asciiarmor/asciiarmor.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/asn.1/asn.1.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/asn.1/asn.1.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/asterisk/asterisk.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/asterisk/asterisk.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/brainfuck/brainfuck.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/brainfuck/brainfuck.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/clike/clike.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/clike/clike.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/clojure/clojure.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/clojure/clojure.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/cmake/cmake.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/cmake/cmake.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/cobol/cobol.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/cobol/cobol.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/coffeescript/coffeescript.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/coffeescript/coffeescript.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/commonlisp/commonlisp.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/commonlisp/commonlisp.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/crystal/crystal.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/crystal/crystal.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/css/css.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/css/css.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/cypher/cypher.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/cypher/cypher.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/d/d.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/d/d.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dart/dart.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dart/dart.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/diff/diff.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/diff/diff.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/django/django.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/django/django.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dockerfile/dockerfile.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dockerfile/dockerfile.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dtd/dtd.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dtd/dtd.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/dylan/dylan.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/dylan/dylan.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ebnf/ebnf.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ebnf/ebnf.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ecl/ecl.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ecl/ecl.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/eiffel/eiffel.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/eiffel/eiffel.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/elm/elm.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/elm/elm.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/erlang/erlang.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/erlang/erlang.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/factor/factor.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/factor/factor.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/fcl/fcl.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/fcl/fcl.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/forth/forth.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/forth/forth.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/fortran/fortran.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/fortran/fortran.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/gas/gas.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/gas/gas.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/gfm/gfm.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/gfm/gfm.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/gherkin/gherkin.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/gherkin/gherkin.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/go/go.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/go/go.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/groovy/groovy.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/groovy/groovy.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haml/haml.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haml/haml.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/handlebars/handlebars.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/handlebars/handlebars.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell/haskell.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell/haskell.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell-literate/haskell-literate.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haskell-literate/haskell-literate.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/haxe/haxe.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/haxe/haxe.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlembedded/htmlembedded.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlembedded/htmlembedded.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlmixed/htmlmixed.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/htmlmixed/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/http/http.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/http/http.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/idl/idl.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/idl/idl.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/jade/jade.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/jade/jade.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/javascript/javascript.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/javascript/javascript.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/jinja2/jinja2.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/jinja2/jinja2.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/jsx/jsx.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/jsx/jsx.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/julia/julia.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/julia/julia.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/livescript/livescript.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/livescript/livescript.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/lua/lua.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/lua/lua.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/markdown/markdown.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/markdown/markdown.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mathematica/mathematica.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mathematica/mathematica.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/meta.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/meta.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mirc/mirc.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mirc/mirc.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mllike/mllike.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mllike/mllike.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/modelica/modelica.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/modelica/modelica.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mscgen/mscgen.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mscgen/mscgen.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/mumps/mumps.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/mumps/mumps.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/nginx/nginx.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/nginx/nginx.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/nsis/nsis.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/nsis/nsis.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ntriples/ntriples.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ntriples/ntriples.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/octave/octave.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/octave/octave.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/oz/oz.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/oz/oz.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/pascal/pascal.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/pascal/pascal.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/pegjs/pegjs.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/pegjs/pegjs.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/perl/perl.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/perl/perl.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/php/php.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/php/php.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/pig/pig.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/pig/pig.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/properties/properties.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/properties/properties.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/protobuf/protobuf.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/protobuf/protobuf.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/puppet/puppet.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/puppet/puppet.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/python/python.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/python/python.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/q/q.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/q/q.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/r/r.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/r/r.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/rpm/rpm.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/rpm/rpm.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/rst/rst.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/rst/rst.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ruby/ruby.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ruby/ruby.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/rust/rust.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/rust/rust.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sass/sass.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sass/sass.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/scheme/scheme.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/scheme/scheme.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/shell/shell.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/shell/shell.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sieve/sieve.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sieve/sieve.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/slim/slim.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/slim/slim.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/smalltalk/smalltalk.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/smalltalk/smalltalk.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/smarty/smarty.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/smarty/smarty.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/solr/solr.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/solr/solr.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/soy/soy.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/soy/soy.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sparql/sparql.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sparql/sparql.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/spreadsheet/spreadsheet.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/spreadsheet/spreadsheet.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/sql/sql.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/sql/sql.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/stex/stex.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/stex/stex.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/stylus/stylus.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/stylus/stylus.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/swift/swift.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/swift/swift.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tcl/tcl.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tcl/tcl.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/textile/textile.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/textile/textile.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tiddlywiki/tiddlywiki.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tiddlywiki/tiddlywiki.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tiki/tiki.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tiki/tiki.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/toml/toml.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/toml/toml.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/tornado/tornado.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/tornado/tornado.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/troff/troff.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/troff/troff.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn/ttcn.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn/ttcn.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn-cfg/ttcn-cfg.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/ttcn-cfg/ttcn-cfg.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/turtle/turtle.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/turtle/turtle.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/twig/twig.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/twig/twig.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vb/vb.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vb/vb.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vbscript/vbscript.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vbscript/vbscript.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/velocity/velocity.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/velocity/velocity.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/verilog/verilog.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/verilog/verilog.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vhdl/vhdl.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vhdl/vhdl.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/vue/vue.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/vue/vue.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/xml/xml.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/xml/xml.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/xquery/xquery.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/xquery/xquery.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml/yaml.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml/yaml.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/yaml-frontmatter/yaml-frontmatter.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/mode/z80/z80.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/mode/z80/z80.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/3024-day.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/3024-day.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/3024-night.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/3024-night.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/abcdef.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/abcdef.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/ambiance.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/ambiance.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/base16-dark.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/base16-dark.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/base16-light.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/base16-light.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/bespin.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/bespin.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/blackboard.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/blackboard.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/cobalt.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/cobalt.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/colorforth.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/colorforth.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/dracula.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/dracula.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/eclipse.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/eclipse.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/elegant.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/elegant.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/erlang-dark.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/erlang-dark.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/hopscotch.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/hopscotch.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/icecoder.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/icecoder.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/isotope.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/isotope.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/lesser-dark.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/lesser-dark.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/liquibyte.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/liquibyte.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/material.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/material.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/mbo.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/mbo.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/mdn-like.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/mdn-like.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/midnight.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/midnight.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/monokai.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/monokai.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/neat.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/neat.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/neo.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/neo.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/night.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/night.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/paraiso-dark.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/paraiso-dark.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/paraiso-light.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/paraiso-light.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/pastel-on-dark.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/pastel-on-dark.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/railscasts.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/railscasts.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/rubyblue.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/rubyblue.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/seti.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/seti.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/solarized.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/solarized.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/the-matrix.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/the-matrix.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/tomorrow-night-bright.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/tomorrow-night-bright.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/tomorrow-night-eighties.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/tomorrow-night-eighties.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/ttcn.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/ttcn.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/twilight.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/twilight.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/vibrant-ink.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/vibrant-ink.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/xq-dark.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/xq-dark.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/xq-light.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/xq-light.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/yeti.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/yeti.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/codemirror/theme/zenburn.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/codemirror/theme/zenburn.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/.bower.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/.bower.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/README.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/README.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.css.map` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.css.map`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.min.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/FontAwesome.otf` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.eot` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.svg` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.ttf` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.woff` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.woff2` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/animated.less` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/animated.less`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/bordered-pulled.less` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/bordered-pulled.less`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/icons.less` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/icons.less`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/mixins.less` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/mixins.less`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/path.less` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/path.less`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/rotated-flipped.less` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/rotated-flipped.less`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/less/variables.less` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/less/variables.less`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_animated.scss` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_animated.scss`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_bordered-pulled.scss` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_bordered-pulled.scss`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_icons.scss` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_icons.scss`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_mixins.scss` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_path.scss` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_path.scss`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_rotated-flipped.scss` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_rotated-flipped.scss`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_variables.scss` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/components-font-awesome/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/GPL-LICENSE.txt` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/GPL-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/MIT-LICENSE.txt` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/Makefile` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/Makefile`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/README.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/README.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/freq.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/freq.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/jshint-check.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/jshint-check.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/lib/jshint.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/lib/jshint.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/lib/parse-js.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/lib/parse-js.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/lib/process.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/lib/process.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/lib/squeeze-more.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/lib/squeeze-more.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/post-compile.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/post-compile.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/release-notes.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/release-notes.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/release-notes.txt` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/release-notes.txt`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/release.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/release.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/sizer.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/sizer.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/build/uglify.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/build/uglify.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/jquery.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/jquery.min.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/benchmarker.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/benchmarker.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/benchmarker.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/benchmarker.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/closest.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/closest.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/css.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/css.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/event.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/event.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/filter.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/filter.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/find.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/find.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/index.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/index.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/jquery-basis.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/jquery-basis.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/speed/slice.vs.concat.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/speed/slice.vs.concat.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/ajax/jsonp.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/ajax/script.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/ajax/xhr.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/ajax.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/attributes.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/attributes.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/callbacks.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/core.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/css.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/data.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/deferred.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/dimensions.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/effects.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/event.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/exports.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/exports.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/intro.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/intro.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/manipulation.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/offset.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/queue.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/support.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/support.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/src/traversing.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/1x1.jpg` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/1x1.jpg`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/include_js.php` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/include_js.php`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/absolute.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/absolute.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/body.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/body.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/fixed.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/fixed.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/relative.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/relative.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/scroll.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/scroll.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/static.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/static.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/table.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/offset/table.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/readywaitloader.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/readywaitloader.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/selector/html5_selector.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/selector/html5_selector.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/support/bodyBackground.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/support/bodyBackground.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/testinit.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/testinit.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/testrunner.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/testrunner.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/testsuite.css` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/testsuite.css`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/ua.txt` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/ua.txt`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/data/with_fries.xml` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/data/with_fries.xml`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/delegatetest.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/delegatetest.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/hovertest.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/hovertest.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/index.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/index.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/localfile.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/localfile.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/networkerror.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/networkerror.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/polluted.php` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/polluted.php`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/readywait.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/readywait.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/ajax.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/ajax.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/attributes.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/attributes.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/callbacks.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/callbacks.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/core.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/core.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/css.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/css.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/data.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/data.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/deferred.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/deferred.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/dimensions.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/dimensions.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/effects.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/effects.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/event.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/event.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/manipulation.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/manipulation.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/offset.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/offset.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/queue.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/queue.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/selector.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/selector.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/support.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/support.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/jquery/test/unit/traversing.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/jquery/test/unit/traversing.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/.bower.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/.bower.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/README.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/README.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/bower.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/bower.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/demo/index.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/demo/index.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/index.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/index.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/markdown-delight-editor-import.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/markdown-delight-editor-import.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/markdown-delight-editor.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/markdown-delight-editor.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/spell-checker.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/spell-checker.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/markdown-delight-editor/static/markdown.png` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/markdown-delight-editor/static/markdown.png`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/.bower.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/.bower.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/LICENSE.txt` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/bower.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/bower.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/build.log` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/build.log`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/polymer-micro.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/polymer-micro.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/polymer-mini.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/polymer-mini.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/polymer/polymer.html` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/polymer/polymer.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/.bower.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/.bower.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/CHANGELOG.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/CONTRIBUTING.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/CREDITS.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/CREDITS.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/DONATIONS.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/DONATIONS.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/README.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/README.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/bower.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/bower.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.js.map` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.js.map`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.min.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.min.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.min.js.map` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/dist/showdown.min.js.map`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/license.txt` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/license.txt`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/package-lock.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/package-lock.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/cli/cli.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/cli/cli.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/cli/makehtml.cmd.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/cli/makehtml.cmd.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/cli/messenger.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/cli/messenger.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/converter.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/converter.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/helpers.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/helpers.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/options.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/options.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/showdown.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/showdown.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/anchors.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/anchors.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/autoLinks.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/autoLinks.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/blockGamut.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/blockGamut.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/blockQuotes.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/blockQuotes.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/codeBlocks.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/codeBlocks.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/codeSpans.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/codeSpans.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/completeHTMLDocument.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/completeHTMLDocument.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/detab.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/detab.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/emoji.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/emoji.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeAmpsAndAngles.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeAmpsAndAngles.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeBackslashEscapes.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeBackslashEscapes.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeCode.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/encodeCode.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/escapeSpecialCharsWithinTagAttributes.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/escapeSpecialCharsWithinTagAttributes.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/githubCodeBlocks.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/githubCodeBlocks.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashCodeTags.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashCodeTags.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashElement.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashElement.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashHTMLBlocks.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashHTMLBlocks.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashHTMLSpans.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashHTMLSpans.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashPreCodeTags.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/hashPreCodeTags.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/headers.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/headers.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/horizontalRule.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/horizontalRule.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/images.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/images.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/italicsAndBold.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/italicsAndBold.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/lists.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/lists.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/blockquote.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/blockquote.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/image.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/image.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/links.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/links.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/list.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/list.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/listItem.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/listItem.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/node.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/node.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/table.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/table.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/txt.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/makeMarkdown/txt.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/metadata.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/metadata.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/outdent.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/outdent.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/paragraphs.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/paragraphs.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/spanGamut.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/spanGamut.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/strikethrough.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/strikethrough.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/stripLinkDefinitions.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/stripLinkDefinitions.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/tables.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/tables.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/underline.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/underline.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/unescapeSpecialChars.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/showdown/src/subParsers/unescapeSpecialChars.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/.bower.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/.bower.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/CustomElements.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/CustomElements.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/CustomElements.min.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/CustomElements.min.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/HTMLImports.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/HTMLImports.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/HTMLImports.min.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/HTMLImports.min.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/MutationObserver.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/MutationObserver.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/MutationObserver.min.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/MutationObserver.min.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/README.md` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/README.md`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/ShadowDOM.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/ShadowDOM.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/ShadowDOM.min.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/ShadowDOM.min.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/build.log` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/build.log`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/package.json` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/package.json`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents-lite.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents-lite.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents-lite.min.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents-lite.min.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents.min.js` & `django-inapp-survey-0.2.6/inapp_survey/static/bower_components_inapp/webcomponentsjs/webcomponents.min.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/images/survey-finished.svg` & `django-inapp-survey-0.2.6/inapp_survey/static/images/survey-finished.svg`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/javascript/extended-markdown.js` & `django-inapp-survey-0.2.6/inapp_survey/static/javascript/extended-markdown.js`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/javascript/script.js` & `django-inapp-survey-0.2.6/inapp_survey/static/javascript/script.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -400,23 +400,30 @@
             _successElement.slideUp('normal', function() {
                 _successElement.remove();
             });
             _inAppOverlayEle.remove();
         };
     }
 
-    function initiateSurvey() {
+    function initiateSurvey(showOnlyHighPriority) {
         var inAppSurveyService = new InAppSurveyService(),
             customParams = inappSurveyParams.customParams,
             userId = inappSurveyParams.userId,
             isAuthenticated = inappSurveyParams.isAuthenticated,
             surveyObj;
         inAppSurveyService.getSurvey(customParams, function(result) {
             if (result) {
                 surveyObj = result;
+                // Show only high priority survey when showOnlyHighPriority is true
+                if (showOnlyHighPriority) {
+                    if (surveyObj.priority !== "high") {
+                        resetTimer(false);
+                        return;
+                    }
+                }
                 if (surveyObj.campaign_type === "announcement") {
                     var announcement = new InAppAnnouncement();
                     announcement.show(surveyObj.description, false);
                     announcement.onClose(function() {
                         if (!isAuthenticated) {
                             var localStorageService = new LocalStorageService()
                             localStorageService.addSurveyId(surveyObj.id);
@@ -471,15 +478,15 @@
                     resetTimer(true);
                 }
             }
         });
     }
 
     // Timer to handle the survey showup based on timeout
-    var TIME_TO_SHOW_CAMPAIGN = 300 * 1000; // 5 min;
+    var TIME_TO_SHOW_CAMPAIGN = 5 * 60 * 1000; // 5 min;
     var timerIntervel = 2000;
     var isLocalStorageAvailable = localStorageService.isAvailable();
 
     function intializeTimer() {
         if (isLocalStorageAvailable) {
             if (localStorageService.getSurveyTimeoutMS() === 0) {
                 localStorageService.setSurveyTimeoutMS(TIME_TO_SHOW_CAMPAIGN);
@@ -487,22 +494,22 @@
             var timer = setInterval(function() {
                 var timeoutSec = localStorageService.getSurveyTimeoutMS();
                 timeoutSec -= timerIntervel;
                 if (timeoutSec <= 0) {
                     // Clear the interval when there are no campaign
                     clearInterval(timer);
                     // Initialize the survey
-                    initiateSurvey();
+                    initiateSurvey(false);
                     // Reset the time
                     timeoutSec = -9999;
                 }
                 localStorageService.setSurveyTimeoutMS(timeoutSec);
             }, timerIntervel);
         } else {
-            initiateSurvey();
+            initiateSurvey(false);
         }
     }
 
     function resetTimer(isNoCampaign) {
         // Initiate the next campaign timer
         localStorageService.setSurveyTimeoutMS(TIME_TO_SHOW_CAMPAIGN);
         // Don't start timer when there are no campaign
@@ -520,11 +527,14 @@
         toastWrap.innerHTML = 'Please Provide An Answer.';
         toastElement.appendChild(toastWrap);
         toastsContainer.appendChild(toastElement);
         setTimeout(() => {
             toastElement.parentNode.removeChild(toastElement);
         }, 2000);
     }
-    // Intialize the timer after a sec
-    setTimeout(intializeTimer, 800);
+    // Check for survey after a second
+    setTimeout(function() {
+        // Check for high priority surveys, if yes display it instantly
+        initiateSurvey(true);
+    }, 1000);
 
 })(jQuery);
```

### Comparing `django-inapp-survey-0.2.5/inapp_survey/static/markdown-delight-editor-inapp/markdown-delight-editor-extended.html` & `django-inapp-survey-0.2.6/inapp_survey/static/markdown-delight-editor-inapp/markdown-delight-editor-extended.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/templates/admin/inapp_survey/change_form.html` & `django-inapp-survey-0.2.6/inapp_survey/templates/admin/inapp_survey/change_form.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/templates/inapp_survey/index.html` & `django-inapp-survey-0.2.6/inapp_survey/templates/inapp_survey/index.html`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/inapp_survey/urls.py` & `django-inapp-survey-0.2.6/inapp_survey/urls.py`

 * *Files identical despite different names*

### Comparing `django-inapp-survey-0.2.5/setup.py` & `django-inapp-survey-0.2.6/setup.py`

 * *Files identical despite different names*

