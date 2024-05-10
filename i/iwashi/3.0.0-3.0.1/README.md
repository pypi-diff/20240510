# Comparing `tmp/iwashi-3.0.0.tar.gz` & `tmp/iwashi-3.0.1.tar.gz`

## Comparing `iwashi-3.0.0.tar` & `iwashi-3.0.1.tar`

### file list

```diff
@@ -1,74 +1,80 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 iwashi-3.0.0/.python-version
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 iwashi-3.0.0/aa copy.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 iwashi-3.0.0/aa.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 iwashi-3.0.0/requirements-dev.lock
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.0/requirements.lock
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 iwashi-3.0.0/.github/scripts/report-failures.sh
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 iwashi-3.0.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 iwashi-3.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 iwashi-3.0.0/.vscode/settings.json
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/__init__.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/__main__.py
--rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/helper.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/iwashi.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/throttle.py
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/visitor.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/__init__.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/bandcamp.py
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/booth.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/fanbox.py
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/github.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/instagram.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/itchio.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/kofi.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/linktree.py
--rw-r--r--   0        0        0    13215 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/litlink.py
--rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/mirrativ.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/nicovideo.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/note.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/patreon.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/pixiv.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/reddit.py
--rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/sketch.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/soundcloud.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/spotify.py
--rw-r--r--   0        0        0    92171 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/tiktok.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/twitcasting.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/twitch.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/twitter.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/youtube/__init__.py
--rw-r--r--   0        0        0     8915 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/youtube/youtube.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/youtube/types/__init__.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/youtube/types/about.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 iwashi-3.0.0/src/iwashi/service/youtube/types/ytinitialdata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/service_tester.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_bandcamp.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_booth.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_fanbox.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_github.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_instagram.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_itchio.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_kofi.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_link_tree.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_linktree.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_litlink.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_mirrativ.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_nicovideo.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_note.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_patreon.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_pixiv.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_reddit.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_sketch.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_soundcloud.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_spotify.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_tiktok.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_twitcasting.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_twitch.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_twitter.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 iwashi-3.0.0/tests/test_youtube.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 iwashi-3.0.0/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 iwashi-3.0.0/LICENSE
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 iwashi-3.0.0/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 iwashi-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 iwashi-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 iwashi-3.0.1/.prettierignore
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 iwashi-3.0.1/.python-version
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 iwashi-3.0.1/requirements-dev.lock
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.1/requirements.lock
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 iwashi-3.0.1/.github/scripts/report-failures.sh
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 iwashi-3.0.1/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 iwashi-3.0.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 iwashi-3.0.1/.vscode/launch.json
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 iwashi-3.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 iwashi-3.0.1/scripts/generate_version.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/__init__.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/__main__.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/helper.py
+-rw-r--r--   0        0        0     4325 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/iwashi.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/throttle.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/version.py
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/visitor.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/__init__.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/bandcamp.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/booth.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/fanbox.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/github.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/instagram.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/itchio.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/kofi.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/linktree.py
+-rw-r--r--   0        0        0    13215 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/litlink.py
+-rw-r--r--   0        0        0     4573 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/mirrativ.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/nicovideo.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/note.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/patreon.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/pixiv.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/reddit.py
+-rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/skeb.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/sketch.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/soundcloud.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/spotify.py
+-rw-r--r--   0        0        0    92171 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/tiktok.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/twitcasting.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/twitch.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/twitter.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/youtube/__init__.py
+-rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/youtube/youtube.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/youtube/types/__init__.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/youtube/types/about.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/youtube/types/ytinitialdata.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/youtube/types/ytinitialdata2.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 iwashi-3.0.1/src/iwashi/service/youtube/types/ytinitialdata3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/service_tester.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_bandcamp.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_booth.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_fanbox.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_github.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_instagram.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_itchio.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_kofi.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_linktree.py
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_litlink.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_mirrativ.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_nicovideo.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_note.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_patreon.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_pixiv.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_reddit.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_skeb.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_sketch.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_soundcloud.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_spotify.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_tiktok.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_tree.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_twitcasting.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_twitch.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_twitter.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 iwashi-3.0.1/tests/test_youtube.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 iwashi-3.0.1/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 iwashi-3.0.1/LICENSE
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 iwashi-3.0.1/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 iwashi-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 iwashi-3.0.1/PKG-INFO
```

