# Comparing `tmp/clusterfun-0.3.0a7.tar.gz` & `tmp/clusterfun-0.3.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterfun-0.3.0a7.tar", max compression
+gzip compressed data, was "clusterfun-0.3.1a7.tar", max compression
```

## Comparing `clusterfun-0.3.0a7.tar` & `clusterfun-0.3.1a7.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0    11357 2024-04-28 22:32:09.819834 clusterfun-0.3.0a7/LICENSE
--rw-r--r--   0        0        0     9280 2024-04-28 22:32:09.820288 clusterfun-0.3.0a7/README.md
--rw-r--r--   0        0        0      660 2024-04-28 22:32:09.852017 clusterfun-0.3.0a7/clusterfun/__init__.py
--rw-r--r--   0        0        0      970 2024-05-02 18:48:38.705980 clusterfun-0.3.0a7/clusterfun/app.py
--rw-r--r--   0        0        0     2137 2024-04-28 22:32:09.852532 clusterfun-0.3.0a7/clusterfun/config.py
--rw-r--r--   0        0        0      715 2024-04-28 22:32:09.852760 clusterfun-0.3.0a7/clusterfun/constants.py
--rw-r--r--   0        0        0     6790 2024-05-07 09:53:06.282457 clusterfun-0.3.0a7/clusterfun/frontend/404.html
--rw-r--r--   0        0        0      224 2024-05-02 18:20:15.920034 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-02 18:20:15.920441 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-07 09:53:06.289880 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/0t2IpDcBx6FIaFpL5-DTX/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-07 09:53:06.288728 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/0t2IpDcBx6FIaFpL5-DTX/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.190992 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.191316 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.192076 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.192715 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-02 18:20:15.921043 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-02 18:20:15.921298 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_ssgManifest.js
--rw-r--r--   0        0        0     8025 2024-05-01 14:48:56.193828 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js
--rw-r--r--   0        0        0   121966 2024-05-07 09:53:06.305902 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js
--rw-r--r--   0        0        0   110785 2024-05-01 14:48:56.198064 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js
--rw-r--r--   0        0        0   143320 2024-05-01 14:48:56.199462 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js
--rw-r--r--   0        0        0   131700 2024-05-02 18:20:15.926209 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js
--rw-r--r--   0        0        0   131700 2024-05-07 09:53:06.297351 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js
--rw-r--r--   0        0        0     7388 2024-05-07 09:53:06.296139 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js
--rw-r--r--   0        0        0     4290 2024-05-07 09:53:06.321491 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js
--rw-r--r--   0        0        0     4290 2024-05-01 14:48:56.203293 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js
--rw-r--r--   0        0        0     1744 2024-05-07 09:53:06.303313 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js
--rw-r--r--   0        0        0     1840 2024-05-01 14:48:56.204570 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js
--rw-r--r--   0        0        0      480 2024-05-02 18:20:15.926928 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/layout-0f23d4766ac3d9e3.js
--rw-r--r--   0        0        0      480 2024-05-07 09:53:06.304580 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/layout-15dece07a8c94bf7.js
--rw-r--r--   0        0        0      477 2024-05-01 14:48:56.206202 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/layout-f917f547d72d1629.js
--rw-r--r--   0        0        0    26631 2024-05-07 09:53:06.301663 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js
--rw-r--r--   0        0        0    26688 2024-05-01 15:15:14.526938 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js
--rw-r--r--   0        0        0    26619 2024-05-01 14:48:56.207662 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js
--rw-r--r--   0        0        0    26640 2024-05-01 14:48:56.208488 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js
--rw-r--r--   0        0        0    27859 2024-05-01 14:48:56.209652 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js
--rw-r--r--   0        0        0  3613214 2024-05-07 09:53:06.299257 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js
--rw-r--r--   0        0        0  3842147 2024-05-01 14:48:56.238679 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js
--rw-r--r--   0        0        0   172831 2024-05-07 09:53:06.306982 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js
--rw-r--r--   0        0        0   163906 2024-05-01 14:48:56.242705 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js
--rw-r--r--   0        0        0   140171 2024-05-01 14:48:56.244603 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js
--rw-r--r--   0        0        0   140981 2024-05-07 09:53:06.312488 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js
--rw-r--r--   0        0        0   115325 2024-05-01 14:48:56.246881 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js
--rw-r--r--   0        0        0   109895 2024-05-07 09:53:06.318305 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js
--rw-r--r--   0        0        0      508 2024-05-01 14:48:56.248662 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-app-27650c6b197f0cd8.js
--rw-r--r--   0        0        0      462 2024-05-07 09:53:06.314953 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-app-e01e327631e02231.js
--rw-r--r--   0        0        0      325 2024-05-01 14:48:56.250189 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/pages/_app-1534f180665c857f.js
--rw-r--r--   0        0        0      280 2024-05-07 09:53:06.316951 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/pages/_app-6a626577ffa902a4.js
--rw-r--r--   0        0        0      247 2024-05-07 09:53:06.317661 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/pages/_error-1be831200e60c5c0.js
--rw-r--r--   0        0        0      247 2024-05-01 14:48:56.252577 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/pages/_error-b646007f40c4f0a8.js
--rw-r--r--   0        0        0    91381 2024-05-07 09:53:06.320646 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
--rw-r--r--   0        0        0    91460 2024-05-01 14:48:56.253498 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     4659 2024-05-01 14:48:56.254092 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js
--rw-r--r--   0        0        0     3824 2024-05-07 09:53:06.309226 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js
--rw-r--r--   0        0        0    28962 2024-05-07 09:53:06.287289 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css
--rw-r--r--   0        0        0    28962 2024-05-01 14:48:56.256127 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.256638 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.256845 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-02 18:20:15.928020 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-02 18:20:15.928227 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_ssgManifest.js
--rw-r--r--   0        0        0      224 2024-05-01 14:48:56.257630 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_buildManifest.js
--rw-r--r--   0        0        0       80 2024-05-01 14:48:56.257857 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_ssgManifest.js
--rw-r--r--   0        0        0    10496 2024-05-07 09:53:06.326401 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2
--rw-r--r--   0        0        0    17612 2024-05-07 09:53:06.331658 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2
--rw-r--r--   0        0        0    22524 2024-05-07 09:53:06.327827 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2
--rw-r--r--   0        0        0     9628 2024-05-07 09:53:06.325530 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff
--rw-r--r--   0        0        0    46552 2024-05-07 09:53:06.329101 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2
--rw-r--r--   0        0        0    80044 2024-05-07 09:53:06.330311 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2
--rw-r--r--   0        0        0    27316 2024-05-07 09:53:06.329676 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2
--rw-r--r--   0        0        0    12768 2024-05-07 09:53:06.331057 clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2
--rw-r--r--   0        0        0     7406 2024-05-07 09:53:06.332516 clusterfun-0.3.0a7/clusterfun/frontend/favicon.ico
--rw-r--r--   0        0        0     9628 2024-05-07 09:53:06.335678 clusterfun-0.3.0a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff
--rw-r--r--   0        0        0     4959 2024-05-07 09:53:06.336748 clusterfun-0.3.0a7/clusterfun/frontend/index.html
--rw-r--r--   0        0        0     2499 2024-05-07 09:53:06.337830 clusterfun-0.3.0a7/clusterfun/frontend/index.txt
--rw-r--r--   0        0        0     3341 2024-05-03 13:14:22.092512 clusterfun-0.3.0a7/clusterfun/main.py
--rw-r--r--   0        0        0        0 2024-04-28 22:32:09.895406 clusterfun-0.3.0a7/clusterfun/models/__init__.py
--rw-r--r--   0        0        0     3111 2024-04-28 22:32:09.895643 clusterfun-0.3.0a7/clusterfun/models/filter.py
--rw-r--r--   0        0        0     1159 2024-04-28 22:32:09.895855 clusterfun-0.3.0a7/clusterfun/models/media_indices.py
--rw-r--r--   0        0        0      945 2024-05-06 22:44:34.090007 clusterfun-0.3.0a7/clusterfun/models/media_item.py
--rw-r--r--   0        0        0     8100 2024-05-03 13:14:27.292482 clusterfun-0.3.0a7/clusterfun/plot.py
--rw-r--r--   0        0        0     1183 2024-04-28 22:32:09.896695 clusterfun-0.3.0a7/clusterfun/plot_types/__init__.py
--rw-r--r--   0        0        0     3586 2024-04-28 22:32:09.898400 clusterfun-0.3.0a7/clusterfun/plot_types/bar_chart.py
--rw-r--r--   0        0        0     3166 2024-04-28 22:32:09.898957 clusterfun-0.3.0a7/clusterfun/plot_types/confusion_matrix.py
--rw-r--r--   0        0        0     1217 2024-04-28 22:32:09.899339 clusterfun-0.3.0a7/clusterfun/plot_types/grid.py
--rw-r--r--   0        0        0     4248 2024-04-28 22:32:09.899527 clusterfun-0.3.0a7/clusterfun/plot_types/histogram.py
--rw-r--r--   0        0        0     6119 2024-04-28 22:32:09.899714 clusterfun-0.3.0a7/clusterfun/plot_types/pie_chart.py
--rw-r--r--   0        0        0     1356 2024-04-28 22:32:09.899978 clusterfun-0.3.0a7/clusterfun/plot_types/scatter.py
--rw-r--r--   0        0        0     4277 2024-04-28 22:32:09.900224 clusterfun-0.3.0a7/clusterfun/plot_types/violin.py
--rw-r--r--   0        0        0     1721 2024-04-28 22:32:09.900538 clusterfun-0.3.0a7/clusterfun/serve_cli.py
--rw-r--r--   0        0        0        0 2024-04-28 22:32:09.900856 clusterfun-0.3.0a7/clusterfun/storage/__init__.py
--rw-r--r--   0        0        0      944 2024-05-07 09:54:30.442488 clusterfun-0.3.0a7/clusterfun/storage/client/__init__.py
--rw-r--r--   0        0        0     1249 2024-05-07 09:18:46.136998 clusterfun-0.3.0a7/clusterfun/storage/client/base.py
--rw-r--r--   0        0        0      800 2024-05-07 09:18:46.136720 clusterfun-0.3.0a7/clusterfun/storage/client/http.py
--rw-r--r--   0        0        0     1071 2024-05-07 09:18:46.140218 clusterfun-0.3.0a7/clusterfun/storage/client/local.py
--rw-r--r--   0        0        0     1680 2024-05-07 09:51:17.155237 clusterfun-0.3.0a7/clusterfun/storage/client/s3.py
--rw-r--r--   0        0        0     2238 2024-04-28 22:32:09.901088 clusterfun-0.3.0a7/clusterfun/storage/loader.py
--rw-r--r--   0        0        0        0 2024-04-28 22:32:09.902140 clusterfun-0.3.0a7/clusterfun/storage/local/__init__.py
--rw-r--r--   0        0        0     5387 2024-04-28 22:32:09.902560 clusterfun-0.3.0a7/clusterfun/storage/local/data.py
--rw-r--r--   0        0        0     4767 2024-05-02 18:20:15.931749 clusterfun-0.3.0a7/clusterfun/storage/local/helpers.py
--rw-r--r--   0        0        0     5113 2024-05-03 13:14:04.608491 clusterfun-0.3.0a7/clusterfun/storage/local/loader.py
--rw-r--r--   0        0        0     2744 2024-04-28 22:32:09.903488 clusterfun-0.3.0a7/clusterfun/storage/local/storer.py
--rw-r--r--   0        0        0     2629 2024-05-06 22:44:34.096055 clusterfun-0.3.0a7/clusterfun/storage/storer.py
--rw-r--r--   0        0        0     2258 2024-04-28 22:32:09.904443 clusterfun-0.3.0a7/clusterfun/validation.py
--rw-r--r--   0        0        0     1130 2024-05-07 09:54:33.240814 clusterfun-0.3.0a7/pyproject.toml
--rw-r--r--   0        0        0    10021 1970-01-01 00:00:00.000000 clusterfun-0.3.0a7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-28 22:32:09.819834 clusterfun-0.3.1a7/LICENSE
+-rw-r--r--   0        0        0     9280 2024-04-28 22:32:09.820288 clusterfun-0.3.1a7/README.md
+-rw-r--r--   0        0        0      660 2024-04-28 22:32:09.852017 clusterfun-0.3.1a7/clusterfun/__init__.py
+-rw-r--r--   0        0        0      970 2024-05-02 18:48:38.705980 clusterfun-0.3.1a7/clusterfun/app.py
+-rw-r--r--   0        0        0     2175 2024-05-09 22:09:16.224964 clusterfun-0.3.1a7/clusterfun/config.py
+-rw-r--r--   0        0        0      715 2024-04-28 22:32:09.852760 clusterfun-0.3.1a7/clusterfun/constants.py
+-rw-r--r--   0        0        0     6790 2024-05-07 09:53:06.282457 clusterfun-0.3.1a7/clusterfun/frontend/404.html
+-rw-r--r--   0        0        0      224 2024-05-02 18:20:15.920034 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-02 18:20:15.920441 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/0L8U1RGbBQqzpAEgBP-4y/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-07 09:53:06.289880 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/0t2IpDcBx6FIaFpL5-DTX/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-07 09:53:06.288728 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/0t2IpDcBx6FIaFpL5-DTX/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.190992 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.191316 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/7K0stYTjLuE1ieiHwaOY8/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.192076 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.192715 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/9m8W0thtsOjMrVxSpss7G/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-02 18:20:15.921043 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-02 18:20:15.921298 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/FajzyA8s2dBSB6nVAodLv/_ssgManifest.js
+-rw-r--r--   0        0        0     8025 2024-05-01 14:48:56.193828 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js
+-rw-r--r--   0        0        0   121966 2024-05-07 09:53:06.305902 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js
+-rw-r--r--   0        0        0   110785 2024-05-01 14:48:56.198064 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js
+-rw-r--r--   0        0        0   143320 2024-05-01 14:48:56.199462 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js
+-rw-r--r--   0        0        0   131700 2024-05-02 18:20:15.926209 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js
+-rw-r--r--   0        0        0   131700 2024-05-07 09:53:06.297351 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js
+-rw-r--r--   0        0        0     7388 2024-05-07 09:53:06.296139 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js
+-rw-r--r--   0        0        0     4290 2024-05-07 09:53:06.321491 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js
+-rw-r--r--   0        0        0     4290 2024-05-01 14:48:56.203293 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js
+-rw-r--r--   0        0        0     1744 2024-05-07 09:53:06.303313 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js
+-rw-r--r--   0        0        0     1840 2024-05-01 14:48:56.204570 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js
+-rw-r--r--   0        0        0      480 2024-05-02 18:20:15.926928 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/layout-0f23d4766ac3d9e3.js
+-rw-r--r--   0        0        0      480 2024-05-07 09:53:06.304580 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/layout-15dece07a8c94bf7.js
+-rw-r--r--   0        0        0      477 2024-05-01 14:48:56.206202 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/layout-f917f547d72d1629.js
+-rw-r--r--   0        0        0    26631 2024-05-07 09:53:06.301663 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js
+-rw-r--r--   0        0        0    26688 2024-05-01 15:15:14.526938 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js
+-rw-r--r--   0        0        0    26619 2024-05-01 14:48:56.207662 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js
+-rw-r--r--   0        0        0    26640 2024-05-01 14:48:56.208488 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js
+-rw-r--r--   0        0        0    27859 2024-05-01 14:48:56.209652 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js
+-rw-r--r--   0        0        0  3613214 2024-05-07 09:53:06.299257 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js
+-rw-r--r--   0        0        0  3842147 2024-05-01 14:48:56.238679 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js
+-rw-r--r--   0        0        0   172831 2024-05-07 09:53:06.306982 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js
+-rw-r--r--   0        0        0   163906 2024-05-01 14:48:56.242705 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js
+-rw-r--r--   0        0        0   140171 2024-05-01 14:48:56.244603 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js
+-rw-r--r--   0        0        0   140981 2024-05-07 09:53:06.312488 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js
+-rw-r--r--   0        0        0   115325 2024-05-01 14:48:56.246881 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js
+-rw-r--r--   0        0        0   109895 2024-05-07 09:53:06.318305 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js
+-rw-r--r--   0        0        0      508 2024-05-01 14:48:56.248662 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/main-app-27650c6b197f0cd8.js
+-rw-r--r--   0        0        0      462 2024-05-07 09:53:06.314953 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/main-app-e01e327631e02231.js
+-rw-r--r--   0        0        0      325 2024-05-01 14:48:56.250189 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/pages/_app-1534f180665c857f.js
+-rw-r--r--   0        0        0      280 2024-05-07 09:53:06.316951 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/pages/_app-6a626577ffa902a4.js
+-rw-r--r--   0        0        0      247 2024-05-07 09:53:06.317661 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/pages/_error-1be831200e60c5c0.js
+-rw-r--r--   0        0        0      247 2024-05-01 14:48:56.252577 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/pages/_error-b646007f40c4f0a8.js
+-rw-r--r--   0        0        0    91381 2024-05-07 09:53:06.320646 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js
+-rw-r--r--   0        0        0    91460 2024-05-01 14:48:56.253498 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     4659 2024-05-01 14:48:56.254092 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js
+-rw-r--r--   0        0        0     3824 2024-05-07 09:53:06.309226 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js
+-rw-r--r--   0        0        0    28962 2024-05-07 09:53:06.287289 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css
+-rw-r--r--   0        0        0    28962 2024-05-01 14:48:56.256127 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.256638 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.256845 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/gTuZP6baQRuoAlSBQfJhW/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-02 18:20:15.928020 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-02 18:20:15.928227 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/lbjNsPpWYZod25BysgHf4/_ssgManifest.js
+-rw-r--r--   0        0        0      224 2024-05-01 14:48:56.257630 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_buildManifest.js
+-rw-r--r--   0        0        0       80 2024-05-01 14:48:56.257857 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/mBEYttyj_pgzUHdneL-73/_ssgManifest.js
+-rw-r--r--   0        0        0    10496 2024-05-07 09:53:06.326401 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2
+-rw-r--r--   0        0        0    17612 2024-05-07 09:53:06.331658 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2
+-rw-r--r--   0        0        0    22524 2024-05-07 09:53:06.327827 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2
+-rw-r--r--   0        0        0     9628 2024-05-07 09:53:06.325530 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff
+-rw-r--r--   0        0        0    46552 2024-05-07 09:53:06.329101 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2
+-rw-r--r--   0        0        0    80044 2024-05-07 09:53:06.330311 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2
+-rw-r--r--   0        0        0    27316 2024-05-07 09:53:06.329676 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2
+-rw-r--r--   0        0        0    12768 2024-05-07 09:53:06.331057 clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2
+-rw-r--r--   0        0        0     7406 2024-05-07 09:53:06.332516 clusterfun-0.3.1a7/clusterfun/frontend/favicon.ico
+-rw-r--r--   0        0        0     9628 2024-05-07 09:53:06.335678 clusterfun-0.3.1a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff
+-rw-r--r--   0        0        0     4959 2024-05-07 09:53:06.336748 clusterfun-0.3.1a7/clusterfun/frontend/index.html
+-rw-r--r--   0        0        0     2499 2024-05-07 09:53:06.337830 clusterfun-0.3.1a7/clusterfun/frontend/index.txt
+-rw-r--r--   0        0        0     3341 2024-05-03 13:14:22.092512 clusterfun-0.3.1a7/clusterfun/main.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:32:09.895406 clusterfun-0.3.1a7/clusterfun/models/__init__.py
+-rw-r--r--   0        0        0     3111 2024-04-28 22:32:09.895643 clusterfun-0.3.1a7/clusterfun/models/filter.py
+-rw-r--r--   0        0        0     1159 2024-04-28 22:32:09.895855 clusterfun-0.3.1a7/clusterfun/models/media_indices.py
+-rw-r--r--   0        0        0      945 2024-05-06 22:44:34.090007 clusterfun-0.3.1a7/clusterfun/models/media_item.py
+-rw-r--r--   0        0        0     8100 2024-05-03 13:14:27.292482 clusterfun-0.3.1a7/clusterfun/plot.py
+-rw-r--r--   0        0        0     1183 2024-04-28 22:32:09.896695 clusterfun-0.3.1a7/clusterfun/plot_types/__init__.py
+-rw-r--r--   0        0        0     3704 2024-05-09 22:09:16.225412 clusterfun-0.3.1a7/clusterfun/plot_types/bar_chart.py
+-rw-r--r--   0        0        0     3166 2024-04-28 22:32:09.898957 clusterfun-0.3.1a7/clusterfun/plot_types/confusion_matrix.py
+-rw-r--r--   0        0        0     1217 2024-04-28 22:32:09.899339 clusterfun-0.3.1a7/clusterfun/plot_types/grid.py
+-rw-r--r--   0        0        0     4363 2024-05-09 22:09:16.225892 clusterfun-0.3.1a7/clusterfun/plot_types/histogram.py
+-rw-r--r--   0        0        0     6119 2024-04-28 22:32:09.899714 clusterfun-0.3.1a7/clusterfun/plot_types/pie_chart.py
+-rw-r--r--   0        0        0     1446 2024-05-09 22:09:16.226351 clusterfun-0.3.1a7/clusterfun/plot_types/scatter.py
+-rw-r--r--   0        0        0     4277 2024-05-09 21:51:05.518619 clusterfun-0.3.1a7/clusterfun/plot_types/violin.py
+-rw-r--r--   0        0        0     1721 2024-04-28 22:32:09.900538 clusterfun-0.3.1a7/clusterfun/serve_cli.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:32:09.900856 clusterfun-0.3.1a7/clusterfun/storage/__init__.py
+-rw-r--r--   0        0        0      991 2024-05-09 22:09:16.226778 clusterfun-0.3.1a7/clusterfun/storage/client/__init__.py
+-rw-r--r--   0        0        0     1249 2024-05-07 09:18:46.136998 clusterfun-0.3.1a7/clusterfun/storage/client/base.py
+-rw-r--r--   0        0        0      800 2024-05-07 09:18:46.136720 clusterfun-0.3.1a7/clusterfun/storage/client/http.py
+-rw-r--r--   0        0        0     1071 2024-05-07 09:18:46.140218 clusterfun-0.3.1a7/clusterfun/storage/client/local.py
+-rw-r--r--   0        0        0     1680 2024-05-07 09:51:17.155237 clusterfun-0.3.1a7/clusterfun/storage/client/s3.py
+-rw-r--r--   0        0        0     2238 2024-04-28 22:32:09.901088 clusterfun-0.3.1a7/clusterfun/storage/loader.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:32:09.902140 clusterfun-0.3.1a7/clusterfun/storage/local/__init__.py
+-rw-r--r--   0        0        0     5772 2024-05-09 22:09:16.227345 clusterfun-0.3.1a7/clusterfun/storage/local/data.py
+-rw-r--r--   0        0        0     4767 2024-05-02 18:20:15.931749 clusterfun-0.3.1a7/clusterfun/storage/local/helpers.py
+-rw-r--r--   0        0        0     5113 2024-05-03 13:14:04.608491 clusterfun-0.3.1a7/clusterfun/storage/local/loader.py
+-rw-r--r--   0        0        0     2744 2024-05-09 21:58:29.650104 clusterfun-0.3.1a7/clusterfun/storage/local/storer.py
+-rw-r--r--   0        0        0     2629 2024-05-06 22:44:34.096055 clusterfun-0.3.1a7/clusterfun/storage/storer.py
+-rw-r--r--   0        0        0     2258 2024-04-28 22:32:09.904443 clusterfun-0.3.1a7/clusterfun/validation.py
+-rw-r--r--   0        0        0     1130 2024-05-09 22:09:29.903543 clusterfun-0.3.1a7/pyproject.toml
+-rw-r--r--   0        0        0    10021 1970-01-01 00:00:00.000000 clusterfun-0.3.1a7/PKG-INFO
```

### Comparing `clusterfun-0.3.0a7/LICENSE` & `clusterfun-0.3.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/README.md` & `clusterfun-0.3.1a7/README.md`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/__init__.py` & `clusterfun-0.3.1a7/clusterfun/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/app.py` & `clusterfun-0.3.1a7/clusterfun/app.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/config.py` & `clusterfun-0.3.1a7/clusterfun/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,7 +57,8 @@
     save_method: str = os.getenv("saver", default="local")
     # used for setting ticks quickly
     colors: Optional[List[str]] = None
     # for the bar chart, used to set the x axis ticks
     x_names: Optional[List[str]] = None
     # used when data is local
     common_media_path: Optional[str] = None
+    color_is_categorical: bool = True
```

