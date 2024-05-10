# Comparing `tmp/dghs_imgutils-0.4.3.tar.gz` & `tmp/dghs_imgutils-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dghs_imgutils-0.4.3.tar", last modified: Fri May  3 17:38:27 2024, max compression
+gzip compressed data, was "dghs_imgutils-0.4.4.tar", last modified: Fri May 10 14:49:50 2024, max compression
```

## Comparing `dghs_imgutils-0.4.3.tar` & `dghs_imgutils-0.4.4.tar`

### file list

```diff
@@ -1,131 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.903425 dghs_imgutils-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-03 17:37:43.000000 dghs_imgutils-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-03 17:37:43.000000 dghs_imgutils-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-03 17:38:27.903425 dghs_imgutils-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-03 17:37:43.000000 dghs_imgutils-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.895425 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-03 17:38:27.000000 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-03 17:38:27.000000 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:38:27.000000 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-03 17:38:27.000000 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 17:38:27.000000 dghs_imgutils-0.4.3/dghs_imgutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.883425 dghs_imgutils-0.4.3/imgutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.883425 dghs_imgutils-0.4.3/imgutils/ascii/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ascii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ascii/drawing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.883425 dghs_imgutils-0.4.3/imgutils/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/data/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/background.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/data/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/detect/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/censor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/eye.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/face.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/halfbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/hand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/head.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/detect/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/edge/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/edge/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/edge/canny.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/edge/lineart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/edge/lineart_anime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/generic/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/generic/classify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/aesthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)    23332 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/ccip.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/dbaesthetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/laplacian.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/lpips.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/metrics/psnr_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.887425 dghs_imgutils-0.4.3/imgutils/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ocr/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ocr/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/ocr/recognize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/operate/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/align.py
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/censor_.py
--rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/emoji_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)    83886 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/heart_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/imgcensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    74310 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/smile_censor.png
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/operate/squeeze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/pose/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/pose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/pose/dwpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/pose/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/pose/visual.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/resource/background.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/restore/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/restore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/restore/adversarial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/restore/nafnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/restore/scunet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/sd/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/sd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/sd/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/sd/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.891425 dghs_imgutils-0.4.3/imgutils/segment/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/segment/isnetis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.895425 dghs_imgutils-0.4.3/imgutils/tagging/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/character.py
--rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/deepdanbooru.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/match.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/mldanbooru.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/tagging/wd14.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.895425 dghs_imgutils-0.4.3/imgutils/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/utils/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/utils/onnxruntime.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/utils/tqdm_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:38:27.895425 dghs_imgutils-0.4.3/imgutils/validate/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/aicheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/bangumi_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/completeness.py
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/dbrating.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/monochrome.py
--rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/nsfw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/portrait.py
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/rating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/real.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/safe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/style_age.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/teen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/imgutils/validate/truncate.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements-model.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements-zoo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:38:27.903425 dghs_imgutils-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-03 17:37:45.000000 dghs_imgutils-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.456571 dghs_imgutils-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-10 14:49:06.000000 dghs_imgutils-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-10 14:49:06.000000 dghs_imgutils-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-10 14:49:50.456571 dghs_imgutils-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-10 14:49:06.000000 dghs_imgutils-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.448571 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19108 2024-05-10 14:49:50.000000 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-10 14:49:50.000000 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:49:50.000000 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-10 14:49:50.000000 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 14:49:50.000000 dghs_imgutils-0.4.4/dghs_imgutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.436571 dghs_imgutils-0.4.4/imgutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ascii/drawing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/data/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/censor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/eye.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/halfbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/hand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/detect/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/edge/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/edge/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/edge/canny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/edge/lineart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/edge/lineart_anime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.440571 dghs_imgutils-0.4.4/imgutils/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/generic/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/generic/enhance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/aesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23332 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/ccip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/dbaesthetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/laplacian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/lpips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/metrics/psnr_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ocr/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ocr/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/ocr/recognize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/operate/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/censor_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/emoji_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83886 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/heart_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/imgcensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74310 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/smile_censor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/operate/squeeze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/pose/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/pose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/pose/dwpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/pose/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/pose/visual.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/resource/background.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/restore/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/restore/adversarial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/restore/nafnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/restore/scunet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/sd/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/sd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19044 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/sd/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/sd/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.444571 dghs_imgutils-0.4.4/imgutils/segment/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/segment/isnetis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.448571 dghs_imgutils-0.4.4/imgutils/tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/deepdanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/mldanbooru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/tagging/wd14.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.448571 dghs_imgutils-0.4.4/imgutils/upscale/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/upscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/upscale/cdc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.448571 dghs_imgutils-0.4.4/imgutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/utils/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/utils/onnxruntime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/utils/tqdm_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:49:50.448571 dghs_imgutils-0.4.4/imgutils/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/aicheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/bangumi_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/dbrating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/nsfw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/portrait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/style_age.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/teen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/imgutils/validate/truncate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements-model.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements-zoo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:49:50.456571 dghs_imgutils-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-10 14:49:08.000000 dghs_imgutils-0.4.4/setup.py
```

### Comparing `dghs_imgutils-0.4.3/LICENSE` & `dghs_imgutils-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/PKG-INFO` & `dghs_imgutils-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.4.3
+Version: 0.4.4
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d7
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dghs_imgutils-0.4.3/README.md` & `dghs_imgutils-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/dghs_imgutils.egg-info/PKG-INFO` & `dghs_imgutils-0.4.4/dghs_imgutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dghs-imgutils
-Version: 0.4.3
+Version: 0.4.4
 Summary: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Home-page: https://github.com/deepghs/imgutils
 Author: narugo1992, 7eu7d7
 Author-email: narugo992@gmail.com
 License: Apache License, Version 2.0
 Keywords: A convenient and user-friendly anime-style image data processing library that integrates various advanced anime-style image processing models.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dghs_imgutils-0.4.3/dghs_imgutils.egg-info/SOURCES.txt` & `dghs_imgutils-0.4.4/dghs_imgutils.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 imgutils/edge/__init__.py
 imgutils/edge/_base.py
 imgutils/edge/canny.py
 imgutils/edge/lineart.py
 imgutils/edge/lineart_anime.py
 imgutils/generic/__init__.py
 imgutils/generic/classify.py