### Comparing `iwashi-3.0.0/requirements-dev.lock` & `iwashi-3.0.1/requirements-dev.lock`

 * *Files 10% similar despite different names*

```diff
@@ -4,39 +4,44 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via iwashi
 aiosignal==1.3.1
     # via aiohttp
 astor==0.8.1
 attrs==23.2.0
     # via aiohttp
 beautifulsoup4==4.12.3
     # via bs4
 bs4==0.0.2
     # via iwashi
-build==1.0.3
+build==1.2.1
+certifi==2024.2.2
+    # via requests
+charset-normalizer==3.3.2
+    # via requests
 click==8.1.7
     # via iwashi
 colorama==0.4.6
     # via build
     # via click
     # via loguru
     # via pytest
 coverage==7.4.3
     # via pytest-cov
 frozenlist==1.4.1
     # via aiohttp
     # via aiosignal
 idna==3.6
+    # via requests
     # via yarl
 iniconfig==2.0.0
     # via pytest
 loguru==0.7.2
     # via iwashi
 multidict==6.0.5
     # via aiohttp
@@ -46,24 +51,27 @@
 packaging==23.2
     # via build
     # via pytest
 pluggy==1.4.0
     # via pytest
 pyproject-hooks==1.0.0
     # via build
-pyright==1.1.359
+pyright==1.1.362
 pytest==8.1.0
     # via pytest-asyncio
     # via pytest-cov
-pytest-asyncio==0.23.5
-pytest-cov==4.1.0
-ruff==0.2.1
+pytest-asyncio==0.23.6
+pytest-cov==5.0.0
+requests==2.31.0
+ruff==0.4.4
 setuptools==69.5.1
     # via nodeenv
 soupsieve==2.5
     # via beautifulsoup4
 strinpy==0.0.4
 typingdict==0.1.3
+urllib3==2.2.1
+    # via requests
 win32-setctime==1.1.0
     # via loguru
 yarl==1.9.4
     # via aiohttp
```

### Comparing `iwashi-3.0.0/requirements.lock` & `iwashi-3.0.1/requirements.lock`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
-aiohttp==3.9.3
+aiohttp==3.9.5
     # via iwashi
 aiosignal==1.3.1
     # via aiohttp
 attrs==23.2.0
     # via aiohttp
 beautifulsoup4==4.12.3
     # via bs4
```

### Comparing `iwashi-3.0.0/.github/workflows/test.yml` & `iwashi-3.0.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/.vscode/settings.json` & `iwashi-3.0.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/helper.py` & `iwashi-3.0.1/src/iwashi/helper.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/iwashi.py` & `iwashi-3.0.1/src/iwashi/iwashi.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,19 +26,20 @@
     def is_visited(self, url: str) -> bool:
         return url in self.visited_urls
 
     def mark_visited(self, url: str):
         self.visited_urls.add(url)
 
     async def tree(self, url: str, context: Optional[Context] = None) -> Result | None:
-        context = context or Context(session=self.session, visitor=self)
-        context = context.create_context()
-        result = await self.visit(url, context)
-        while self.tasks:
-            await self.tasks.pop()
+        async with self.session:
+            context = context or Context(session=self.session, visitor=self)
+            context = context.create_context()
+            result = await self.visit(url, context)
+            while self.tasks:
+                await self.tasks.pop()
 
         return result
 
     def enqueue_visit(self, url: str, context: Context) -> None:
         coro = self.visit(url, context)
         task = asyncio.create_task(coro)
         self.tasks.append(task)
@@ -83,15 +84,22 @@
                 logger.warning(f"[No Service] No service matched {normalized_url}")
 
         return context.result
 
     async def try_redirect(self, url: str, context: Context) -> bool:
         try:
             res = await context.session.get(
-                url, headers=BASE_HEADERS, allow_redirects=True, timeout=5
+                url,
+                headers=BASE_HEADERS
+                | {
+                    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36 Edg/124.0.0.0",
+                    "Referer": url,
+                },
+                allow_redirects=True,
+                timeout=5,
             )
             res.raise_for_status()
         except aiohttp.ClientError as e:
             logger.exception(e)
             logger.warning(f"[Redirect] failed to redirect {url}")
             return False
         except asyncio.TimeoutError as e:
```

### Comparing `iwashi-3.0.0/src/iwashi/throttle.py` & `iwashi-3.0.1/src/iwashi/throttle.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/visitor.py` & `iwashi-3.0.1/src/iwashi/visitor.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/__init__.py` & `iwashi-3.0.1/src/iwashi/service/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from .twitter import Twitter
 from .youtube import Youtube
 from .spotify import Spotify
 from .github import Github
 from .itchio import Itchio
 from .kofi import Kofi
 from .patreon import Patreon
+from .skeb import Skeb
+
 
 __all__ = [
     "Bandcamp",
     "Booth",
     "Fanbox",
     "Instagram",
     "Linktree",
@@ -42,14 +44,15 @@
     "Twitter",
     "Youtube",
     "Spotify",
     "Github",
     "Itchio",
     "Kofi",
     "Patreon",
+    "Skeb",
 ]
 
 SERVICES = {
     Bandcamp(),
     Booth(),
     Fanbox(),
     Instagram(),
@@ -68,8 +71,9 @@
     Twitter(),
     Youtube(),
     Spotify(),
     Github(),
     Itchio(),
     Kofi(),
     Patreon(),
+    Skeb(),
 }
```

### Comparing `iwashi-3.0.0/src/iwashi/service/bandcamp.py` & `iwashi-3.0.1/src/iwashi/service/bandcamp.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/booth.py` & `iwashi-3.0.1/src/iwashi/service/booth.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/fanbox.py` & `iwashi-3.0.1/src/iwashi/service/fanbox.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/github.py` & `iwashi-3.0.1/src/iwashi/service/github.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/instagram.py` & `iwashi-3.0.1/src/iwashi/service/instagram.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/itchio.py` & `iwashi-3.0.1/src/iwashi/service/itchio.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/kofi.py` & `iwashi-3.0.1/src/iwashi/service/kofi.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/linktree.py` & `iwashi-3.0.1/src/iwashi/service/linktree.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/litlink.py` & `iwashi-3.0.1/src/iwashi/service/litlink.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/mirrativ.py` & `iwashi-3.0.1/src/iwashi/service/mirrativ.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/nicovideo.py` & `iwashi-3.0.1/src/iwashi/service/nicovideo.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/note.py` & `iwashi-3.0.1/src/iwashi/service/note.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/patreon.py` & `iwashi-3.0.1/src/iwashi/service/patreon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 import json
 import re
-from typing import List, TypedDict
+from typing import List, NotRequired, TypedDict
 
 import bs4
 from iwashi.helper import HTTP_REGEX
 from iwashi.visitor import Context, Service
 
 
 class Patreon(Service):
@@ -34,15 +34,15 @@
             id=id,
             url=url,
             name=data_root["author"]["name"],
             description=data_root["about"]["description"],
             profile_picture=data_root["author"]["image"]["contentUrl"],
         )
 
-        for link in data_root["sameAs"]:
+        for link in data_root.get("sameAs", []):
             context.enqueue_visit(link)
 
 
 class Image(TypedDict):
     contentUrl: str
     thumbnailUrl: str
 
@@ -63,8 +63,8 @@
 
 
 class Root(TypedDict):
     author: Author
     about: About
     primaryImageOfPage: Primaryimageofpage
     datePublished: str
-    sameAs: List[str]
+    sameAs: NotRequired[List[str]]
```

### Comparing `iwashi-3.0.0/src/iwashi/service/pixiv.py` & `iwashi-3.0.1/src/iwashi/service/pixiv.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/reddit.py` & `iwashi-3.0.1/src/iwashi/service/reddit.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/sketch.py` & `iwashi-3.0.1/src/iwashi/service/sketch.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/soundcloud.py` & `iwashi-3.0.1/src/iwashi/service/soundcloud.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/spotify.py` & `iwashi-3.0.1/src/iwashi/service/spotify.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/tiktok.py` & `iwashi-3.0.1/src/iwashi/service/tiktok.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/twitcasting.py` & `iwashi-3.0.1/src/iwashi/service/twitcasting.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/twitch.py` & `iwashi-3.0.1/src/iwashi/service/twitch.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/twitter.py` & `iwashi-3.0.1/src/iwashi/service/twitter.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/src/iwashi/service/youtube/youtube.py` & `iwashi-3.0.1/src/iwashi/service/youtube/youtube.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 import json
 import re