### Comparing `clusterfun-0.3.0a7/clusterfun/constants.py` & `clusterfun-0.3.1a7/clusterfun/constants.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/404.html` & `clusterfun-0.3.1a7/clusterfun/frontend/404.html`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/22.94ebc66962dcd0f8.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/23-8126128752749016.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/472-07a7dd51a787971b.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/483-2d99a375fdcaeaa9.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/500-9855c0cda36bb0be.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/500-9beb637c2f8db305.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/8.d9282dffb5cd6834.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-4049d31c55f7218c.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/870fdd6f-51765f2c6413dd54.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/_not-found/page-6eda385f9819e210.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/_not-found-bee08356a690a144.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/page-0dc09429eb1650c3.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/page-0dcd9b5adc14930a.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/page-4f1f75de895ef2e9.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/page-cc11fa76e9925a25.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/app/page-facced18ab368811.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/f2d0f643.3ca4096564deaa88.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/f2d0f643.db7d448233298422.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/fd9d1056-3324b1349d932382.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/fd9d1056-e13d3c2807942cb7.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/framework-8883d1e9be70c3da.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/framework-aec844d2ccbe7592.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/main-01a7d75e7a6a7c98.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/main-0ba5df58c56b45df.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/polyfills-78c92fac7aa8fdd8.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/webpack-60a4426b837ea404.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/chunks/webpack-9c62b174fdbd129f.js`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/css/23cc4be46f2171d6.css`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/css/64b8c25cc96a1f37.css`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/05a31a2ca4975f99-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/513657b02c5c193f-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/51ed15f9841b9f9d-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/Oliver-Regular-400.365d360e.woff`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/c9a5bc6a7c948fb0-s.p.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/d6b16ce4a6175f26-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/ec159349637c90ad-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2` & `clusterfun-0.3.1a7/clusterfun/frontend/_next/static/media/fd4db3eb5472fc27-s.woff2`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/favicon.ico` & `clusterfun-0.3.1a7/clusterfun/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff` & `clusterfun-0.3.1a7/clusterfun/frontend/fonts/Oliver-Regular-400.woff`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/index.html` & `clusterfun-0.3.1a7/clusterfun/frontend/index.html`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/frontend/index.txt` & `clusterfun-0.3.1a7/clusterfun/frontend/index.txt`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/main.py` & `clusterfun-0.3.1a7/clusterfun/main.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/models/filter.py` & `clusterfun-0.3.1a7/clusterfun/models/filter.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/models/media_indices.py` & `clusterfun-0.3.1a7/clusterfun/models/media_indices.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/models/media_item.py` & `clusterfun-0.3.1a7/clusterfun/models/media_item.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/plot.py` & `clusterfun-0.3.1a7/clusterfun/plot.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/plot_types/__init__.py` & `clusterfun-0.3.1a7/clusterfun/plot_types/__init__.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/plot_types/bar_chart.py` & `clusterfun-0.3.1a7/clusterfun/plot_types/bar_chart.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     df: pd.DataFrame,
     x: str,
     media: str,
     color: Optional[str] = None,
     bounding_box: Optional[str] = None,
     title: Optional[str] = None,
     show: bool = True,
