# Comparing `tmp/xklb-2.8.6.tar.gz` & `tmp/xklb-2.8.7.tar.gz`

## Comparing `xklb-2.8.6.tar` & `xklb-2.8.7.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.8.6/.gitattributes
--rw-r--r--   0        0        0   216245 2020-02-02 00:00:00.000000 xklb-2.8.6/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/examples/art.avif
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/workflows/green.yaml
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/__init__.py
--rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/lb.py
--rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/media_printer.py
--rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/readme.py
--rw-r--r--   0        0        0   112540 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/__init__.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/av.py
--rw-r--r--   0        0        0    20488 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/fs_add.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/gallery_add.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/gallery_backend.py
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/hn_add.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/links_add.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/places_import.py
--rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/reddit_add.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/row_add.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/site_add.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/substack.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/subtitle.py
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/tabs_add.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/tildes.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/tube_add.py
--rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/tube_backend.py
--rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/data/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/__init__.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/dedupe_db.py
--rw-r--r--   0        0        0    18995 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/dedupe_media.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/merge_online_local.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/mpv_watchlater.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/pushshift.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/reddit_selftext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/files/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/files/christen.py
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/files/sample_compare.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/files/sample_hash.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/files/similar_files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/__init__.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/big_dirs.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/merge_folders.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/mount_stats.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/move_list.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/rel_mv.py
--rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/scatter.py
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/similar_folders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/fsdb/__init__.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/fsdb/disk_usage.py
--rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/fsdb/search_db.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/__init__.py
--rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/block.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/db_history.py
--rw-r--r--   0        0        0    19221 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/db_media.py
--rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/db_playlists.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/download.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/download_status.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/history.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/history_add.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/optimize_db.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/playlists.py
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/redownload.py
--rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/search.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/stats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediafiles/__init__.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediafiles/media_check.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediafiles/process_ffmpeg.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediafiles/process_image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/misc/__init__.py
--rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/misc/dedupe_czkawka.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/misc/export_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/multidb/__init__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/multidb/copy_play_counts.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/multidb/merge_dbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/__init__.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/links_open.py
--rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/media_player.py
--rw-r--r--   0        0        0    11678 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/play_actions.py
--rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/playback_control.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/post_actions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/surf.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/tabs_open.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/tablefiles/__init__.py
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/tablefiles/eda.py
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/tablefiles/incremental_diff.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/tablefiles/mcda.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/__init__.py
--rw-r--r--   0        0        0    12694 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/cluster_sort.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/extract_links.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/extract_text.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/markdown_links.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/nouns.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/__init__.py
--rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    29962 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/consts.py
--rw-r--r--   0        0        0     9380 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/devices.py
--rw-r--r--   0        0        0    15831 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/nums.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/objects.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/printing.py
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/processes.py
--rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0    15672 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/sqlgroups.py
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/strings.py
--rw-r--r--   0        0        0    23222 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/web.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/assets/__init__.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.8.6/.gitignore
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 xklb-2.8.6/pyproject.toml
--rw-r--r--   0        0        0   156256 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/README.md
--rw-r--r--   0        0        0   160037 2020-02-02 00:00:00.000000 xklb-2.8.6/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.8.7/.gitattributes
+-rw-r--r--   0        0        0   216245 2020-02-02 00:00:00.000000 xklb-2.8.7/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/examples/art.avif
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/__init__.py
+-rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/lb.py
+-rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/media_printer.py
+-rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/readme.py
+-rw-r--r--   0        0        0   112540 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/__init__.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/av.py
+-rw-r--r--   0        0        0    20579 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/fs_add.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/gallery_add.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/gallery_backend.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/hn_add.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/links_add.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/places_import.py
+-rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/reddit_add.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/row_add.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/site_add.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/substack.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/subtitle.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/tabs_add.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/tildes.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/tube_add.py
+-rw-r--r--   0        0        0    20249 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/tube_backend.py
+-rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/createdb/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/data/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/__init__.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/dedupe_db.py
+-rw-r--r--   0        0        0    18995 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/dedupe_media.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/merge_online_local.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/mpv_watchlater.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/pushshift.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/editdb/reddit_selftext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/files/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/files/christen.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/files/sample_compare.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/files/sample_hash.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/files/similar_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/__init__.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/big_dirs.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/merge_folders.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/mount_stats.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/move_list.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/rel_mv.py
+-rw-r--r--   0        0        0    11782 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/scatter.py
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/folders/similar_folders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/fsdb/__init__.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/fsdb/disk_usage.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/fsdb/search_db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/__init__.py
+-rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/block.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/db_history.py
+-rw-r--r--   0        0        0    19259 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/db_media.py
+-rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/db_playlists.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/download.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/download_status.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/history.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/history_add.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/optimize_db.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/playlists.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/redownload.py
+-rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/search.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediadb/stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediafiles/__init__.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediafiles/media_check.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediafiles/process_ffmpeg.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/mediafiles/process_image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/misc/__init__.py
+-rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/misc/dedupe_czkawka.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/misc/export_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/multidb/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/multidb/copy_play_counts.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/multidb/merge_dbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/links_open.py
+-rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/media_player.py
+-rw-r--r--   0        0        0    11690 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/play_actions.py
+-rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/playback_control.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/post_actions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/surf.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/playback/tabs_open.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/tablefiles/__init__.py
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/tablefiles/eda.py
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/tablefiles/incremental_diff.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/tablefiles/mcda.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/__init__.py
+-rw-r--r--   0        0        0    12694 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/cluster_sort.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/extract_links.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/extract_text.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/markdown_links.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/text/nouns.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    29978 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/consts.py
+-rw-r--r--   0        0        0     9522 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15831 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/nums.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/processes.py
+-rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0    15807 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/sqlgroups.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/strings.py
+-rw-r--r--   0        0        0    23222 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/utils/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/assets/__init__.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.8.7/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.8.7/.gitignore
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 xklb-2.8.7/pyproject.toml
+-rw-r--r--   0        0        0   156256 2020-02-02 00:00:00.000000 xklb-2.8.7/.github/README.md
+-rw-r--r--   0        0        0   160037 2020-02-02 00:00:00.000000 xklb-2.8.7/PKG-INFO
```

### Comparing `xklb-2.8.6/pdm.lock` & `xklb-2.8.7/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/.github/LICENSE` & `xklb-2.8.7/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/.github/Windows.md` & `xklb-2.8.7/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/.github/examples/art.avif` & `xklb-2.8.7/.github/examples/art.avif`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/.github/examples/extract.svg` & `xklb-2.8.7/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/.github/examples/tubeadd.svg` & `xklb-2.8.7/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/.github/workflows/push.yaml` & `xklb-2.8.7/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/lb.py` & `xklb-2.8.7/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/media_printer.py` & `xklb-2.8.7/xklb/media_printer.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/readme.py` & `xklb-2.8.7/xklb/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/usage.py` & `xklb-2.8.7/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/createdb/av.py` & `xklb-2.8.7/xklb/createdb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/createdb/fs_add.py` & `xklb-2.8.7/xklb/createdb/fs_add.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     consts,
     db_utils,
     file_utils,
     iterables,
     nums,
     objects,
     path_utils,
+    printing,
     processes,
     strings,
 )
 from xklb.utils.consts import SC, DBType
 from xklb.utils.log_utils import log
 
 REGEX_SENTENCE_ENDS = re.compile(r";|,|\.|\*|\n|\t")
@@ -62,14 +63,15 @@
     )
     arggroups.debug(parser)
 
     arggroups.database(parser)
     if action == SC.fs_add:
         parser.add_argument("paths", nargs="+")
     args = parser.parse_intermixed_args()
+    arggroups.args_post(args, parser, create_db=action == SC.fs_add)
 
     if not args.profiles:
         args.profiles = [DBType.video]
 
     if args.move:
         args.move = Path(args.move).expanduser().resolve()
 
@@ -79,15 +81,14 @@
     if not which("ffprobe") and (DBType.audio in args.profiles or DBType.video in args.profiles):
         log.error("ffmpeg is not installed. Install it with your package manager.")
         raise SystemExit(3)
 
     arggroups.process_ffmpeg_post(args)
     arggroups.media_check_post(args)
 
-    arggroups.args_post(args, parser, create_db=action == SC.fs_add)
     return args
 
 
 def munge_book_tags(path) -> dict:
     try:
         import textract  # type: ignore
     except ModuleNotFoundError:
@@ -532,22 +533,25 @@
             pool_fn = ThreadPoolExecutor
         else:
             pool_fn = ProcessPoolExecutor
 
         with pool_fn(n_jobs) as parallel:
             for idx, chunk_paths in enumerate(files_chunked):
                 percent = ((batch_count * idx) + len(chunk_paths)) / len(new_files) * 100
-                print(f"[{path}] Extracting metadata {percent:3.1f}% (chunk {idx + 1} of {chunks_count})")
+                printing.print_overwrite(
+                    f"[{path}] Extracting metadata {percent:3.1f}% (chunk {idx + 1} of {chunks_count})"
+                )
 
                 mp_args = argparse.Namespace(
                     playlist_path=path, **{k: v for k, v in args.__dict__.items() if k not in {"db"}}
                 )
                 metadata = parallel.map(partial(extract_metadata, mp_args), chunk_paths)
                 metadata = list(filter(None, metadata))
                 extract_chunk(args, metadata)
+            print()
 
     return len(new_files)
 
 
 def extractor(args, paths) -> None:
     new_files = 0
     for path in paths:
```