+imgutils/generic/enhance.py
 imgutils/metrics/__init__.py
 imgutils/metrics/aesthetic.py
 imgutils/metrics/ccip.py
 imgutils/metrics/dbaesthetic.py
 imgutils/metrics/laplacian.py
 imgutils/metrics/lpips.py
 imgutils/metrics/psnr_.py
@@ -82,14 +83,16 @@
 imgutils/tagging/deepdanbooru.py
 imgutils/tagging/format.py
 imgutils/tagging/match.py
 imgutils/tagging/mldanbooru.py
 imgutils/tagging/order.py
 imgutils/tagging/overlap.py
 imgutils/tagging/wd14.py
+imgutils/upscale/__init__.py
+imgutils/upscale/cdc.py
 imgutils/utils/__init__.py
 imgutils/utils/area.py
 imgutils/utils/onnxruntime.py
 imgutils/utils/storage.py
 imgutils/utils/tqdm_.py
 imgutils/validate/__init__.py
 imgutils/validate/aicheck.py
```

### Comparing `dghs_imgutils-0.4.3/dghs_imgutils.egg-info/requires.txt` & `dghs_imgutils-0.4.4/dghs_imgutils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/ascii/drawing.py` & `dghs_imgutils-0.4.4/imgutils/ascii/drawing.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/config/meta.py` & `dghs_imgutils-0.4.4/imgutils/config/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Meta information for imgutils package.
 """
 
 #: Title of this project (should be `imgutils`).
 __TITLE__ = 'imgutils'
 
 #: Version of this project.
-__VERSION__ = '0.4.3'
+__VERSION__ = '0.4.4'
 
 #: Short description of the project, will be included in ``setup.py``.
 __DESCRIPTION__ = 'A convenient and user-friendly anime-style image data processing library that integrates ' \
                   'various advanced anime-style image processing models.'
 
 #: Author of this project.
 __AUTHOR__ = 'narugo1992, 7eu7d7'
```

### Comparing `dghs_imgutils-0.4.3/imgutils/data/background.py` & `dghs_imgutils-0.4.4/imgutils/data/background.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/data/decode.py` & `dghs_imgutils-0.4.4/imgutils/data/decode.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/data/encode.py` & `dghs_imgutils-0.4.4/imgutils/data/encode.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/data/image.py` & `dghs_imgutils-0.4.4/imgutils/data/image.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/data/layer.py` & `dghs_imgutils-0.4.4/imgutils/data/layer.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/__init__.py` & `dghs_imgutils-0.4.4/imgutils/detect/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/_yolo.py` & `dghs_imgutils-0.4.4/imgutils/detect/_yolo.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/censor.py` & `dghs_imgutils-0.4.4/imgutils/detect/censor.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/eye.py` & `dghs_imgutils-0.4.4/imgutils/detect/eye.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/face.py` & `dghs_imgutils-0.4.4/imgutils/detect/face.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/halfbody.py` & `dghs_imgutils-0.4.4/imgutils/detect/halfbody.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/hand.py` & `dghs_imgutils-0.4.4/imgutils/detect/hand.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/head.py` & `dghs_imgutils-0.4.4/imgutils/detect/head.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/person.py` & `dghs_imgutils-0.4.4/imgutils/detect/person.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/text.py` & `dghs_imgutils-0.4.4/imgutils/detect/text.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/detect/visual.py` & `dghs_imgutils-0.4.4/imgutils/detect/visual.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/edge/__init__.py` & `dghs_imgutils-0.4.4/imgutils/edge/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/edge/_base.py` & `dghs_imgutils-0.4.4/imgutils/edge/_base.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/edge/canny.py` & `dghs_imgutils-0.4.4/imgutils/edge/canny.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/edge/lineart.py` & `dghs_imgutils-0.4.4/imgutils/edge/lineart.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/edge/lineart_anime.py` & `dghs_imgutils-0.4.4/imgutils/edge/lineart_anime.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/metrics/aesthetic.py` & `dghs_imgutils-0.4.4/imgutils/metrics/aesthetic.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/metrics/ccip.py` & `dghs_imgutils-0.4.4/imgutils/metrics/ccip.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/metrics/dbaesthetic.py` & `dghs_imgutils-0.4.4/imgutils/metrics/dbaesthetic.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/metrics/laplacian.py` & `dghs_imgutils-0.4.4/imgutils/metrics/laplacian.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/metrics/lpips.py` & `dghs_imgutils-0.4.4/imgutils/metrics/lpips.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/metrics/psnr_.py` & `dghs_imgutils-0.4.4/imgutils/metrics/psnr_.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/ocr/__init__.py` & `dghs_imgutils-0.4.4/imgutils/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/ocr/detect.py` & `dghs_imgutils-0.4.4/imgutils/ocr/detect.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/ocr/entry.py` & `dghs_imgutils-0.4.4/imgutils/ocr/entry.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/ocr/recognize.py` & `dghs_imgutils-0.4.4/imgutils/ocr/recognize.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/operate/align.py` & `dghs_imgutils-0.4.4/imgutils/operate/align.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/operate/censor_.py` & `dghs_imgutils-0.4.4/imgutils/operate/censor_.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/operate/emoji_censor.png` & `dghs_imgutils-0.4.4/imgutils/operate/emoji_censor.png`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/operate/heart_censor.png` & `dghs_imgutils-0.4.4/imgutils/operate/heart_censor.png`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/operate/imgcensor.py` & `dghs_imgutils-0.4.4/imgutils/operate/imgcensor.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/operate/smile_censor.png` & `dghs_imgutils-0.4.4/imgutils/operate/smile_censor.png`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/operate/squeeze.py` & `dghs_imgutils-0.4.4/imgutils/operate/squeeze.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/pose/dwpose.py` & `dghs_imgutils-0.4.4/imgutils/pose/dwpose.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/pose/format.py` & `dghs_imgutils-0.4.4/imgutils/pose/format.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/pose/visual.py` & `dghs_imgutils-0.4.4/imgutils/pose/visual.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/resource/background.py` & `dghs_imgutils-0.4.4/imgutils/resource/background.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/restore/adversarial.py` & `dghs_imgutils-0.4.4/imgutils/restore/adversarial.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/restore/nafnet.py` & `dghs_imgutils-0.4.4/imgutils/restore/nafnet.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,23 +10,30 @@
     .. image:: nafnet_benchmark.plot.py.svg
         :align: center
 
     .. warning::
         Currently, we've identified a significant issue with NafNet when images contain gaussian noise.
         To ensure your code functions correctly, please ensure the credibility of
         your image source or preprocess them using SCUNet.
+
+    .. note::
+        New in version v0.4.4, **images with alpha channel supported**.
+
+        If you use an image with alpha channel (e.g. RGBA images),
+        it will return a RGBA image, otherwise return RGG image.
 """
 from functools import lru_cache
 from typing import Literal
 
 import numpy as np
 from PIL import Image
 from huggingface_hub import hf_hub_download
 
