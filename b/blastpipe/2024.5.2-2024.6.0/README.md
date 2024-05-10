# Comparing `tmp/blastpipe-2024.5.2.tar.gz` & `tmp/blastpipe-2024.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastpipe-2024.5.2.tar", last modified: Fri May 10 03:26:48 2024, max compression
+gzip compressed data, was "blastpipe-2024.6.0.tar", last modified: Fri May 10 20:10:07 2024, max compression
```

## Comparing `blastpipe-2024.5.2.tar` & `blastpipe-2024.6.0.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.250954 blastpipe-2024.5.2/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.190954 blastpipe-2024.5.2/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.194954 blastpipe-2024.5.2/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     6614 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/.github/workflows/ozi.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/.github/workflows/scorecards.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/.pre-commit-config.yaml
--rw-rw-r--   0 runner    (1001) docker     (127)   101850 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12458 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/LICENSE.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-10 03:26:47.906957 blastpipe-2024.5.2/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     3214 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.246954 blastpipe-2024.5.2/blastpipe/
--rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/backports.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/buffer.py
--rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/buffer.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/loop.py
--rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/loop.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/malloc.py
--rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/malloc.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/mixin.py
--rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/mixin.pyi
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.246954 blastpipe-2024.5.2/blastpipe/ozi_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)      361 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/.gitignore.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/CHANGELOG.md.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      344 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/LICENSE.txt.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      114 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/PKG-INFO.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/README.rst.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1867 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      663 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/__init__.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/bandit.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/bandit.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      268 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/black.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/black.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/coverage.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/doc8.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      126 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/doc8.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     2801 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/filter.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/filter.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)      387 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/flake8.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/flake8.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.202954 blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     1650 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      604 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/ozi.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      759 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/publish.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1377 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/release.yml.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.202954 blastpipe-2024.5.2/blastpipe/ozi_templates/gitlab_workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/gitlab_workflows/ozi.yml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      351 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/isort.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/isort.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.238954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.202954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.210954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      849 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/mit.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/wtfpl.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/zlib.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.210954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/
--rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.230954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.210954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/
--rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.210954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/
--rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.214954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/
--rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      433 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.214954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.214954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.214954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.214954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.214954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.218954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.218954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.218954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
--rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.218954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.218954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.218954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.222954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      457 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.222954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.222954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.222954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.222954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.222954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.226954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.226954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.226954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.226954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      461 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.226954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.226954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/mit.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.230954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.230954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.230954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.230954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
--rw-rw-r--   0 runner    (1001) docker     (127)      456 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.230954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.230954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
--rw-rw-r--   0 runner    (1001) docker     (127)      456 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1641 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.230954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/
--rw-rw-r--   0 runner    (1001) docker     (127)      437 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.234954 blastpipe-2024.5.2/blastpipe/ozi_templates/license/Public_Domain/
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/Public_Domain/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/Public_Domain/licenseref-public-domain.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/Public_Domain/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/agpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/apache-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/artistic-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/bsd-3-clause.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/cc0-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/epl-1.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/gfdl-1.3.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/gpl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/gpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/isc.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/lgpl-2.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/lgpl-2.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/lgpl-3.0.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1185 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/mit.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/ofl-1.1.txt
--rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/license/zlib.txt
--rw-rw-r--   0 runner    (1001) docker     (127)     1878 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      885 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/meson.options.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/mypy.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/mypy.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1153 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/new_child.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      355 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/ozi.wrap.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     2505 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     1140 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.array.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      623 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.feature.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.integer.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     3702 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.242954 blastpipe-2024.5.2/blastpipe/ozi_templates/project.name/
--rw-rw-r--   0 runner    (1001) docker     (127)      280 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.name/__init__.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      291 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.name/__init__.pyi.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.name/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1127 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.name/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.name/new_ext.pyx.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.name/new_module.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      131 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.name/py.typed.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      211 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/project.ozi.wrap.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/pydocstyle.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      280 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/pylint.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      682 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/pyproject.toml.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      233 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/pyright.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/pyright.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      394 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/pytest.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      424 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/pytest.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      152 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/requirements.in.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      231 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/restructuredtext-lint.meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     1283 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/root.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1128 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/ruff.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)     1126 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/semantic_release.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      343 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/setuptools_scm.pyproject.toml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.246954 blastpipe-2024.5.2/blastpipe/ozi_templates/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/tests/meson.build.j2
--rw-rw-r--   0 runner    (1001) docker     (127)      262 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/tests/new_test.py.j2
--rw-rw-r--   0 runner    (1001) docker     (127)     1429 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/ozi_templates/tox.pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/sequence.py
--rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/sequence.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/tailcall.py
--rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/blastpipe/tailcall.pyi
--rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)     8389 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)       33 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.250954 blastpipe-2024.5.2/subprojects/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.250954 blastpipe-2024.5.2/subprojects/docs/
--rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/docs/LICENSE.txt
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.246954 blastpipe-2024.5.2/subprojects/docs/_static/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.246954 blastpipe-2024.5.2/subprojects/docs/_static/css/
--rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/docs/_static/css/custom.css
--rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/docs/_static/css/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/docs/_static/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.246954 blastpipe-2024.5.2/subprojects/docs/_templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/docs/_templates/layout.html
--rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/docs/_templates/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/docs/conf.cfg
--rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/docs/index.rst
--rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/docs/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/docs/meson.options
--rw-rw-r--   0 runner    (1001) docker     (127)      115 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/subprojects/ozi.wrap
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 03:26:48.250954 blastpipe-2024.5.2/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/tests/test_backports.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/tests/test_filter.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/tests/test_fuzz.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-05-10 03:22:51.000000 blastpipe-2024.5.2/tests/test_tailcall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.548756 blastpipe-2024.6.0/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.492756 blastpipe-2024.6.0/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)       56 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      111 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.496756 blastpipe-2024.6.0/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     2886 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)      968 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     6374 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/.github/workflows/ozi.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3060 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/.github/workflows/scorecards.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3105 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)      309 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/.pre-commit-config.yaml
+-rw-rw-r--   0 runner    (1001) docker     (127)   104030 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12458 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/LICENSE.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     2710 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-10 20:09:58.204757 blastpipe-2024.6.0/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     3214 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.544756 blastpipe-2024.6.0/blastpipe/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1279 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      138 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3202 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1006 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/backports.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1717 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/buffer.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      213 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/buffer.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1762 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/loop.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      331 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/loop.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3316 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/malloc.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      301 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/malloc.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1250 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1475 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/mixin.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      453 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/mixin.pyi
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.544756 blastpipe-2024.6.0/blastpipe/ozi_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)      361 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/.gitignore.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      212 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/CHANGELOG.md.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      344 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/LICENSE.txt.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      114 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/PKG-INFO.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      620 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/README.rst.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1867 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      663 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/__init__.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)      271 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/bandit.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      269 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/bandit.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      268 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/black.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      230 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/black.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      629 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/coverage.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      222 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/doc8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      126 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/doc8.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2801 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/filter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1379 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/filter.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)      387 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/flake8.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/flake8.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.504756 blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1650 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      804 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      554 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      604 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      759 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/publish.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1377 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/release.yml.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.504756 blastpipe-2024.6.0/blastpipe/ozi_templates/gitlab_workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)      337 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/gitlab_workflows/ozi.yml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      351 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/isort.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      285 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/isort.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.540756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.504756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      357 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/CC0_1_0_Universal__CC0_1_0__Public_Domain_Dedication/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.512756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18660 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20141 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      849 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      485 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/wtfpl.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.512756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/
+-rw-rw-r--   0 runner    (1001) docker     (127)    11067 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      373 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.532756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.512756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    10315 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.512756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apache_Software_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.512756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)    19765 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    20209 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    19902 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    21198 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      433 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.516756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      376 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Artistic_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.516756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      710 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1346 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1729 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       40 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1713 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      471 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.516756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1340 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.516756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    22960 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.516756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_1_0__EPL_1_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.516756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    14199 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.520756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13154 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.520756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)    13831 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      372 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.520756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.520756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/agpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Affero_General_Public_License_v3_or_later__AGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.520756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/gfdl-1.3-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Free_Documentation_License__FDL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.520756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      457 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License__GPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.524756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2__GPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.524756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/gpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v2_or_later__GPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.524756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      405 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3__GPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.524756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/gpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      380 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_General_Public_License_v3_or_later__GPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.524756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2__LGPLv2_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.524756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v2_or_later__LGPLv2__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.528756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      407 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3__LGPLv3_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.528756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      381 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Lesser_General_Public_License_v3_or_later__LGPLv3__/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.528756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-2.1-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-only.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       36 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/lgpl-3.0-or-later.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      461 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/GNU_Library_or_Lesser_General_Public_License__LGPL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.528756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/ISC_License__ISCL_/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.528756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      367 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       31 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_License/mit.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.528756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      369 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      952 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.528756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       88 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Mozilla_Public_License_2_0__MPL_2_0_/mpl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.532756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      477 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     9269 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.532756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      456 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10302 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.532756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      374 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1069 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.532756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/
+-rw-rw-r--   0 runner    (1001) docker     (127)      456 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/SIL_Open_Font_License_1_1__OFL_1_1_/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1641 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.532756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/
+-rw-rw-r--   0 runner    (1001) docker     (127)      437 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       32 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/zlib_libpng_License/zlib.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.532756 blastpipe-2024.6.0/blastpipe/ozi_templates/license/Public_Domain/
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/Public_Domain/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)       35 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/Public_Domain/licenseref-public-domain.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      414 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/Public_Domain/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1213 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    34525 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/agpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11359 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/apache-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     8896 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/artistic-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1544 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/bsd-3-clause.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7050 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/cc0-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    11587 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/epl-1.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    22965 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/gfdl-1.3.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    18094 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/gpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    35151 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/gpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      788 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/isc.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    25381 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/lgpl-2.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)    26528 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/lgpl-2.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     7654 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/lgpl-3.0.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1185 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1114 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/mit.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      260 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/ofl-1.1.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)      901 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/license/zlib.txt
+-rw-rw-r--   0 runner    (1001) docker     (127)     1878 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      420 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      885 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/meson.options.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      170 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/mypy.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      248 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/mypy.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1153 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/new_child.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      355 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     2505 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     1140 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.array.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      623 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.feature.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      546 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.integer.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     3702 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.540756 blastpipe-2024.6.0/blastpipe/ozi_templates/project.name/
+-rw-rw-r--   0 runner    (1001) docker     (127)      280 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.name/__init__.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      291 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.name/__init__.pyi.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.name/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1127 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.name/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.name/new_ext.pyx.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      251 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.name/new_module.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      131 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.name/py.typed.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      211 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/project.ozi.wrap.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      253 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/pydocstyle.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      280 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/pylint.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      682 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/pyproject.toml.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      233 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/pyright.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      247 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/pyright.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      394 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/pytest.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      424 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/pytest.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      152 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/requirements.in.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      231 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/restructuredtext-lint.meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     1283 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/root.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1128 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/ruff.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1126 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/semantic_release.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      343 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/setuptools_scm.pyproject.toml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.544756 blastpipe-2024.6.0/blastpipe/ozi_templates/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      371 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      723 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/tests/meson.build.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)      262 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/tests/new_test.py.j2
+-rw-rw-r--   0 runner    (1001) docker     (127)     1429 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/ozi_templates/tox.pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     1865 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/sequence.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      101 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/sequence.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/tailcall.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      329 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/blastpipe/tailcall.pyi
+-rw-rw-r--   0 runner    (1001) docker     (127)     3291 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4520 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)     8389 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)       33 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.548756 blastpipe-2024.6.0/subprojects/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.548756 blastpipe-2024.6.0/subprojects/docs/
+-rw-rw-r--   0 runner    (1001) docker     (127)    12501 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/docs/LICENSE.txt
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.548756 blastpipe-2024.6.0/subprojects/docs/_static/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.548756 blastpipe-2024.6.0/subprojects/docs/_static/css/
+-rw-rw-r--   0 runner    (1001) docker     (127)      767 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/docs/_static/css/custom.css
+-rw-rw-r--   0 runner    (1001) docker     (127)      693 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/docs/_static/css/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      633 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/docs/_static/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.548756 blastpipe-2024.6.0/subprojects/docs/_templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1033 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/docs/_templates/layout.html
+-rw-rw-r--   0 runner    (1001) docker     (127)      694 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/docs/_templates/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      860 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/docs/conf.cfg
+-rw-rw-r--   0 runner    (1001) docker     (127)     1751 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)     2680 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/docs/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2058 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/docs/meson.options
+-rw-rw-r--   0 runner    (1001) docker     (127)      115 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/subprojects/ozi.wrap
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:09:58.552756 blastpipe-2024.6.0/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      832 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     1219 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/tests/test_backports.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1072 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/tests/test_filter.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2583 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/tests/test_fuzz.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1872 2024-05-10 20:07:17.000000 blastpipe-2024.6.0/tests/test_tailcall.py
```

### Comparing `blastpipe-2024.5.2/.github/workflows/codeql.yml` & `blastpipe-2024.6.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/.github/workflows/dependency-review.yml` & `blastpipe-2024.6.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/.github/workflows/ozi.yml` & `blastpipe-2024.6.0/.github/workflows/ozi.yml`

 * *Files 6% similar despite different names*

```diff
@@ -34,42 +34,14 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-  checkpoint-pp310-ubuntu-latest:
-    name: checkpoint (PyPy 3.10 on ubuntu-latest)
-    runs-on: ubuntu-latest
-    strategy:
-      fail-fast: false
-    permissions:
-        id-token: write
-    steps:
-      - name: Harden Runner
-        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
-        with:
-          disable-sudo: true
-          egress-policy: block
-          allowed-endpoints: >
-            files.pythonhosted.org:443
-            github.com:443
-            oziproject.dev:443
-            pypi.org:443
-            registry.npmjs.org:443
-            objects.githubusercontent.com:443
-            fulcio.sigstore.dev:443
-            rekor.sigstore.dev:443
-            tuf-repo-cdn.sigstore.dev:443
-
-      - uses: OZI-Project/checkpoint@1ad9ec15d60558ee3da890634bb8b0406838e17a
-        with:
-          python-version: "pypy3.10"
-
   checkpoint-cp311-ubuntu-latest:
     name: checkpoint (Python 3.11 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
     permissions:
         id-token: write
@@ -128,30 +100,54 @@
     steps:
       - name: Harden Runner
         uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
           disable-sudo: true
           egress-policy: block
 
-  release:
+  draft:
     needs: checkpoint
     runs-on: ubuntu-latest
-    concurrency: release
+    concurrency: draft
+    strategy:
+      fail-fast: true
+    permissions:
+      contents: write
+      id-token: write
+    outputs:
+      drafted: ${{ steps.draft.outputs.drafted }}
+      tag: ${{ steps.draft.outputs.tag }}
+    steps:
+      - name: Harden Runner
+        uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
+        with:
+          disable-sudo: true
+          egress-policy: block
+          allowed-endpoints: >
+            api.github.com:443
+            github.com:443
+
+      - uses: OZI-Project/draft@12b9a4f0d4e25ff5466bf2b0486d11aa4f3bf30d
+        id: draft
+        with:
+          github-token: ${{ secrets.GITHUB_TOKEN }}
+
+  release:
+    needs: [draft, checkpoint]
+    runs-on: ubuntu-latest
     strategy:
       matrix:
         py:
           - 'py310'
           - 'py311'
           - 'py312'
       fail-fast: true
       max-parallel: 1
     outputs:
-      drafted: ${{ steps.release.outputs.drafted }}
       hashes: ${{ steps.release.outputs.hashes }}
-      tag: ${{ steps.release.outputs.tag }}
     permissions:
       contents: write
       id-token: write
     steps:
       - name: Harden Runner
         uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
         with:
@@ -162,40 +158,40 @@
             files.pythonhosted.org:443
             fulcio.sigstore.dev:443
             github.com:443
             pypi.org:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/release@41916dbfb9a8fd0e73da21453fb999796cda9b52
+      - uses: OZI-Project/release@8b5e46e9d8899289f676ca2b432a63fe2faa93f9
         id: release
         with:
+          tag: ${{ needs.draft.outputs.tag }}
           python-dist: ${{ matrix.py }}
           github-token: ${{ secrets.GITHUB_TOKEN }}
 
   generate-provenance:
-    needs: [release, checkpoint]
+    needs: [draft, release, checkpoint]
     name: Generate build provenance
     permissions:
       actions: read # To read the workflow path.
       id-token: write # To sign the provenance.
       contents: write # To add assets to a release.
     # Currently this action needs to be referred by tag. More details at:
     # https://github.com/slsa-framework/slsa-github-generator#verification-of-provenance
     uses: slsa-framework/slsa-github-generator/.github/workflows/generator_generic_slsa3.yml@v2.0.0
     with:
-      provenance-name: provenance-${{ github.event.repository.name }}-${{ needs.release.outputs.tag }}.intoto.jsonl
+      provenance-name: provenance-${{ github.event.repository.name }}-${{ needs.draft.outputs.tag }}.intoto.jsonl
       base64-subjects: "${{ needs.release.outputs.hashes }}"
-      upload-tag-name: "${{ needs.release.outputs.tag }}"
+      upload-tag-name: "${{ needs.draft.outputs.tag }}"
       upload-assets: true
 
   publish:
     runs-on: ubuntu-latest
-    needs: [release, generate-provenance]
-    if: needs.release.outputs.drafted == 'true'
+    needs: [draft, release, generate-provenance]
     permissions:
       actions: read
       contents: write
       id-token: write
     steps:
     - name: Harden Runner
       uses: step-security/harden-runner@a4aa98b93cab29d9b1101a6143fb8bce00e2eac4 # v2.7.1
```

### Comparing `blastpipe-2024.5.2/.github/workflows/scorecards.yml` & `blastpipe-2024.6.0/.github/workflows/scorecards.yml`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
       - name: "Checkout code"
         uses: actions/checkout@44c2b7a8a4ea60a981eaca3cf939b5f4305c123b # v4.1.5
         with:
           persist-credentials: false
 
       - name: "Run analysis"
-        uses: ossf/scorecard-action@0864cf19026789058feabb7e87baa5f140aac736 # v2.3.1
+        uses: ossf/scorecard-action@dc50aa9510b46c811795eb24b2f1ba02a914e534 # v2.3.3
         with:
           results_file: results.sarif
           results_format: sarif
           # (Optional) "write" PAT token. Uncomment the `repo_token` line below if:
           # - you want to enable the Branch-Protection check on a *public* repository, or
           # - you are installing Scorecards on a *private* repository
           # To create the PAT, follow the steps in https://github.com/ossf/scorecard-action#authentication-with-pat.
```

### Comparing `blastpipe-2024.5.2/.gitignore` & `blastpipe-2024.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/CHANGELOG.md` & `blastpipe-2024.6.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,62 @@
 # CHANGELOG
 
 
 
+## v2024.6.0 (2024-05-10)
+
+### :arrow_up:
+
+* :arrow_up: Bump ossf/scorecard-action from 2.3.1 to 2.3.3
+
+Bumps [ossf/scorecard-action](https://github.com/ossf/scorecard-action) from 2.3.1 to 2.3.3.
+- [Release notes](https://github.com/ossf/scorecard-action/releases)
+- [Changelog](https://github.com/ossf/scorecard-action/blob/main/RELEASE.md)
+- [Commits](https://github.com/ossf/scorecard-action/compare/0864cf19026789058feabb7e87baa5f140aac736...dc50aa9510b46c811795eb24b2f1ba02a914e534)
+
+---
+updated-dependencies:
+- dependency-name: ossf/scorecard-action
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`0cf8d28`](https://github.com/OZI-Project/blastpipe/commit/0cf8d285935bb2ccddd55f986a914efc6c5fcf7f))
+
+### :pencil2:
+
+* :pencil2: fix release pin
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`ffd1c77`](https://github.com/OZI-Project/blastpipe/commit/ffd1c7727c3a84a8d34bbaaf12012c948f3dbaa5))
+
+### :sparkles:
+
+* :sparkles: add spec 0.2 isolated release drafting.
+
+Signed-off-by: rjdbcm &lt;rjdbcm@outlook.com&gt; ([`b8206e7`](https://github.com/OZI-Project/blastpipe/commit/b8206e79ef757b4dba37588a9a8d0709d9937879))
+
+### Other
+
+* Update ozi.yml
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`d19756f`](https://github.com/OZI-Project/blastpipe/commit/d19756f7bd1efc0922436375ba79260283972261))
+
+* Merge pull request #83 from OZI-Project/dependabot/github_actions/ossf/scorecard-action-2.3.3
+
+⬆️ Bump ossf/scorecard-action from 2.3.1 to 2.3.3 ([`cebe82b`](https://github.com/OZI-Project/blastpipe/commit/cebe82be76da9323151c2796f54a77e99cb12450))
+
+* Merge pull request #84 from OZI-Project/spec-0.2-workflow
+
+:sparkles: add spec 0.2 isolated release drafting. ([`1464321`](https://github.com/OZI-Project/blastpipe/commit/1464321ede5b872764e7131ec95c480de2e4ef8a))
+
+* Merge branch &#39;dependabot/github_actions/ossf/scorecard-action-2.3.3&#39; into spec-0.2-workflow
+
+Signed-off-by: Eden Rose, MSc &lt;ozi.project@outlook.com&gt; ([`c4e2a03`](https://github.com/OZI-Project/blastpipe/commit/c4e2a03b7f5f6b84a55573795cbcefe1fb1393ad))
+
+
 ## v2024.5.2 (2024-05-10)
 
 ### :pencil2:
 
 * :pencil2: relicense templates to The Unlicense.
 
 Also cleans up metadata
```

### Comparing `blastpipe-2024.5.2/LICENSE.txt` & `blastpipe-2024.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/NOTICE.md` & `blastpipe-2024.6.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/PKG-INFO` & `blastpipe-2024.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: blastpipe
-Version: 2024.5.2
+Version: 2024.6.0
 Summary: OZI integrated test library.
 Home-page: https://oziproject.dev
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
-Download-URL: https://github.com/OZI-Project/blastpipe/archive/refs/tags/2024.5.2.tar.gz
+Download-URL: https://github.com/OZI-Project/blastpipe/archive/refs/tags/2024.6.0.tar.gz
 Requires-Python: >=3.10, <3.13
 Keywords: ozi,meson
 Provides-Dist: ozi-templates
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `blastpipe-2024.5.2/README.rst` & `blastpipe-2024.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/__init__.py` & `blastpipe-2024.6.0/blastpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/backports.py` & `blastpipe-2024.6.0/blastpipe/backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/backports.pyi` & `blastpipe-2024.6.0/blastpipe/backports.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/buffer.py` & `blastpipe-2024.6.0/blastpipe/buffer.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/loop.py` & `blastpipe-2024.6.0/blastpipe/loop.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/malloc.py` & `blastpipe-2024.6.0/blastpipe/malloc.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/meson.build` & `blastpipe-2024.6.0/blastpipe/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/mixin.py` & `blastpipe-2024.6.0/blastpipe/mixin.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/README.rst.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/README.rst.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/__init__.py` & `blastpipe-2024.6.0/blastpipe/ozi_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/__init__.pyi` & `blastpipe-2024.6.0/blastpipe/ozi_templates/__init__.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/coverage.pyproject.toml` & `blastpipe-2024.6.0/blastpipe/ozi_templates/coverage.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/filter.py` & `blastpipe-2024.6.0/blastpipe/ozi_templates/filter.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/filter.pyi` & `blastpipe-2024.6.0/blastpipe/ozi_templates/filter.pyi`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/checkpoint.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/generate_provenance.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/meson.build` & `blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/ozi.yml.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/ozi.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/publish.yml.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/publish.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/github_workflows/release.yml.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/github_workflows/release.yml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/DFSG_approved/meson.build` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/DFSG_approved/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/Free_To_Use_But_Restricted/ncsa.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Academic_Free_License__AFL_/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-1.2.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Apple_Public_Source_License/apsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/0bsd.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/BSD_License/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Boost_Software_License_1_0__BSL_1_0_/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/CEA_CNRS_Inria_Logiciel_Libre_License__version_2_1__CeCILL_2_1_/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Eclipse_Public_License_2_0__EPL_2_0_/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_1__EUPL_1_1_/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/European_Union_Public_Licence_1_2__EUPL_1_2_/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/MIT_No_Attribution_License__MIT_0_/mit-0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Mulan_Permissive_Software_License_v2__MulanPSL_2_0_/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/Open_Software_License_3_0__OSL_3_0_/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/PostgreSQL_License/postgresql.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/OSI_Approved/meson.build` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/OSI_Approved/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/Public_Domain/unlicense.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/agpl-3.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/apache-2.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/artistic-2.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/bsd-3-clause.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/cc0-1.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/epl-1.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/gfdl-1.3.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/gpl-2.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/gpl-3.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/isc.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/isc.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/lgpl-2.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/lgpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/lgpl-2.1.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/lgpl-3.0.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/meson.build` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/mit.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/mit.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/license/zlib.txt` & `blastpipe-2024.6.0/blastpipe/ozi_templates/license/zlib.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/meson.build` & `blastpipe-2024.6.0/blastpipe/ozi_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/meson.options.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/meson.options.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/new_child.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/new_child.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/project.PKG-INFO` & `blastpipe-2024.6.0/blastpipe/ozi_templates/project.PKG-INFO`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/project.array.meson.options` & `blastpipe-2024.6.0/blastpipe/ozi_templates/project.array.meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/project.feature.meson.options` & `blastpipe-2024.6.0/blastpipe/ozi_templates/project.feature.meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/project.integer.meson.options` & `blastpipe-2024.6.0/blastpipe/ozi_templates/project.integer.meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/project.meson.build` & `blastpipe-2024.6.0/blastpipe/ozi_templates/project.meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/project.name/meson.build.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/project.name/meson.build.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/pyproject.toml.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/root.pyproject.toml` & `blastpipe-2024.6.0/blastpipe/ozi_templates/root.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/ruff.pyproject.toml` & `blastpipe-2024.6.0/blastpipe/ozi_templates/ruff.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/semantic_release.pyproject.toml` & `blastpipe-2024.6.0/blastpipe/ozi_templates/semantic_release.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/tests/meson.build.j2` & `blastpipe-2024.6.0/blastpipe/ozi_templates/tests/meson.build.j2`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/ozi_templates/tox.pyproject.toml` & `blastpipe-2024.6.0/blastpipe/ozi_templates/tox.pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/sequence.py` & `blastpipe-2024.6.0/blastpipe/sequence.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/blastpipe/tailcall.py` & `blastpipe-2024.6.0/blastpipe/tailcall.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/meson.build` & `blastpipe-2024.6.0/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/meson.options` & `blastpipe-2024.6.0/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/pyproject.toml` & `blastpipe-2024.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/subprojects/docs/LICENSE.txt` & `blastpipe-2024.6.0/subprojects/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/subprojects/docs/_static/css/custom.css` & `blastpipe-2024.6.0/subprojects/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/subprojects/docs/_static/css/meson.build` & `blastpipe-2024.6.0/subprojects/docs/_static/css/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/subprojects/docs/_static/meson.build` & `blastpipe-2024.6.0/subprojects/docs/_static/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/subprojects/docs/_templates/layout.html` & `blastpipe-2024.6.0/subprojects/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/subprojects/docs/_templates/meson.build` & `blastpipe-2024.6.0/subprojects/docs/_templates/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/subprojects/docs/conf.cfg` & `blastpipe-2024.6.0/subprojects/docs/conf.cfg`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/subprojects/docs/index.rst` & `blastpipe-2024.6.0/subprojects/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/subprojects/docs/meson.build` & `blastpipe-2024.6.0/subprojects/docs/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/subprojects/docs/meson.options` & `blastpipe-2024.6.0/subprojects/docs/meson.options`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/tests/meson.build` & `blastpipe-2024.6.0/tests/meson.build`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/tests/test_backports.py` & `blastpipe-2024.6.0/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/tests/test_filter.py` & `blastpipe-2024.6.0/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/tests/test_fuzz.py` & `blastpipe-2024.6.0/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `blastpipe-2024.5.2/tests/test_tailcall.py` & `blastpipe-2024.6.0/tests/test_tailcall.py`

 * *Files identical despite different names*