+    color_is_categorical: bool = True,
 ):  # pylint: disable=too-many-arguments,missing-function-docstring,too-many-locals
-    if color is None:
+    if color is None or not color_is_categorical:
         start_index = 0
         for index, (value, count) in enumerate(df[x].value_counts().items()):
             df.loc[df[x] == value, "_x"] = np.random.uniform(low=start_index + index, high=0.7 + index, size=count)
             df.loc[df[x] == value, "_y"] = np.random.uniform(low=0, high=count, size=count)
     else:
         start_index = 0
         for x_index, (x_value, _) in enumerate(df[x].value_counts().items()):
@@ -51,14 +52,15 @@
         y="_y",
         media=media,
         columns=get_columns_for_db(df, media, "bar_chart", "_y", "_x"),
         color=color,
         bounding_box=bounding_box,
         title=title,
         x_names=x_names,
+        color_is_categorical=color_is_categorical,
     )
     validate(df, cfg)
     return Plot.save(df, cfg).show(show)
 
 
 bar_chart.__doc__ = """
     :param df: pd.DataFrame
```

### Comparing `clusterfun-0.3.0a7/clusterfun/plot_types/confusion_matrix.py` & `clusterfun-0.3.1a7/clusterfun/plot_types/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/plot_types/grid.py` & `clusterfun-0.3.1a7/clusterfun/plot_types/grid.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/plot_types/histogram.py` & `clusterfun-0.3.1a7/clusterfun/plot_types/histogram.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,18 +28,19 @@
     x: str,
     media: str,
     bins: int = 20,
     color: Optional[str] = None,
     bounding_box: Optional[str] = None,
     title: Optional[str] = None,
     show: bool = True,
+    color_is_categorical: bool = True,
 ) -> Path:
     if "_x" in df.columns or "_y" in df.columns:
         raise KeyError('"_y" is a protected clusterfun columns and should not be included in the original dataframe.')
-    if color is not None:
+    if color is not None and color_is_categorical:
         dfs = []
         for color_item in df[color].unique():
             data_color = get_x_and_y(df[df[color] == color_item][x], bins)
             dff = pd.DataFrame(data_color, columns=["_x", "_y"])[["_y"]]
             dff.index = df[df[color] == color_item].index
             dfs.append(dff)
         dff = pd.concat(dfs)
@@ -52,14 +53,15 @@
         x=x,
         y="_y",
         media=media,
         columns=get_columns_for_db(df=df, media=media, plot_type="histogram", x=x, y="_y"),
         color=color,
         bounding_box=bounding_box,
         title=title,
+        color_is_categorical=color_is_categorical,
     )
     validate(df, cfg)
     return Plot.save(df, cfg).show(show)
 
 
 histogram.__doc__ = (
     """
