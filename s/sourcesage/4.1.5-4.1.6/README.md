# Comparing `tmp/sourcesage-4.1.5.tar.gz` & `tmp/sourcesage-4.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcesage-4.1.5.tar", last modified: Tue Apr 30 07:27:23 2024, max compression
+gzip compressed data, was "sourcesage-4.1.6.tar", last modified: Fri May 10 14:17:22 2024, max compression
```

## Comparing `sourcesage-4.1.5.tar` & `sourcesage-4.1.6.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:27:23.185902 sourcesage-4.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-30 07:27:19.000000 sourcesage-4.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18164 2024-04-30 07:27:23.185902 sourcesage-4.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17781 2024-04-30 07:27:19.000000 sourcesage-4.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:27:23.189902 sourcesage-4.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-30 07:27:19.000000 sourcesage-4.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:27:23.181903 sourcesage-4.1.5/sourcesage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:27:23.185902 sourcesage-4.1.5/sourcesage/config/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/config/.SourceSageignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:27:23.185902 sourcesage-4.1.5/sourcesage/config/ISSUES_RESOLVE/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:27:23.185902 sourcesage-4.1.5/sourcesage/config/STAGE_INFO/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/config/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/config/language_map.json
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:27:23.185902 sourcesage-4.1.5/sourcesage/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/ChangelogGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/ChangelogUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/DiffChangelogGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/EnvFileHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/GitHubIssueRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/GitHubUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/IssuesToMarkdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/StageInfoGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/StagedDiffGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/markdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-30 07:27:19.000000 sourcesage-4.1.5/sourcesage/modules/source_sage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:27:23.185902 sourcesage-4.1.5/sourcesage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18164 2024-04-30 07:27:23.000000 sourcesage-4.1.5/sourcesage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-30 07:27:23.000000 sourcesage-4.1.5/sourcesage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:27:23.000000 sourcesage-4.1.5/sourcesage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 07:27:23.000000 sourcesage-4.1.5/sourcesage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-30 07:27:23.000000 sourcesage-4.1.5/sourcesage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 07:27:23.000000 sourcesage-4.1.5/sourcesage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:27:23.185902 sourcesage-4.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-30 07:27:19.000000 sourcesage-4.1.5/tests/test_sourcesage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 14:17:17.000000 sourcesage-4.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-10 14:17:22.028912 sourcesage-4.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-05-10 14:17:17.000000 sourcesage-4.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:17:22.028912 sourcesage-4.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-10 14:17:18.000000 sourcesage-4.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.024912 sourcesage-4.1.6/sourcesage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/sourcesage/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/.SourceSageignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/sourcesage/config/ISSUES_RESOLVE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/sourcesage/config/STAGE_INFO/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/config/language_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/sourcesage/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/ChangelogGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/ChangelogUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/DiffChangelogGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/EnvFileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/GitHubIssueRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/GitHubUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/IssuesToMarkdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/StageInfoGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/StagedDiffGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/markdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-10 14:17:18.000000 sourcesage-4.1.6/sourcesage/modules/source_sage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/sourcesage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 14:17:22.000000 sourcesage-4.1.6/sourcesage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:17:22.028912 sourcesage-4.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-10 14:17:18.000000 sourcesage-4.1.6/tests/test_sourcesage.py
```

### Comparing `sourcesage-4.1.5/LICENSE` & `sourcesage-4.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/PKG-INFO` & `sourcesage-4.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.1.5
+Version: 4.1.6
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
@@ -25,20 +25,23 @@
   <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
   <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/sourcesage">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/sourcesage">
   <a href="https://app.codacy.com/gh/Sunwood-ai-labs/SourceSage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade"><img src="https://app.codacy.com/project/badge/Grade/77ab7715dd23499d82caca4e7ea3b093"/></a>
 
   [![SourceSage - Sunwood-ai-labs](https://img.shields.io/static/v1?label=SourceSage&message=Sunwood-ai-labs&color=blue&logo=github)](https://github.com/Sunwood-ai-labs/SourceSage "Go to GitHub repo")
-[![stars - Sunwood-ai-labs](https://img.shields.io/github/stars/SourceSage/Sunwood-ai-labs?style=social)](https://github.com/Sunwood-ai-labs/SourceSage)
+![GitHub Repo stars](https://img.shields.io/github/stars/Sunwood-ai-labs/SourceSage)
 [![forks - Sunwood-ai-labs](https://img.shields.io/github/forks/SourceSage/Sunwood-ai-labs?style=social)](https://github.com/Sunwood-ai-labs/SourceSage)
 [![GitHub Last Commit](https://img.shields.io/github/last-commit/Sunwood-ai-labs/SourceSage)](https://github.com/Sunwood-ai-labs/SourceSage)
 [![GitHub Top Language](https://img.shields.io/github/languages/top/Sunwood-ai-labs/SourceSage)](https://github.com/Sunwood-ai-labs/SourceSage)
-[![GitHub Release](https://img.shields.io/github/v/release/Sunwood-ai-labs/SourceSage?sort=date&color=red)](https://github.com/Sunwood-ai-labs/SourceSage)
-[![GitHub Tag](https://img.shields.io/github/v/tag/Sunwood-ai-labs/SourceSage?color=orange)](https://github.com/Sunwood-ai-labs/SourceSage)
+![GitHub Release](https://img.shields.io/github/v/release/Sunwood-ai-labs/SourceSage?color=red)
+![GitHub Tag](https://img.shields.io/github/v/tag/Sunwood-ai-labs/SourceSage?sort=semver&color=orange)
+<img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/Sunwood-ai-labs/SourceSage/publish-to-pypi.yml">
+
+
 
   <br>
 
 </h2>
 
 
 </p>
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1 Name: sourcesage Version: 4.1.5 Home-page: https://
+Metadata-Version: 2.1 Name: sourcesage Version: 4.1.6 Home-page: https://
 github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
                            ************ SSoouurrcceeSSaaggee ************
                      ********** ?ï?½?TTrraannssffoorrmmiinngg ccooddee ffoorr AAII?ï?½?
  [[PPyyPPII -- VVeerrssiioonn]][[PPyyPPII -- FFoorrmmaatt]][[PPyyPPII -- IImmpplleemmeennttaattiioonn]][[PPyyPPII -- SSttaattuuss]][[PPyyPPII --
    DDoowwnnllooaaddss]][[PPyyPPII -- DDoowwnnllooaaddss]]_[[_hh_tt_tt_pp_ss_::_//_//_aa_pp_pp_.._cc_oo_dd_aa_cc_yy_.._cc_oo_mm_//_pp_rr_oo_jj_ee_cc_tt_//_bb_aa_dd_gg_ee_//_GG_rr_aa_dd_ee_//
   _77_77_aa_bb_77_77_11_55_dd_dd_22_33_44_99_99_dd_88_22_cc_aa_cc_aa_44_ee_77_ee_aa_33_bb_00_99_33_]][[!![[SSoouurrcceeSSaaggee -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////
          iimmgg..sshhiieellddss..iioo//ssttaattiicc//vv11??llaabbeell==SSoouurrcceeSSaaggee&&mmeessssaaggee==SSuunnwwoooodd--aaii--
 llaabbss&&ccoolloorr==bblluuee&&llooggoo==ggiitthhuubb))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee ""GGoo
-  ttoo GGiittHHuubb rreeppoo"")) [[!![[ssttaarrss -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//
-ssttaarrss//SSoouurrcceeSSaaggee//SSuunnwwoooodd--aaii--llaabbss??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--
-  llaabbss//SSoouurrcceeSSaaggee)) [[!![[ffoorrkkss -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//
-ffoorrkkss//SSoouurrcceeSSaaggee//SSuunnwwoooodd--aaii--llaabbss??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--
-  llaabbss//SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb LLaasstt CCoommmmiitt]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//llaasstt--
-    ccoommmmiitt//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//
- SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb TToopp LLaanngguuaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//llaanngguuaaggeess//
-ttoopp//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))
-  [[!![[GGiittHHuubb RReelleeaassee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//rreelleeaassee//SSuunnwwoooodd--aaii--llaabbss//
-SSoouurrcceeSSaaggee??ssoorrtt==ddaattee&&ccoolloorr==rreedd))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))
-      [[!![[GGiittHHuubb TTaagg]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//ttaagg//SSuunnwwoooodd--aaii--llaabbss//
-   SSoouurrcceeSSaaggee??ccoolloorr==oorraannggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))
+  ttoo GGiittHHuubb rreeppoo"")) !![[GGiittHHuubb RReeppoo ssttaarrss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//ssttaarrss//
+SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee)) [[!![[ffoorrkkss -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//
+  ggiitthhuubb//ffoorrkkss//SSoouurrcceeSSaaggee//SSuunnwwoooodd--aaii--llaabbss??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ggiitthhuubb..ccoomm//
+  SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb LLaasstt CCoommmmiitt]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//
+ggiitthhuubb//llaasstt--ccoommmmiitt//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--
+    llaabbss//SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb TToopp LLaanngguuaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//
+llaanngguuaaggeess//ttoopp//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//
+SSoouurrcceeSSaaggee)) !![[GGiittHHuubb RReelleeaassee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//rreelleeaassee//SSuunnwwoooodd--
+ aaii--llaabbss//SSoouurrcceeSSaaggee??ccoolloorr==rreedd)) !![[GGiittHHuubb TTaagg]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//
+    ttaagg//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee??ssoorrtt==sseemmvveerr&&ccoolloorr==oorraannggee))[[GGiittHHuubb AAccttiioonnss
+                               WWoorrkkffllooww SSttaattuuss]]
                                      **********
 SourceSageã¯ããã­ã¸ã§ã¯ãã®ã½ã¼ã¹ã³ã¼ãã¨ãã¡ã¤ã«æ§æãåä¸ã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ã«çµ±åããAIã«ããèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãå®ç¾ããPythonã¹ã¯ãªããã§ããéçºã®ã©ã¤ããµã¤ã¯ã«å¨ä½ãéãã¦ãã³ã¼ãã®åè³ªåä¸ã¨çç£æ§ã®åä¸ãæ¯æ´ãã¾ãã
 >[!IMPORTANT] >ãã®ãªãã¸ããªèªä½ã[SourceSage](https://github.com/
 Sunwood-ai-labs/
 SourceSage)ãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯
 [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ï¼ [claude.ai]
 (https://claude.ai/)ã§çæãã¦ãã¾ãã ## æ´æ°åå®¹ - [ã2024/04/
```

### Comparing `sourcesage-4.1.5/README.md` & `sourcesage-4.1.6/sourcesage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: sourcesage
+Version: 4.1.6
+Home-page: https://github.com/Sunwood-ai-labs/SourceSage
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: loguru
+Requires-Dist: GitPython
+Requires-Dist: requests
+Requires-Dist: art
+
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
 <br>
 <h1 align="center">SourceSage</h1>
 <h2 align="center">
   ～Transforming code for AI～
 
@@ -11,20 +25,23 @@
   <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
   <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/sourcesage">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/sourcesage">
   <a href="https://app.codacy.com/gh/Sunwood-ai-labs/SourceSage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade"><img src="https://app.codacy.com/project/badge/Grade/77ab7715dd23499d82caca4e7ea3b093"/></a>
 
   [![SourceSage - Sunwood-ai-labs](https://img.shields.io/static/v1?label=SourceSage&message=Sunwood-ai-labs&color=blue&logo=github)](https://github.com/Sunwood-ai-labs/SourceSage "Go to GitHub repo")
-[![stars - Sunwood-ai-labs](https://img.shields.io/github/stars/SourceSage/Sunwood-ai-labs?style=social)](https://github.com/Sunwood-ai-labs/SourceSage)
+![GitHub Repo stars](https://img.shields.io/github/stars/Sunwood-ai-labs/SourceSage)
 [![forks - Sunwood-ai-labs](https://img.shields.io/github/forks/SourceSage/Sunwood-ai-labs?style=social)](https://github.com/Sunwood-ai-labs/SourceSage)
 [![GitHub Last Commit](https://img.shields.io/github/last-commit/Sunwood-ai-labs/SourceSage)](https://github.com/Sunwood-ai-labs/SourceSage)
 [![GitHub Top Language](https://img.shields.io/github/languages/top/Sunwood-ai-labs/SourceSage)](https://github.com/Sunwood-ai-labs/SourceSage)
-[![GitHub Release](https://img.shields.io/github/v/release/Sunwood-ai-labs/SourceSage?sort=date&color=red)](https://github.com/Sunwood-ai-labs/SourceSage)
-[![GitHub Tag](https://img.shields.io/github/v/tag/Sunwood-ai-labs/SourceSage?color=orange)](https://github.com/Sunwood-ai-labs/SourceSage)
+![GitHub Release](https://img.shields.io/github/v/release/Sunwood-ai-labs/SourceSage?color=red)
+![GitHub Tag](https://img.shields.io/github/v/tag/Sunwood-ai-labs/SourceSage?sort=semver&color=orange)
+<img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/Sunwood-ai-labs/SourceSage/publish-to-pypi.yml">
+
+
 
   <br>
 
 </h2>
 
 
 </p>
@@ -262,8 +279,8 @@
 
 ## 貢献
 
 SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
 
 ## ライセンス
 
-このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
+このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
```

#### html2text {}

```diff
@@ -1,28 +1,32 @@
+Metadata-Version: 2.1 Name: sourcesage Version: 4.1.6 Home-page: https://
+github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
+Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
                            ************ SSoouurrcceeSSaaggee ************
                      ********** ?ï?½?TTrraannssffoorrmmiinngg ccooddee ffoorr AAII?ï?½?
  [[PPyyPPII -- VVeerrssiioonn]][[PPyyPPII -- FFoorrmmaatt]][[PPyyPPII -- IImmpplleemmeennttaattiioonn]][[PPyyPPII -- SSttaattuuss]][[PPyyPPII --
    DDoowwnnllooaaddss]][[PPyyPPII -- DDoowwnnllooaaddss]]_[[_hh_tt_tt_pp_ss_::_//_//_aa_pp_pp_.._cc_oo_dd_aa_cc_yy_.._cc_oo_mm_//_pp_rr_oo_jj_ee_cc_tt_//_bb_aa_dd_gg_ee_//_GG_rr_aa_dd_ee_//
   _77_77_aa_bb_77_77_11_55_dd_dd_22_33_44_99_99_dd_88_22_cc_aa_cc_aa_44_ee_77_ee_aa_33_bb_00_99_33_]][[!![[SSoouurrcceeSSaaggee -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////
          iimmgg..sshhiieellddss..iioo//ssttaattiicc//vv11??llaabbeell==SSoouurrcceeSSaaggee&&mmeessssaaggee==SSuunnwwoooodd--aaii--
 llaabbss&&ccoolloorr==bblluuee&&llooggoo==ggiitthhuubb))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee ""GGoo
-  ttoo GGiittHHuubb rreeppoo"")) [[!![[ssttaarrss -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//
-ssttaarrss//SSoouurrcceeSSaaggee//SSuunnwwoooodd--aaii--llaabbss??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--
-  llaabbss//SSoouurrcceeSSaaggee)) [[!![[ffoorrkkss -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//
-ffoorrkkss//SSoouurrcceeSSaaggee//SSuunnwwoooodd--aaii--llaabbss??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--
-  llaabbss//SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb LLaasstt CCoommmmiitt]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//llaasstt--
-    ccoommmmiitt//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//
- SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb TToopp LLaanngguuaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//llaanngguuaaggeess//
-ttoopp//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))
-  [[!![[GGiittHHuubb RReelleeaassee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//rreelleeaassee//SSuunnwwoooodd--aaii--llaabbss//
-SSoouurrcceeSSaaggee??ssoorrtt==ddaattee&&ccoolloorr==rreedd))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))
-      [[!![[GGiittHHuubb TTaagg]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//ttaagg//SSuunnwwoooodd--aaii--llaabbss//
-   SSoouurrcceeSSaaggee??ccoolloorr==oorraannggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))
+  ttoo GGiittHHuubb rreeppoo"")) !![[GGiittHHuubb RReeppoo ssttaarrss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//ssttaarrss//
+SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee)) [[!![[ffoorrkkss -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//
+  ggiitthhuubb//ffoorrkkss//SSoouurrcceeSSaaggee//SSuunnwwoooodd--aaii--llaabbss??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ggiitthhuubb..ccoomm//
+  SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb LLaasstt CCoommmmiitt]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//
+ggiitthhuubb//llaasstt--ccoommmmiitt//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--
+    llaabbss//SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb TToopp LLaanngguuaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//
+llaanngguuaaggeess//ttoopp//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//
+SSoouurrcceeSSaaggee)) !![[GGiittHHuubb RReelleeaassee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//rreelleeaassee//SSuunnwwoooodd--
+ aaii--llaabbss//SSoouurrcceeSSaaggee??ccoolloorr==rreedd)) !![[GGiittHHuubb TTaagg]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//
+    ttaagg//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee??ssoorrtt==sseemmvveerr&&ccoolloorr==oorraannggee))[[GGiittHHuubb AAccttiioonnss
+                               WWoorrkkffllooww SSttaattuuss]]
                                      **********
 SourceSageã¯ããã­ã¸ã§ã¯ãã®ã½ã¼ã¹ã³ã¼ãã¨ãã¡ã¤ã«æ§æãåä¸ã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ã«çµ±åããAIã«ããèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãå®ç¾ããPythonã¹ã¯ãªããã§ããéçºã®ã©ã¤ããµã¤ã¯ã«å¨ä½ãéãã¦ãã³ã¼ãã®åè³ªåä¸ã¨çç£æ§ã®åä¸ãæ¯æ´ãã¾ãã
 >[!IMPORTANT] >ãã®ãªãã¸ããªèªä½ã[SourceSage](https://github.com/
 Sunwood-ai-labs/
 SourceSage)ãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯
 [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ï¼ [claude.ai]
 (https://claude.ai/)ã§çæãã¦ãã¾ãã ## æ´æ°åå®¹ - [ã2024/04/
```

### Comparing `sourcesage-4.1.5/setup.py` & `sourcesage-4.1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    required = f.read().splitlines()
 
 setup(
     # パッケージの名前
     name='sourcesage',
     
     # パッケージのバージョン
-    version='4.1.5',
+    version='4.1.6',
     
     # パッケージに含めるモジュールを自動的に探す
     packages=find_packages(),
     
     # パッケージの分類情報
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `sourcesage-4.1.5/sourcesage/cli.py` & `sourcesage-4.1.6/sourcesage/cli.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md` & `sourcesage-4.1.6/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md` & `sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md` & `sourcesage-4.1.6/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/config/constants.py` & `sourcesage-4.1.6/sourcesage/config/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,8 +30,9 @@
         self.ISSUES_RESOLVE_TEMPLATE_MD = "ISSUES_RESOLVE_TEMPLATE.md"
 
         self.TEMPLATE_STAGE_INFO_DIR = os.path.join(self.DOCS_DIR, "STAGE_INFO")
         self.STAGE_INFO_OUTPUT_MD = "STAGE_INFO_AND_ISSUES_AND_PROMT.md"
         self.STAGE_INFO_TEMPLATE_MD = "STAGE_INFO_AND_ISSUES_TEMPLATE.md"
 
         self.STAGE_INFO_SIMPLE_OUTPUT_MD = "STAGE_INFO_AND_PROMT.md"
-        self.STAGE_INFO_SIMPLE_TEMPLATE_MD = "STAGE_INFO_TEMPLATE.md"
+        self.STAGE_INFO_SIMPLE_TEMPLATE_MD = "STAGE_INFO_TEMPLATE.md"
+        self.STAGE_INFO_SIMPLE_TEMPLATE_MD_EMOJI = "STAGE_INFO_TEMPLATE_EMOJI.md"
```

### Comparing `sourcesage-4.1.5/sourcesage/config/language_map.json` & `sourcesage-4.1.6/sourcesage/config/language_map.json`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/core.py` & `sourcesage-4.1.6/sourcesage/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,14 +64,19 @@
 
         # Generate stage info
         stage_info_generator = StageInfoGenerator(issue_file_path=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
                                                   stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
                                                   template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_TEMPLATE_MD),
                                                   output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_OUTPUT_MD))
         stage_info_generator.run()
+        stage_info_generator = StageInfoGenerator(issue_file_path=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
+                                                  stage_diff_file_path=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.STAGED_DIFF_MD),
+                                                  template_file_path=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_TEMPLATE_MD_EMOJI),
+                                                  output_file_path=os.path.join(self.constants.STAGE_INFO_DIR, self.constants.STAGE_INFO_SIMPLE_OUTPUT_MD))
+        stage_info_generator.run()
 
         # Convert issues to markdown
         issues_to_markdown = IssuesToMarkdown(issues_file=os.path.join(self.constants.ISSUE_LOG_DIR, self.constants.ISSUES_FILE_NAME),
                                               sourcesage_file=os.path.join(self.constants.SOURCE_SAGE_ASSETS_DIR, self.constants.SOURCE_SAGE_MD),
                                               template_file=os.path.join(self.constants.DOCS_DIR, self.constants.TEMPLATE_ISSUES_RESOLVE_DIR, self.constants.ISSUES_RESOLVE_TEMPLATE_MD),
                                               output_folder=self.constants.ISSUES_RESOLVE_DIR)
         issues_to_markdown.load_data()
```

### Comparing `sourcesage-4.1.5/sourcesage/modules/ChangelogGenerator.py` & `sourcesage-4.1.6/sourcesage/modules/ChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/ChangelogUtils.py` & `sourcesage-4.1.6/sourcesage/modules/ChangelogUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/DiffChangelogGenerator.py` & `sourcesage-4.1.6/sourcesage/modules/DiffChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/EnvFileHandler.py` & `sourcesage-4.1.6/sourcesage/modules/EnvFileHandler.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/GitHubIssueRetrieve.py` & `sourcesage-4.1.6/sourcesage/modules/GitHubIssueRetrieve.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/GitHubUtils.py` & `sourcesage-4.1.6/sourcesage/modules/GitHubUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/IssuesToMarkdown.py` & `sourcesage-4.1.6/sourcesage/modules/IssuesToMarkdown.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/StageInfoGenerator.py` & `sourcesage-4.1.6/sourcesage/modules/StageInfoGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/StagedDiffGenerator.py` & `sourcesage-4.1.6/sourcesage/modules/StagedDiffGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/file_utils.py` & `sourcesage-4.1.6/sourcesage/modules/file_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/markdown_utils.py` & `sourcesage-4.1.6/sourcesage/modules/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage/modules/source_sage.py` & `sourcesage-4.1.6/sourcesage/modules/source_sage.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.1.5/sourcesage.egg-info/PKG-INFO` & `sourcesage-4.1.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: sourcesage
-Version: 4.1.5
-Home-page: https://github.com/Sunwood-ai-labs/SourceSage
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: loguru
-Requires-Dist: GitPython
-Requires-Dist: requests
-Requires-Dist: art
-
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
 <br>
 <h1 align="center">SourceSage</h1>
 <h2 align="center">
   ～Transforming code for AI～
 
@@ -25,20 +11,23 @@
   <img alt="PyPI - Implementation" src="https://img.shields.io/pypi/implementation/sourcesage">
   <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/sourcesage">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/sourcesage">
   <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dw/sourcesage">
   <a href="https://app.codacy.com/gh/Sunwood-ai-labs/SourceSage/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade"><img src="https://app.codacy.com/project/badge/Grade/77ab7715dd23499d82caca4e7ea3b093"/></a>
 
   [![SourceSage - Sunwood-ai-labs](https://img.shields.io/static/v1?label=SourceSage&message=Sunwood-ai-labs&color=blue&logo=github)](https://github.com/Sunwood-ai-labs/SourceSage "Go to GitHub repo")
-[![stars - Sunwood-ai-labs](https://img.shields.io/github/stars/SourceSage/Sunwood-ai-labs?style=social)](https://github.com/Sunwood-ai-labs/SourceSage)
+![GitHub Repo stars](https://img.shields.io/github/stars/Sunwood-ai-labs/SourceSage)
 [![forks - Sunwood-ai-labs](https://img.shields.io/github/forks/SourceSage/Sunwood-ai-labs?style=social)](https://github.com/Sunwood-ai-labs/SourceSage)
 [![GitHub Last Commit](https://img.shields.io/github/last-commit/Sunwood-ai-labs/SourceSage)](https://github.com/Sunwood-ai-labs/SourceSage)
 [![GitHub Top Language](https://img.shields.io/github/languages/top/Sunwood-ai-labs/SourceSage)](https://github.com/Sunwood-ai-labs/SourceSage)
-[![GitHub Release](https://img.shields.io/github/v/release/Sunwood-ai-labs/SourceSage?sort=date&color=red)](https://github.com/Sunwood-ai-labs/SourceSage)
-[![GitHub Tag](https://img.shields.io/github/v/tag/Sunwood-ai-labs/SourceSage?color=orange)](https://github.com/Sunwood-ai-labs/SourceSage)
+![GitHub Release](https://img.shields.io/github/v/release/Sunwood-ai-labs/SourceSage?color=red)
+![GitHub Tag](https://img.shields.io/github/v/tag/Sunwood-ai-labs/SourceSage?sort=semver&color=orange)
+<img alt="GitHub Actions Workflow Status" src="https://img.shields.io/github/actions/workflow/status/Sunwood-ai-labs/SourceSage/publish-to-pypi.yml">
+
+
 
   <br>
 
 </h2>
 
 
 </p>
@@ -276,8 +265,8 @@
 
 ## 貢献
 
 SourceSageの改善にご協力ください！バグの報告や機能追加の提案がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/SourceSage)でIssueを開くかプルリクエストを送信してください。
 
 ## ライセンス
 
-このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
+このプロジェクトは[MITライセンス](LICENSE)の下で公開されています。
```

#### html2text {}

```diff
@@ -1,33 +1,27 @@
-Metadata-Version: 2.1 Name: sourcesage Version: 4.1.5 Home-page: https://
-github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
-Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
                            ************ SSoouurrcceeSSaaggee ************
                      ********** ?ï?½?TTrraannssffoorrmmiinngg ccooddee ffoorr AAII?ï?½?
  [[PPyyPPII -- VVeerrssiioonn]][[PPyyPPII -- FFoorrmmaatt]][[PPyyPPII -- IImmpplleemmeennttaattiioonn]][[PPyyPPII -- SSttaattuuss]][[PPyyPPII --
    DDoowwnnllooaaddss]][[PPyyPPII -- DDoowwnnllooaaddss]]_[[_hh_tt_tt_pp_ss_::_//_//_aa_pp_pp_.._cc_oo_dd_aa_cc_yy_.._cc_oo_mm_//_pp_rr_oo_jj_ee_cc_tt_//_bb_aa_dd_gg_ee_//_GG_rr_aa_dd_ee_//
   _77_77_aa_bb_77_77_11_55_dd_dd_22_33_44_99_99_dd_88_22_cc_aa_cc_aa_44_ee_77_ee_aa_33_bb_00_99_33_]][[!![[SSoouurrcceeSSaaggee -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////
          iimmgg..sshhiieellddss..iioo//ssttaattiicc//vv11??llaabbeell==SSoouurrcceeSSaaggee&&mmeessssaaggee==SSuunnwwoooodd--aaii--
 llaabbss&&ccoolloorr==bblluuee&&llooggoo==ggiitthhuubb))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee ""GGoo
-  ttoo GGiittHHuubb rreeppoo"")) [[!![[ssttaarrss -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//
-ssttaarrss//SSoouurrcceeSSaaggee//SSuunnwwoooodd--aaii--llaabbss??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--
-  llaabbss//SSoouurrcceeSSaaggee)) [[!![[ffoorrkkss -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//
-ffoorrkkss//SSoouurrcceeSSaaggee//SSuunnwwoooodd--aaii--llaabbss??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--
-  llaabbss//SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb LLaasstt CCoommmmiitt]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//llaasstt--
-    ccoommmmiitt//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//
- SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb TToopp LLaanngguuaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//llaanngguuaaggeess//
-ttoopp//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))
-  [[!![[GGiittHHuubb RReelleeaassee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//rreelleeaassee//SSuunnwwoooodd--aaii--llaabbss//
-SSoouurrcceeSSaaggee??ssoorrtt==ddaattee&&ccoolloorr==rreedd))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))
-      [[!![[GGiittHHuubb TTaagg]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//ttaagg//SSuunnwwoooodd--aaii--llaabbss//
-   SSoouurrcceeSSaaggee??ccoolloorr==oorraannggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))
+  ttoo GGiittHHuubb rreeppoo"")) !![[GGiittHHuubb RReeppoo ssttaarrss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//ssttaarrss//
+SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee)) [[!![[ffoorrkkss -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//
+  ggiitthhuubb//ffoorrkkss//SSoouurrcceeSSaaggee//SSuunnwwoooodd--aaii--llaabbss??ssttyyllee==ssoocciiaall))]]((hhttttppss::////ggiitthhuubb..ccoomm//
+  SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb LLaasstt CCoommmmiitt]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//
+ggiitthhuubb//llaasstt--ccoommmmiitt//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--
+    llaabbss//SSoouurrcceeSSaaggee)) [[!![[GGiittHHuubb TToopp LLaanngguuaaggee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//
+llaanngguuaaggeess//ttoopp//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee))]]((hhttttppss::////ggiitthhuubb..ccoomm//SSuunnwwoooodd--aaii--llaabbss//
+SSoouurrcceeSSaaggee)) !![[GGiittHHuubb RReelleeaassee]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//rreelleeaassee//SSuunnwwoooodd--
+ aaii--llaabbss//SSoouurrcceeSSaaggee??ccoolloorr==rreedd)) !![[GGiittHHuubb TTaagg]]((hhttttppss::////iimmgg..sshhiieellddss..iioo//ggiitthhuubb//vv//
+    ttaagg//SSuunnwwoooodd--aaii--llaabbss//SSoouurrcceeSSaaggee??ssoorrtt==sseemmvveerr&&ccoolloorr==oorraannggee))[[GGiittHHuubb AAccttiioonnss
+                               WWoorrkkffllooww SSttaattuuss]]
                                      **********
 SourceSageã¯ããã­ã¸ã§ã¯ãã®ã½ã¼ã¹ã³ã¼ãã¨ãã¡ã¤ã«æ§æãåä¸ã®ãã¼ã¯ãã¦ã³ãã¡ã¤ã«ã«çµ±åããAIã«ããèªåä¿®æ­£ããã­ã¥ã¡ã³ãåãå®ç¾ããPythonã¹ã¯ãªããã§ããéçºã®ã©ã¤ããµã¤ã¯ã«å¨ä½ãéãã¦ãã³ã¼ãã®åè³ªåä¸ã¨çç£æ§ã®åä¸ãæ¯æ´ãã¾ãã
 >[!IMPORTANT] >ãã®ãªãã¸ããªèªä½ã[SourceSage](https://github.com/
 Sunwood-ai-labs/
 SourceSage)ãæ´»ç¨ãã¦ããããªãªã¼ã¹ãã¼ããREADMEãã³ãããã¡ãã»ã¼ã¸ã®9å²ã¯
 [SourceSage](https://github.com/Sunwood-ai-labs/SourceSage) ï¼ [claude.ai]
 (https://claude.ai/)ã§çæãã¦ãã¾ãã ## æ´æ°åå®¹ - [ã2024/04/
```

### Comparing `sourcesage-4.1.5/sourcesage.egg-info/SOURCES.txt` & `sourcesage-4.1.6/sourcesage.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 sourcesage.egg-info/top_level.txt
 sourcesage/config/.SourceSageignore
 sourcesage/config/constants.py
 sourcesage/config/language_map.json
 sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
 sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
+sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md
 sourcesage/modules/ChangelogGenerator.py
 sourcesage/modules/ChangelogUtils.py
 sourcesage/modules/DiffChangelogGenerator.py
 sourcesage/modules/EnvFileHandler.py
 sourcesage/modules/GitHubIssueRetrieve.py
 sourcesage/modules/GitHubUtils.py
 sourcesage/modules/IssuesToMarkdown.py
```

### Comparing `sourcesage-4.1.5/tests/test_sourcesage.py` & `sourcesage-4.1.6/tests/test_sourcesage.py`

 * *Files identical despite different names*