-from ..data import ImageTyping, load_image
+from ..data import ImageTyping
+from ..generic import ImageEnhancer
 from ..utils import open_onnx_model, area_batch_run
 
 NafNetModelTyping = Literal['REDS', 'GoPro', 'SIDD']
 
 
 @lru_cache()
 def _open_nafnet_model(model: NafNetModelTyping):
@@ -39,40 +46,60 @@
     """
     return open_onnx_model(hf_hub_download(
         f'deepghs/image_restoration',
         f'NAFNet-{model}-width64.onnx',
     ))
 
 
+class _Enhancer(ImageEnhancer):
+    def __init__(self, model: NafNetModelTyping = 'REDS', tile_size: int = 256, tile_overlap: int = 16,
+                 batch_size: int = 4, silent: bool = False):
+        self.model = model
+        self.tile_size = tile_size
+        self.tile_overlap = tile_overlap
+        self.batch_size = batch_size
+        self.silent = silent
+
+    def _process_rgb(self, rgb_array: np.ndarray):
+        input_ = rgb_array[None, ...]
+
+        def _method(ix):
+            ox, = _open_nafnet_model(self.model).run(['output'], {'input': ix})
+            return ox
+
+        output_ = area_batch_run(
+            input_, _method,
+            tile_size=self.tile_size, tile_overlap=self.tile_overlap, batch_size=self.batch_size,
+            silent=self.silent, process_title='NafNet Restore',
+        )
+        output_ = np.clip(output_, a_min=0.0, a_max=1.0)
+        return output_[0]
+
+
+@lru_cache()
+def _get_enhancer(model: NafNetModelTyping = 'REDS', tile_size: int = 256, tile_overlap: int = 16,
+                  batch_size: int = 4, silent: bool = False) -> _Enhancer:
+    return _Enhancer(model, tile_size, tile_overlap, batch_size, silent)
+
+
 def restore_with_nafnet(image: ImageTyping, model: NafNetModelTyping = 'REDS',
-                        tile_size: int = 256, tile_overlap: int = 16, silent: bool = False) -> Image.Image:
+                        tile_size: int = 256, tile_overlap: int = 16, batch_size: int = 4,
+                        silent: bool = False) -> Image.Image:
     """
     Restore an image using the NAFNet model.
 
     :param image: The input image.
     :type image: ImageTyping
     :param model: The NAFNet model type ('REDS', 'GoPro', 'SIDD'). Default is 'REDS'.
     :type model: NafNetModelTyping
     :param tile_size: The size of processing tiles. Default is 256.
     :type tile_size: int
     :param tile_overlap: The overlap between tiles. Default is 16.
     :type tile_overlap: int