-from typing import Tuple
+from typing import Any
 from urllib import parse
 
 import bs4
 
-from iwashi.helper import BASE_HEADERS, HTTP_REGEX, traverse
+from iwashi.helper import HTTP_REGEX, normalize_url
+from iwashi.service.youtube.types.ytinitialdata2 import ProfileRes2
+from iwashi.service.youtube.types.ytinitialdata3 import ProfileRes3
 from iwashi.visitor import Context, Service
 
 from .types import thumbnails, ytinitialdata
 from .types.about import AboutRes
 
-VANITY_ID_REGEX = re.compile(r"youtube.com/@(?P<id>[\w-]+)")
+VANITY_ID_REGEX = re.compile(r"youtube.com/@(?P<id>[\w\-.]+)")
 
 
 class Youtube(Service):
     def __init__(self):
         super().__init__(
             name="Youtube",
             regex=re.compile(
                 HTTP_REGEX + r"((m|gaming)\.)?(youtube\.com|youtu\.be)",
             ),
         )
 
     async def resolve_id(self, context: Context, url: str) -> str | None:
-        uri = parse.urlparse(url)
+        normalized_url = normalize_url(url)
+        if normalized_url is None:
+            return None
+        uri = parse.urlparse(normalized_url)
         if uri.hostname == "youtu.be":
             return await self._channel_by_video(context, uri.path[1:])
         type = next(filter(None, uri.path.split("/")))
         if type.startswith("@"):
             return self._id_from_vanity_url(url)
         if type == "playlist":
             return None
         if type == "watch":
             return await self._channel_by_video(
                 context, parse.parse_qs(uri.query)["v"][0]
             )
         if type in ("channel", "user", "c"):
             return await self._channel_by_url(context, url)