```

### Comparing `clusterfun-0.3.0a7/clusterfun/plot_types/pie_chart.py` & `clusterfun-0.3.1a7/clusterfun/plot_types/pie_chart.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/plot_types/scatter.py` & `clusterfun-0.3.1a7/clusterfun/plot_types/scatter.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,24 +21,26 @@
     x: str,
     y: str,
     media: str,
     color: Optional[str] = None,
     bounding_box: Optional[str] = None,
     title: Optional[str] = None,
     show: bool = True,
+    color_is_categorical: bool = True,
 ):  # pylint: disable=too-many-arguments,missing-function-docstring
     cfg = Config(
         type="scatter",
         x=x,
         y=y,
         media=media,
         columns=get_columns_for_db(df, media, "scatter", x, y),
         color=color,
         bounding_box=bounding_box,
         title=title,
+        color_is_categorical=color_is_categorical,
     )
     validate(df, cfg)
     return Plot.save(df, cfg).show(show)
 
 
 scatter.__doc__ = (
     """
```

### Comparing `clusterfun-0.3.0a7/clusterfun/plot_types/violin.py` & `clusterfun-0.3.1a7/clusterfun/plot_types/violin.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/serve_cli.py` & `clusterfun-0.3.1a7/clusterfun/serve_cli.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/client/__init__.py` & `clusterfun-0.3.1a7/clusterfun/storage/client/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 from clusterfun.storage.client.base import BaseStorageClient
 from clusterfun.storage.client.http import HttpStorageClient
 from clusterfun.storage.client.local import LocalStorageClient
 from clusterfun.storage.client.s3 import S3StorageClient
 
 T = TypeVar("T", bound=BaseStorageClient)
 
-CLIENT_REGISTRY = {"s3": S3StorageClient, "http": HttpStorageClient, "local": LocalStorageClient}
+CLIENT_REGISTRY = {
+    "s3": S3StorageClient,
+    "http": HttpStorageClient,
+    "https": HttpStorageClient,
+    "local": LocalStorageClient,
+}
 
 
 def get_storage_client(uri: str, common_media_path: Optional[str]) -> BaseStorageClient:
     """Get storage client from start of URI, default to LocalStorageClient.
 
     Args:
         uri (str): input uri.
```

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/client/base.py` & `clusterfun-0.3.1a7/clusterfun/storage/client/base.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/client/http.py` & `clusterfun-0.3.1a7/clusterfun/storage/client/http.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/client/local.py` & `clusterfun-0.3.1a7/clusterfun/storage/client/local.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/client/s3.py` & `clusterfun-0.3.1a7/clusterfun/storage/client/s3.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/loader.py` & `clusterfun-0.3.1a7/clusterfun/storage/loader.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/local/data.py` & `clusterfun-0.3.1a7/clusterfun/storage/local/data.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,25 +35,27 @@
     Tuple[List[Dict[str, Any]], Optional[List[str]]]
         Data for plotly graph.
         List of dicts with keys: id, x, y, mode, type, name (optional) and marker (optional)
 
         List of colors for each data point. Used for coloring the data points.
     """
     colors = None
-    if cfg.color is not None:
+    if cfg.color is not None and cfg.color_is_categorical:
         return get_data_per_color(cfg, con, query_addition)
     if cfg.type == "grid":
         data = get_grid_data(con, query_addition)
     else:
         data = get_data_standard(cfg, con, query_addition)
     return data, colors
 
 
 def get_data_standard(
-    cfg: Config, con: sqlite3.Connection, query_addition: Optional[str] = None
+    cfg: Config,
+    con: sqlite3.Connection,
+    query_addition: Optional[str] = None,
 ) -> List[Dict[str, Any]]:
     """Get data for standard plotly graph, in case there is no color column.
 
     Parameters
     ----------
     cfg : Config
         Configuration object
@@ -65,34 +67,41 @@
 
     Returns
     -------
     List[Dict[str, Any]]
         Data for plotly graph.
         List of dicts with keys: id, x, y, mode, type
     """
+    select_columns = ["id"]
+    if cfg.x is not None:
+        select_columns.append(cfg.x)
     if cfg.y is not None:
-        query = f"SELECT id,{cfg.x},{cfg.y} FROM database"
-    elif cfg.x is not None:
-        query = f"SELECT id,{cfg.x} FROM database"
-    else:
-        query = "SELECT id FROM database"
+        select_columns.append(cfg.y)
+    if cfg.color is not None and not cfg.color_is_categorical:
+        select_columns.append(cfg.color)
+
+    query = f"SELECT {','.join(select_columns)} FROM database"
+
     if query_addition:
         query += f" WHERE {query_addition}"
     res = con.execute(query).fetchall()
     data = [
         {
             "id": [x[0] for x in res],
             "mode": "markers",
             "type": "scattergl",
         }
     ]
     if cfg.x is not None:
         data[0]["x"] = [x[1] for x in res]
     if cfg.y is not None:
         data[0]["y"] = [x[2] for x in res]
+    if cfg.color is not None and not cfg.color_is_categorical:
+        # Color is always categorical here, index always the last column
+        data[0]["marker"] = {"color": [x[-1] for x in res], "colorscale": "Viridis", "showscale": True}
     return data
 
 
 def get_grid_data(con: sqlite3.Connection, query_addition: Optional[str] = None) -> List[Dict[str, List[int]]]:
     """Get data for the grid. The grid is a special case as it does not have x and y values,
     so we can be more efficient here.
```

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/local/helpers.py` & `clusterfun-0.3.1a7/clusterfun/storage/local/helpers.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/local/loader.py` & `clusterfun-0.3.1a7/clusterfun/storage/local/loader.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/local/storer.py` & `clusterfun-0.3.1a7/clusterfun/storage/local/storer.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/storage/storer.py` & `clusterfun-0.3.1a7/clusterfun/storage/storer.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/clusterfun/validation.py` & `clusterfun-0.3.1a7/clusterfun/validation.py`

 * *Files identical despite different names*

### Comparing `clusterfun-0.3.0a7/pyproject.toml` & `clusterfun-0.3.1a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clusterfun"
-version = "0.3.0a7"
+version = "0.3.1a7"
 description = "Clusterfun - a plotting library to inspect data"
 authors = ["Jochem Gietema <jochem@giete.ma>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 pandas = "^2.0.0"
```

### Comparing `clusterfun-0.3.0a7/PKG-INFO` & `clusterfun-0.3.1a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterfun
-Version: 0.3.0a7
+Version: 0.3.1a7
 Summary: Clusterfun - a plotting library to inspect data
 Author: Jochem Gietema
 Author-email: jochem@giete.ma
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