+    :param batch_size: The batch size of inference. Default is 4.
+    :type batch_size: int
     :param silent: If True, the progress will not be displayed. Default is False.
     :type silent: bool
     :return: The restored image.
     :rtype: Image.Image
     """
-    image = load_image(image, mode='RGB', force_background='white')
-    input_ = np.array(image).astype(np.float32) / 255.0
-    input_ = input_.transpose((2, 0, 1))[None, ...]
-
-    def _method(ix):
-        ox, = _open_nafnet_model(model).run(['output'], {'input': ix})
-        return ox
-
-    output_ = area_batch_run(
-        input_, _method,
-        tile_size=tile_size, tile_overlap=tile_overlap, silent=silent,
-        process_title='NafNet Restore',
-    )
-    output_ = np.clip(output_, a_min=0.0, a_max=1.0)
-    return Image.fromarray((output_[0].transpose((1, 2, 0)) * 255).astype(np.int8), 'RGB')
+    return _get_enhancer(model, tile_size, tile_overlap, batch_size, silent).process(image)
```

### Comparing `dghs_imgutils-0.4.3/imgutils/restore/scunet.py` & `dghs_imgutils-0.4.4/imgutils/restore/scunet.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,23 +6,29 @@
         :align: center
 
     This is an overall benchmark of all the SCUNet models:
 
     .. image:: scunet_benchmark.plot.py.svg
         :align: center
 
+    .. note::
+        New in version v0.4.4, **images with alpha channel supported**.
+
+        If you use an image with alpha channel (e.g. RGBA images),
+        it will return a RGBA image, otherwise return RGG image.
 """
 from functools import lru_cache
 from typing import Literal
 
 import numpy as np
 from PIL import Image
 from huggingface_hub import hf_hub_download
 
