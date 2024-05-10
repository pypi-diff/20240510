# Comparing `tmp/xklb-2.8.3.tar.gz` & `tmp/xklb-2.8.6.tar.gz`

## Comparing `xklb-2.8.3.tar` & `xklb-2.8.6.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.8.3/.gitattributes
--rw-r--r--   0        0        0   216245 2020-02-02 00:00:00.000000 xklb-2.8.3/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/LICENSE
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/examples/art.avif
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/workflows/green.yaml
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/__init__.py
--rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/lb.py
--rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/media_printer.py
--rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/readme.py
--rw-r--r--   0        0        0   112540 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/__init__.py
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/av.py
--rw-r--r--   0        0        0    20488 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/fs_add.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/gallery_add.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/gallery_backend.py
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/hn_add.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/links_add.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/places_import.py
--rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/reddit_add.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/row_add.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/site_add.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/substack.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/subtitle.py
--rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/tabs_add.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/tildes.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/tube_add.py
--rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/tube_backend.py
--rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/createdb/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/data/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/editdb/__init__.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/editdb/dedupe_db.py
--rw-r--r--   0        0        0    18923 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/editdb/dedupe_media.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/editdb/merge_online_local.py
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/editdb/mpv_watchlater.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/editdb/pushshift.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/editdb/reddit_selftext.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/files/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/files/christen.py
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/files/sample_compare.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/files/sample_hash.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/files/similar_files.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/folders/__init__.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/folders/big_dirs.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/folders/merge_folders.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/folders/mount_stats.py
--rw-r--r--   0        0        0     7369 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/folders/move_list.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/folders/rel_mv.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/folders/scatter.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/folders/similar_folders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/fsdb/__init__.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/fsdb/disk_usage.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/fsdb/search_db.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/__init__.py
--rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/block.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/db_history.py
--rw-r--r--   0        0        0    19221 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/db_media.py
--rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/db_playlists.py
--rw-r--r--   0        0        0     7262 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/download.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/download_status.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/history.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/history_add.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/optimize_db.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/playlists.py
--rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/redownload.py
--rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/search.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediadb/stats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediafiles/__init__.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediafiles/media_check.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediafiles/process_ffmpeg.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/mediafiles/process_image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/misc/__init__.py
--rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/misc/dedupe_czkawka.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/misc/export_text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/multidb/__init__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/multidb/copy_play_counts.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/multidb/merge_dbs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/playback/__init__.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/playback/links_open.py
--rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/playback/media_player.py
--rw-r--r--   0        0        0    11678 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/playback/play_actions.py
--rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/playback/playback_control.py
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/playback/post_actions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/playback/surf.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/playback/tabs_open.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/tablefiles/__init__.py
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/tablefiles/eda.py
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/tablefiles/incremental_diff.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/tablefiles/mcda.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/text/__init__.py
--rw-r--r--   0        0        0    12699 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/text/cluster_sort.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/text/extract_links.py
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/text/extract_text.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/text/markdown_links.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/text/nouns.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/__init__.py
--rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    29767 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/consts.py
--rw-r--r--   0        0        0     9380 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/devices.py
--rw-r--r--   0        0        0    15831 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/nums.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/objects.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/printing.py
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/processes.py
--rw-r--r--   0        0        0    13007 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/sqlgroups.py
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/strings.py
--rw-r--r--   0        0        0    23222 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/utils/web.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/assets/__init__.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.8.3/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.8.3/.gitignore
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 xklb-2.8.3/pyproject.toml
--rw-r--r--   0        0        0   156256 2020-02-02 00:00:00.000000 xklb-2.8.3/.github/README.md
--rw-r--r--   0        0        0   160037 2020-02-02 00:00:00.000000 xklb-2.8.3/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.8.6/.gitattributes
+-rw-r--r--   0        0        0   216245 2020-02-02 00:00:00.000000 xklb-2.8.6/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/examples/art.avif
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/__init__.py
+-rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/lb.py
+-rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/media_printer.py
+-rw-r--r--   0        0        0    13906 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/readme.py
+-rw-r--r--   0        0        0   112540 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/__init__.py
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/av.py
+-rw-r--r--   0        0        0    20488 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/fs_add.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/gallery_add.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/gallery_backend.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/hn_add.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/links_add.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/places_import.py
+-rw-r--r--   0        0        0    13142 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/reddit_add.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/row_add.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/site_add.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/substack.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/subtitle.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/tabs_add.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/tildes.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/tube_add.py
+-rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/tube_backend.py
+-rw-r--r--   0        0        0     9874 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/createdb/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/data/__init__.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17080 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/__init__.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/dedupe_db.py
+-rw-r--r--   0        0        0    18995 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/dedupe_media.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/merge_online_local.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/mpv_watchlater.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/pushshift.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/editdb/reddit_selftext.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/files/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/files/christen.py
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/files/sample_compare.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/files/sample_hash.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/files/similar_files.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/__init__.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/big_dirs.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/merge_folders.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/mount_stats.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/move_list.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/rel_mv.py
+-rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/scatter.py
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/folders/similar_folders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/fsdb/__init__.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/fsdb/disk_usage.py
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/fsdb/search_db.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/__init__.py
+-rw-r--r--   0        0        0    11549 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/block.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/db_history.py
+-rw-r--r--   0        0        0    19221 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/db_media.py
+-rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/db_playlists.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/download.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/download_status.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/history.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/history_add.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/optimize_db.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/playlists.py
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/redownload.py
+-rw-r--r--   0        0        0     4466 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/search.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediadb/stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediafiles/__init__.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediafiles/media_check.py
+-rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediafiles/process_ffmpeg.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/mediafiles/process_image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/misc/__init__.py
+-rw-r--r--   0        0        0    13877 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/misc/dedupe_czkawka.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/misc/export_text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/multidb/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/multidb/copy_play_counts.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/multidb/merge_dbs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/__init__.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/links_open.py
+-rw-r--r--   0        0        0    24252 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/media_player.py
+-rw-r--r--   0        0        0    11678 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/play_actions.py
+-rw-r--r--   0        0        0     9829 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/playback_control.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/post_actions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/surf.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/playback/tabs_open.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8683 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/tablefiles/__init__.py
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/tablefiles/eda.py
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/tablefiles/incremental_diff.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/tablefiles/mcda.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/__init__.py
+-rw-r--r--   0        0        0    12694 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/cluster_sort.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/extract_links.py
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/extract_text.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/markdown_links.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/text/nouns.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    29962 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/consts.py
+-rw-r--r--   0        0        0     9380 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15831 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/nums.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/processes.py
+-rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0    15672 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/sqlgroups.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/strings.py
+-rw-r--r--   0        0        0    23222 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/utils/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/assets/__init__.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.8.6/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.8.6/.gitignore
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 xklb-2.8.6/pyproject.toml
+-rw-r--r--   0        0        0   156256 2020-02-02 00:00:00.000000 xklb-2.8.6/.github/README.md
+-rw-r--r--   0        0        0   160037 2020-02-02 00:00:00.000000 xklb-2.8.6/PKG-INFO
```

### Comparing `xklb-2.8.3/pdm.lock` & `xklb-2.8.6/pdm.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1991,35 +1991,35 @@
 files = [
     {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
     {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
 ]
 
 [[package]]
 name = "ruff"
-version = "0.4.3"
+version = "0.4.4"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter and code formatter, written in Rust."
 files = [
-    {file = "ruff-0.4.3-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:b70800c290f14ae6fcbb41bbe201cf62dfca024d124a1f373e76371a007454ce"},
-    {file = "ruff-0.4.3-py3-none-macosx_11_0_arm64.whl", hash = "sha256:08a0d6a22918ab2552ace96adeaca308833873a4d7d1d587bb1d37bae8728eb3"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:eba1f14df3c758dd7de5b55fbae7e1c8af238597961e5fb628f3de446c3c40c5"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:819fb06d535cc76dfddbfe8d3068ff602ddeb40e3eacbc90e0d1272bb8d97113"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0bfc9e955e6dc6359eb6f82ea150c4f4e82b660e5b58d9a20a0e42ec3bb6342b"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:510a67d232d2ebe983fddea324dbf9d69b71c4d2dfeb8a862f4a127536dd4cfb"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:dc9ff11cd9a092ee7680a56d21f302bdda14327772cd870d806610a3503d001f"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:29efff25bf9ee685c2c8390563a5b5c006a3fee5230d28ea39f4f75f9d0b6f2f"},
-    {file = "ruff-0.4.3-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:18b00e0bcccf0fc8d7186ed21e311dffd19761cb632241a6e4fe4477cc80ef6e"},
-    {file = "ruff-0.4.3-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:262f5635e2c74d80b7507fbc2fac28fe0d4fef26373bbc62039526f7722bca1b"},
-    {file = "ruff-0.4.3-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:7363691198719c26459e08cc17c6a3dac6f592e9ea3d2fa772f4e561b5fe82a3"},
-    {file = "ruff-0.4.3-py3-none-musllinux_1_2_i686.whl", hash = "sha256:eeb039f8428fcb6725bb63cbae92ad67b0559e68b5d80f840f11914afd8ddf7f"},
-    {file = "ruff-0.4.3-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:927b11c1e4d0727ce1a729eace61cee88a334623ec424c0b1c8fe3e5f9d3c865"},
-    {file = "ruff-0.4.3-py3-none-win32.whl", hash = "sha256:25cacda2155778beb0d064e0ec5a3944dcca9c12715f7c4634fd9d93ac33fd30"},
-    {file = "ruff-0.4.3-py3-none-win_amd64.whl", hash = "sha256:7a1c3a450bc6539ef00da6c819fb1b76b6b065dec585f91456e7c0d6a0bbc725"},
-    {file = "ruff-0.4.3-py3-none-win_arm64.whl", hash = "sha256:71ca5f8ccf1121b95a59649482470c5601c60a416bf189d553955b0338e34614"},
-    {file = "ruff-0.4.3.tar.gz", hash = "sha256:ff0a3ef2e3c4b6d133fbedcf9586abfbe38d076041f2dc18ffb2c7e0485d5a07"},
+    {file = "ruff-0.4.4-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:29d44ef5bb6a08e235c8249294fa8d431adc1426bfda99ed493119e6f9ea1bf6"},
+    {file = "ruff-0.4.4-py3-none-macosx_11_0_arm64.whl", hash = "sha256:c4efe62b5bbb24178c950732ddd40712b878a9b96b1d02b0ff0b08a090cbd891"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4c8e2f1e8fc12d07ab521a9005d68a969e167b589cbcaee354cb61e9d9de9c15"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:60ed88b636a463214905c002fa3eaab19795679ed55529f91e488db3fe8976ab"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b90fc5e170fc71c712cc4d9ab0e24ea505c6a9e4ebf346787a67e691dfb72e85"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:8e7e6ebc10ef16dcdc77fd5557ee60647512b400e4a60bdc4849468f076f6eef"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:b9ddb2c494fb79fc208cd15ffe08f32b7682519e067413dbaf5f4b01a6087bcd"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c51c928a14f9f0a871082603e25a1588059b7e08a920f2f9fa7157b5bf08cfe9"},
+    {file = "ruff-0.4.4-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b5eb0a4bfd6400b7d07c09a7725e1a98c3b838be557fee229ac0f84d9aa49c36"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:b1867ee9bf3acc21778dcb293db504692eda5f7a11a6e6cc40890182a9f9e595"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:1aecced1269481ef2894cc495647392a34b0bf3e28ff53ed95a385b13aa45768"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_i686.whl", hash = "sha256:9da73eb616b3241a307b837f32756dc20a0b07e2bcb694fec73699c93d04a69e"},
+    {file = "ruff-0.4.4-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:958b4ea5589706a81065e2a776237de2ecc3e763342e5cc8e02a4a4d8a5e6f95"},
+    {file = "ruff-0.4.4-py3-none-win32.whl", hash = "sha256:cb53473849f011bca6e754f2cdf47cafc9c4f4ff4570003a0dad0b9b6890e876"},
+    {file = "ruff-0.4.4-py3-none-win_amd64.whl", hash = "sha256:424e5b72597482543b684c11def82669cc6b395aa8cc69acc1858b5ef3e5daae"},
+    {file = "ruff-0.4.4-py3-none-win_arm64.whl", hash = "sha256:39df0537b47d3b597293edbb95baf54ff5b49589eb7ff41926d8243caa995ea6"},
+    {file = "ruff-0.4.4.tar.gz", hash = "sha256:f87ea42d5cdebdc6a69761a9d0bc83ae9b3b30d0ad78952005ba6568d6c022af"},
 ]
 
 [[package]]
 name = "scikit-learn"
 version = "1.4.2"
 requires_python = ">=3.9"
 summary = "A set of python modules for machine learning and data mining"
```

### Comparing `xklb-2.8.3/.github/LICENSE` & `xklb-2.8.6/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/.github/Windows.md` & `xklb-2.8.6/.github/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/.github/examples/art.avif` & `xklb-2.8.6/.github/examples/art.avif`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/.github/examples/extract.svg` & `xklb-2.8.6/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/.github/examples/tubeadd.svg` & `xklb-2.8.6/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/.github/workflows/push.yaml` & `xklb-2.8.6/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/lb.py` & `xklb-2.8.6/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/media_printer.py` & `xklb-2.8.6/xklb/media_printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import csv, json, os, shlex, statistics
 from copy import deepcopy
 from io import StringIO
 from numbers import Number
 from pathlib import Path
 
-from tabulate import tabulate
-
 from xklb.mediadb import db_history, db_media
 from xklb.playback import post_actions
 from xklb.utils import consts, db_utils, iterables, printing, processes, sql_utils, strings
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
@@ -246,15 +244,15 @@
         tbl = [{k: f"{v:.4f}" if isinstance(v, float) else v for k, v in d.items()} for d in tbl]
         max_col_widths = printing.calculate_max_col_widths(tbl)
         adjusted_widths = printing.distribute_excess_width(max_col_widths)
         for k, v in adjusted_widths.items():
             printing.col_resize(tbl, k, v)
 
         colalign = ["right" if should_align_right(k, v) else "left" for k, v in tbl[0].items()]
-        print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False, colalign=colalign))
+        printing.table(tbl, colalign=colalign)
 
         if len(media) > 1:
             print(
                 f"{media_len or len(media)} {units}"
                 + (
                     f" (limited by --limit {args.limit})"
                     if args.limit and int(args.limit) <= len(media) and len(tbl) <= int(args.limit)
```

### Comparing `xklb-2.8.3/xklb/readme.py` & `xklb-2.8.6/xklb/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/usage.py` & `xklb-2.8.6/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/av.py` & `xklb-2.8.6/xklb/createdb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/fs_add.py` & `xklb-2.8.6/xklb/createdb/fs_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/gallery_add.py` & `xklb-2.8.6/xklb/createdb/gallery_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/gallery_backend.py` & `xklb-2.8.6/xklb/createdb/gallery_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/hn_add.py` & `xklb-2.8.6/xklb/createdb/hn_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/links_add.py` & `xklb-2.8.6/xklb/createdb/links_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/places_import.py` & `xklb-2.8.6/xklb/createdb/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/reddit_add.py` & `xklb-2.8.6/xklb/createdb/reddit_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/row_add.py` & `xklb-2.8.6/xklb/createdb/row_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/site_add.py` & `xklb-2.8.6/xklb/createdb/site_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/substack.py` & `xklb-2.8.6/xklb/createdb/substack.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/subtitle.py` & `xklb-2.8.6/xklb/createdb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/tabs_add.py` & `xklb-2.8.6/xklb/createdb/tabs_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,25 +116,25 @@
     arggroups.args_post(args, parser)
 
     tabs = list(
         args.db.query(
             f"""
         WITH m as (
             SELECT
-                media.id
+                m.id
                 , path
                 , frequency
                 , COALESCE(MAX(h.time_played), 0) time_last_played
                 , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , hostname
                 , category
-            FROM media
-            LEFT JOIN history h on h.media_id = media.id
+            FROM media m
+            LEFT JOIN history h on h.media_id = m.id
             WHERE COALESCE(time_deleted, 0)=0
-            GROUP BY media.id
+            GROUP BY m.id
         )
         SELECT
             id
             , path
             , frequency
             , time_last_played
         FROM m
```

### Comparing `xklb-2.8.3/xklb/createdb/tildes.py` & `xklb-2.8.6/xklb/createdb/tildes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/tube_add.py` & `xklb-2.8.6/xklb/createdb/tube_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/tube_backend.py` & `xklb-2.8.6/xklb/createdb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/createdb/web_add.py` & `xklb-2.8.6/xklb/createdb/web_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/data/imagemagick_errors.py` & `xklb-2.8.6/xklb/data/imagemagick_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/data/wordbank.py` & `xklb-2.8.6/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/data/yt_dlp_errors.py` & `xklb-2.8.6/xklb/data/yt_dlp_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/editdb/dedupe_db.py` & `xklb-2.8.6/xklb/editdb/dedupe_db.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         action=argparse_utils.ArgparseList,
         required=True,
         help="Comma separated business keys",
     )
     arggroups.debug(parser)
 
     arggroups.database(parser)
-    parser.add_argument("table")
+    parser.add_argument("target_table")
     args = parser.parse_intermixed_args()
 
     arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def dedupe_rows(args, tablename, primary_keys, business_keys):
@@ -46,17 +46,17 @@
         )
 
 
 def dedupe_db() -> None:
     args = parse_args()
 
     upsert_columns = args.only_columns
-    target_columns = args.db[args.table].columns_dict
+    target_columns = args.db[args.target_table].columns_dict
     if not args.primary_keys:
-        args.primary_keys = list(o.name for o in args.db[args.table].columns if o.is_pk)
+        args.primary_keys = list(o.name for o in args.db[args.target_table].columns if o.is_pk)
     if not upsert_columns:
         upsert_columns = [s for s in target_columns if s not in args.primary_keys + args.business_keys]
 
     missing_columns = [s for s in upsert_columns if s not in target_columns]
     if missing_columns:
         raise ValueError("At least one upsert column not available in target table: %s", missing_columns)
 
@@ -71,35 +71,37 @@
         log.info("Upserting data in %s", ",".join(upsert_columns))
 
         for col in upsert_columns:
             data = list(
                 args.db.query(
                     f"""
                     SELECT {','.join([*args.business_keys, col])}
-                    FROM {args.table}
+                    FROM {args.target_table}
                     WHERE {f'NULLIF({col}, 0)' if args.skip_0 else col} IS NOT NULL
                     AND ({','.join(args.business_keys)}) IN (
                         SELECT {','.join(args.business_keys)}
-                        FROM {args.table}
+                        FROM {args.target_table}
                         WHERE {col} IS NULL
                     )
                     ORDER BY {','.join(args.primary_keys)}
                     """,
                 ),
             )
             log.info("%s (%s rows)", col, len(data))
 
             with args.db.conn:
 
                 def gen_where_sql(row):
                     return " AND ".join([f"{key} = {args.db.quote(row[key])}" for key in args.business_keys])
 
                 def gen_update_sql(row):
-                    return f"UPDATE {args.table} SET {col} = {args.db.quote(row[col])} WHERE {gen_where_sql(row)};"
+                    return (
+                        f"UPDATE {args.target_table} SET {col} = {args.db.quote(row[col])} WHERE {gen_where_sql(row)};"
+                    )
 
                 args.db.conn.executescript("\n".join([gen_update_sql(row) for row in data]))
 
-    dedupe_rows(args, args.table, primary_keys=args.primary_keys, business_keys=args.business_keys)
+    dedupe_rows(args, args.target_table, primary_keys=args.primary_keys, business_keys=args.business_keys)
 
 
 if __name__ == "__main__":
     dedupe_db()
```

### Comparing `xklb-2.8.3/xklb/editdb/dedupe_media.py` & `xklb-2.8.6/xklb/editdb/dedupe_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     if not COMPARE_DIRS:
         args.table2 = args.table
 
     return args
 
 
 def get_rows(args, m_columns) -> list[dict]:
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     query = f"""
     SELECT
         {', '.join(s for s in db_utils.config["media"]["search_columns"] if s in m_columns)}
     FROM
         {args.table}
     WHERE 1=1
@@ -171,15 +171,15 @@
     """
 
     return args.db.query(query, args.filter_bindings)
 
 
 def get_music_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
@@ -219,15 +219,15 @@
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
 def get_id_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
@@ -263,15 +263,15 @@
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
 def get_title_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
@@ -307,15 +307,15 @@
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
 def get_duration_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     query = f"""
     SELECT
         m1.path keep_path
         -- , length(m1.path)-length(REPLACE(m1.path, '{os.sep}', '')) num_slash
         -- , length(m1.path)-length(REPLACE(m1.path, '.', '')) num_dot
         -- , length(m1.path) len_p
@@ -351,15 +351,15 @@
     media = list(args.db.query(query, args.filter_bindings))
 
     return media
 
 
 def get_fs_duplicates(args) -> list[dict]:
     m_columns = db_utils.columns(args, "media")
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     query = f"""
     SELECT
         path
         , size
         {', hash' if 'hash' in m_columns else ''}
     FROM
```

### Comparing `xklb-2.8.3/xklb/editdb/merge_online_local.py` & `xklb-2.8.6/xklb/editdb/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/editdb/mpv_watchlater.py` & `xklb-2.8.6/xklb/editdb/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/editdb/pushshift.py` & `xklb-2.8.6/xklb/editdb/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/editdb/reddit_selftext.py` & `xklb-2.8.6/xklb/editdb/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/files/christen.py` & `xklb-2.8.6/xklb/files/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/files/sample_compare.py` & `xklb-2.8.6/xklb/files/sample_compare.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/files/sample_hash.py` & `xklb-2.8.6/xklb/files/sample_hash.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/files/similar_files.py` & `xklb-2.8.6/xklb/files/similar_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
 
 import humanize
-from tabulate import tabulate
 
 from xklb import usage
 from xklb.folders.similar_folders import cluster_folders, map_and_name
-from xklb.utils import arg_utils, arggroups, argparse_utils, consts, nums, printing
+from xklb.utils import arg_utils, arggroups, argparse_utils, file_utils, nums, printing
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse_utils.ArgumentParser(usage=usage.similar_files)
     arggroups.cluster(parser)
 
@@ -28,34 +27,33 @@
     parser.add_argument("--filter-durations", action=argparse.BooleanOptionalAction, default=True)
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
     arggroups.args_post(args, parser)
 
-    if not args.filter_sizes:
-        args.sizes_delta = 200.0
-    if not args.filter_durations:
-        args.durations_delta = 200.0
-
     if not args.filter_names and not args.filter_sizes and not args.filter_durations:
         print("Nothing to do")
         raise NotImplementedError
 
     return args
 
 
 def is_same_size_group(args, m0, m):
-    size_diff = nums.percentage_difference(m0["size"], m["size"])
+    bools = []
+
+    if args.filter_sizes:
+        size_diff = nums.percentage_difference(m0["size"], m["size"])
+        bools.append(size_diff < args.sizes_delta)
 
-    if "duration" in m:
+    if args.filter_durations and m.get("duration"):
         duration_diff = nums.percentage_difference(m0["duration"], m["duration"])
-        return size_diff < args.sizes_delta and duration_diff < args.durations_delta
+        bools.append(duration_diff < args.durations_delta)
 
-    return size_diff < args.sizes_delta
+    return all(bools)
 
 
 def cluster_by_size(args, media):
     group_id = 0
     temp_groups = []
     media_groups = []
     for m in media:
@@ -98,14 +96,15 @@
     groups = [group for group in groups if group]
     return groups
 
 
 def similar_files():
     args = parse_args()
     media = list(arg_utils.gen_d(args))
+    media = [d if "size" in d else file_utils.get_filesize(d) for d in media]
 
     groups: list[dict] = []
     if args.filter_sizes or args.filter_durations:
         clusters = cluster_by_size(args, media)
         groups = map_and_name(media, clusters)
         log.info("file size/duration clustering sorted %s files into %s groups", len(media), len(groups))
         single_file_groups = [d for d in groups if len(d["grouped_paths"]) == 1]
@@ -138,28 +137,23 @@
         if args.only_duplicates:
             media = media[1:]
 
         if "f" in args.print:
             for d in media:
                 printing.pipe_print(d["path"])
         else:
-            print(
-                tabulate(
-                    [
-                        {
-                            f'group {group["common_path"]}': d["path"],
-                            "size": humanize.naturalsize(d["size"], binary=True),
-                            "duration": printing.human_duration(d["duration"]),
-                        }
-                        for d in media
-                    ],
-                    tablefmt=consts.TABULATE_STYLE,
-                    headers="keys",
-                    showindex=False,
-                )
+            printing.table(
+                [
+                    {
+                        f'group {group["common_path"]}': d["path"],
+                        "size": humanize.naturalsize(d["size"], binary=True),
+                        "duration": printing.human_duration(d.get("duration")),
+                    }
+                    for d in media
+                ]
             )
 
         if not args.only_originals and not args.only_duplicates:
             print()
 
     if not args.only_originals and not args.only_duplicates:
         print(len(groups), "groups found")
```

### Comparing `xklb-2.8.3/xklb/folders/big_dirs.py` & `xklb-2.8.6/xklb/folders/big_dirs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse, os
-from collections import defaultdict
+from collections import Counter, defaultdict
 from pathlib import Path
 
 from xklb import media_printer, usage
 from xklb.tablefiles import mcda
 from xklb.utils import arg_utils, arggroups, argparse_utils, file_utils, iterables, nums
 
 
@@ -11,38 +11,31 @@
     parser = argparse_utils.ArgumentParser(
         prog="library big_dirs",
         usage=usage.big_dirs,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     arggroups.cluster(parser)
     arggroups.group_folders(parser)
-    parser.set_defaults(limit="4000", lower=4, depth=0)
+    parser.set_defaults(limit="4000", depth=0)
     arggroups.debug(parser)
 
     arggroups.paths_or_stdin(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
     arggroups.args_post(args, parser)
 
+    if not any([args.folders_counts, args.folder_counts, args.folder_sizes]):
+        args.folder_counts = ["+3", "-3000"]
+        args.folder_sizes = ["+30MiB"]
+
     arggroups.group_folders_post(args)
 
     return args
 
 
-def filter_deleted(args, d):
-    for path, pdict in list(d.items()):
-        if pdict["exists"] == 0:
-            d.pop(path)
-
-    if args.folder_counts and not args.depth:
-        for path, pdict in list(d.items()):
-            if not args.folder_counts(pdict["exists"]):
-                d.pop(path)
-
-
 def group_files_by_parents(args, media) -> list[dict]:
     p_media = {}
     min_parts = 10
     for m in media:
         p = m["path"].split(os.sep)
         min_parts = min(min_parts, len(p))
         while len(p) >= 2:
@@ -54,64 +47,60 @@
             else:
                 p_media[parent].append(m)
 
     d = {}
     for parent, media in list(p_media.items()):
         d[parent] = {
             "size": sum(m.get("size") or 0 for m in media if not bool(m.get("time_deleted"))),
-            "median_size": nums.safe_median(m.get("size") or 0 for m in media if not bool(m.get("time_deleted"))),
+            "median_size": nums.safe_median(m.get("size") for m in media if not bool(m.get("time_deleted"))),
             "duration": sum(m.get("duration") or 0 for m in media if not bool(m.get("time_deleted"))),
-            "median_duration": nums.safe_median(
-                m.get("duration") or 0 for m in media if not bool(m.get("time_deleted"))
-            ),
+            "median_duration": nums.safe_median(m.get("duration") for m in media if not bool(m.get("time_deleted"))),
             "total": len(media),
             "exists": sum(not bool(m.get("time_deleted")) for m in media),
             "deleted": sum(bool(m.get("time_deleted")) for m in media),
             "deleted_size": sum(m.get("size") or 0 for m in media if bool(m.get("time_deleted"))),
             "deleted_duration": sum(m.get("duration") or 0 for m in media if bool(m.get("time_deleted"))),
             "played": sum(bool(m.get("time_last_played")) for m in media),
         }
 
     for parent, _ in list(d.items()):
         if len(parent.split(os.sep)) < min_parts:
             d.pop(parent)
 
-    filter_deleted(args, d)
-
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def group_files_by_parent(args, media) -> list[dict]:
     p_media = defaultdict(list)
     for m in media:
         p_media[str(Path(m["path"]).parent)].append(m)
 
     d = {}
     for parent, media in list(p_media.items()):
         d[parent] = {
             "size": sum(m.get("size") or 0 for m in media if not bool(m.get("time_deleted"))),
-            "median_size": nums.safe_median(m.get("size") or 0 for m in media if not bool(m.get("time_deleted"))),
+            "median_size": nums.safe_median(m.get("size") for m in media if not bool(m.get("time_deleted"))),
             "duration": sum(m.get("duration") or 0 for m in media if not bool(m.get("time_deleted"))),
-            "median_duration": nums.safe_median(
-                m.get("duration") or 0 for m in media if not bool(m.get("time_deleted"))
-            ),
+            "median_duration": nums.safe_median(m.get("duration") for m in media if not bool(m.get("time_deleted"))),
             "total": len(media),
             "exists": sum(not bool(m.get("time_deleted")) for m in media),
             "deleted": sum(bool(m.get("time_deleted")) for m in media),
             "deleted_size": sum(m.get("size") or 0 for m in media if bool(m.get("time_deleted"))),
             "deleted_duration": sum(m.get("duration") or 0 for m in media if bool(m.get("time_deleted"))),
             "played": sum(bool(m.get("time_last_played")) for m in media),
         }
 
-    filter_deleted(args, d)
+    parent_counts = Counter(str(Path(p).parent) for p in d.keys())
+    for parent, data in d.items():
+        data["folders"] = parent_counts[parent]
 
     return [{**v, "path": k} for k, v in d.items()]
 
 
-def folder_depth(args, folders) -> list[dict]:
+def reaggregate_at_depth(args, folders) -> list[dict]:
     d = {}
     for f in folders:
         p = f["path"].split(os.sep)
         p.pop()
 
         depth = 1 + args.depth
         parent = os.sep.join(p[:depth]) + os.sep
@@ -121,32 +110,33 @@
         if d.get(parent):
             d[parent]["size"] += f["size"]
             d[parent]["duration"] += f["duration"]
             d[parent]["total"] += f["total"]
             d[parent]["exists"] += f["exists"]
             d[parent]["deleted"] += f["deleted"]
             d[parent]["played"] += f["played"]
+            d[parent]["folders"] += f["folders"]
         else:
             d[parent] = f
 
-    if args.folder_counts:
-        for path, pdict in list(d.items()):
-            if not args.folder_counts(pdict["exists"]):
-                d.pop(path)
-
     return [{**v, "path": k} for k, v in d.items()]
 
 
 def process_big_dirs(args, folders) -> list[dict]:
     folders = [d for d in folders if d["total"] != d["deleted"]]  # remove folders where all deleted
 
     if args.depth:
-        folders = folder_depth(args, folders)
+        folders = reaggregate_at_depth(args, folders)
+
     if args.folder_sizes:
         folders = [d for d in folders if args.folder_sizes(d["size"])]
+    if args.folder_counts:
+        folders = [d for d in folders if args.folder_counts(d["exists"])]
+    if args.folders_counts:
+        folders = [d for d in folders if args.folders_counts(d["folders"])]
 
     return folders
 
 
 def big_dirs() -> None:
     args = parse_args()
 
@@ -173,25 +163,25 @@
                 ),
                 "size": sum(
                     media_keyed[s].get("size") or 0
                     for s in group["grouped_paths"]
                     if not bool(media_keyed[s].get("time_deleted"))
                 ),
                 "median_size": nums.safe_median(
-                    media_keyed[s].get("size") or 0
+                    media_keyed[s].get("size")
                     for s in group["grouped_paths"]
                     if not bool(media_keyed[s].get("time_deleted"))
                 ),
                 "duration": sum(
                     media_keyed[s].get("duration") or 0
                     for s in group["grouped_paths"]
                     if not bool(media_keyed[s].get("time_deleted"))
                 ),
                 "median_duration": nums.safe_median(
-                    media_keyed[s].get("duration") or 0
+                    media_keyed[s].get("duration")
                     for s in group["grouped_paths"]
                     if not bool(media_keyed[s].get("time_deleted"))
                 ),
             }
             for group in groups
         ]
     elif args.parents:
```

### Comparing `xklb-2.8.3/xklb/folders/merge_folders.py` & `xklb-2.8.6/xklb/folders/merge_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/folders/mount_stats.py` & `xklb-2.8.6/xklb/folders/mount_stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/folders/move_list.py` & `xklb-2.8.6/xklb/folders/move_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse, shutil, tempfile
 from copy import deepcopy
 from pathlib import Path
 
 import humanize
-from tabulate import tabulate
 
 from xklb import usage
 from xklb.utils import arggroups, argparse_utils, consts, devices, iterables, printing, sqlgroups
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse_utils.ArgumentParser(
@@ -69,15 +68,15 @@
 
 def iterate_and_show_options(args, tbl) -> tuple[list[dict], list[dict]]:
     vew = tbl[-int(args.limit) :] if args.limit else tbl
 
     vew = iterables.list_dict_filter_bool(vew, keep_0=False)
     vew = printing.col_resize_percent(vew, "path", 60)
     vew = printing.col_naturalsize(vew, "size")
-    print(tabulate(vew, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
+    printing.table(tbl)
     print(len(tbl) - len(vew), "other folders not shown")
 
     if args.limit:
         return tbl[-int(args.limit) :], tbl[: -int(args.limit)]
     else:
         return tbl, tbl
```

### Comparing `xklb-2.8.3/xklb/folders/rel_mv.py` & `xklb-2.8.6/xklb/folders/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/folders/scatter.py` & `xklb-2.8.6/xklb/folders/scatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import argparse, math, random, sys, tempfile
 from collections import Counter
 from pathlib import Path
 
 from humanize import naturalsize
-from tabulate import tabulate
 
 from xklb import usage
 from xklb.utils import arggroups, argparse_utils, consts, db_utils, devices, file_utils, iterables, nums, printing
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
@@ -118,15 +117,15 @@
 def print_path_stats(tbl) -> None:
     tbl = iterables.list_dict_filter_bool(tbl, keep_0=False)
     tbl = printing.col_naturalsize(tbl, "total_size")
     tbl = printing.col_naturalsize(tbl, "median_size")
     for t in consts.EPOCH_COLUMNS:
         printing.col_naturaldate(tbl, t)
 
-    print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
+    printing.table(tbl)
 
 
 def rebin_files(args, disk_stats, all_files) -> tuple[list, list]:
     total_size = sum(d["size"] or 0 for d in all_files)
 
     untouched = []
     to_rebin = []
@@ -247,15 +246,15 @@
         tbl = []
         for existing_path, new_path in rebinned:
             tbl.append({"existing_path": existing_path, "new_path": new_path})
             if len(tbl) > 10:
                 break
         tbl = printing.col_resize_percent(tbl, "existing_path", 20)
         tbl = printing.col_resize_percent(tbl, "new_path", 20)
-        print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False))
+        printing.table(tbl)
         print(len(rebinned), "files would be moved (only 10 shown)")
         print(len(untouched), "files would not be moved")
         file_utils.move_files_bash(rebinned)
         sys.exit(0)
 
     if args.targets:
         disk_stats = devices.get_mount_stats(args.targets)
```

### Comparing `xklb-2.8.3/xklb/folders/similar_folders.py` & `xklb-2.8.6/xklb/folders/similar_folders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import argparse
 from pathlib import Path
 
 import humanize
-from tabulate import tabulate
 
 from xklb import usage
 from xklb.folders import big_dirs
 from xklb.text import cluster_sort
-from xklb.utils import arg_utils, arggroups, argparse_utils, consts, file_utils, nums, path_utils, printing, strings
+from xklb.utils import arg_utils, arggroups, argparse_utils, file_utils, nums, path_utils, printing, strings
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse_utils.ArgumentParser(usage=usage.similar_folders)
     arggroups.group_folders(parser)
     arggroups.cluster(parser)
@@ -42,26 +41,21 @@
 
     arggroups.paths_or_stdin(parser)
     args = parser.parse_args()
     arggroups.args_post(args, parser)
 
     arggroups.group_folders_post(args)
 
-    if not args.filter_counts:
-        args.counts_delta = 200.0
-    if not args.filter_sizes:
-        args.sizes_delta = 200.0
-    if not args.filter_durations:
-        args.duration_delta = 200.0
-
     if not args.filter_names and not args.filter_counts and not args.filter_sizes and not args.filter_durations:
         print("Nothing to do")
         raise NotImplementedError
 
-    arggroups.sql_fs_post(args)
+    if args.filter_counts and not any([args.folders_counts, args.folder_counts, args.folder_sizes]):
+        args.folder_counts = ["+2"]
+
     arggroups.group_folders_post(args)
 
     return args
 
 
 def map_and_name(media, clusters):
     bound_dicts = cluster_sort.map_cluster_to_paths(media, clusters)
@@ -91,26 +85,37 @@
     clusters = cluster_sort.find_clusters(n_clusters, sentence_strings, stop_words=args.stop_words)
     groups = map_and_name(media, clusters)
 
     return groups
 
 
 def is_same_group(args, m0, m):
-    count_diff = nums.percentage_difference(m0["exists"], m["exists"])
-    if args.total_sizes:
-        size_diff = nums.percentage_difference(m0["size"], m["size"])
-    else:
-        size_diff = nums.percentage_difference(m0["median_size"], m["median_size"])
+    bools = []
 
-    if args.total_durations:
-        duration_diff = nums.percentage_difference(m0["duration"], m["duration"])
-    else:
-        duration_diff = nums.percentage_difference(m0["median_duration"], m["median_duration"])
+    if args.filter_counts:
+        count_diff = nums.percentage_difference(m0["exists"], m["exists"])
+        bools.append(count_diff < args.counts_delta)
+
+    if args.filter_sizes:
+        if args.total_sizes:
+            size_diff = nums.percentage_difference(m0["size"], m["size"])
+        else:
+            size_diff = nums.percentage_difference(m0["median_size"], m["median_size"])
+
+        bools.append(size_diff < args.sizes_delta)
+
+    if args.filter_durations and m.get("duration"):
+        if args.total_durations:
+            duration_diff = nums.percentage_difference(m0["duration"], m["duration"])
+        else:
+            duration_diff = nums.percentage_difference(m0["median_duration"], m["median_duration"])
+
+        bools.append(duration_diff < args.durations_delta)
 
-    return size_diff < args.sizes_delta and count_diff < args.counts_delta and duration_diff < args.durations_delta
+    return all(bools)
 
 
 def cluster_by_numbers(args, media):
     group_id = 0
     temp_groups = []
     media_groups = []
     for m in media:
@@ -155,25 +160,23 @@
 
 
 def similar_folders():
     args = parse_args()
     media = arg_utils.gen_d(args)
     media = [d if "size" in d else file_utils.get_filesize(d) for d in media]
     media = big_dirs.group_files_by_parent(args, media)
-    if args.folder_sizes:
-        media = [d for d in media if args.folder_sizes(d["size"])]
+    media = big_dirs.process_big_dirs(args, media)
 
     if args.filter_sizes or args.filter_counts or args.filter_durations:
         clusters = cluster_by_numbers(args, media)
         groups = map_and_name(media, clusters)
         log.info("Folder size/duration/count clustering sorted %s folders into %s groups", len(media), len(groups))
         single_folder_groups = [d for d in groups if len(d["grouped_paths"]) == 1]
         groups = [d for d in groups if len(d["grouped_paths"]) > 1]
         log.info("Filtered out %s single-folder groups", len(single_folder_groups))
-        log.debug(single_folder_groups)
 
         if args.filter_names:
             media = [d for group in groups for d in group["grouped_paths"]]
 
     if args.filter_names:
         groups = cluster_folders(args, media)
         groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_path"])))
@@ -196,32 +199,27 @@
         if args.only_duplicates:
             media = media[1:]
 
         if "f" in args.print:
             for d in media:
                 printing.pipe_print(d["path"])
         else:
-            print(
-                tabulate(
-                    [
-                        {
-                            f'group {group["common_path"]}': d["path"],
-                            "total_size": humanize.naturalsize(d["size"], binary=True),
-                            "median_size": humanize.naturalsize(d["median_size"], binary=True),
-                            "total_duration": printing.human_duration(d["duration"]),
-                            "median_duration": printing.human_duration(d["median_duration"]),
-                            "median_size": humanize.naturalsize(d["median_size"], binary=True),
-                            "files": d["exists"],
-                        }
-                        for d in media
-                    ],
-                    tablefmt=consts.TABULATE_STYLE,
-                    headers="keys",
-                    showindex=False,
-                )
+            printing.table(
+                [
+                    {
+                        f'group {group["common_path"]}': d["path"],
+                        "total_size": humanize.naturalsize(d["size"], binary=True),
+                        "median_size": humanize.naturalsize(d["median_size"], binary=True),
+                        "total_duration": printing.human_duration(d.get("duration")),
+                        "median_duration": printing.human_duration(d.get("median_duration")),
+                        "median_size": humanize.naturalsize(d.get("median_size"), binary=True),
+                        "files": d["exists"],
+                    }
+                    for d in media
+                ]
             )
 
         if not args.only_originals and not args.only_duplicates:
             print()
 
     if not args.only_originals and not args.only_duplicates:
         print(len(groups), "groups found")
```

### Comparing `xklb-2.8.3/xklb/fsdb/disk_usage.py` & `xklb-2.8.6/xklb/fsdb/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/fsdb/search_db.py` & `xklb-2.8.6/xklb/fsdb/search_db.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,78 +6,78 @@
 
 def parse_args() -> argparse.Namespace:
     parser = argparse_utils.ArgumentParser(prog="library search-db", usage=usage.search_db)
     arggroups.sql_fs(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
-    parser.add_argument("table")
+    parser.add_argument("search_table")
     parser.add_argument("search", nargs="+")
     args = parser.parse_intermixed_args()
 
     arggroups.sql_fs_post(args)
 
     arggroups.args_post(args, parser, create_db=True)
     return args
 
 
 def get_table_name(args):
-    if args.table in args.db.table_names():
-        return args.table
+    if args.search_table in args.db.table_names():
+        return args.search_table
 
     valid_tables = []
     for s in args.db.table_names():
         if "_fts_" in s or s.endswith("_fts") or "sqlite_stat" in s:
             continue
         valid_tables.append(s)
 
     matching_tables = []
     for s in valid_tables:
-        if s.startswith(args.table):
+        if s.startswith(args.search_table):
             matching_tables.append(s)
 
     if len(matching_tables) == 1:
         return matching_tables[0]
 
-    msg = f"Table {args.table} does not exist in {args.database}"
+    msg = f"Table {args.search_table} does not exist in {args.database}"
     raise ValueError(msg)
 
 
 def search_db() -> None:
     args = parse_args()
-    args.table = get_table_name(args)
+    args.search_table = get_table_name(args)
 
     args.filter_sql = []
     args.filter_bindings = {}
 
-    columns = args.db[args.table].columns_dict
+    columns = args.db[args.search_table].columns_dict
     sql_utils.construct_search_bindings(args, columns)
 
     if args.delete_rows:  # TODO: replace with media_printer?
         deleted_count = 0
         with args.db.conn:
             cursor = args.db.conn.execute(
-                f"DELETE FROM {args.table} WHERE 1=1 " + " ".join(args.filter_sql),
+                f"DELETE FROM {args.search_table} WHERE 1=1 " + " ".join(args.filter_sql),
                 args.filter_bindings,
             )
             deleted_count += cursor.rowcount
         print(f"Deleted {deleted_count} rows")
     elif args.mark_deleted:
         modified_row_count = 0
         with args.db.conn:
             cursor = args.db.conn.execute(
-                f"UPDATE {args.table} SET time_deleted={consts.APPLICATION_START} WHERE 1=1 "
+                f"UPDATE {args.search_table} SET time_deleted={consts.APPLICATION_START} WHERE 1=1 "
                 + " ".join(args.filter_sql),
                 args.filter_bindings,
             )
             modified_row_count += cursor.rowcount
         print(f"Marked {modified_row_count} rows as deleted")
     else:
         for row in args.db.execute_returning_dicts(
-            f"SELECT * FROM {args.table} WHERE 1=1 " + " ".join(args.filter_sql),
+            f"SELECT * FROM {args.search_table} WHERE 1=1 " + " ".join(args.filter_sql),
             args.filter_bindings,
         ):
             print(json.dumps(row))
 
 
 if __name__ == "__main__":
     search_db()
```

### Comparing `xklb-2.8.3/xklb/mediadb/block.py` & `xklb-2.8.6/xklb/mediadb/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediadb/db_history.py` & `xklb-2.8.6/xklb/mediadb/db_history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediadb/db_media.py` & `xklb-2.8.6/xklb/mediadb/db_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediadb/db_playlists.py` & `xklb-2.8.6/xklb/mediadb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediadb/download.py` & `xklb-2.8.6/xklb/mediadb/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     parser.add_argument("--photos", action="store_true", help="Image: Download JPG and WEBP")
     parser.add_argument("--drawings", action="store_true", help="Image: Download PNG")
     parser.add_argument("--gifs", action="store_true", help="Image: Download MP4 and GIFs")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     arggroups.paths_or_stdin(parser)
-    parser.set_defaults(paths=None)
+    parser.set_defaults(paths=None, fts=False)
 
     args, unk = parser.parse_known_intermixed_args()
     arggroups.args_post(args, parser)
 
     if unk and not args.profile in (DBType.video, DBType.audio):
         parser.error(f"unrecognized arguments: {' '.join(unk)}")
     args.unk = unk
```

### Comparing `xklb-2.8.3/xklb/mediadb/download_status.py` & `xklb-2.8.6/xklb/mediadb/download_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
     parser.set_defaults(print="p")
 
     arggroups.download(parser)
 
     arggroups.debug(parser)
     arggroups.database(parser)
+
+    parser.set_defaults(fts=False)
     args = parser.parse_args()
     arggroups.args_post(args, parser)
 
     arggroups.sql_fs_post(args)
     return args
```

### Comparing `xklb-2.8.3/xklb/mediadb/history.py` & `xklb-2.8.6/xklb/mediadb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediadb/history_add.py` & `xklb-2.8.6/xklb/mediadb/history_add.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediadb/playlists.py` & `xklb-2.8.6/xklb/mediadb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediadb/redownload.py` & `xklb-2.8.6/xklb/mediadb/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediadb/search.py` & `xklb-2.8.6/xklb/mediadb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediadb/stats.py` & `xklb-2.8.6/xklb/mediadb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediafiles/media_check.py` & `xklb-2.8.6/xklb/mediafiles/media_check.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediafiles/process_ffmpeg.py` & `xklb-2.8.6/xklb/mediafiles/process_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/mediafiles/process_image.py` & `xklb-2.8.6/xklb/mediafiles/process_image.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/misc/dedupe_czkawka.py` & `xklb-2.8.6/xklb/misc/dedupe_czkawka.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/misc/export_text.py` & `xklb-2.8.6/xklb/misc/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/multidb/copy_play_counts.py` & `xklb-2.8.6/xklb/multidb/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/multidb/merge_dbs.py` & `xklb-2.8.6/xklb/multidb/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/playback/links_open.py` & `xklb-2.8.6/xklb/playback/links_open.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     arggroups.related(parser)
 
     parser.add_argument("--browser")
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
+
+    parser.set_defaults(limit="7")
     args = parser.parse_intermixed_args()
     arggroups.args_post(args, parser)
 
     arggroups.sql_fs_post(args)
 
     if not args.title_prefix:
         args.title_prefix = ["https://www.google.com/search?q=%"]
```

### Comparing `xklb-2.8.3/xklb/playback/media_player.py` & `xklb-2.8.6/xklb/playback/media_player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/playback/play_actions.py` & `xklb-2.8.6/xklb/playback/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/playback/playback_control.py` & `xklb-2.8.6/xklb/playback/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/playback/post_actions.py` & `xklb-2.8.6/xklb/playback/post_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,21 @@
     keep_path.mkdir(exist_ok=True)
 
     try:
         new_path = shutil.move(media_file, keep_path)
     except shutil.Error as e:
         if "already exists" not in str(e):
             raise
+
         p = Path(media_file)
         new_path = Path(keep_path) / p.name
 
+        if media_file == keep_path:
+            raise shutil.SameFileError
+
         src_size = p.stat().st_size
         dst_size = new_path.stat().st_size
 
         src_size_str = humanize.naturalsize(src_size, binary=True)
         dst_size_str = humanize.naturalsize(dst_size, binary=True)
         diff_size_str = humanize.naturalsize(src_size - dst_size, binary=True)
```

### Comparing `xklb-2.8.3/xklb/playback/surf.py` & `xklb-2.8.6/xklb/playback/surf.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/playback/tabs_open.py` & `xklb-2.8.6/xklb/playback/tabs_open.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from xklb import media_printer, usage
 from xklb.mediadb import db_history
 from xklb.utils import arggroups, argparse_utils, consts, processes
 from xklb.utils.log_utils import log
 from xklb.utils.sqlgroups import construct_tabs_query
 
 
-def parse_args(action) -> argparse.Namespace:
+def parse_args() -> argparse.Namespace:
     parser = argparse_utils.ArgumentParser(
         prog="library tabs",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         usage=usage.tabs_open,
     )
 
     arggroups.sql_fs(parser)
@@ -50,15 +50,15 @@
 
         filtered_media.extend([m for m in media if m["frequency"] == freq][:num_tabs])
 
     return filtered_media
 
 
 def tabs_open() -> None:
-    args = parse_args(consts.SC.tabs_open)
+    args = parse_args()
     db_history.create(args)
 
     query, bindings = construct_tabs_query(args)
 
     if args.print or args.delete_rows or args.mark_deleted or args.mark_watched:
         media_printer.printer(args, query, bindings)
         return
```

### Comparing `xklb-2.8.3/xklb/scratch/javguru.py` & `xklb-2.8.6/xklb/scratch/javguru.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/scratch/javtiful.py` & `xklb-2.8.6/xklb/scratch/javtiful.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/scratch/mam_search.py` & `xklb-2.8.6/xklb/scratch/mam_search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/scratch/mam_slots.py` & `xklb-2.8.6/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/tablefiles/eda.py` & `xklb-2.8.6/xklb/tablefiles/eda.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/tablefiles/incremental_diff.py` & `xklb-2.8.6/xklb/tablefiles/incremental_diff.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/tablefiles/mcda.py` & `xklb-2.8.6/xklb/tablefiles/mcda.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
     df = auto_mcda(args, df, alternatives, minimize_cols={s.lstrip("-") for s in columns if s.startswith("-")})
     return df
 
 
 def group_sort_by(args, folders):
     if args.sort_groups_by is None:
-        sort_func = lambda x: (0, x["size"] / x["exists"]) if x["exists"] else (1, x["size"] / x["total"])
+        sort_func = lambda x: (0, -x["size"] / x["exists"]) if x["exists"] else (1, -x["size"] / x["total"])
     elif args.sort_groups_by.startswith("mcda "):
         import pandas as pd
 
         if not isinstance(folders, pd.DataFrame):
             folders = pd.DataFrame(folders)
         values = args.sort_groups_by.replace("mcda ", "", 1)
         df = sort(args, folders, values)
```

### Comparing `xklb-2.8.3/xklb/text/cluster_sort.py` & `xklb-2.8.6/xklb/text/cluster_sort.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                     **group,
                     "size": sum(
                         media_keyed[s].get("size") or 0
                         for s in group["grouped_paths"]
                         if not bool(media_keyed[s].get("time_deleted"))
                     ),
                     "median_size": nums.safe_median(
-                        media_keyed[s].get("size") or 0
+                        media_keyed[s].get("size")
                         for s in group["grouped_paths"]
                         if not bool(media_keyed[s].get("time_deleted"))
                     ),
                     "total": len(group["grouped_paths"]),
                     "exists": sum(not bool(media_keyed[s].get("time_deleted")) for s in group["grouped_paths"]),
                     "deleted": sum(bool(media_keyed[s].get("time_deleted")) for s in group["grouped_paths"]),
                     "deleted_size": sum(
```

### Comparing `xklb-2.8.3/xklb/text/extract_links.py` & `xklb-2.8.6/xklb/text/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/text/extract_text.py` & `xklb-2.8.6/xklb/text/extract_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/text/markdown_links.py` & `xklb-2.8.6/xklb/text/markdown_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/text/nouns.py` & `xklb-2.8.6/xklb/text/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/arg_utils.py` & `xklb-2.8.6/xklb/utils/arg_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                     else:
                         yield path
 
 
 def gen_d(args):
     if args.from_file:
         for path in args.paths:
-            with open(path) as f:
+            with open(path, "r") as f:
                 for line in f:
                     line = line.rstrip("\n")
                     if line.strip():
                         if args.from_json:
                             json_data = json.loads(line)
                             if isinstance(json_data, list):
                                 yield from json_data
```

### Comparing `xklb-2.8.3/xklb/utils/arggroups.py` & `xklb-2.8.6/xklb/utils/arggroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 
 def get_caller_name():
     import inspect
 
     frame = inspect.currentframe()
     while frame:
         frame = frame.f_back
-        if frame.f_code.co_name == "parse_args":
+
+        if frame is None:
+            return "No parse_args()"
+        elif frame.f_code.co_name == "parse_args":
             frame = frame.f_back
             return frame.f_code.co_name
 
 
 def args_post(args, parser, create_db=False):
     args.defaults = [k for k, v in args.__dict__.items() if parser.get_default(k) == v]
     settings = {k: v for k, v in args.__dict__.items() if k not in ["database", "verbose", "defaults"] + args.defaults}
@@ -252,14 +255,15 @@
         )
     if args.downloaded_before:
         args.filter_sql.append(
             f"and time_downloaded < cast(STRFTIME('%s', datetime( 'now', '-{nums.sql_human_time(args.downloaded_before)}')) as int)",
         )
 
     if getattr(args, "keep_dir", False) and Path(args.keep_dir).exists():
+        args.keep_dir = Path(args.keep_dir).expanduser().resolve()
         args.filter_sql.append(f'and path not like "{args.keep_dir}%"')
 
     if args.no_video:
         args.filter_sql.append(" and video_count=0 ")
     if args.no_audio:
         args.filter_sql.append(" and audio_count=0 ")
     if args.subtitles:
@@ -337,17 +341,14 @@
     parser.add_argument("--exit-code-confirm", action="store_true")
     parser.add_argument("--gui", action="store_true")
     parser.add_argument("--keep-dir", "--keepdir")
     parser.add_argument("--post-action", "--action", "-k", default="keep")
 
 
 def post_actions_post(args):
-    if args.keep_dir:
-        args.keep_dir = Path(args.keep_dir).expanduser().resolve()
-
     if args.post_action:
         args.post_action = args.post_action.replace("-", "_")
 
 
 def multiple_playback(parent_parser):
     parser = parent_parser.add_argument_group("Multiple Playback")
     parser.add_argument(
@@ -422,27 +423,31 @@
         "--files",
         "--counts",
         "--episodes",
         "-FC",
         action="append",
         help="Number of files per folder",
     )
-    parser.add_argument("--folders-count", action="append", help="TODO: Number of folders per folder")
+    parser.add_argument(
+        "--folders-counts", action="append", help="Only include folders with specific number of subfolders"
+    )
 
 
 def group_folders_post(args) -> None:
     if args.solo:
         args.folder_counts = ["1"]
     if args.sibling:
         args.folder_counts = ["+2"]
 
     if args.folder_sizes:
         args.folder_sizes = sql_utils.parse_human_to_lambda(nums.human_to_bytes, args.folder_sizes)
     if args.folder_counts:
         args.folder_counts = sql_utils.parse_human_to_lambda(int, args.folder_counts)
+    if args.folders_counts:
+        args.folders_counts = sql_utils.parse_human_to_lambda(int, args.folders_counts)
 
     if args.sort_groups_by:
         args.sort_groups_by = arg_utils.parse_ambiguous_sort(args.sort_groups_by)
         args.sort_groups_by = ",".join(args.sort_groups_by)
 
 
 def cluster(parent_parser):
```

### Comparing `xklb-2.8.3/xklb/utils/argparse_utils.py` & `xklb-2.8.6/xklb/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/consts.py` & `xklb-2.8.6/xklb/utils/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/db_utils.py` & `xklb-2.8.6/xklb/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/devices.py` & `xklb-2.8.6/xklb/utils/devices.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/file_utils.py` & `xklb-2.8.6/xklb/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/gui.py` & `xklb-2.8.6/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/iterables.py` & `xklb-2.8.6/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/log_utils.py` & `xklb-2.8.6/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/mpv_utils.py` & `xklb-2.8.6/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/nums.py` & `xklb-2.8.6/xklb/utils/nums.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,15 +51,24 @@
         return s
 
 
 def safe_median(l) -> float | None:
     if not l:
         return None
     try:
-        return statistics.median(l)
+        return statistics.median(v for v in l if v is not None)
+    except statistics.StatisticsError:
+        return None
+
+
+def safe_mean(l) -> float | None:
+    if not l:
+        return None
+    try:
+        return statistics.mean(v for v in l if v is not None)
     except statistics.StatisticsError:
         return None
 
 
 def human_to_bytes(input_str) -> int:
     byte_map = {"b": 1, "kb": 1024, "mb": 1024**2, "gb": 1024**3, "tb": 1024**4, "pb": 1024**5}
```

### Comparing `xklb-2.8.3/xklb/utils/objects.py` & `xklb-2.8.6/xklb/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/path_utils.py` & `xklb-2.8.6/xklb/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/pd_utils.py` & `xklb-2.8.6/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/printing.py` & `xklb-2.8.6/xklb/utils/printing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 import csv, math, os, platform, sys, textwrap
 from datetime import datetime, timedelta
 
 import humanize
+from tabulate import tabulate
 
 from xklb.utils import consts
 
 
 def print_overwrite(*text):
     if os.name == "posix":
         print("\r" + text[0], *text[1:], end="\033[K", flush=True)
     elif platform.system() == "Windows":
         print("\r" + text[0], *text[1:], end="", flush=True)
     else:
         print(text)
 
 
+def table(tbl, *args, **kwargs) -> None:
+    try:
+        print(tabulate(tbl, tablefmt=consts.TABULATE_STYLE, headers="keys", showindex=False, *args, **kwargs))
+    except BrokenPipeError:
+        sys.stdout = None
+        sys.exit(141)
+
+
 def pipe_print(*args) -> None:
     try:
         print(*args, flush=True)
     except BrokenPipeError:
         sys.stdout = None
         sys.exit(141)
```

### Comparing `xklb-2.8.3/xklb/utils/processes.py` & `xklb-2.8.6/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/sql_utils.py` & `xklb-2.8.6/xklb/utils/sql_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,18 +339,18 @@
         if getattr(args, "exact", False):
             args.filter_bindings[f"exclude{idx}"] = exc
         else:
             args.filter_bindings[f"exclude{idx}"] = "%" + exc.replace(" ", "%").replace("%%", " ") + "%"
 
 
 def search_filter(args, m_columns):
-    args.table = "media"
+    table = "media"
     if args.db["media"].detect_fts() and args.fts:
         if args.include:
-            args.table, search_bindings = fts_search_sql(
+            table, search_bindings = fts_search_sql(
                 "media",
                 fts_table=args.db["media"].detect_fts(),
                 include=args.include,
                 exclude=args.exclude,
                 flexible=args.flexible_search,
             )
             args.filter_bindings = {**args.filter_bindings, **search_bindings}
@@ -362,8 +362,8 @@
             )
     else:
         construct_search_bindings(
             args,
             [f"m.{k}" for k in m_columns if k in db_utils.config["media"]["search_columns"] if k in m_columns],
         )
 
-    return m_columns
+    return table, m_columns
```

### Comparing `xklb-2.8.3/xklb/utils/sqlgroups.py` & `xklb-2.8.6/xklb/utils/sqlgroups.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     select_sql = "\n        , ".join(args.select)
     return select_sql
 
 
 def fs_sql(args) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     query = f"""
         SELECT
             {media_select_sql(args, m_columns)}
         FROM {args.table} m
         WHERE 1=1
             {" ".join(args.filter_sql)}
@@ -36,15 +36,15 @@
         {sql_utils.limit_sql(args)}
     """
 
     return query, args.filter_bindings
 
 
 def perf_randomize_using_ids(args, m_columns):
-    if args.table == "media" and args.random and not args.print and args.limit in args.defaults:
+    if args.random and not args.include and not args.print and args.limit in args.defaults:
         limit = 16 * (args.limit or consts.DEFAULT_PLAY_QUEUE)
         where_not_deleted = (
             "where COALESCE(time_deleted,0) = 0"
             if "time_deleted" in m_columns
             and "deleted" not in args.sort_groups_by
             and "time_deleted" not in " ".join(args.where)
             else ""
@@ -52,15 +52,15 @@
         args.filter_sql.append(
             f"and m.id in (select id from media {where_not_deleted} order by random() limit {limit})",
         )
 
 
 def media_sql(args) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     perf_randomize_using_ids(args, m_columns)
 
     select_sql = media_select_sql(args, m_columns)
 
     query = f"""WITH m as (
             SELECT
@@ -95,15 +95,15 @@
     ]  # only use random id constraint in first query
 
     return query, args.filter_bindings
 
 
 def historical_media(args):
     m_columns = args.db["media"].columns_dict
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     query = f"""WITH m as (
             SELECT
                 SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , MIN(h.time_played) time_first_played
                 , MAX(h.time_played) time_last_played
                 , FIRST_VALUE(h.playhead) OVER (PARTITION BY h.media_id ORDER BY h.time_played DESC) playhead
@@ -127,34 +127,34 @@
         LIMIT {args.limit or 5}
     """
     return query, args.filter_bindings
 
 
 def construct_links_query(args) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     args.select = ["path"]
     if args.cols:
         args.select.extend(args.cols)
     for s in ["title", "hostname", "category"]:
         if s in m_columns:
             args.select.append(s)
 
     query = f"""WITH m as (
             SELECT
                 {', '.join(args.select) if args.select else ''}
                 , COALESCE(MAX(h.time_played), 0) time_last_played
                 , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , time_deleted
-            FROM media m
-            LEFT JOIN history h on h.media_id = media.id
+            FROM {args.table} m
+            LEFT JOIN history h on h.media_id = m.id
             WHERE 1=1
                 {" ".join(args.filter_sql)}
-            GROUP BY media.id
+            GROUP BY m.id
         )
         SELECT
         {', '.join(args.select) if args.select else ''}
         {", time_last_played" if args.print else ''}
     FROM m
     WHERE 1=1
         {" ".join(args.aggregate_filter_sql)}
@@ -168,26 +168,26 @@
     """
 
     return query, args.filter_bindings
 
 
 def construct_tabs_query(args) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     query = f"""WITH m as (
             SELECT
                 path
                 , frequency
                 , COALESCE(MAX(h.time_played), 0) time_last_played
                 , SUM(CASE WHEN h.done = 1 THEN 1 ELSE 0 END) play_count
                 , time_deleted
                 , hostname
                 , category
-            FROM media m
+            FROM {args.table} m
             LEFT JOIN history h on h.media_id = m.id
             WHERE 1=1
                 {" ".join(args.filter_sql)}
             GROUP BY m.id
         )
         SELECT path
         , frequency
@@ -226,15 +226,15 @@
     return query, args.filter_bindings
 
 
 def construct_captions_search_query(args) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
     c_columns = db_utils.columns(args, "captions")
 
-    m_columns = sql_utils.search_filter(args, m_columns)
+    m_table, m_columns = sql_utils.search_filter(args, m_columns)
 
     table = "captions"
     cols = args.cols or ["path", "text", "time", "title"]
 
     is_fts = args.db["captions"].detect_fts()
     if is_fts and args.include:
         table, search_bindings = sql_utils.fts_search_sql(
@@ -259,32 +259,32 @@
         SELECT * FROM {table} m
         WHERE 1=1
             {" ".join(args.filter_sql)}
     )
     SELECT
         {select_sql}
     FROM c
-    JOIN media m on m.id = c.media_id
+    JOIN {m_table} m on m.id = c.media_id
     WHERE 1=1
         {" ".join(args.aggregate_filter_sql)}
     ORDER BY 1=1
         , {args.sort}
     {limit_sql}
     """
 
     return query, args.filter_bindings
 
 
 def construct_playlists_query(args) -> tuple[str, dict]:
     pl_columns = db_utils.columns(args, "playlists")
 
-    args.table = "playlists"
+    pl_table = "playlists"
     if args.db["playlists"].detect_fts():
         if args.include:
-            args.table, search_bindings = sql_utils.fts_search_sql(
+            pl_table, search_bindings = sql_utils.fts_search_sql(
                 "playlists",
                 fts_table=args.db["playlists"].detect_fts(),
                 include=args.include,
                 exclude=args.exclude,
                 flexible=args.flexible_search,
             )
             args.filter_bindings = {**args.filter_bindings, **search_bindings}
@@ -296,15 +296,15 @@
     else:
         sql_utils.construct_search_bindings(
             args,
             [k for k in pl_columns if k in db_utils.config["playlists"]["search_columns"] if k in pl_columns],
         )
 
     query = f"""SELECT *
-    FROM {args.table} m
+    FROM {pl_table} m
     WHERE 1=1
         {" ".join(args.filter_sql)}
         {'AND extractor_key != "Local"' if args.online_media_only else ''}
         {'AND extractor_key = "Local"' if args.local_media_only else ''}
     ORDER BY 1=1
         {', ' + args.playlists_sort if args.playlists_sort else ''}
         , path
@@ -315,15 +315,15 @@
     return query, args.filter_bindings
 
 
 def construct_download_query(args) -> tuple[str, dict]:
     m_columns = db_utils.columns(args, "media")
     pl_columns = db_utils.columns(args, "playlists")
 
-    m_columns = sql_utils.search_filter(args, m_columns)
+    args.table, m_columns = sql_utils.search_filter(args, m_columns)
 
     if args.action == SC.download and "time_modified" in m_columns:
         args.filter_sql.append(
             f"""and cast(STRFTIME('%s',
             datetime( COALESCE(m.time_modified,0), 'unixepoch', '+{args.retry_delay}')
             ) as int) < STRFTIME('%s', datetime()) """,
         )
@@ -349,15 +349,15 @@
                 {', m.size' if 'size' in m_columns else ''}
                 {', m.time_modified' if 'time_modified' in m_columns else ''}
                 {', m.time_downloaded' if 'time_downloaded' in m_columns else ''}
                 {', m.time_deleted' if 'time_deleted' in m_columns else ''}
                 {', m.error' if 'error' in m_columns and args.verbose >= consts.LOG_DEBUG else ''}
                 {', p.extractor_config' if 'extractor_config' in pl_columns else ''}
                 , p.extractor_key
-            FROM media m
+            FROM {args.table} m
             LEFT JOIN playlists p on p.id = m.playlists_id
             WHERE 1=1
                 {'and COALESCE(m.time_downloaded,0) = 0' if 'time_downloaded' in m_columns else ''}
                 {'and COALESCE(p.time_deleted, 0) = 0' if 'time_deleted' in pl_columns else ''}
                 and m.path like "http%"
                 {same_subdomain if getattr(args, 'same_domain', False) else ''}
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
@@ -378,15 +378,15 @@
                 {', m.time_created' if 'time_created' in m_columns else ''}
                 {', m.size' if 'size' in m_columns else ''}
                 {', m.time_modified' if 'time_modified' in m_columns else ''}
                 {', m.time_downloaded' if 'time_downloaded' in m_columns else ''}
                 {', m.time_deleted' if 'time_deleted' in m_columns else ''}
                 {', m.error' if 'error' in m_columns and args.verbose >= consts.LOG_DEBUG else ''}
                 , 'Playlist-less media' as extractor_key
-            FROM media m
+            FROM {args.table} m
             WHERE 1=1
                 {'and COALESCE(m.time_downloaded,0) = 0' if 'time_downloaded' in m_columns else ''}
                 {'and COALESCE(m.time_deleted,0) = 0' if 'time_deleted' in m_columns else ''}
                 and m.path like "http%"
                 {same_subdomain if getattr(args, 'same_domain', '') else ''}
                 {'AND (score IS NULL OR score > 7)' if 'score' in m_columns else ''}
                 {'AND (upvote_ratio IS NULL OR upvote_ratio > 0.73)' if 'upvote_ratio' in m_columns else ''}
```

### Comparing `xklb-2.8.3/xklb/utils/strings.py` & `xklb-2.8.6/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/utils/web.py` & `xklb-2.8.6/xklb/utils/web.py`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/xklb/assets/kotobago.png` & `xklb-2.8.6/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/.gitignore` & `xklb-2.8.6/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/pyproject.toml` & `xklb-2.8.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.8.3/.github/README.md` & `xklb-2.8.6/.github/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    library (v2.8.003; 72 subcommands)
+    library (v2.8.006; 72 subcommands)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
```

### Comparing `xklb-2.8.3/PKG-INFO` & `xklb-2.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.8.3
+Version: 2.8.6
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
-    library (v2.8.003; 72 subcommands)
+    library (v2.8.006; 72 subcommands)
 
     Create database subcommands:
     ╭───────────────┬──────────────────────────────────────────╮
     │ fs-add        │ Add local media                          │
     ├───────────────┼──────────────────────────────────────────┤
     │ tube-add      │ Add online video media (yt-dlp)          │
     ├───────────────┼──────────────────────────────────────────┤
```