### Comparing `xklb-2.8.6/xklb/createdb/gallery_add.py` & `xklb-2.8.7/xklb/createdb/gallery_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/createdb/gallery_backend.py` & `xklb-2.8.7/xklb/createdb/gallery_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/createdb/hn_add.py` & `xklb-2.8.7/xklb/createdb/hn_add.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 def parse_args(prog, usage) -> argparse.Namespace:
     parser = argparse_utils.ArgumentParser(prog, usage)
     parser.add_argument("--oldest", action="store_true")
     arggroups.requests(parser)
     arggroups.debug(parser)
     arggroups.database(parser)
     args = parser.parse_args()
-
     arggroups.args_post(args, parser, create_db=True)
+
     return args
 
 
 def db_worker(args, input_queue):
     conn = sqlite3.connect(args.database, isolation_level=None)
     db_conn = db_utils.connect(args, conn)
     while True:
```

### Comparing `xklb-2.8.6/xklb/createdb/links_add.py` & `xklb-2.8.7/xklb/createdb/links_add.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -39,23 +39,23 @@
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
     if "add" in action:
         arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
+    arggroups.args_post(args, parser, create_db=True)
 
     if args.auto_pager:
         args.fixed_pages = 1
 
     arggroups.extractor_post(args)
     arggroups.filter_links_post(args)
     arggroups.selenium_post(args)
 