-from ..data import ImageTyping, load_image
+from ..data import ImageTyping
+from ..generic import ImageEnhancer
 from ..utils import open_onnx_model, area_batch_run
 
 SCUNetModelTyping = Literal['GAN', 'PSNR']
 
 
 @lru_cache()
 def _open_scunet_model(model: SCUNetModelTyping):
@@ -35,40 +41,60 @@
     """
     return open_onnx_model(hf_hub_download(
         f'deepghs/image_restoration',
         f'SCUNet-{model}.onnx'
     ))
 
 
+class _Enhancer(ImageEnhancer):
+    def __init__(self, model: SCUNetModelTyping = 'GAN', tile_size: int = 128, tile_overlap: int = 16,
+                 batch_size: int = 4, silent: bool = False):
+        self.model = model
+        self.tile_size = tile_size
+        self.tile_overlap = tile_overlap
+        self.batch_size = batch_size
+        self.silent = silent
+
+    def _process_rgb(self, rgb_array: np.ndarray):
+        input_ = rgb_array[None, ...]
+
+        def _method(ix):
+            ox, = _open_scunet_model(self.model).run(['output'], {'input': ix})
+            return ox
+
+        output_ = area_batch_run(
+            input_, _method,
+            tile_size=self.tile_size, tile_overlap=self.tile_overlap, batch_size=self.batch_size,
+            silent=self.silent, process_title='SCUNet Restore',
+        )
+        output_ = np.clip(output_, a_min=0.0, a_max=1.0)
+        return output_[0]
+
+
+@lru_cache()
+def _get_enhancer(model: SCUNetModelTyping = 'GAN', tile_size: int = 128, tile_overlap: int = 16,
+                  batch_size: int = 4, silent: bool = False) -> _Enhancer:
+    return _Enhancer(model, tile_size, tile_overlap, batch_size, silent)
+
+
 def restore_with_scunet(image: ImageTyping, model: SCUNetModelTyping = 'GAN',
-                        tile_size: int = 128, tile_overlap: int = 16, silent: bool = False) -> Image.Image:
+                        tile_size: int = 128, tile_overlap: int = 16, batch_size: int = 4,
+                        silent: bool = False) -> Image.Image:
     """
     Restore an image using the SCUNet model.
 
     :param image: The input image.
     :type image: ImageTyping
     :param model: The SCUNet model type ('GAN', 'PSNR'). Default is 'GAN'.
     :type model: SCUNetModelTyping
     :param tile_size: The size of processing tiles. Default is 128.
     :type tile_size: int
     :param tile_overlap: The overlap between tiles. Default is 16.
     :type tile_overlap: int