-        return uri.path.split("/")[1]
+        if len(uri.path) > 1:
+            maybe_vanity = uri.path.split("/")[1]
+            return self._id_from_vanity_url(f"https://youtube.com/@{maybe_vanity}")
+        return None
 
     async def _channel_by_video(self, context: Context, video_id: str) -> str | None:
         result = await self._channel_by_oembed(context, video_id)
         if result is not None:
             return result
         response = await context.session.get(
             f"https://www.youtube.com/watch?v={video_id}"
@@ -93,84 +101,64 @@
             if thumbnail["width"] > size:
                 size = thumbnail["width"]
                 url = thumbnail["url"]
         if url is None:
             raise RuntimeError("Thumbnail not found")
         return url
 
-    def parse_token(
-        self, data: ytinitialdata
-    ) -> Tuple[str | None, Tuple[str, str] | None]:
-        # FIXME: 地獄
-        first_link: str | None = None
-        # c4TabbedHeaderRenderer = data["header"]["c4TabbedHeaderRenderer"]
-        c4TabbedHeaderRenderer = (
-            traverse(data)
-            .map(lambda x: x.get("header"))
-            .map(lambda x: x.get("c4TabbedHeaderRenderer"))
-            .get()
-        )
-        if (
-            c4TabbedHeaderRenderer is None
-            or "headerLinks" not in c4TabbedHeaderRenderer
-        ):
-            return (first_link, None)
-        first_link = (
-            traverse(c4TabbedHeaderRenderer)
-            .map(lambda x: x.get("headerLinks"))
-            .map(lambda x: x.get("channelHeaderLinksViewModel"))
-            .map(lambda x: x.get("firstLink"))
-            .map(lambda x: x.get("commandRuns"))
-            .map(lambda x: x[0])
-            .map(lambda x: x.get("onTap"))
-            .map(lambda x: x.get("innertubeCommand"))
-            .map(lambda x: x.get("urlEndpoint"))
-            .map(lambda x: x.get("url"))
-            .get()
-        )
-        endpoint = (
-            traverse(c4TabbedHeaderRenderer)
-            .map(lambda x: x.get("headerLinks"))
-            .map(lambda x: x.get("channelHeaderLinksViewModel"))
-            .map(lambda x: x.get("more"))
-            .map(lambda x: x.get("commandRuns"))
-            .map(lambda x: x[0])
-            .map(lambda x: x.get("onTap"))
-            .map(lambda x: x.get("innertubeCommand"))
-            .map(lambda x: x.get("showEngagementPanelEndpoint"))
-            .map(lambda x: x.get("engagementPanel"))
-            .map(lambda x: x.get("engagementPanelSectionListRenderer"))
-            .map(lambda x: x.get("content"))
-            .map(lambda x: x.get("sectionListRenderer"))
-            .map(lambda x: x.get("contents"))
-            .map(lambda x: x[0])
-            .map(lambda x: x.get("itemSectionRenderer"))
-            .map(lambda x: x.get("contents"))
-            .map(lambda x: x[0])
-            .map(lambda x: x.get("continuationItemRenderer"))
-            .map(lambda x: x.get("continuationEndpoint"))
-            .get()
-        )
-        if endpoint is None:
-            return (first_link, None)
-        api_url = endpoint["commandMetadata"]["webCommandMetadata"]["apiUrl"]
-        token = endpoint["continuationCommand"]["token"]
-        return (first_link, (api_url, token))
+    async def get_token(self, data: Any) -> str | None:
+        data2: ProfileRes2 = data
+        if "pageHeaderRenderer" in data2["header"]:
+            suffix = data2["header"]["pageHeaderRenderer"]["content"][
+                "pageHeaderViewModel"
+            ]["attribution"]["attributionViewModel"]["suffix"]
+            if not suffix:
+                return None
+            for a in suffix["commandRuns"]:
+                for b in a["onTap"]["innertubeCommand"]["showEngagementPanelEndpoint"][
+                    "engagementPanel"
+                ]["engagementPanelSectionListRenderer"]["content"][
+                    "sectionListRenderer"
+                ]["contents"]:
+                    for c in b["itemSectionRenderer"]["contents"]:
+                        endpoint = c["continuationItemRenderer"]["continuationEndpoint"]
+                        if endpoint["commandMetadata"]["webCommandMetadata"][
+                            "apiUrl"
+                        ].startswith("/youtubei/v1/browse"):
+                            return endpoint["continuationCommand"]["token"]
+        else:
+            data3: ProfileRes3 = data
+            for a in data3["header"]["c4TabbedHeaderRenderer"]["headerLinks"][
+                "channelHeaderLinksViewModel"
+            ]["more"]["commandRuns"]:
+                for b in a["onTap"]["innertubeCommand"]["showEngagementPanelEndpoint"][
+                    "engagementPanel"
+                ]["engagementPanelSectionListRenderer"]["content"][
+                    "sectionListRenderer"
+                ]["contents"]:
+                    for c in b["itemSectionRenderer"]["contents"]:
+                        endpoint = c["continuationItemRenderer"]["continuationEndpoint"]
+                        if endpoint["commandMetadata"]["webCommandMetadata"][
+                            "apiUrl"
+                        ].startswith("/youtubei/v1/browse"):
+                            return endpoint["continuationCommand"]["token"]
+        return None
 
     def parse_redirect(self, url: str) -> str:
         uri = parse.urlparse(url)
         if uri.hostname != "www.youtube.com":
             return url
         if uri.path == "/redirect":
             return parse.parse_qs(uri.query)["q"][0]
         return url
 
     async def visit(self, context: Context, id: str):
         url = f"https://www.youtube.com/@{id}"
         res = await context.session.get(url)
+
         res.raise_for_status()
         soup = bs4.BeautifulSoup(await res.text(), "html.parser")
         data = self.extract_initial_data(soup)
         vanity_id = data["metadata"]["channelMetadataRenderer"]["vanityChannelUrl"]
         name = data["metadata"]["channelMetadataRenderer"]["title"]
         description = data["metadata"]["channelMetadataRenderer"]["description"]
         profile_picture = self.parse_thumbnail(
@@ -180,48 +168,44 @@
             self,
             id=id,
             url=f"https://www.youtube.com/@{vanity_id.split('@')[1]}",
             name=name,
             description=description,
             profile_picture=profile_picture,
         )
-
-        first_link, api = self.parse_token(data)
-        if first_link is not None:
-            context.enqueue_visit(self.parse_redirect(first_link))
-        if api is None:
+        token = await self.get_token(data)
+        if token is None:
             return
-        api_url, token = api
         about_res = await context.session.post(
-            f"https://www.youtube.com{api_url}",
-            data=json.dumps(
-                {
-                    "context": {
-                        "client": {
-                            "userAgent": context.session.headers.get(
-                                "User-Agent", BASE_HEADERS["User-Agent"]
-                            ),
-                            "clientName": "WEB",
-                            "clientVersion": "2.20231219.04.00",
-                        }
+            "https://www.youtube.com/youtubei/v1/browse",
+            json={
+                "context": {
+                    "client": {
+                        "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36,gzip(gfe)",
+                        "clientName": "WEB",
+                        "clientVersion": "2.20240509.00.00",
                     },
-                    "continuation": token,
-                }
-            ),
+                },
+                "continuation": token,
+            },
         )
         about_res.raise_for_status()
         about_data: AboutRes = await about_res.json()
-        links = about_data["onResponseReceivedEndpoints"][0][
-            "appendContinuationItemsAction"
-        ]["continuationItems"][0]["aboutChannelRenderer"]["metadata"][
-            "aboutChannelViewModel"
-        ]["links"]
+        links: list[str] = []
+        for a in about_data["onResponseReceivedEndpoints"]:
+            for b in a["appendContinuationItemsAction"]["continuationItems"]:
+                for c in b["aboutChannelRenderer"]["metadata"]["aboutChannelViewModel"][
+                    "links"
+                ]:
+                    for d in c["channelExternalLinkViewModel"]["link"]["commandRuns"]:
+                        url = d["onTap"]["innertubeCommand"]["urlEndpoint"]["url"]
+                        links.append(url)
+
         for link in links:
-            link_url = link["channelExternalLinkViewModel"]["link"]["content"]
-            context.enqueue_visit(self.parse_redirect(link_url))
+            context.enqueue_visit(self.parse_redirect(link))
 
     def extract_initial_data(self, soup: bs4.BeautifulSoup) -> ytinitialdata:
         for script in soup.select("script"):
             if script.string is None:
                 continue
             match = re.search(r"ytInitialData\s*=\s*({.*?});", script.string)
             if match is not None:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `iwashi-3.0.0/src/iwashi/service/youtube/types/about.py` & `iwashi-3.0.1/src/iwashi/service/youtube/types/about.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,66 @@
-from __future__ import annotations
+from typing import TypedDict
 
-from typing import List, TypedDict
 
+class UrlEndpoint(TypedDict):
+    url: str
 
-class Title(TypedDict):
-    content: str
 
+class InnertubeCommand(TypedDict):
+    urlEndpoint: UrlEndpoint
 
-class Channelexternallinkviewmodel(TypedDict):
-    title: Title
-    link: Title
+
+class OnTap(TypedDict):
+    innertubeCommand: InnertubeCommand
+
+
+class CommandRunsItem(TypedDict):
+    onTap: OnTap
+
+
+type CommandRuns = list[CommandRunsItem]
+
+
+class Link(TypedDict):
+    commandRuns: CommandRuns
+
+
+class ChannelExternalLinkViewModel(TypedDict):
+    link: Link
 
 
 class LinksItem(TypedDict):
-    channelExternalLinkViewModel: Channelexternallinkviewmodel
+    channelExternalLinkViewModel: ChannelExternalLinkViewModel
+
 
+type Links = list[LinksItem]
 
-class Aboutchannelviewmodel(TypedDict):
-    description: str
-    links: List[LinksItem]
+
+class AboutChannelViewModel(TypedDict):
+    links: Links
 
 
 class Metadata(TypedDict):
-    aboutChannelViewModel: Aboutchannelviewmodel
+    aboutChannelViewModel: AboutChannelViewModel
 
 
-class Aboutchannelrenderer(TypedDict):
+class AboutChannelRenderer(TypedDict):
     metadata: Metadata
 
 
-class ContinuationitemsItem(TypedDict):
-    aboutChannelRenderer: Aboutchannelrenderer
+class ContinuationItemsItem(TypedDict):
+    aboutChannelRenderer: AboutChannelRenderer
+
+
+type ContinuationItems = list[ContinuationItemsItem]
 
 
-class Appendcontinuationitemsaction(TypedDict):
-    continuationItems: List[ContinuationitemsItem]
+class AppendContinuationItemsAction(TypedDict):
+    continuationItems: ContinuationItems
 
 
-class OnresponsereceivedendpointsItem(TypedDict):
-    appendContinuationItemsAction: Appendcontinuationitemsaction
+class OnResponseReceivedEndpointsItem(TypedDict):
+    appendContinuationItemsAction: AppendContinuationItemsAction
 
 
 class AboutRes(TypedDict):
-    onResponseReceivedEndpoints: List[OnresponsereceivedendpointsItem]
+    onResponseReceivedEndpoints: list[OnResponseReceivedEndpointsItem]
```

### Comparing `iwashi-3.0.0/src/iwashi/service/youtube/types/ytinitialdata.py` & `iwashi-3.0.1/src/iwashi/service/youtube/types/ytinitialdata.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/service_tester.py` & `iwashi-3.0.1/tests/service_tester.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_bandcamp.py` & `iwashi-3.0.1/tests/test_bandcamp.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_booth.py` & `iwashi-3.0.1/tests/test_booth.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_fanbox.py` & `iwashi-3.0.1/tests/test_fanbox.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_github.py` & `iwashi-3.0.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_instagram.py` & `iwashi-3.0.1/tests/test_instagram.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_itchio.py` & `iwashi-3.0.1/tests/test_itchio.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_kofi.py` & `iwashi-3.0.1/tests/test_kofi.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_linktree.py` & `iwashi-3.0.1/tests/test_linktree.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_litlink.py` & `iwashi-3.0.1/tests/test_litlink.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_mirrativ.py` & `iwashi-3.0.1/tests/test_mirrativ.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_nicovideo.py` & `iwashi-3.0.1/tests/test_nicovideo.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 async def test_nicovideo():
     service = Nicovideo()
     correct = Result(
         service=service,
         id="128134532",
         url="https://www.nicovideo.jp/user/128134532",
         name="ラベンダーP",
-        description="鉄道、東方、艦これ、ボカロ、ボイロ、野球、応援歌、阪神タイガース、千葉ロッテマリーンズ、埼玉西武ライオンズ、オリックスバファローズ、東方のすくすく白沢、艦これの連装砲ちゃんが好きな人です<br><br>2006年4月17日生まれで岡山県備前市日生町(カキオコで有名な町)に住んでます",
+        description="岡山県備前市日生町に住む2006年生まれの人 <br>好きなもの（鉄道、東方、艦これ、ボカロ、ボイロ、野球、中日、阪神、西武、オリックス、ロッテ、railwars、すくすく白沢）",
         profile_picture="https://secure-dcdn.cdn.nimg.jp/nicoaccount/usericon/12813/128134532.jpg?1710066983",
         links={
             "https://www.youtube.com/channel/UC4jehnRY1GBPBpg-Np4WFNg",
             "https://twitter.com/lavenderp2018",
         },
     )
     await _test_service(service, correct, "https://www.nicovideo.jp/user/128134532")
```

### Comparing `iwashi-3.0.0/tests/test_note.py` & `iwashi-3.0.1/tests/test_note.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_patreon.py` & `iwashi-3.0.1/tests/test_patreon.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_pixiv.py` & `iwashi-3.0.1/tests/test_pixiv.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_reddit.py` & `iwashi-3.0.1/tests/test_reddit.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_sketch.py` & `iwashi-3.0.1/tests/test_sketch.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_soundcloud.py` & `iwashi-3.0.1/tests/test_soundcloud.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_spotify.py` & `iwashi-3.0.1/tests/test_spotify.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_tiktok.py` & `iwashi-3.0.1/tests/test_tiktok.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_twitcasting.py` & `iwashi-3.0.1/tests/test_twitcasting.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_twitch.py` & `iwashi-3.0.1/tests/test_twitch.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/tests/test_twitter.py` & `iwashi-3.0.1/tests/test_twitter.py`

 * *Files identical despite different names*

### Comparing `iwashi-3.0.0/LICENSE` & `iwashi-3.0.1/LICENSE`

 * *Files identical despite different names*