-    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def add_playlist(args, path):
     info = {
         "hostname": urlparse(path).hostname,
         "category": getattr(args, "category", None) or "Uncategorized",
```

### Comparing `xklb-2.8.6/xklb/createdb/places_import.py` & `xklb-2.8.7/xklb/createdb/places_import.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 def parse_args() -> argparse.Namespace:
     parser = argparse_utils.ArgumentParser(prog="library places-import", usage=usage.places_import)
     arggroups.database(parser)
     parser.add_argument("paths", nargs="+")
     arggroups.debug(parser)
     args = parser.parse_intermixed_args()
-
     arggroups.args_post(args, parser, create_db=True)
+
     return args
 
 
 def google_maps_takeout(df):
     import pandas as pd
 
     new_df = pd.DataFrame()
```

### Comparing `xklb-2.8.6/xklb/createdb/reddit_add.py` & `xklb-2.8.7/xklb/createdb/reddit_add.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,27 +55,27 @@
     parser.add_argument("--redditors", action="store_true")
 
     arggroups.debug(parser)
     arggroups.database(parser)
     if action == "redditadd":
         parser.add_argument("paths", nargs="+")
     args = parser.parse_intermixed_args()
+    arggroups.args_post(args, parser, create_db=True)
 
     if action == "redditadd":
         args.paths = iterables.conform(args.paths)
 
     try:
         import praw
 
         args.reddit = praw.Reddit(args.praw_site, config_interpolation="basic")
     except Exception as e:
         print(PRAW_SETUP_INSTRUCTIONS)
         raise SystemExit(e) from e
 
-    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 """
 Catherine Devlin's reddit-to-sqlite project was very helpful in understanding
 how to work with praw. Any lines of code which can be attributed to that person
 should be.
```

### Comparing `xklb-2.8.6/xklb/createdb/row_add.py` & `xklb-2.8.7/xklb/createdb/row_add.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 from xklb import usage
 from xklb.utils import arggroups, argparse_utils, nums
 
 
+def parse_utils():
+    parser = argparse_utils.ArgumentParser(description="Add arbitrary rows to a SQLITE db", usage=usage.row_add)
+    parser.add_argument("--table-name", "--table", "-t", default="media")
+    arggroups.debug(parser)
+
+    arggroups.database(parser)
+    args, unknown_args = parser.parse_known_args()
+    arggroups.args_post(args, parser, create_db=True)
+    return args, unknown_args
+
+
 def parse_unknown_args_to_dict(unknown_args):
     kwargs = {}
     key = None
     values = []
 
     def get_val():
         if len(values) == 1:
@@ -26,18 +37,11 @@
     if len(values) > 0:
         kwargs[key] = get_val()
 
     return kwargs
 
 
 def row_add():
-    parser = argparse_utils.ArgumentParser(description="Add arbitrary rows to a SQLITE db", usage=usage.row_add)
-    parser.add_argument("--table-name", "--table", "-t", default="media")
-    arggroups.debug(parser)
-
-    arggroups.database(parser)
-    args, unknown_args = parser.parse_known_args()
-
-    arggroups.args_post(args, parser, create_db=True)
+    args, unknown_args = parse_utils()
 
     kwargs = parse_unknown_args_to_dict(unknown_args)
-    args.db[args.table_name].insert(kwargs, alter=True)  # type: ignore
+    args.db[args.table_name].insert(kwargs, alter=True)
```

### Comparing `xklb-2.8.6/xklb/createdb/site_add.py` & `xklb-2.8.7/xklb/createdb/site_add.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,18 @@
     parser.add_argument("--extract-html", action="store_true", help="Extract data from HTML")
     parser.add_argument("--extract-xml", action="store_true", help="Extract data from XML")
 
     arggroups.debug(parser)
     arggroups.database(parser)
     arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
+    arggroups.args_post(args, parser, create_db=True)
 
     arggroups.selenium_post(args)
 
-    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def extract_tables(dict_, table_name):
     dict_ = objects.flatten_dict_single_parents(dict_)
     dict_ = objects.flatten_grandparents(dict_)
```

### Comparing `xklb-2.8.6/xklb/createdb/substack.py` & `xklb-2.8.7/xklb/createdb/substack.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     parser = argparse_utils.ArgumentParser(prog="library substack", usage=usage.substack)
     arggroups.requests(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("paths", nargs="+", help="Substack path to extract article for")
     args = parser.parse_intermixed_args()
-
     arggroups.args_post(args, parser, create_db=True)
+
     return args
 
 
 def save_page(args, url):
     response = web.get(args, url)
     if response:
         soup = BeautifulSoup(response.text, "lxml")
```

### Comparing `xklb-2.8.6/xklb/createdb/subtitle.py` & `xklb-2.8.7/xklb/createdb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/createdb/tabs_add.py` & `xklb-2.8.7/xklb/createdb/tabs_add.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 
     parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
     parser.add_argument("--allow-immediate", action="store_true")
     arggroups.debug(parser)
     arggroups.database(parser)
     arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
+    arggroups.args_post(args, parser, create_db=True)
 
     arggroups.extractor_post(args)
     arggroups.frequency_post(args)
 
-    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def get_days(frequency):
     d = {"weekly": 7, "monthly": 30, "quarterly": 89, "yearly": 364, "decadally": 3640}
     return d.get(frequency, 7)
```

### Comparing `xklb-2.8.6/xklb/createdb/tildes.py` & `xklb-2.8.7/xklb/createdb/tildes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     parser = argparse_utils.ArgumentParser(prog="library tildes", usage=usage.tildes)
     arggroups.requests(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("username", help="Tildes.net user to extract comments for")
     args = parser.parse_intermixed_args()
-
     arggroups.args_post(args, parser, create_db=True)
+
     return args
 
 
 def save_page(args, text):
     soup = BeautifulSoup(text, "lxml")
 
     comment_elements = soup.find_all("article", class_="comment")
```

### Comparing `xklb-2.8.6/xklb/createdb/tube_add.py` & `xklb-2.8.7/xklb/createdb/tube_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     if action == SC.tube_add:
         arggroups.paths_or_stdin(parser)
 
     args = parser.parse_intermixed_args()
     arggroups.args_post(args, parser, create_db=action == SC.tube_add)
 
     arggroups.extractor_post(args)
+
     return args
 
 
 def tube_add(args=None) -> None:
     if args:
         sys.argv = ["tubeadd", *args]
```

### Comparing `xklb-2.8.6/xklb/createdb/tube_backend.py` & `xklb-2.8.7/xklb/createdb/tube_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,16 +210,15 @@
                 "ignoreerrors": True,
             },
             playlist_opts=playlist_dl_opts,
         )
     ) as ydl:
         videos = set(
             args.db.execute(
-                f"""
-                SELECT
+                f"""SELECT
                     id
                     , path
                     , null as playlists_id
                 FROM media
                 WHERE COALESCE(time_deleted, 0)=0
                     AND path = ?
                     {'and width is null' if 'width' in m_columns else ''}
@@ -227,16 +226,15 @@
                 [playlist_path],
             ).fetchall()
         )
 
         if "playlists" in tables:
             videos |= set(
                 args.db.execute(
-                    f"""
-                    SELECT
+                    f"""SELECT
                         id
                         , path
                         , playlists_id
                     FROM media
                     WHERE COALESCE(time_deleted, 0)=0
                         AND playlists_id = (select id from playlists where path = ?)
                         {'AND width is null' if 'width' in m_columns else ''}
```

### Comparing `xklb-2.8.6/xklb/createdb/web_add.py` & `xklb-2.8.7/xklb/createdb/web_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/data/imagemagick_errors.py` & `xklb-2.8.7/xklb/data/imagemagick_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/data/wordbank.py` & `xklb-2.8.7/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/data/yt_dlp_errors.py` & `xklb-2.8.7/xklb/data/yt_dlp_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/editdb/dedupe_db.py` & `xklb-2.8.7/xklb/editdb/dedupe_db.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         help="Comma separated business keys",
     )
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("target_table")
     args = parser.parse_intermixed_args()
-
     arggroups.args_post(args, parser, create_db=True)
+
     return args
 
 
 def dedupe_rows(args, tablename, primary_keys, business_keys):
     with args.db.conn:
         args.db.conn.execute(
             f"""
```

### Comparing `xklb-2.8.6/xklb/editdb/dedupe_media.py` & `xklb-2.8.7/xklb/editdb/dedupe_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/editdb/merge_online_local.py` & `xklb-2.8.7/xklb/editdb/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/editdb/mpv_watchlater.py` & `xklb-2.8.7/xklb/editdb/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/editdb/pushshift.py` & `xklb-2.8.7/xklb/editdb/pushshift.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 def parse_args(action, usage) -> argparse.Namespace:
     parser = argparse_utils.ArgumentParser(prog="library " + action, usage=usage)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     args = parser.parse_args()
-
     arggroups.args_post(args, parser, create_db=True)
+
     return args
 
 
 def save_data(args, reddit_posts, media) -> None:
     if len(reddit_posts) > 0:
         args.db["reddit_posts"].insert_all(reddit_posts, alter=True)
         reddit_posts.clear()
```

### Comparing `xklb-2.8.6/xklb/editdb/reddit_selftext.py` & `xklb-2.8.7/xklb/editdb/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/files/christen.py` & `xklb-2.8.7/xklb/files/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/files/sample_compare.py` & `xklb-2.8.7/xklb/files/sample_compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
     arggroups.args_post(args, parser)
 
     arggroups.sample_hash_bytes_post(args)
+
     return args
 
 
 def full_hash_file(path):
     sha256_hash = hashlib.sha256()
 
     try:
```

### Comparing `xklb-2.8.6/xklb/files/sample_hash.py` & `xklb-2.8.7/xklb/files/sample_hash.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/files/similar_files.py` & `xklb-2.8.7/xklb/files/similar_files.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/folders/big_dirs.py` & `xklb-2.8.7/xklb/folders/big_dirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/folders/merge_folders.py` & `xklb-2.8.7/xklb/folders/merge_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/folders/mount_stats.py` & `xklb-2.8.7/xklb/folders/mount_stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/folders/move_list.py` & `xklb-2.8.7/xklb/folders/move_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             if not args.folder_counts(pdict["count"]):
                 d.pop(path)
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def get_table(args) -> list[dict]:
-    media = list(args.db.query(*sqlgroups.fs_sql(args)))
+    media = list(args.db.query(*sqlgroups.fs_sql(args, limit=None)))
 
     folders = group_by_folder(args, media)
     return sorted(folders, key=lambda x: x["size"] / x["count"])
 
 
 def iterate_and_show_options(args, tbl) -> tuple[list[dict], list[dict]]:
     vew = tbl[-int(args.limit) :] if args.limit else tbl
```

### Comparing `xklb-2.8.6/xklb/folders/rel_mv.py` & `xklb-2.8.7/xklb/folders/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/folders/scatter.py` & `xklb-2.8.7/xklb/folders/scatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, math, random, sys, tempfile
+import argparse, math, os, random, sys, tempfile
 from collections import Counter
 from pathlib import Path
 
 from humanize import naturalsize
 
 from xklb import usage
 from xklb.utils import arggroups, argparse_utils, consts, db_utils, devices, file_utils, iterables, nums, printing
@@ -22,15 +22,15 @@
     parser.add_argument("--sort", default="random()", help="Sort files before moving")
     parser.add_argument("--targets", "--srcmounts", "-m", help="Colon separated destinations eg. /mnt/d1:/mnt/d2")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument(
         "relative_paths",
-        nargs="+",
+        nargs="*",
         help="Paths to scatter; if using -m any path substring is valid (relative to the root of your mergerfs mount)",
     )
     args = parser.parse_intermixed_args()
     arggroups.args_post(args, parser)
 
     if args.targets:
         args.targets = [m.rstrip("\\/") for m in args.targets.split(":")]
@@ -59,14 +59,15 @@
 
     return args
 
 
 def get_table(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
     or_paths = [f"path like :path_{i}" for i, _path in enumerate(args.relative_paths)]
+    or_paths_sql = f"and ({' or '.join(or_paths)})"
 
     media = list(
         args.db.query(
             f"""
         select
             path
             , size
@@ -74,32 +75,39 @@
             , time_modified
             , time_downloaded
         from media
         where 1=1
             and coalesce(time_deleted, 0)=0
             and path not like "http%"
             {'and coalesce(is_dir, 0)=0' if 'is_dir' in m_columns else ""}
-            and ({' or '.join(or_paths)})
+            {or_paths_sql if args.relative_paths else ''}
         order by {args.sort}
         {'limit :limit' if args.limit else ''}
         """,
             {
                 "limit": args.limit,
-                **{f"path_{i}": f"%{path}%" for i, path in enumerate(args.relative_paths) if args.relative_paths},
+                **{
+                    f"path_{i}": f"{path}%" if path.startswith(os.sep) else f"%{path}%"
+                    for i, path in enumerate(args.relative_paths)
+                    if args.relative_paths
+                },
             },
         ),
     )
 
     return media
 
 
 def get_path_stats(args, data) -> list[dict]:
     read_only_mounts = [
         s for s in args.relative_paths if Path(s).is_absolute() and not any(m in s for m in args.targets)
     ]
+    if read_only_mounts:
+        log.info("Treating as depletion targets: %s", read_only_mounts)
+
     result = []
     for srcmount in args.targets + read_only_mounts:
         disk_files = [d for d in data if d["path"].startswith(srcmount)]
         if disk_files:
             result.append(
                 {
                     "mount": srcmount,
```

### Comparing `xklb-2.8.6/xklb/folders/similar_folders.py` & `xklb-2.8.7/xklb/folders/similar_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/fsdb/disk_usage.py` & `xklb-2.8.7/xklb/fsdb/disk_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     parser.add_argument("--folders-only", "-td", action="store_true", help="Only print folders")
     parser.add_argument("--files-only", "-tf", action="store_true", help="Only print files")
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
-    parser.add_argument("search", nargs="*", default=os.sep)
+    parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
     arggroups.args_post(args, parser)
 
     arggroups.sql_fs_post(args)
     arggroups.group_folders_post(args)
 
     return args
@@ -87,15 +87,15 @@
         processes.no_media_found()
 
     args.cwd = os.sep.join(args.subset[0]["path"].split(os.sep)[: level - 1]) + os.sep
     return args.cwd, args.subset
 
 
 def get_data(args) -> list[dict]:
-    media = list(args.db.query(*sqlgroups.fs_sql(args)))
+    media = list(args.db.query(*sqlgroups.fs_sql(args, limit=None)))
 
     if not media:
         processes.no_media_found()
     return media
 
 
 def disk_usage():
```

### Comparing `xklb-2.8.6/xklb/fsdb/search_db.py` & `xklb-2.8.7/xklb/fsdb/search_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,17 @@
     arggroups.sql_fs(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search_table")
     parser.add_argument("search", nargs="+")
     args = parser.parse_intermixed_args()
+    arggroups.args_post(args, parser, create_db=True)
 
     arggroups.sql_fs_post(args)
-
-    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def get_table_name(args):
     if args.search_table in args.db.table_names():
         return args.search_table
```

### Comparing `xklb-2.8.6/xklb/mediadb/block.py` & `xklb-2.8.7/xklb/mediadb/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/mediadb/db_history.py` & `xklb-2.8.7/xklb/mediadb/db_history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/mediadb/db_media.py` & `xklb-2.8.7/xklb/mediadb/db_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,15 +444,15 @@
             GROUP BY m.id, m.path
         )
         SELECT *
         FROM m
         ORDER BY play_count
             , path
             {'' if 'sort' in args.defaults else ', ' + args.sort}
-        {sql_utils.limit_sql(args)}
+        {sql_utils.limit_sql(args.limit, args.offset)}
     """
 
     bindings = {**playlists_params}
     bindings = {**bindings, **{k: v for k, v in args.filter_bindings.items() if k.startswith("FTS")}}
 
     media = list(args.db.query(query, bindings))
     log.debug("len(playlist_media) = %s", len(media))
@@ -539,15 +539,15 @@
         FROM m
         WHERE 1=1
             {'' if args.related >= consts.RELATED_NO_FILTER else (" ".join(args.aggregate_filter_sql) or '')}
         ORDER BY play_count
             , m.path like "http%"
             , {'rank' if 'sort' in args.defaults else f'ntile(1000) over (order by rank)' + (f', {args.sort}' if args.sort else '')}
             , path
-        {sql_utils.limit_sql(args, limit_adj=-1)}
+        {sql_utils.limit_sql(args.limit, args.offset, limit_adj=-1)}
     """
 
     bindings = {"path": m["path"]}
     if args.related >= consts.RELATED_NO_FILTER:
         bindings = {**bindings, **{k: v for k, v in args.filter_bindings.items() if k.startswith("FTS")}}
     else:
         bindings = {**bindings, **args.filter_bindings}
```

### Comparing `xklb-2.8.6/xklb/mediadb/db_playlists.py` & `xklb-2.8.7/xklb/mediadb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/mediadb/download.py` & `xklb-2.8.7/xklb/mediadb/download.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,16 +74,16 @@
     parser.add_argument("--photos", action="store_true", help="Image: Download JPG and WEBP")
     parser.add_argument("--drawings", action="store_true", help="Image: Download PNG")
     parser.add_argument("--gifs", action="store_true", help="Image: Download MP4 and GIFs")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     arggroups.paths_or_stdin(parser)
-    parser.set_defaults(paths=None, fts=False)
 
+    parser.set_defaults(paths=None, fts=False)
     args, unk = parser.parse_known_intermixed_args()
     arggroups.args_post(args, parser)
 
     if unk and not args.profile in (DBType.video, DBType.audio):
         parser.error(f"unrecognized arguments: {' '.join(unk)}")
     args.unk = unk
```

### Comparing `xklb-2.8.6/xklb/mediadb/download_status.py` & `xklb-2.8.7/xklb/mediadb/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/mediadb/history.py` & `xklb-2.8.7/xklb/mediadb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/mediadb/history_add.py` & `xklb-2.8.7/xklb/mediadb/history_add.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     arggroups.extractor(parser)
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
     arggroups.paths_or_stdin(parser)
     args = parser.parse_intermixed_args()
+    arggroups.args_post(args, parser, create_db=True)
 
     arggroups.extractor_post(args)
 
-    arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def history_add() -> None:
     args = parse_args(prog="library history-add", usage=usage.history_add)
 
     history_exists = set()
```

### Comparing `xklb-2.8.6/xklb/mediadb/playlists.py` & `xklb-2.8.7/xklb/mediadb/playlists.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
     arggroups.sql_fs(parser)
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
+
+    parser.set_defaults(fts=False)
     args = parser.parse_intermixed_args()
     arggroups.args_post(args, parser)
 
     arggroups.sql_fs_post(args)
 
     return args
```

### Comparing `xklb-2.8.6/xklb/mediadb/redownload.py` & `xklb-2.8.7/xklb/mediadb/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/mediadb/search.py` & `xklb-2.8.7/xklb/mediadb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/mediadb/stats.py` & `xklb-2.8.7/xklb/mediadb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/mediafiles/media_check.py` & `xklb-2.8.7/xklb/mediafiles/media_check.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/mediafiles/process_ffmpeg.py` & `xklb-2.8.7/xklb/mediafiles/process_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/mediafiles/process_image.py` & `xklb-2.8.7/xklb/mediafiles/process_image.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/misc/dedupe_czkawka.py` & `xklb-2.8.7/xklb/misc/dedupe_czkawka.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/misc/export_text.py` & `xklb-2.8.7/xklb/misc/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/multidb/copy_play_counts.py` & `xklb-2.8.7/xklb/multidb/copy_play_counts.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     parser.add_argument("--source-prefix", default="")
     parser.add_argument("--target-prefix", default="")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("source_dbs", nargs="+")
     args = parser.parse_intermixed_args()
-
     arggroups.args_post(args, parser, create_db=True)
+
     return args
 
 
 def copy_play_count(args, source_db) -> None:
     s_db = db_utils.connect(argparse.Namespace(database=source_db, verbose=args.verbose))
     m_columns = s_db["media"].columns_dict
```

### Comparing `xklb-2.8.6/xklb/multidb/merge_dbs.py` & `xklb-2.8.7/xklb/multidb/merge_dbs.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     parser.add_argument("--where", "-w", nargs="+", action="extend", help=argparse.SUPPRESS)
 
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("source_dbs", nargs="+")
     args = parser.parse_intermixed_args()
-
     arggroups.args_post(args, parser, create_db=True)
+
     return args
 
 
 def merge_db(args, source_db) -> None:
     source_db = str(Path(source_db).resolve())
 
     s_db = db_utils.connect(args, conn=sqlite3.connect(args.database))
```

### Comparing `xklb-2.8.6/xklb/playback/links_open.py` & `xklb-2.8.7/xklb/playback/links_open.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     parser.add_argument("--browser")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
 
-    parser.set_defaults(limit="7")
+    parser.set_defaults(limit="7", fts=False)
     args = parser.parse_intermixed_args()
     arggroups.args_post(args, parser)
 
     arggroups.sql_fs_post(args)
 
     if not args.title_prefix:
         args.title_prefix = ["https://www.google.com/search?q=%"]
```

### Comparing `xklb-2.8.6/xklb/playback/media_player.py` & `xklb-2.8.7/xklb/playback/media_player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/playback/play_actions.py` & `xklb-2.8.7/xklb/playback/play_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
             else:
                 media.extend([{"path": s} for s in file_utils.rglob(str(p))[0]])
     return media
 
 
 def process_playqueue(args) -> None:
     if args.action == SC.filesystem:
-        query, bindings = sqlgroups.fs_sql(args)
+        query, bindings = sqlgroups.fs_sql(args, args.limit)
     else:
         db_history.create(args)
         query, bindings = sqlgroups.media_sql(args)
 
     if args.print and not any(
         [
             args.partial,
```

### Comparing `xklb-2.8.6/xklb/playback/playback_control.py` & `xklb-2.8.7/xklb/playback/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/playback/post_actions.py` & `xklb-2.8.7/xklb/playback/post_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/playback/surf.py` & `xklb-2.8.7/xklb/playback/surf.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/playback/tabs_open.py` & `xklb-2.8.7/xklb/playback/tabs_open.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     )
 
     arggroups.sql_fs(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
+
+    parser.set_defaults(fts=False)
     args = parser.parse_intermixed_args()
     arggroups.args_post(args, parser)
 
     arggroups.sql_fs_post(args)
     return args
```

### Comparing `xklb-2.8.6/xklb/scratch/javguru.py` & `xklb-2.8.7/xklb/scratch/javguru.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/scratch/javtiful.py` & `xklb-2.8.7/xklb/scratch/javtiful.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/scratch/mam_search.py` & `xklb-2.8.7/xklb/scratch/mam_search.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     parser.add_argument("--cookie", required=True)
     arggroups.requests(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search_text", nargs="+")
     args = parser.parse_intermixed_args()
-
     arggroups.args_post(args, parser, create_db=True)
+
     return args
 
 
 def get_page(args, query_data):
     import pandas as pd
 
     response = web.requests_session(args).post(
```

### Comparing `xklb-2.8.6/xklb/scratch/mam_slots.py` & `xklb-2.8.7/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/tablefiles/eda.py` & `xklb-2.8.7/xklb/tablefiles/eda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/tablefiles/incremental_diff.py` & `xklb-2.8.7/xklb/tablefiles/incremental_diff.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/tablefiles/mcda.py` & `xklb-2.8.7/xklb/tablefiles/mcda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/text/cluster_sort.py` & `xklb-2.8.7/xklb/text/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/text/extract_links.py` & `xklb-2.8.7/xklb/text/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/text/extract_text.py` & `xklb-2.8.7/xklb/text/extract_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/text/markdown_links.py` & `xklb-2.8.7/xklb/text/markdown_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/text/nouns.py` & `xklb-2.8.7/xklb/text/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/arg_utils.py` & `xklb-2.8.7/xklb/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/arggroups.py` & `xklb-2.8.7/xklb/utils/arggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     while frame:
         frame = frame.f_back
 
         if frame is None:
             return "No parse_args()"
         elif frame.f_code.co_name == "parse_args":
             frame = frame.f_back
-            return frame.f_code.co_name
+            return frame.f_code.co_name  # type: ignore
 
 
 def args_post(args, parser, create_db=False):
     args.defaults = [k for k, v in args.__dict__.items() if parser.get_default(k) == v]
     settings = {k: v for k, v in args.__dict__.items() if k not in ["database", "verbose", "defaults"] + args.defaults}
     args.extractor_config = {
         k: v for k, v in settings.items() if k not in ["db", "paths", "actions", "backfill_pages"]
```

### Comparing `xklb-2.8.6/xklb/utils/argparse_utils.py` & `xklb-2.8.7/xklb/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/consts.py` & `xklb-2.8.7/xklb/utils/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/db_utils.py` & `xklb-2.8.7/xklb/utils/db_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,26 @@
 config = {
     "playlists": {
         "search_columns": ["path", "title"],
         "column_order": ["id", "path", "extractor_key"],
         "ignore_columns": ["extractor_playlist_id"],
     },
     "media": {
-        "search_columns": ["path", "title", "mood", "genre", "description", "artist", "album", "category", "frequency"],
+        "search_columns": [
+            "path",
+            "webpath",
+            "title",
+            "mood",
+            "genre",
+            "description",
+            "artist",
+            "album",
+            "category",
+            "frequency",
+        ],
         "column_order": ["id", "path", "webpath", "extractor_id"],
         "ignore_columns": ["extractor_id"],
     },
     "history": {"column_order": ["id"]},
     "captions": {"search_columns": ["text"]},
     "reddit_posts": {
         "search_columns": ["title", "selftext"],
```

### Comparing `xklb-2.8.6/xklb/utils/devices.py` & `xklb-2.8.7/xklb/utils/devices.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/file_utils.py` & `xklb-2.8.7/xklb/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/gui.py` & `xklb-2.8.7/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/iterables.py` & `xklb-2.8.7/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/log_utils.py` & `xklb-2.8.7/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/mpv_utils.py` & `xklb-2.8.7/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/nums.py` & `xklb-2.8.7/xklb/utils/nums.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/objects.py` & `xklb-2.8.7/xklb/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/path_utils.py` & `xklb-2.8.7/xklb/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/pd_utils.py` & `xklb-2.8.7/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/printing.py` & `xklb-2.8.7/xklb/utils/printing.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/processes.py` & `xklb-2.8.7/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/sql_utils.py` & `xklb-2.8.7/xklb/utils/sql_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,17 +277,17 @@
             {filter_play_count(args)}
         GROUP BY {freq_label}
     """
 
     return list(args.db.query(query))
 
 
-def limit_sql(args, limit_adj=0):
-    sql = f"LIMIT {args.limit + limit_adj}" if args.limit else ""
-    offset_sql = f"OFFSET {args.offset}" if args.offset and args.limit else ""
+def limit_sql(limit, offset, limit_adj=0):
+    sql = f"LIMIT {limit + limit_adj}" if limit else ""
+    offset_sql = f"OFFSET {offset}" if offset and limit else ""
     sql = f"{sql} {offset_sql}"
     return sql
 
 
 def fts_quote(query: list[str]) -> list[str]:
     fts_words = [" NOT ", " AND ", " OR ", "*", ":", "NEAR("]
     return [s if any(r in s for r in fts_words) else '"' + s + '"' for s in query]
```

### Comparing `xklb-2.8.6/xklb/utils/sqlgroups.py` & `xklb-2.8.7/xklb/utils/sqlgroups.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,28 @@
             args.select.remove("duration")
         args.select += ["cast(length(tags) / 4.2 / 220 * 60 as INT) + 10 duration"]
 
     select_sql = "\n        , ".join(args.select)
     return select_sql
 
 
-def fs_sql(args) -> tuple[str, dict]:
+def fs_sql(args, limit) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
     args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     query = f"""
         SELECT
             {media_select_sql(args, m_columns)}
         FROM {args.table} m
         WHERE 1=1
             {" ".join(args.filter_sql)}
             {" ".join(args.aggregate_filter_sql)}
         ORDER BY 1=1
             {', ' + args.sort if args.sort else ''}
-        {sql_utils.limit_sql(args)}
+        {sql_utils.limit_sql(limit, args.offset)}
     """
 
     return query, args.filter_bindings
 
 
 def perf_randomize_using_ids(args, m_columns):
     if args.random and not args.include and not args.print and args.limit in args.defaults:
@@ -83,15 +83,15 @@
             , time_last_played
             , playhead
         FROM m
         WHERE 1=1
             {" ".join(args.aggregate_filter_sql)}
         ORDER BY 1=1
             {', ' + args.sort if args.sort else ''}
-        {sql_utils.limit_sql(args)}
+        {sql_utils.limit_sql(args.limit, args.offset)}
     """
 
     args.filter_sql = [
         s for s in args.filter_sql if "in (select id from media" not in s
     ]  # only use random id constraint in first query
 
     return query, args.filter_bindings
@@ -160,15 +160,15 @@
         {" ".join(args.aggregate_filter_sql)}
     ORDER BY 1=1
         {', ' + args.sort if args.sort else ''}
         , play_count
         {', ROW_NUMBER() OVER ( PARTITION BY hostname )' if 'hostname' in m_columns else ''}
         {', ROW_NUMBER() OVER ( PARTITION BY category )' if 'category' in m_columns else ''}
         , random()
-    {sql_utils.limit_sql(args)}
+    {sql_utils.limit_sql(args.limit, args.offset)}
     """
 
     return query, args.filter_bindings
 
 
 def construct_tabs_query(args) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
@@ -216,15 +216,15 @@
         , ROW_NUMBER() OVER ( PARTITION BY
             play_count
             , frequency
             , hostname
             , category
         ) -- prefer to spread hostname, category over time
         , random()
-    {sql_utils.limit_sql(args)}
+    {sql_utils.limit_sql(args.limit, args.offset)}
     """
 
     return query, args.filter_bindings
 
 
 def construct_captions_search_query(args) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
@@ -305,15 +305,15 @@
         {" ".join(args.filter_sql)}
         {'AND extractor_key != "Local"' if args.online_media_only else ''}
         {'AND extractor_key = "Local"' if args.local_media_only else ''}
     ORDER BY 1=1
         {', ' + args.playlists_sort if args.playlists_sort else ''}
         , path
         , random()
-    {sql_utils.limit_sql(args)}
+    {sql_utils.limit_sql(args.limit, args.offset)}
     """
 
     return query, args.filter_bindings
 
 
 def construct_download_query(args) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
@@ -364,15 +364,15 @@
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
                 {" ".join(args.filter_sql)}
             ORDER BY 1=1
                 , COALESCE(m.time_modified, 0) = 0 DESC
                 {', p.extractor_key IS NOT NULL DESC' if 'sort' in args.defaults else ''}
                 {', m.error IS NULL DESC' if 'error' in m_columns else ''}
                 {', random()' if 'sort' in args.defaults else ', ' + args.sort}
-            {sql_utils.limit_sql(args)}
+            {sql_utils.limit_sql(args.limit, args.offset)}
         """
     else:
         query = f"""select
                 m.path
                 {', m.title' if 'title' in m_columns else ''}
                 {', m.duration' if 'duration' in m_columns else ''}
                 {', m.time_created' if 'time_created' in m_columns else ''}
@@ -391,11 +391,11 @@
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
                 {" ".join(args.filter_sql)}
             ORDER BY 1=1
                 , COALESCE(m.time_modified, 0) = 0 DESC
                 {', m.error IS NULL DESC' if 'error' in m_columns else ''}
                 {', random()' if 'sort' in args.defaults else ', ' + args.sort}
-        {sql_utils.limit_sql(args)}
+        {sql_utils.limit_sql(args.limit, args.offset)}
         """
 
     return query, args.filter_bindings
```

### Comparing `xklb-2.8.6/xklb/utils/strings.py` & `xklb-2.8.7/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/utils/web.py` & `xklb-2.8.7/xklb/utils/web.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/xklb/assets/kotobago.png` & `xklb-2.8.7/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/.gitignore` & `xklb-2.8.7/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/pyproject.toml` & `xklb-2.8.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.8.6/.github/README.md` & `xklb-2.8.7/.github/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    library (v2.8.006; 72 subcommands)
+    library (v2.8.007; 72 subcommands)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
```

### Comparing `xklb-2.8.6/PKG-INFO` & `xklb-2.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.8.6
+Version: 2.8.7
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -182,15 +182,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    library (v2.8.006; 72 subcommands)
+    library (v2.8.007; 72 subcommands)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
```