+    :param batch_size: The batch size of inference. Default is 4.
+    :type batch_size: int
     :param silent: If True, the progress will not be displayed. Default is False.
     :type silent: bool
     :return: The restored image.
     :rtype: Image.Image
     """
-    image = load_image(image, mode='RGB', force_background='white')
-    input_ = np.array(image).astype(np.float32) / 255.0
-    input_ = input_.transpose((2, 0, 1))[None, ...]
-
-    def _method(ix):
-        ox, = _open_scunet_model(model).run(['output'], {'input': ix})
-        return ox
-
-    output_ = area_batch_run(
-        input_, _method,
-        tile_size=tile_size, tile_overlap=tile_overlap, silent=silent,
-        process_title='SCUNet Restore',
-    )
-    output_ = np.clip(output_, a_min=0.0, a_max=1.0)
-    return Image.fromarray((output_[0].transpose((1, 2, 0)) * 255).astype(np.int8), 'RGB')
+    return _get_enhancer(model, tile_size, tile_overlap, batch_size, silent).process(image)
```

### Comparing `dghs_imgutils-0.4.3/imgutils/sd/metadata.py` & `dghs_imgutils-0.4.4/imgutils/sd/metadata.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/sd/model.py` & `dghs_imgutils-0.4.4/imgutils/sd/model.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/segment/isnetis.py` & `dghs_imgutils-0.4.4/imgutils/segment/isnetis.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/tagging/__init__.py` & `dghs_imgutils-0.4.4/imgutils/tagging/__init__.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/tagging/blacklist.py` & `dghs_imgutils-0.4.4/imgutils/tagging/blacklist.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/tagging/character.py` & `dghs_imgutils-0.4.4/imgutils/tagging/character.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/tagging/deepdanbooru.py` & `dghs_imgutils-0.4.4/imgutils/tagging/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/tagging/format.py` & `dghs_imgutils-0.4.4/imgutils/tagging/format.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/tagging/match.py` & `dghs_imgutils-0.4.4/imgutils/tagging/match.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/tagging/mldanbooru.py` & `dghs_imgutils-0.4.4/imgutils/tagging/mldanbooru.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/tagging/order.py` & `dghs_imgutils-0.4.4/imgutils/tagging/order.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/tagging/overlap.py` & `dghs_imgutils-0.4.4/imgutils/tagging/overlap.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/tagging/wd14.py` & `dghs_imgutils-0.4.4/imgutils/tagging/wd14.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/utils/area.py` & `dghs_imgutils-0.4.4/imgutils/utils/area.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     :rtype: np.ndarray
     """
     batch, channels, height, width = origin_input.shape
     assert channels == input_channels, f'Input channels {input_channels!r} expected, but {channels!r} found.'
 
     tile = min(tile_size, height, width)
     stride = tile - tile_overlap
-    h_idx_list = list(range(0, height - tile, stride)) + [height - tile]
-    w_idx_list = list(range(0, width - tile, stride)) + [width - tile]
+    h_idx_list = sorted(set(list(range(0, height - tile, stride)) + [height - tile]))
+    w_idx_list = sorted(set(list(range(0, width - tile, stride)) + [width - tile]))
     sum_ = np.zeros((batch, output_channels, height * scale, width * scale), dtype=origin_input.dtype)
     weight = np.zeros_like(sum_, dtype=origin_input.dtype)
 
     all_patch = []
     all_idx = []
 
     with tqdm(total=math.ceil(len(h_idx_list) * len(w_idx_list) / batch_size),
```

### Comparing `dghs_imgutils-0.4.3/imgutils/utils/onnxruntime.py` & `dghs_imgutils-0.4.4/imgutils/utils/onnxruntime.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/utils/tqdm_.py` & `dghs_imgutils-0.4.4/imgutils/utils/tqdm_.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/aicheck.py` & `dghs_imgutils-0.4.4/imgutils/validate/aicheck.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/bangumi_char.py` & `dghs_imgutils-0.4.4/imgutils/validate/bangumi_char.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/classify.py` & `dghs_imgutils-0.4.4/imgutils/validate/classify.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/color.py` & `dghs_imgutils-0.4.4/imgutils/validate/color.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/completeness.py` & `dghs_imgutils-0.4.4/imgutils/validate/completeness.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/dbrating.py` & `dghs_imgutils-0.4.4/imgutils/validate/dbrating.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/monochrome.py` & `dghs_imgutils-0.4.4/imgutils/validate/monochrome.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/nsfw.py` & `dghs_imgutils-0.4.4/imgutils/validate/nsfw.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/portrait.py` & `dghs_imgutils-0.4.4/imgutils/validate/portrait.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/rating.py` & `dghs_imgutils-0.4.4/imgutils/validate/rating.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/real.py` & `dghs_imgutils-0.4.4/imgutils/validate/real.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/safe.py` & `dghs_imgutils-0.4.4/imgutils/validate/safe.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/style_age.py` & `dghs_imgutils-0.4.4/imgutils/validate/style_age.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/teen.py` & `dghs_imgutils-0.4.4/imgutils/validate/teen.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/imgutils/validate/truncate.py` & `dghs_imgutils-0.4.4/imgutils/validate/truncate.py`

 * *Files identical despite different names*

### Comparing `dghs_imgutils-0.4.3/setup.py` & `dghs_imgutils-0.4.4/setup.py`

 * *Files identical despite different names*

