# Comparing `tmp/sky130-0.8.0.tar.gz` & `tmp/sky130-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sky130-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sky130-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sky130-0.8.0.tar` & `sky130-0.9.0.tar`

### file list

```diff
@@ -1,934 +1,934 @@
--rw-r--r--   0        0        0     1077 2023-08-13 15:12:40.019613 sky130-0.8.0/LICENSE
--rw-r--r--   0        0        0      760 2023-08-13 15:12:40.019613 sky130-0.8.0/README.md
--rw-r--r--   0        0        0     2161 2023-08-13 15:12:40.019613 sky130-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1106 2023-08-13 15:12:40.019613 sky130-0.8.0/sky130/__init__.py
--rw-r--r--   0        0        0      422 2023-08-13 15:12:40.019613 sky130-0.8.0/sky130/circuits/sample.pic.yml
--rw-r--r--   0        0        0   276603 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/components.py
--rw-r--r--   0        0        0     1069 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/config.py
--rw-r--r--   0        0        0     8838 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111o_1.gds
--rw-r--r--   0        0        0     9206 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111o_2.gds
--rw-r--r--   0        0        0    12500 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111o_4.gds
--rw-r--r--   0        0        0     7594 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111oi_0.gds
--rw-r--r--   0        0        0     7928 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111oi_1.gds
--rw-r--r--   0        0        0     8374 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111oi_2.gds
--rw-r--r--   0        0        0    14310 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111oi_4.gds
--rw-r--r--   0        0        0     6490 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211o_1.gds
--rw-r--r--   0        0        0     6708 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211o_2.gds
--rw-r--r--   0        0        0     9204 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211o_4.gds
--rw-r--r--   0        0        0     6794 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211oi_1.gds
--rw-r--r--   0        0        0     9088 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211oi_2.gds
--rw-r--r--   0        0        0    10726 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211oi_4.gds
--rw-r--r--   0        0        0     7690 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21bo_1.gds
--rw-r--r--   0        0        0     6440 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21bo_2.gds
--rw-r--r--   0        0        0     8392 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21bo_4.gds
--rw-r--r--   0        0        0     5322 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21boi_0.gds
--rw-r--r--   0        0        0     6382 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21boi_1.gds
--rw-r--r--   0        0        0     6778 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21boi_2.gds
--rw-r--r--   0        0        0     9578 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21boi_4.gds
--rw-r--r--   0        0        0     6134 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21o_1.gds
--rw-r--r--   0        0        0     5698 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21o_2.gds
--rw-r--r--   0        0        0     8308 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21o_4.gds
--rw-r--r--   0        0        0     4814 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21oi_1.gds
--rw-r--r--   0        0        0     6008 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21oi_2.gds
--rw-r--r--   0        0        0     8678 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21oi_4.gds
--rw-r--r--   0        0        0     7276 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221o_1.gds
--rw-r--r--   0        0        0     7820 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221o_2.gds
--rw-r--r--   0        0        0    12334 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221o_4.gds
--rw-r--r--   0        0        0     6716 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221oi_1.gds
--rw-r--r--   0        0        0     9320 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221oi_2.gds
--rw-r--r--   0        0        0    13368 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221oi_4.gds
--rw-r--r--   0        0        0     7222 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a222oi_1.gds
--rw-r--r--   0        0        0     6732 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22o_1.gds
--rw-r--r--   0        0        0     6892 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22o_2.gds
--rw-r--r--   0        0        0     9818 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22o_4.gds
--rw-r--r--   0        0        0     5758 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22oi_1.gds
--rw-r--r--   0        0        0     8630 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22oi_2.gds
--rw-r--r--   0        0        0    12136 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22oi_4.gds
--rw-r--r--   0        0        0     7314 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_1.gds
--rw-r--r--   0        0        0     7874 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_2.gds
--rw-r--r--   0        0        0    11550 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_4.gds
--rw-r--r--   0        0        0     6994 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_1.gds
--rw-r--r--   0        0        0     8944 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_2.gds
--rw-r--r--   0        0        0    14388 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_4.gds
--rw-r--r--   0        0        0     6652 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311o_1.gds
--rw-r--r--   0        0        0     7464 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311o_2.gds
--rw-r--r--   0        0        0    11866 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311o_4.gds
--rw-r--r--   0        0        0     6300 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311oi_1.gds
--rw-r--r--   0        0        0    10464 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311oi_2.gds
--rw-r--r--   0        0        0    15692 2023-08-13 15:12:40.023613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311oi_4.gds
--rw-r--r--   0        0        0     6630 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31o_1.gds
--rw-r--r--   0        0        0     6632 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31o_2.gds
--rw-r--r--   0        0        0    10006 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31o_4.gds
--rw-r--r--   0        0        0     5390 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31oi_1.gds
--rw-r--r--   0        0        0     9146 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31oi_2.gds
--rw-r--r--   0        0        0    13010 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31oi_4.gds
--rw-r--r--   0        0        0     7518 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32o_1.gds
--rw-r--r--   0        0        0     8526 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32o_2.gds
--rw-r--r--   0        0        0    12280 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32o_4.gds
--rw-r--r--   0        0        0     6110 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32oi_1.gds
--rw-r--r--   0        0        0    11378 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32oi_2.gds
--rw-r--r--   0        0        0    16306 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32oi_4.gds
--rw-r--r--   0        0        0     8026 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41o_1.gds
--rw-r--r--   0        0        0     8398 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41o_2.gds
--rw-r--r--   0        0        0    12610 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41o_4.gds
--rw-r--r--   0        0        0     6866 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41oi_1.gds
--rw-r--r--   0        0        0    10214 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41oi_2.gds
--rw-r--r--   0        0        0    16690 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41oi_4.gds
--rw-r--r--   0        0        0     4566 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2_0.gds
--rw-r--r--   0        0        0     4986 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2_1.gds
--rw-r--r--   0        0        0     5530 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2_2.gds
--rw-r--r--   0        0        0     5830 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2_4.gds
--rw-r--r--   0        0        0     5620 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2b_1.gds
--rw-r--r--   0        0        0     5748 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2b_2.gds
--rw-r--r--   0        0        0     5802 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2b_4.gds
--rw-r--r--   0        0        0     7250 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3_1.gds
--rw-r--r--   0        0        0     5956 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3_2.gds
--rw-r--r--   0        0        0     6980 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3_4.gds
--rw-r--r--   0        0        0     6486 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3b_1.gds
--rw-r--r--   0        0        0     6680 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3b_2.gds
--rw-r--r--   0        0        0     6728 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3b_4.gds
--rw-r--r--   0        0        0     6498 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4_1.gds
--rw-r--r--   0        0        0     7362 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4_2.gds
--rw-r--r--   0        0        0     7534 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4_4.gds
--rw-r--r--   0        0        0     7698 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4b_1.gds
--rw-r--r--   0        0        0     8356 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4b_2.gds
--rw-r--r--   0        0        0     7822 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4b_4.gds
--rw-r--r--   0        0        0     8486 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4bb_1.gds
--rw-r--r--   0        0        0     8082 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4bb_2.gds
--rw-r--r--   0        0        0     8804 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4bb_4.gds
--rw-r--r--   0        0        0     4050 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_1.gds
--rw-r--r--   0        0        0    11278 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_12.gds
--rw-r--r--   0        0        0    15620 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_16.gds
--rw-r--r--   0        0        0     4578 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_2.gds
--rw-r--r--   0        0        0     5490 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_4.gds
--rw-r--r--   0        0        0     7120 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_6.gds
--rw-r--r--   0        0        0     8974 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_8.gds
--rw-r--r--   0        0        0    18348 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__bufbuf_16.gds
--rw-r--r--   0        0        0    10618 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__bufbuf_8.gds
--rw-r--r--   0        0        0    16972 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__bufinv_16.gds
--rw-r--r--   0        0        0    10298 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__bufinv_8.gds
--rw-r--r--   0        0        0     3896 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkbuf_1.gds
--rw-r--r--   0        0        0    12806 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkbuf_16.gds
--rw-r--r--   0        0        0     4680 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkbuf_2.gds
--rw-r--r--   0        0        0     5302 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkbuf_4.gds
--rw-r--r--   0        0        0     7900 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkbuf_8.gds
--rw-r--r--   0        0        0     6272 2023-08-13 15:12:40.027613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s15_1.gds
--rw-r--r--   0        0        0     6718 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s15_2.gds
--rw-r--r--   0        0        0     6380 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s18_1.gds
--rw-r--r--   0        0        0     6262 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s18_2.gds
--rw-r--r--   0        0        0     6272 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s25_1.gds
--rw-r--r--   0        0        0     6764 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s25_2.gds
--rw-r--r--   0        0        0     6304 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s50_1.gds
--rw-r--r--   0        0        0     6752 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s50_2.gds
--rw-r--r--   0        0        0     3920 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinv_1.gds
--rw-r--r--   0        0        0    13134 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinv_16.gds
--rw-r--r--   0        0        0     4388 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinv_2.gds
--rw-r--r--   0        0        0     5952 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinv_4.gds
--rw-r--r--   0        0        0     9336 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinv_8.gds
--rw-r--r--   0        0        0     3738 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinvlp_2.gds
--rw-r--r--   0        0        0     5188 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinvlp_4.gds
--rw-r--r--   0        0        0     6766 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__conb_1.gds
--rw-r--r--   0        0        0     4224 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__decap_12.gds
--rw-r--r--   0        0        0     2750 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__decap_3.gds
--rw-r--r--   0        0        0     2878 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__decap_4.gds
--rw-r--r--   0        0        0     3230 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__decap_6.gds
--rw-r--r--   0        0        0     3614 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__decap_8.gds
--rw-r--r--   0        0        0    19682 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfbbn_1.gds
--rw-r--r--   0        0        0    20130 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfbbn_2.gds
--rw-r--r--   0        0        0    19150 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfbbp_1.gds
--rw-r--r--   0        0        0    17770 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrbp_1.gds
--rw-r--r--   0        0        0    18498 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrbp_2.gds
--rw-r--r--   0        0        0    15246 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrtn_1.gds
--rw-r--r--   0        0        0    15372 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrtp_1.gds
--rw-r--r--   0        0        0    16228 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrtp_2.gds
--rw-r--r--   0        0        0    18008 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrtp_4.gds
--rw-r--r--   0        0        0    17898 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfsbp_1.gds
--rw-r--r--   0        0        0    19000 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfsbp_2.gds
--rw-r--r--   0        0        0    15674 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfstp_1.gds
--rw-r--r--   0        0        0    16244 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfstp_2.gds
--rw-r--r--   0        0        0    17806 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfstp_4.gds
--rw-r--r--   0        0        0    14106 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfxbp_1.gds
--rw-r--r--   0        0        0    15214 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfxbp_2.gds
--rw-r--r--   0        0        0    12206 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfxtp_1.gds
--rw-r--r--   0        0        0    12638 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfxtp_2.gds
--rw-r--r--   0        0        0    14238 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfxtp_4.gds
--rw-r--r--   0        0        0     3586 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__diode_2.gds
--rw-r--r--   0        0        0    10112 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlclkp_1.gds
--rw-r--r--   0        0        0    10400 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlclkp_2.gds
--rw-r--r--   0        0        0    12932 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlclkp_4.gds
--rw-r--r--   0        0        0    13888 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrbn_1.gds
--rw-r--r--   0        0        0    13486 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrbn_2.gds
--rw-r--r--   0        0        0    13368 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrbp_1.gds
--rw-r--r--   0        0        0    14986 2023-08-13 15:12:40.031613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrbp_2.gds
--rw-r--r--   0        0        0    11712 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtn_1.gds
--rw-r--r--   0        0        0    11538 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtn_2.gds
--rw-r--r--   0        0        0    12858 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtn_4.gds
--rw-r--r--   0        0        0    10882 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtp_1.gds
--rw-r--r--   0        0        0    11326 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtp_2.gds
--rw-r--r--   0        0        0    12854 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtp_4.gds
--rw-r--r--   0        0        0    13134 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxbn_1.gds
--rw-r--r--   0        0        0    13000 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxbn_2.gds
--rw-r--r--   0        0        0    12630 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxbp_1.gds
--rw-r--r--   0        0        0    10746 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxtn_1.gds
--rw-r--r--   0        0        0    10216 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxtn_2.gds
--rw-r--r--   0        0        0    11836 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxtn_4.gds
--rw-r--r--   0        0        0    10294 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxtp_1.gds
--rw-r--r--   0        0        0     5552 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd1_1.gds
--rw-r--r--   0        0        0     6010 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd2_1.gds
--rw-r--r--   0        0        0     6070 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd3_1.gds
--rw-r--r--   0        0        0     7928 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s2s_1.gds
--rw-r--r--   0        0        0     7928 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s4s_1.gds
--rw-r--r--   0        0        0     7676 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s6s_1.gds
--rw-r--r--   0        0        0     6962 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ebufn_1.gds
--rw-r--r--   0        0        0     7340 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ebufn_2.gds
--rw-r--r--   0        0        0     9578 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ebufn_4.gds
--rw-r--r--   0        0        0    14044 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ebufn_8.gds
--rw-r--r--   0        0        0    19118 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__edfxbp_1.gds
--rw-r--r--   0        0        0    17568 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__edfxtp_1.gds
--rw-r--r--   0        0        0     4386 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvn_0.gds
--rw-r--r--   0        0        0     5210 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvn_1.gds
--rw-r--r--   0        0        0     6430 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvn_2.gds
--rw-r--r--   0        0        0     7922 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvn_4.gds
--rw-r--r--   0        0        0    12408 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvn_8.gds
--rw-r--r--   0        0        0     4656 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvp_1.gds
--rw-r--r--   0        0        0     6332 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvp_2.gds
--rw-r--r--   0        0        0     8108 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvp_4.gds
--rw-r--r--   0        0        0    12766 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvp_8.gds
--rw-r--r--   0        0        0    13092 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fa_1.gds
--rw-r--r--   0        0        0    13746 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fa_2.gds
--rw-r--r--   0        0        0    15828 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fa_4.gds
--rw-r--r--   0        0        0    19582 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fah_1.gds
--rw-r--r--   0        0        0    19430 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fahcin_1.gds
--rw-r--r--   0        0        0    18950 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fahcon_1.gds
--rw-r--r--   0        0        0     1384 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fill_1.gds
--rw-r--r--   0        0        0     1512 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fill_2.gds
--rw-r--r--   0        0        0     1768 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fill_4.gds
--rw-r--r--   0        0        0     2280 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fill_8.gds
--rw-r--r--   0        0        0     9028 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ha_1.gds
--rw-r--r--   0        0        0     9718 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ha_2.gds
--rw-r--r--   0        0        0    14160 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ha_4.gds
--rw-r--r--   0        0        0     3636 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_1.gds
--rw-r--r--   0        0        0    10452 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_12.gds
--rw-r--r--   0        0        0    11632 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_16.gds
--rw-r--r--   0        0        0     7652 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_2.gds
--rw-r--r--   0        0        0     5132 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_4.gds
--rw-r--r--   0        0        0     6092 2023-08-13 15:12:40.035613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_6.gds
--rw-r--r--   0        0        0     7642 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_8.gds
--rw-r--r--   0        0        0     3134 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_bleeder_1.gds
--rw-r--r--   0        0        0     4242 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_1.gds
--rw-r--r--   0        0        0    14752 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_16.gds
--rw-r--r--   0        0        0     4934 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_2.gds
--rw-r--r--   0        0        0     6080 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_4.gds
--rw-r--r--   0        0        0     9014 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_8.gds
--rw-r--r--   0        0        0     4284 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_1.gds
--rw-r--r--   0        0        0    15400 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_16.gds
--rw-r--r--   0        0        0     4862 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_2.gds
--rw-r--r--   0        0        0     6778 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_4.gds
--rw-r--r--   0        0        0    10626 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_8.gds
--rw-r--r--   0        0        0     5274 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_12.gds
--rw-r--r--   0        0        0     3224 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_3.gds
--rw-r--r--   0        0        0     3416 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_4.gds
--rw-r--r--   0        0        0     3896 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_6.gds
--rw-r--r--   0        0        0     4408 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_8.gds
--rw-r--r--   0        0        0     5018 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso0n_1.gds
--rw-r--r--   0        0        0     5650 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso0p_1.gds
--rw-r--r--   0        0        0     5062 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso1n_1.gds
--rw-r--r--   0        0        0     4340 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso1p_1.gds
--rw-r--r--   0        0        0     9080 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputisolatch_1.gds
--rw-r--r--   0        0        0     4422 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_1.gds
--rw-r--r--   0        0        0    23764 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_16.gds
--rw-r--r--   0        0        0     6098 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_2.gds
--rw-r--r--   0        0        0     8674 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_4.gds
--rw-r--r--   0        0        0    13458 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_8.gds
--rw-r--r--   0        0        0    22078 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrckapwr_16.gds
--rw-r--r--   0        0        0    13400 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_1.gds
--rw-r--r--   0        0        0    13432 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_2.gds
--rw-r--r--   0        0        0    14664 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_4.gds
--rw-r--r--   0        0        0    13068 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_4.gds
--rw-r--r--   0        0        0    13396 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_1.gds
--rw-r--r--   0        0        0    13428 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_2.gds
--rw-r--r--   0        0        0    14660 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_4.gds
--rw-r--r--   0        0        0     4066 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__macro_sparecell.gds
--rw-r--r--   0        0        0     6268 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__maj3_1.gds
--rw-r--r--   0        0        0     6592 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__maj3_2.gds
--rw-r--r--   0        0        0     8014 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__maj3_4.gds
--rw-r--r--   0        0        0     6972 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2_1.gds
--rw-r--r--   0        0        0     7334 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2_2.gds
--rw-r--r--   0        0        0     8478 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2_4.gds
--rw-r--r--   0        0        0    12804 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2_8.gds
--rw-r--r--   0        0        0     7040 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2i_1.gds
--rw-r--r--   0        0        0     8158 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2i_2.gds
--rw-r--r--   0        0        0    12286 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2i_4.gds
--rw-r--r--   0        0        0    15620 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux4_1.gds
--rw-r--r--   0        0        0    14382 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux4_2.gds
--rw-r--r--   0        0        0    15752 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux4_4.gds
--rw-r--r--   0        0        0     4036 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2_1.gds
--rw-r--r--   0        0        0    10118 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2_2.gds
--rw-r--r--   0        0        0     7726 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2_4.gds
--rw-r--r--   0        0        0    12436 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2_8.gds
--rw-r--r--   0        0        0     4676 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2b_1.gds
--rw-r--r--   0        0        0     6708 2023-08-13 15:12:40.039613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2b_2.gds
--rw-r--r--   0        0        0     9202 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2b_4.gds
--rw-r--r--   0        0        0     4486 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3_1.gds
--rw-r--r--   0        0        0     7370 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3_2.gds
--rw-r--r--   0        0        0    11280 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3_4.gds
--rw-r--r--   0        0        0     5680 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3b_1.gds
--rw-r--r--   0        0        0     7094 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3b_2.gds
--rw-r--r--   0        0        0    11932 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3b_4.gds
--rw-r--r--   0        0        0     5348 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4_1.gds
--rw-r--r--   0        0        0     8872 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4_2.gds
--rw-r--r--   0        0        0    13550 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4_4.gds
--rw-r--r--   0        0        0     5960 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4b_1.gds
--rw-r--r--   0        0        0    10202 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4b_2.gds
--rw-r--r--   0        0        0    15074 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4b_4.gds
--rw-r--r--   0        0        0     7302 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4bb_1.gds
--rw-r--r--   0        0        0    10534 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4bb_2.gds
--rw-r--r--   0        0        0    15134 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4bb_4.gds
--rw-r--r--   0        0        0     3750 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2_1.gds
--rw-r--r--   0        0        0     9642 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2_2.gds
--rw-r--r--   0        0        0     7190 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2_4.gds
--rw-r--r--   0        0        0    11542 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2_8.gds
--rw-r--r--   0        0        0     4398 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2b_1.gds
--rw-r--r--   0        0        0     6074 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2b_2.gds
--rw-r--r--   0        0        0     8650 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2b_4.gds
--rw-r--r--   0        0        0     4324 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3_1.gds
--rw-r--r--   0        0        0     6692 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3_2.gds
--rw-r--r--   0        0        0     9460 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3_4.gds
--rw-r--r--   0        0        0     4888 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3b_1.gds
--rw-r--r--   0        0        0     7960 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3b_2.gds
--rw-r--r--   0        0        0    10244 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3b_4.gds
--rw-r--r--   0        0        0     4864 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4_1.gds
--rw-r--r--   0        0        0     7794 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4_2.gds
--rw-r--r--   0        0        0    12462 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4_4.gds
--rw-r--r--   0        0        0     5350 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4b_1.gds
--rw-r--r--   0        0        0     9414 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4b_2.gds
--rw-r--r--   0        0        0    13638 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4b_4.gds
--rw-r--r--   0        0        0     6506 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4bb_1.gds
--rw-r--r--   0        0        0     9470 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4bb_2.gds
--rw-r--r--   0        0        0    13670 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4bb_4.gds
--rw-r--r--   0        0        0     8548 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111a_1.gds
--rw-r--r--   0        0        0     8254 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111a_2.gds
--rw-r--r--   0        0        0    11072 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111a_4.gds
--rw-r--r--   0        0        0     6182 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111ai_1.gds
--rw-r--r--   0        0        0     9610 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111ai_2.gds
--rw-r--r--   0        0        0    15556 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111ai_4.gds
--rw-r--r--   0        0        0     6928 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211a_1.gds
--rw-r--r--   0        0        0     6468 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211a_2.gds
--rw-r--r--   0        0        0     9140 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211a_4.gds
--rw-r--r--   0        0        0     5542 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211ai_1.gds
--rw-r--r--   0        0        0     7542 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211ai_2.gds
--rw-r--r--   0        0        0    10166 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211ai_4.gds
--rw-r--r--   0        0        0     5716 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21a_1.gds
--rw-r--r--   0        0        0     5652 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21a_2.gds
--rw-r--r--   0        0        0     8068 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21a_4.gds
--rw-r--r--   0        0        0     4406 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ai_0.gds
--rw-r--r--   0        0        0     4862 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ai_1.gds
--rw-r--r--   0        0        0     6588 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ai_2.gds
--rw-r--r--   0        0        0     8198 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ai_4.gds
--rw-r--r--   0        0        0     6248 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ba_1.gds
--rw-r--r--   0        0        0     6432 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ba_2.gds
--rw-r--r--   0        0        0     9144 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ba_4.gds
--rw-r--r--   0        0        0     5658 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21bai_1.gds
--rw-r--r--   0        0        0     7202 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21bai_2.gds
--rw-r--r--   0        0        0    10954 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21bai_4.gds
--rw-r--r--   0        0        0     7374 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221a_1.gds
--rw-r--r--   0        0        0     7620 2023-08-13 15:12:40.043614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221a_2.gds
--rw-r--r--   0        0        0    10954 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221a_4.gds
--rw-r--r--   0        0        0     6552 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221ai_1.gds
--rw-r--r--   0        0        0     8812 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221ai_2.gds
--rw-r--r--   0        0        0    13560 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221ai_4.gds
--rw-r--r--   0        0        0     6162 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22a_1.gds
--rw-r--r--   0        0        0     6738 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22a_2.gds
--rw-r--r--   0        0        0     9770 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22a_4.gds
--rw-r--r--   0        0        0     4980 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22ai_1.gds
--rw-r--r--   0        0        0     8020 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22ai_2.gds
--rw-r--r--   0        0        0    10748 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22ai_4.gds
--rw-r--r--   0        0        0     6538 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_1.gds
--rw-r--r--   0        0        0     7194 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_2.gds
--rw-r--r--   0        0        0    11278 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_4.gds
--rw-r--r--   0        0        0     6316 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_1.gds
--rw-r--r--   0        0        0     8644 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_2.gds
--rw-r--r--   0        0        0    14908 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_4.gds
--rw-r--r--   0        0        0     7760 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311a_1.gds
--rw-r--r--   0        0        0     8494 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311a_2.gds
--rw-r--r--   0        0        0    12436 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311a_4.gds
--rw-r--r--   0        0        0     7572 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311ai_0.gds
--rw-r--r--   0        0        0     6994 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311ai_1.gds
--rw-r--r--   0        0        0    10542 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311ai_2.gds
--rw-r--r--   0        0        0    15998 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311ai_4.gds
--rw-r--r--   0        0        0     6708 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31a_1.gds
--rw-r--r--   0        0        0     7410 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31a_2.gds
--rw-r--r--   0        0        0    11256 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31a_4.gds
--rw-r--r--   0        0        0     6418 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31ai_1.gds
--rw-r--r--   0        0        0     9072 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31ai_2.gds
--rw-r--r--   0        0        0    14628 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31ai_4.gds
--rw-r--r--   0        0        0     7188 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32a_1.gds
--rw-r--r--   0        0        0     7878 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32a_2.gds
--rw-r--r--   0        0        0    12392 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32a_4.gds
--rw-r--r--   0        0        0     6820 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32ai_1.gds
--rw-r--r--   0        0        0    10070 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32ai_2.gds
--rw-r--r--   0        0        0    16122 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32ai_4.gds
--rw-r--r--   0        0        0     8298 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41a_1.gds
--rw-r--r--   0        0        0     9224 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41a_2.gds
--rw-r--r--   0        0        0    13248 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41a_4.gds
--rw-r--r--   0        0        0     7390 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41ai_1.gds
--rw-r--r--   0        0        0    11188 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41ai_2.gds
--rw-r--r--   0        0        0    18202 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41ai_4.gds
--rw-r--r--   0        0        0     4036 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2_0.gds
--rw-r--r--   0        0        0     4308 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2_1.gds
--rw-r--r--   0        0        0     4500 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2_2.gds
--rw-r--r--   0        0        0     5844 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2_4.gds
--rw-r--r--   0        0        0     5032 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2b_1.gds
--rw-r--r--   0        0        0     5608 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2b_2.gds
--rw-r--r--   0        0        0     6920 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2b_4.gds
--rw-r--r--   0        0        0     5212 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3_1.gds
--rw-r--r--   0        0        0     5756 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3_2.gds
--rw-r--r--   0        0        0     7200 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3_4.gds
--rw-r--r--   0        0        0     6350 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3b_1.gds
--rw-r--r--   0        0        0     5934 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3b_2.gds
--rw-r--r--   0        0        0     6578 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3b_4.gds
--rw-r--r--   0        0        0     6164 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4_1.gds
--rw-r--r--   0        0        0     6692 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4_2.gds
--rw-r--r--   0        0        0     7388 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4_4.gds
--rw-r--r--   0        0        0     7368 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4b_1.gds
--rw-r--r--   0        0        0     6638 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4b_2.gds
--rw-r--r--   0        0        0     8576 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4b_4.gds
--rw-r--r--   0        0        0     7192 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4bb_1.gds
--rw-r--r--   0        0        0     7752 2023-08-13 15:12:40.047613 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4bb_2.gds
--rw-r--r--   0        0        0     8902 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4bb_4.gds
--rw-r--r--   0        0        0    10154 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__probe_p_8.gds
--rw-r--r--   0        0        0    12944 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__probec_p_8.gds
--rw-r--r--   0        0        0    23076 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfbbn_1.gds
--rw-r--r--   0        0        0    23508 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfbbn_2.gds
--rw-r--r--   0        0        0    22448 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfbbp_1.gds
--rw-r--r--   0        0        0    21054 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrbp_1.gds
--rw-r--r--   0        0        0    20788 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrbp_2.gds
--rw-r--r--   0        0        0    18978 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrtn_1.gds
--rw-r--r--   0        0        0    18974 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_1.gds
--rw-r--r--   0        0        0    19486 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_2.gds
--rw-r--r--   0        0        0    20574 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_4.gds
--rw-r--r--   0        0        0    21818 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfsbp_1.gds
--rw-r--r--   0        0        0    22778 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfsbp_2.gds
--rw-r--r--   0        0        0    19738 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfstp_1.gds
--rw-r--r--   0        0        0    20650 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfstp_2.gds
--rw-r--r--   0        0        0    21592 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfstp_4.gds
--rw-r--r--   0        0        0    17148 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfxbp_1.gds
--rw-r--r--   0        0        0    18028 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfxbp_2.gds
--rw-r--r--   0        0        0    15352 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_1.gds
--rw-r--r--   0        0        0    15944 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_2.gds
--rw-r--r--   0        0        0    16604 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_4.gds
--rw-r--r--   0        0        0    11122 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_1.gds
--rw-r--r--   0        0        0    11746 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_2.gds
--rw-r--r--   0        0        0    13554 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_4.gds
--rw-r--r--   0        0        0    22832 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sedfxbp_1.gds
--rw-r--r--   0        0        0    23984 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sedfxbp_2.gds
--rw-r--r--   0        0        0    21282 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_1.gds
--rw-r--r--   0        0        0    21858 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_2.gds
--rw-r--r--   0        0        0    23010 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_4.gds
--rw-r--r--   0        0        0     1958 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__tap_1.gds
--rw-r--r--   0        0        0     2406 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__tap_2.gds
--rw-r--r--   0        0        0     1968 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__tapvgnd2_1.gds
--rw-r--r--   0        0        0     1966 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__tapvgnd_1.gds
--rw-r--r--   0        0        0     1758 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__tapvpwrvgnd_1.gds
--rw-r--r--   0        0        0     5448 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor2_1.gds
--rw-r--r--   0        0        0     8824 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor2_2.gds
--rw-r--r--   0        0        0    14184 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor2_4.gds
--rw-r--r--   0        0        0    11750 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor3_1.gds
--rw-r--r--   0        0        0    12322 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor3_2.gds
--rw-r--r--   0        0        0    13330 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor3_4.gds
--rw-r--r--   0        0        0     5526 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor2_1.gds
--rw-r--r--   0        0        0     9222 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor2_2.gds
--rw-r--r--   0        0        0    14550 2023-08-13 15:12:40.051614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor2_4.gds
--rw-r--r--   0        0        0    11956 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor3_1.gds
--rw-r--r--   0        0        0    12450 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor3_2.gds
--rw-r--r--   0        0        0    13442 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor3_4.gds
--rw-r--r--   0        0        0     9062 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111o_1.gds
--rw-r--r--   0        0        0     9080 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111o_2.gds
--rw-r--r--   0        0        0    13964 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111o_4.gds
--rw-r--r--   0        0        0     6816 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111oi_1.gds
--rw-r--r--   0        0        0    10046 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111oi_2.gds
--rw-r--r--   0        0        0    16246 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111oi_4.gds
--rw-r--r--   0        0        0     7314 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211o_1.gds
--rw-r--r--   0        0        0     7536 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211o_2.gds
--rw-r--r--   0        0        0    11728 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211o_4.gds
--rw-r--r--   0        0        0     5798 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211oi_1.gds
--rw-r--r--   0        0        0     9072 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211oi_2.gds
--rw-r--r--   0        0        0    14822 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211oi_4.gds
--rw-r--r--   0        0        0     7384 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21bo_1.gds
--rw-r--r--   0        0        0     6860 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21bo_2.gds
--rw-r--r--   0        0        0    10170 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21bo_4.gds
--rw-r--r--   0        0        0     6936 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21boi_1.gds
--rw-r--r--   0        0        0     8126 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21boi_2.gds
--rw-r--r--   0        0        0    13102 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21boi_4.gds
--rw-r--r--   0        0        0     6532 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21o_1.gds
--rw-r--r--   0        0        0     7074 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21o_2.gds
--rw-r--r--   0        0        0     9972 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21o_4.gds
--rw-r--r--   0        0        0     5046 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21oi_1.gds
--rw-r--r--   0        0        0     7058 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21oi_2.gds
--rw-r--r--   0        0        0    10398 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21oi_4.gds
--rw-r--r--   0        0        0     8604 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221o_1.gds
--rw-r--r--   0        0        0     8450 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221o_2.gds
--rw-r--r--   0        0        0    13584 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221o_4.gds
--rw-r--r--   0        0        0     7992 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221oi_1.gds
--rw-r--r--   0        0        0    10096 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221oi_2.gds
--rw-r--r--   0        0        0    18014 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221oi_4.gds
--rw-r--r--   0        0        0     9100 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a222o_1.gds
--rw-r--r--   0        0        0     8818 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a222o_2.gds
--rw-r--r--   0        0        0     8968 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a222oi_1.gds
--rw-r--r--   0        0        0    11714 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a222oi_2.gds
--rw-r--r--   0        0        0     7592 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22o_1.gds
--rw-r--r--   0        0        0     7360 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22o_2.gds
--rw-r--r--   0        0        0    11488 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22o_4.gds
--rw-r--r--   0        0        0     5858 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22oi_1.gds
--rw-r--r--   0        0        0     8374 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22oi_2.gds
--rw-r--r--   0        0        0    13672 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22oi_4.gds
--rw-r--r--   0        0        0     8276 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_1.gds
--rw-r--r--   0        0        0     8708 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_2.gds
--rw-r--r--   0        0        0    11684 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_4.gds
--rw-r--r--   0        0        0     6766 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_1.gds
--rw-r--r--   0        0        0     9084 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_2.gds
--rw-r--r--   0        0        0    14706 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_4.gds
--rw-r--r--   0        0        0     7712 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311o_1.gds
--rw-r--r--   0        0        0     7348 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311o_2.gds
--rw-r--r--   0        0        0    12498 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311o_4.gds
--rw-r--r--   0        0        0     6622 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311oi_1.gds
--rw-r--r--   0        0        0    10382 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311oi_2.gds
--rw-r--r--   0        0        0    16532 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311oi_4.gds
--rw-r--r--   0        0        0     7150 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31o_1.gds
--rw-r--r--   0        0        0     7138 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31o_2.gds
--rw-r--r--   0        0        0    12970 2023-08-13 15:12:40.055614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31o_4.gds
--rw-r--r--   0        0        0     6208 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31oi_1.gds
--rw-r--r--   0        0        0     8372 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31oi_2.gds
--rw-r--r--   0        0        0    14192 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31oi_4.gds
--rw-r--r--   0        0        0     7170 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32o_1.gds
--rw-r--r--   0        0        0     7108 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32o_2.gds
--rw-r--r--   0        0        0    13552 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32o_4.gds
--rw-r--r--   0        0        0     6658 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32oi_1.gds
--rw-r--r--   0        0        0    10626 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32oi_2.gds
--rw-r--r--   0        0        0    17348 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32oi_4.gds
--rw-r--r--   0        0        0     8176 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41o_1.gds
--rw-r--r--   0        0        0     8876 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41o_2.gds
--rw-r--r--   0        0        0    13542 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41o_4.gds
--rw-r--r--   0        0        0     6118 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41oi_1.gds
--rw-r--r--   0        0        0    10286 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41oi_2.gds
--rw-r--r--   0        0        0    16672 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41oi_4.gds
--rw-r--r--   0        0        0     5204 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2_1.gds
--rw-r--r--   0        0        0     5334 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2_2.gds
--rw-r--r--   0        0        0     7706 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2_4.gds
--rw-r--r--   0        0        0     6250 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2b_1.gds
--rw-r--r--   0        0        0     5582 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2b_2.gds
--rw-r--r--   0        0        0     8556 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2b_4.gds
--rw-r--r--   0        0        0     6146 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3_1.gds
--rw-r--r--   0        0        0     6546 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3_2.gds
--rw-r--r--   0        0        0    10552 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3_4.gds
--rw-r--r--   0        0        0     7096 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3b_1.gds
--rw-r--r--   0        0        0     7872 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3b_2.gds
--rw-r--r--   0        0        0    10858 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3b_4.gds
--rw-r--r--   0        0        0     7430 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4_1.gds
--rw-r--r--   0        0        0     7336 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4_2.gds
--rw-r--r--   0        0        0    11062 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4_4.gds
--rw-r--r--   0        0        0     8018 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4b_1.gds
--rw-r--r--   0        0        0     6730 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4b_2.gds
--rw-r--r--   0        0        0    11374 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4b_4.gds
--rw-r--r--   0        0        0     8078 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4bb_1.gds
--rw-r--r--   0        0        0     8762 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4bb_2.gds
--rw-r--r--   0        0        0    14658 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4bb_4.gds
--rw-r--r--   0        0        0     4452 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__buf_1.gds
--rw-r--r--   0        0        0    18612 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__buf_16.gds
--rw-r--r--   0        0        0     4822 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__buf_2.gds
--rw-r--r--   0        0        0     5850 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__buf_4.gds
--rw-r--r--   0        0        0     9922 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__buf_8.gds
--rw-r--r--   0        0        0    21314 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__bufbuf_16.gds
--rw-r--r--   0        0        0    11088 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__bufbuf_8.gds
--rw-r--r--   0        0        0    20254 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__bufinv_16.gds
--rw-r--r--   0        0        0     9306 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__bufinv_8.gds
--rw-r--r--   0        0        0     4930 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkbuf_1.gds
--rw-r--r--   0        0        0    16060 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkbuf_16.gds
--rw-r--r--   0        0        0     4300 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkbuf_2.gds
--rw-r--r--   0        0        0     5630 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkbuf_4.gds
--rw-r--r--   0        0        0     8876 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkbuf_8.gds
--rw-r--r--   0        0        0     5952 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd1_1.gds
--rw-r--r--   0        0        0     5952 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd2_1.gds
--rw-r--r--   0        0        0     5936 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd3_1.gds
--rw-r--r--   0        0        0     8112 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd1_1.gds
--rw-r--r--   0        0        0     8112 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd2_1.gds
--rw-r--r--   0        0        0     8064 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd3_1.gds
--rw-r--r--   0        0        0     4134 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkinv_1.gds
--rw-r--r--   0        0        0    18546 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkinv_16.gds
--rw-r--r--   0        0        0     4236 2023-08-13 15:12:40.059614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkinv_2.gds
--rw-r--r--   0        0        0     6184 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkinv_4.gds
--rw-r--r--   0        0        0    10004 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkinv_8.gds
--rw-r--r--   0        0        0     4476 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__conb_1.gds
--rw-r--r--   0        0        0     2994 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__decap_4.gds
--rw-r--r--   0        0        0     4082 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__decap_8.gds
--rw-r--r--   0        0        0    20744 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfbbn_1.gds
--rw-r--r--   0        0        0    21584 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfbbn_2.gds
--rw-r--r--   0        0        0    20052 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfbbp_1.gds
--rw-r--r--   0        0        0    17626 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrbp_1.gds
--rw-r--r--   0        0        0    19776 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrbp_2.gds
--rw-r--r--   0        0        0    16856 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrtn_1.gds
--rw-r--r--   0        0        0    16474 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrtp_1.gds
--rw-r--r--   0        0        0    17522 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrtp_2.gds
--rw-r--r--   0        0        0    18906 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrtp_4.gds
--rw-r--r--   0        0        0    18242 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfsbp_1.gds
--rw-r--r--   0        0        0    19460 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfsbp_2.gds
--rw-r--r--   0        0        0    17482 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfstp_1.gds
--rw-r--r--   0        0        0    17252 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfstp_2.gds
--rw-r--r--   0        0        0    18930 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfstp_4.gds
--rw-r--r--   0        0        0    15130 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfxbp_1.gds
--rw-r--r--   0        0        0    16412 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfxbp_2.gds
--rw-r--r--   0        0        0    12764 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfxtp_1.gds
--rw-r--r--   0        0        0    13500 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfxtp_2.gds
--rw-r--r--   0        0        0    14984 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfxtp_4.gds
--rw-r--r--   0        0        0     3950 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__diode_2.gds
--rw-r--r--   0        0        0    10900 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlclkp_1.gds
--rw-r--r--   0        0        0    12624 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlclkp_2.gds
--rw-r--r--   0        0        0    13088 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlclkp_4.gds
--rw-r--r--   0        0        0    13742 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrbn_1.gds
--rw-r--r--   0        0        0    14132 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrbn_2.gds
--rw-r--r--   0        0        0    12896 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrbp_1.gds
--rw-r--r--   0        0        0    13922 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrbp_2.gds
--rw-r--r--   0        0        0    11104 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtn_1.gds
--rw-r--r--   0        0        0    11760 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtn_2.gds
--rw-r--r--   0        0        0    14376 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtn_4.gds
--rw-r--r--   0        0        0    10418 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtp_1.gds
--rw-r--r--   0        0        0    11154 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtp_2.gds
--rw-r--r--   0        0        0    13924 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtp_4.gds
--rw-r--r--   0        0        0    13118 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxbn_1.gds
--rw-r--r--   0        0        0    13966 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxbn_2.gds
--rw-r--r--   0        0        0    13180 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxbp_1.gds
--rw-r--r--   0        0        0    11300 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxtn_1.gds
--rw-r--r--   0        0        0    11436 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxtn_2.gds
--rw-r--r--   0        0        0    12508 2023-08-13 15:12:40.063614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxtn_4.gds
--rw-r--r--   0        0        0    11848 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxtp_1.gds
--rw-r--r--   0        0        0     6620 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd1_1.gds
--rw-r--r--   0        0        0     6620 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd2_1.gds
--rw-r--r--   0        0        0     6588 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd3_1.gds
--rw-r--r--   0        0        0     8188 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s2s_1.gds
--rw-r--r--   0        0        0     8236 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s4s_1.gds
--rw-r--r--   0        0        0     8236 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s6s_1.gds
--rw-r--r--   0        0        0     6522 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ebufn_1.gds
--rw-r--r--   0        0        0     7324 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ebufn_2.gds
--rw-r--r--   0        0        0     9612 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ebufn_4.gds
--rw-r--r--   0        0        0    14906 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ebufn_8.gds
--rw-r--r--   0        0        0    20468 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__edfxbp_1.gds
--rw-r--r--   0        0        0    18594 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__edfxtp_1.gds
--rw-r--r--   0        0        0     4956 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvn_1.gds
--rw-r--r--   0        0        0     7078 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvn_2.gds
--rw-r--r--   0        0        0     9292 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvn_4.gds
--rw-r--r--   0        0        0    14230 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvn_8.gds
--rw-r--r--   0        0        0     5128 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvp_1.gds
--rw-r--r--   0        0        0     6854 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvp_2.gds
--rw-r--r--   0        0        0     9576 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvp_4.gds
--rw-r--r--   0        0        0    14452 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvp_8.gds
--rw-r--r--   0        0        0    14168 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fa_1.gds
--rw-r--r--   0        0        0    13544 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fa_2.gds
--rw-r--r--   0        0        0    17172 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fa_4.gds
--rw-r--r--   0        0        0    20584 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fah_1.gds
--rw-r--r--   0        0        0    19798 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fah_2.gds
--rw-r--r--   0        0        0    22438 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fah_4.gds
--rw-r--r--   0        0        0    19264 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fahcin_1.gds
--rw-r--r--   0        0        0    18432 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fahcon_1.gds
--rw-r--r--   0        0        0     1424 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_1.gds
--rw-r--r--   0        0        0     1552 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_2.gds
--rw-r--r--   0        0        0     1808 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_4.gds
--rw-r--r--   0        0        0     2320 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_8.gds
--rw-r--r--   0        0        0     2088 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_diode_2.gds
--rw-r--r--   0        0        0     2600 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_diode_4.gds
--rw-r--r--   0        0        0     3880 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_diode_8.gds
--rw-r--r--   0        0        0     9352 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ha_1.gds
--rw-r--r--   0        0        0     9138 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ha_2.gds
--rw-r--r--   0        0        0    15250 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ha_4.gds
--rw-r--r--   0        0        0     4062 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__inv_1.gds
--rw-r--r--   0        0        0    14252 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__inv_16.gds
--rw-r--r--   0        0        0     4478 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__inv_2.gds
--rw-r--r--   0        0        0     5284 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__inv_4.gds
--rw-r--r--   0        0        0     7702 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__inv_8.gds
--rw-r--r--   0        0        0     7028 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__maj3_1.gds
--rw-r--r--   0        0        0     7956 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__maj3_2.gds
--rw-r--r--   0        0        0    12438 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__maj3_4.gds
--rw-r--r--   0        0        0     6994 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2_1.gds
--rw-r--r--   0        0        0     8132 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2_2.gds
--rw-r--r--   0        0        0    12544 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2_4.gds
--rw-r--r--   0        0        0     7112 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2i_1.gds
--rw-r--r--   0        0        0    10010 2023-08-13 15:12:40.067614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2i_2.gds
--rw-r--r--   0        0        0    14492 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2i_4.gds
--rw-r--r--   0        0        0    14562 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux4_1.gds
--rw-r--r--   0        0        0    15604 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux4_2.gds
--rw-r--r--   0        0        0    25202 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux4_4.gds
--rw-r--r--   0        0        0     4388 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2_1.gds
--rw-r--r--   0        0        0     5224 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2_2.gds
--rw-r--r--   0        0        0     8050 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2_4.gds
--rw-r--r--   0        0        0    12224 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2_8.gds
--rw-r--r--   0        0        0     4846 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2b_1.gds
--rw-r--r--   0        0        0     5982 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2b_2.gds
--rw-r--r--   0        0        0     9482 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2b_4.gds
--rw-r--r--   0        0        0     5456 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3_1.gds
--rw-r--r--   0        0        0     6760 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3_2.gds
--rw-r--r--   0        0        0    10832 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3_4.gds
--rw-r--r--   0        0        0     5770 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3b_1.gds
--rw-r--r--   0        0        0     8264 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3b_2.gds
--rw-r--r--   0        0        0    10450 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3b_4.gds
--rw-r--r--   0        0        0     5512 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4_1.gds
--rw-r--r--   0        0        0     9054 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4_2.gds
--rw-r--r--   0        0        0    14382 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4_4.gds
--rw-r--r--   0        0        0     6140 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4b_1.gds
--rw-r--r--   0        0        0    10308 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4b_2.gds
--rw-r--r--   0        0        0    14142 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4b_4.gds
--rw-r--r--   0        0        0     7662 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4bb_1.gds
--rw-r--r--   0        0        0    10750 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4bb_2.gds
--rw-r--r--   0        0        0    16040 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4bb_4.gds
--rw-r--r--   0        0        0     3960 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2_1.gds
--rw-r--r--   0        0        0     5380 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2_2.gds
--rw-r--r--   0        0        0     8288 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2_4.gds
--rw-r--r--   0        0        0    12336 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2_8.gds
--rw-r--r--   0        0        0     4954 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2b_1.gds
--rw-r--r--   0        0        0     6540 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2b_2.gds
--rw-r--r--   0        0        0     8586 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2b_4.gds
--rw-r--r--   0        0        0     4914 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3_1.gds
--rw-r--r--   0        0        0     7010 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3_2.gds
--rw-r--r--   0        0        0    10124 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3_4.gds
--rw-r--r--   0        0        0     5338 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3b_1.gds
--rw-r--r--   0        0        0     8854 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3b_2.gds
--rw-r--r--   0        0        0    11926 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3b_4.gds
--rw-r--r--   0        0        0     5742 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4_1.gds
--rw-r--r--   0        0        0     8252 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4_2.gds
--rw-r--r--   0        0        0    14130 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4_4.gds
--rw-r--r--   0        0        0     6134 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4b_1.gds
--rw-r--r--   0        0        0    10352 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4b_2.gds
--rw-r--r--   0        0        0    16104 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4b_4.gds
--rw-r--r--   0        0        0     7596 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4bb_1.gds
--rw-r--r--   0        0        0    12042 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4bb_2.gds
--rw-r--r--   0        0        0    16138 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4bb_4.gds
--rw-r--r--   0        0        0     7934 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111a_1.gds
--rw-r--r--   0        0        0     8436 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111a_2.gds
--rw-r--r--   0        0        0    13056 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111a_4.gds
--rw-r--r--   0        0        0     6994 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111ai_1.gds
--rw-r--r--   0        0        0    11050 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111ai_2.gds
--rw-r--r--   0        0        0    15894 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111ai_4.gds
--rw-r--r--   0        0        0     8144 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211a_1.gds
--rw-r--r--   0        0        0     7412 2023-08-13 15:12:40.071614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211a_2.gds
--rw-r--r--   0        0        0    11204 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211a_4.gds
--rw-r--r--   0        0        0     6462 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211ai_1.gds
--rw-r--r--   0        0        0     9316 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211ai_2.gds
--rw-r--r--   0        0        0    13998 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211ai_4.gds
--rw-r--r--   0        0        0     6732 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21a_1.gds
--rw-r--r--   0        0        0     7120 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21a_2.gds
--rw-r--r--   0        0        0     9846 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21a_4.gds
--rw-r--r--   0        0        0     5158 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ai_1.gds
--rw-r--r--   0        0        0     6662 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ai_2.gds
--rw-r--r--   0        0        0    10192 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ai_4.gds
--rw-r--r--   0        0        0     7460 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ba_1.gds
--rw-r--r--   0        0        0     6954 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ba_2.gds
--rw-r--r--   0        0        0    10150 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ba_4.gds
--rw-r--r--   0        0        0     6500 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21bai_1.gds
--rw-r--r--   0        0        0     7722 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21bai_2.gds
--rw-r--r--   0        0        0    12418 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21bai_4.gds
--rw-r--r--   0        0        0     8082 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221a_1.gds
--rw-r--r--   0        0        0     8466 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221a_2.gds
--rw-r--r--   0        0        0    13182 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221a_4.gds
--rw-r--r--   0        0        0     7598 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221ai_1.gds
--rw-r--r--   0        0        0    10328 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221ai_2.gds
--rw-r--r--   0        0        0    16248 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221ai_4.gds
--rw-r--r--   0        0        0     7682 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22a_1.gds
--rw-r--r--   0        0        0     7254 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22a_2.gds
--rw-r--r--   0        0        0    11140 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22a_4.gds
--rw-r--r--   0        0        0     5812 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22ai_1.gds
--rw-r--r--   0        0        0     8818 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22ai_2.gds
--rw-r--r--   0        0        0    12830 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22ai_4.gds
--rw-r--r--   0        0        0     8008 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_1.gds
--rw-r--r--   0        0        0     8186 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_2.gds
--rw-r--r--   0        0        0    11528 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_4.gds
--rw-r--r--   0        0        0     6734 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_1.gds
--rw-r--r--   0        0        0     9994 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_2.gds
--rw-r--r--   0        0        0    17300 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_4.gds
--rw-r--r--   0        0        0     7984 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311a_1.gds
--rw-r--r--   0        0        0     8108 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311a_2.gds
--rw-r--r--   0        0        0    13778 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311a_4.gds
--rw-r--r--   0        0        0     6910 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311ai_1.gds
--rw-r--r--   0        0        0    10888 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311ai_2.gds
--rw-r--r--   0        0        0    17046 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311ai_4.gds
--rw-r--r--   0        0        0     6498 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31a_1.gds
--rw-r--r--   0        0        0     6946 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31a_2.gds
--rw-r--r--   0        0        0    12418 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31a_4.gds
--rw-r--r--   0        0        0     6304 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31ai_1.gds
--rw-r--r--   0        0        0     8912 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31ai_2.gds
--rw-r--r--   0        0        0    13844 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31ai_4.gds
--rw-r--r--   0        0        0     7216 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32a_1.gds
--rw-r--r--   0        0        0     8472 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32a_2.gds
--rw-r--r--   0        0        0    12894 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32a_4.gds
--rw-r--r--   0        0        0     6812 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32ai_1.gds
--rw-r--r--   0        0        0    11062 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32ai_2.gds
--rw-r--r--   0        0        0    18084 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32ai_4.gds
--rw-r--r--   0        0        0     8404 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41a_1.gds
--rw-r--r--   0        0        0     8856 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41a_2.gds
--rw-r--r--   0        0        0    13274 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41a_4.gds
--rw-r--r--   0        0        0     6892 2023-08-13 15:12:40.075614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41ai_1.gds
--rw-r--r--   0        0        0    10848 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41ai_2.gds
--rw-r--r--   0        0        0    16862 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41ai_4.gds
--rw-r--r--   0        0        0     4900 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2_1.gds
--rw-r--r--   0        0        0     5454 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2_2.gds
--rw-r--r--   0        0        0     7446 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2_4.gds
--rw-r--r--   0        0        0     6072 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2b_1.gds
--rw-r--r--   0        0        0     5786 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2b_2.gds
--rw-r--r--   0        0        0    10298 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2b_4.gds
--rw-r--r--   0        0        0     5396 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3_1.gds
--rw-r--r--   0        0        0     6622 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3_2.gds
--rw-r--r--   0        0        0     9566 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3_4.gds
--rw-r--r--   0        0        0     7346 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3b_1.gds
--rw-r--r--   0        0        0     6502 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3b_2.gds
--rw-r--r--   0        0        0    10324 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3b_4.gds
--rw-r--r--   0        0        0     6160 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4_1.gds
--rw-r--r--   0        0        0     7558 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4_2.gds
--rw-r--r--   0        0        0    11670 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4_4.gds
--rw-r--r--   0        0        0     7616 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4b_1.gds
--rw-r--r--   0        0        0     7568 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4b_2.gds
--rw-r--r--   0        0        0    12512 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4b_4.gds
--rw-r--r--   0        0        0     8468 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4bb_1.gds
--rw-r--r--   0        0        0     8202 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4bb_2.gds
--rw-r--r--   0        0        0    12948 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4bb_4.gds
--rw-r--r--   0        0        0    24580 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfbbn_1.gds
--rw-r--r--   0        0        0    26280 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfbbn_2.gds
--rw-r--r--   0        0        0    23670 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfbbp_1.gds
--rw-r--r--   0        0        0    21900 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrbp_1.gds
--rw-r--r--   0        0        0    21876 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrbp_2.gds
--rw-r--r--   0        0        0    20580 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrtn_1.gds
--rw-r--r--   0        0        0    20632 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_1.gds
--rw-r--r--   0        0        0    21136 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_2.gds
--rw-r--r--   0        0        0    21380 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_4.gds
--rw-r--r--   0        0        0    21582 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfsbp_1.gds
--rw-r--r--   0        0        0    25042 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfsbp_2.gds
--rw-r--r--   0        0        0    20846 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfstp_1.gds
--rw-r--r--   0        0        0    21784 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfstp_2.gds
--rw-r--r--   0        0        0    23098 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfstp_4.gds
--rw-r--r--   0        0        0    19098 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfxbp_1.gds
--rw-r--r--   0        0        0    19818 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfxbp_2.gds
--rw-r--r--   0        0        0    16784 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_1.gds
--rw-r--r--   0        0        0    17176 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_2.gds
--rw-r--r--   0        0        0    17596 2023-08-13 15:12:40.079614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_4.gds
--rw-r--r--   0        0        0    11910 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_1.gds
--rw-r--r--   0        0        0    12598 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_2.gds
--rw-r--r--   0        0        0    13494 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_4.gds
--rw-r--r--   0        0        0    22998 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sedfxbp_1.gds
--rw-r--r--   0        0        0    24322 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sedfxbp_2.gds
--rw-r--r--   0        0        0    22398 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_1.gds
--rw-r--r--   0        0        0    22344 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_2.gds
--rw-r--r--   0        0        0    23366 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_4.gds
--rw-r--r--   0        0        0     2830 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tap_1.gds
--rw-r--r--   0        0        0     3982 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tap_2.gds
--rw-r--r--   0        0        0     2962 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tapmet1_2.gds
--rw-r--r--   0        0        0     2040 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tapvgnd2_1.gds
--rw-r--r--   0        0        0     2038 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tapvgnd_1.gds
--rw-r--r--   0        0        0     1758 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tapvpwrvgnd_1.gds
--rw-r--r--   0        0        0     6092 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor2_1.gds
--rw-r--r--   0        0        0     8426 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor2_2.gds
--rw-r--r--   0        0        0    13058 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor2_4.gds
--rw-r--r--   0        0        0    12680 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor3_1.gds
--rw-r--r--   0        0        0    13416 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor3_2.gds
--rw-r--r--   0        0        0    15998 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor3_4.gds
--rw-r--r--   0        0        0     6424 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor2_1.gds
--rw-r--r--   0        0        0     7828 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor2_2.gds
--rw-r--r--   0        0        0    12988 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor2_4.gds
--rw-r--r--   0        0        0    14044 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor3_1.gds
--rw-r--r--   0        0        0    14716 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor3_2.gds
--rw-r--r--   0        0        0    15794 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor3_4.gds
--rw-r--r--   0        0        0    11766 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__a21o_1.gds
--rw-r--r--   0        0        0     9658 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__a21oi_1.gds
--rw-r--r--   0        0        0    13980 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__a22o_1.gds
--rw-r--r--   0        0        0    10616 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__a22oi_1.gds
--rw-r--r--   0        0        0     9098 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__and2_1.gds
--rw-r--r--   0        0        0    10302 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__and3_1.gds
--rw-r--r--   0        0        0     7688 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_1.gds
--rw-r--r--   0        0        0    39408 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_16.gds
--rw-r--r--   0        0        0     8694 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_2.gds
--rw-r--r--   0        0        0    59888 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_32.gds
--rw-r--r--   0        0        0    11338 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_4.gds
--rw-r--r--   0        0        0    20202 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_8.gds
--rw-r--r--   0        0        0     6942 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__conb_1.gds
--rw-r--r--   0        0        0     4884 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__decap_4.gds
--rw-r--r--   0        0        0     6964 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__decap_8.gds
--rw-r--r--   0        0        0    31398 2023-08-13 15:12:40.083614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfrbp_1.gds
--rw-r--r--   0        0        0    29300 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfrtp_1.gds
--rw-r--r--   0        0        0    33566 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfsbp_1.gds
--rw-r--r--   0        0        0    29300 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfstp_1.gds
--rw-r--r--   0        0        0    28546 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfxbp_1.gds
--rw-r--r--   0        0        0    24170 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfxtp_1.gds
--rw-r--r--   0        0        0     5168 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__diode_2.gds
--rw-r--r--   0        0        0    24070 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dlclkp_1.gds
--rw-r--r--   0        0        0    19870 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dlrtp_1.gds
--rw-r--r--   0        0        0    16574 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dlxtp_1.gds
--rw-r--r--   0        0        0     9902 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__einvn_1.gds
--rw-r--r--   0        0        0     9690 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__einvp_1.gds
--rw-r--r--   0        0        0     2512 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__fill_1.gds
--rw-r--r--   0        0        0     2896 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__fill_2.gds
--rw-r--r--   0        0        0     3664 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__fill_4.gds
--rw-r--r--   0        0        0     5200 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__fill_8.gds
--rw-r--r--   0        0        0     5838 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__inv_1.gds
--rw-r--r--   0        0        0    29772 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__inv_16.gds
--rw-r--r--   0        0        0     7110 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__inv_2.gds
--rw-r--r--   0        0        0    10288 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__inv_4.gds
--rw-r--r--   0        0        0    17150 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__inv_8.gds
--rw-r--r--   0        0        0    12836 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2hv_hl_1.gds
--rw-r--r--   0        0        0    21610 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2hv_lh_1.gds
--rw-r--r--   0        0        0    18828 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2lv_1.gds
--rw-r--r--   0        0        0    13082 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2lv_simple_1.gds
--rw-r--r--   0        0        0    23376 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_1.gds
--rw-r--r--   0        0        0    53092 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_clkiso_hlkg_3.gds
--rw-r--r--   0        0        0    29020 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_isosrchvaon_1.gds
--rw-r--r--   0        0        0    23514 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_symmetric_1.gds
--rw-r--r--   0        0        0    12504 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__mux2_1.gds
--rw-r--r--   0        0        0    25182 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__mux4_1.gds
--rw-r--r--   0        0        0     6892 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__nand2_1.gds
--rw-r--r--   0        0        0     9498 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__nand3_1.gds
--rw-r--r--   0        0        0     7454 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__nor2_1.gds
--rw-r--r--   0        0        0     8292 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__nor3_1.gds
--rw-r--r--   0        0        0    11886 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__o21a_1.gds
--rw-r--r--   0        0        0     9088 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__o21ai_1.gds
--rw-r--r--   0        0        0    12868 2023-08-13 15:12:40.087614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__o22a_1.gds
--rw-r--r--   0        0        0     9922 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__o22ai_1.gds
--rw-r--r--   0        0        0     8814 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__or2_1.gds
--rw-r--r--   0        0        0    10460 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__or3_1.gds
--rw-r--r--   0        0        0    20954 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__probe_p_8.gds
--rw-r--r--   0        0        0    23282 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__probec_p_8.gds
--rw-r--r--   0        0        0    11536 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__schmittbuf_1.gds
--rw-r--r--   0        0        0    34228 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfrbp_1.gds
--rw-r--r--   0        0        0    36482 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfrtp_1.gds
--rw-r--r--   0        0        0    38850 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfsbp_1.gds
--rw-r--r--   0        0        0    35086 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfstp_1.gds
--rw-r--r--   0        0        0    37804 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfxbp_1.gds
--rw-r--r--   0        0        0    29122 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfxtp_1.gds
--rw-r--r--   0        0        0    23000 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdlclkp_1.gds
--rw-r--r--   0        0        0    24080 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdlxtp_1.gds
--rw-r--r--   0        0        0    12322 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__xnor2_1.gds
--rw-r--r--   0        0        0    12192 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__xor2_1.gds
--rw-r--r--   0        0        0     3411 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/klayout/grain.xml
--rw-r--r--   0        0        0   231824 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/klayout/layers.lyp
--rw-r--r--   0        0        0    75766 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/klayout/layers.yaml
--rw-r--r--   0        0        0     5937 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/klayout/pymacros/klayout_Library.lym
--rw-r--r--   0        0        0      697 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/klayout/pymacros/set_menus.lym
--rw-r--r--   0        0        0     6801 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/klayout/sky130.lyt
--rw-r--r--   0        0        0     7117 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/klayout/sky130.xs
--rw-r--r--   0        0        0    13414 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/klayout/sky130_xs.lyp
--rw-r--r--   0        0        0     2156 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/klayout/sky_x64.png
--rw-r--r--   0        0        0     7646 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/klayout/tech.lyt
--rw-r--r--   0        0        0    21395 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/layers.py
--rw-r--r--   0        0        0     2419 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/nmos.py
--rw-r--r--   0        0        0      705 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/__init__.py
--rw-r--r--   0        0        0     4411 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/mimcap_1.py
--rw-r--r--   0        0        0     3556 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/mimcap_2.py
--rw-r--r--   0        0        0    15422 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/nmos.py
--rw-r--r--   0        0        0    14299 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/nmos_5v.py
--rw-r--r--   0        0        0    23719 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/npn_W1L1.py
--rw-r--r--   0        0        0    24647 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/npn_W1L2.py
--rw-r--r--   0        0        0     6875 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/p_n_poly.py
--rw-r--r--   0        0        0     6878 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/p_p_poly.py
--rw-r--r--   0        0        0    15208 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/pmos.py
--rw-r--r--   0        0        0    13696 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/pmos_5v.py
--rw-r--r--   0        0        0    23889 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/pnp.py
--rw-r--r--   0        0        0     5207 2023-08-13 15:12:40.091614 sky130-0.8.0/sky130/pcells/via_generator.py
--rw-r--r--   0        0        0   926242 2023-08-13 15:12:40.095615 sky130-0.8.0/sky130/spice/sky130_fd_sc_hd.spice
--rwxr-xr-x   0        0        0   967549 2023-08-13 15:12:40.099614 sky130-0.8.0/sky130/spice/sky130_fd_sc_hs.spice
--rw-r--r--   0        0        0   140107 2023-08-13 15:12:40.099614 sky130-0.8.0/sky130/spice/sky130_fd_sc_hvl.spice
--rw-r--r--   0        0        0    72993 2023-08-13 15:12:40.099614 sky130-0.8.0/sky130/spice_models.py
--rw-r--r--   0        0        0      456 2023-08-13 15:12:40.099614 sky130-0.8.0/sky130/tech.py
--rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 sky130-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-11-18 19:15:28.736098 sky130-0.9.0/LICENSE
+-rw-r--r--   0        0        0      760 2023-11-18 19:15:28.736098 sky130-0.9.0/README.md
+-rw-r--r--   0        0        0     3895 2023-11-18 19:15:28.740098 sky130-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1106 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/__init__.py
+-rw-r--r--   0        0        0      422 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/circuits/sample.pic.yml
+-rw-r--r--   0        0        0   273948 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/components.py
+-rw-r--r--   0        0        0     1069 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/config.py
+-rw-r--r--   0        0        0     8838 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111o_1.gds
+-rw-r--r--   0        0        0     9206 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111o_2.gds
+-rw-r--r--   0        0        0    12500 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111o_4.gds
+-rw-r--r--   0        0        0     7594 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111oi_0.gds
+-rw-r--r--   0        0        0     7928 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111oi_1.gds
+-rw-r--r--   0        0        0     8374 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111oi_2.gds
+-rw-r--r--   0        0        0    14310 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111oi_4.gds
+-rw-r--r--   0        0        0     6490 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211o_1.gds
+-rw-r--r--   0        0        0     6708 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211o_2.gds
+-rw-r--r--   0        0        0     9204 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211o_4.gds
+-rw-r--r--   0        0        0     6794 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211oi_1.gds
+-rw-r--r--   0        0        0     9088 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211oi_2.gds
+-rw-r--r--   0        0        0    10726 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211oi_4.gds
+-rw-r--r--   0        0        0     7690 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21bo_1.gds
+-rw-r--r--   0        0        0     6440 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21bo_2.gds
+-rw-r--r--   0        0        0     8392 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21bo_4.gds
+-rw-r--r--   0        0        0     5322 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21boi_0.gds
+-rw-r--r--   0        0        0     6382 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21boi_1.gds
+-rw-r--r--   0        0        0     6778 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21boi_2.gds
+-rw-r--r--   0        0        0     9578 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21boi_4.gds
+-rw-r--r--   0        0        0     6134 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21o_1.gds
+-rw-r--r--   0        0        0     5698 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21o_2.gds
+-rw-r--r--   0        0        0     8308 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21o_4.gds
+-rw-r--r--   0        0        0     4814 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21oi_1.gds
+-rw-r--r--   0        0        0     6008 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21oi_2.gds
+-rw-r--r--   0        0        0     8678 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21oi_4.gds
+-rw-r--r--   0        0        0     7276 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221o_1.gds
+-rw-r--r--   0        0        0     7820 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221o_2.gds
+-rw-r--r--   0        0        0    12334 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221o_4.gds
+-rw-r--r--   0        0        0     6716 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221oi_1.gds
+-rw-r--r--   0        0        0     9320 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221oi_2.gds
+-rw-r--r--   0        0        0    13368 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221oi_4.gds
+-rw-r--r--   0        0        0     7222 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a222oi_1.gds
+-rw-r--r--   0        0        0     6732 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22o_1.gds
+-rw-r--r--   0        0        0     6892 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22o_2.gds
+-rw-r--r--   0        0        0     9818 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22o_4.gds
+-rw-r--r--   0        0        0     5758 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22oi_1.gds
+-rw-r--r--   0        0        0     8630 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22oi_2.gds
+-rw-r--r--   0        0        0    12136 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22oi_4.gds
+-rw-r--r--   0        0        0     7314 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_1.gds
+-rw-r--r--   0        0        0     7874 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_2.gds
+-rw-r--r--   0        0        0    11550 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_4.gds
+-rw-r--r--   0        0        0     6994 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_1.gds
+-rw-r--r--   0        0        0     8944 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_2.gds
+-rw-r--r--   0        0        0    14388 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_4.gds
+-rw-r--r--   0        0        0     6652 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311o_1.gds
+-rw-r--r--   0        0        0     7464 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311o_2.gds
+-rw-r--r--   0        0        0    11866 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311o_4.gds
+-rw-r--r--   0        0        0     6300 2023-11-18 19:15:28.740098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311oi_1.gds
+-rw-r--r--   0        0        0    10464 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311oi_2.gds
+-rw-r--r--   0        0        0    15692 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311oi_4.gds
+-rw-r--r--   0        0        0     6630 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31o_1.gds
+-rw-r--r--   0        0        0     6632 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31o_2.gds
+-rw-r--r--   0        0        0    10006 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31o_4.gds
+-rw-r--r--   0        0        0     5390 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31oi_1.gds
+-rw-r--r--   0        0        0     9146 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31oi_2.gds
+-rw-r--r--   0        0        0    13010 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31oi_4.gds
+-rw-r--r--   0        0        0     7518 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32o_1.gds
+-rw-r--r--   0        0        0     8526 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32o_2.gds
+-rw-r--r--   0        0        0    12280 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32o_4.gds
+-rw-r--r--   0        0        0     6110 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32oi_1.gds
+-rw-r--r--   0        0        0    11378 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32oi_2.gds
+-rw-r--r--   0        0        0    16306 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32oi_4.gds
+-rw-r--r--   0        0        0     8026 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41o_1.gds
+-rw-r--r--   0        0        0     8398 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41o_2.gds
+-rw-r--r--   0        0        0    12610 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41o_4.gds
+-rw-r--r--   0        0        0     6866 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41oi_1.gds
+-rw-r--r--   0        0        0    10214 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41oi_2.gds
+-rw-r--r--   0        0        0    16690 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41oi_4.gds
+-rw-r--r--   0        0        0     4566 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2_0.gds
+-rw-r--r--   0        0        0     4986 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2_1.gds
+-rw-r--r--   0        0        0     5530 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2_2.gds
+-rw-r--r--   0        0        0     5830 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2_4.gds
+-rw-r--r--   0        0        0     5620 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2b_1.gds
+-rw-r--r--   0        0        0     5748 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2b_2.gds
+-rw-r--r--   0        0        0     5802 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2b_4.gds
+-rw-r--r--   0        0        0     7250 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3_1.gds
+-rw-r--r--   0        0        0     5956 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3_2.gds
+-rw-r--r--   0        0        0     6980 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3_4.gds
+-rw-r--r--   0        0        0     6486 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3b_1.gds
+-rw-r--r--   0        0        0     6680 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3b_2.gds
+-rw-r--r--   0        0        0     6728 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3b_4.gds
+-rw-r--r--   0        0        0     6498 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4_1.gds
+-rw-r--r--   0        0        0     7362 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4_2.gds
+-rw-r--r--   0        0        0     7534 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4_4.gds
+-rw-r--r--   0        0        0     7698 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4b_1.gds
+-rw-r--r--   0        0        0     8356 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4b_2.gds
+-rw-r--r--   0        0        0     7822 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4b_4.gds
+-rw-r--r--   0        0        0     8486 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4bb_1.gds
+-rw-r--r--   0        0        0     8082 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4bb_2.gds
+-rw-r--r--   0        0        0     8804 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4bb_4.gds
+-rw-r--r--   0        0        0     4050 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_1.gds
+-rw-r--r--   0        0        0    11278 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_12.gds
+-rw-r--r--   0        0        0    15620 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_16.gds
+-rw-r--r--   0        0        0     4578 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_2.gds
+-rw-r--r--   0        0        0     5490 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_4.gds
+-rw-r--r--   0        0        0     7120 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_6.gds
+-rw-r--r--   0        0        0     8974 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_8.gds
+-rw-r--r--   0        0        0    18348 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__bufbuf_16.gds
+-rw-r--r--   0        0        0    10618 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__bufbuf_8.gds
+-rw-r--r--   0        0        0    16972 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__bufinv_16.gds
+-rw-r--r--   0        0        0    10298 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__bufinv_8.gds
+-rw-r--r--   0        0        0     3896 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkbuf_1.gds
+-rw-r--r--   0        0        0    12806 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkbuf_16.gds
+-rw-r--r--   0        0        0     4680 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkbuf_2.gds
+-rw-r--r--   0        0        0     5302 2023-11-18 19:15:28.744098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkbuf_4.gds
+-rw-r--r--   0        0        0     7900 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkbuf_8.gds
+-rw-r--r--   0        0        0     6272 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s15_1.gds
+-rw-r--r--   0        0        0     6718 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s15_2.gds
+-rw-r--r--   0        0        0     6380 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s18_1.gds
+-rw-r--r--   0        0        0     6262 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s18_2.gds
+-rw-r--r--   0        0        0     6272 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s25_1.gds
+-rw-r--r--   0        0        0     6764 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s25_2.gds
+-rw-r--r--   0        0        0     6304 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s50_1.gds
+-rw-r--r--   0        0        0     6752 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s50_2.gds
+-rw-r--r--   0        0        0     3920 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinv_1.gds
+-rw-r--r--   0        0        0    13134 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinv_16.gds
+-rw-r--r--   0        0        0     4388 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinv_2.gds
+-rw-r--r--   0        0        0     5952 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinv_4.gds
+-rw-r--r--   0        0        0     9336 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinv_8.gds
+-rw-r--r--   0        0        0     3738 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinvlp_2.gds
+-rw-r--r--   0        0        0     5188 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinvlp_4.gds
+-rw-r--r--   0        0        0     6766 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__conb_1.gds
+-rw-r--r--   0        0        0     4224 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__decap_12.gds
+-rw-r--r--   0        0        0     2750 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__decap_3.gds
+-rw-r--r--   0        0        0     2878 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__decap_4.gds
+-rw-r--r--   0        0        0     3230 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__decap_6.gds
+-rw-r--r--   0        0        0     3614 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__decap_8.gds
+-rw-r--r--   0        0        0    19682 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfbbn_1.gds
+-rw-r--r--   0        0        0    20130 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfbbn_2.gds
+-rw-r--r--   0        0        0    19150 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfbbp_1.gds
+-rw-r--r--   0        0        0    17770 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrbp_1.gds
+-rw-r--r--   0        0        0    18498 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrbp_2.gds
+-rw-r--r--   0        0        0    15246 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrtn_1.gds
+-rw-r--r--   0        0        0    15372 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrtp_1.gds
+-rw-r--r--   0        0        0    16228 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrtp_2.gds
+-rw-r--r--   0        0        0    18008 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrtp_4.gds
+-rw-r--r--   0        0        0    17898 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfsbp_1.gds
+-rw-r--r--   0        0        0    19000 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfsbp_2.gds
+-rw-r--r--   0        0        0    15674 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfstp_1.gds
+-rw-r--r--   0        0        0    16244 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfstp_2.gds
+-rw-r--r--   0        0        0    17806 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfstp_4.gds
+-rw-r--r--   0        0        0    14106 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfxbp_1.gds
+-rw-r--r--   0        0        0    15214 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfxbp_2.gds
+-rw-r--r--   0        0        0    12206 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfxtp_1.gds
+-rw-r--r--   0        0        0    12638 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfxtp_2.gds
+-rw-r--r--   0        0        0    14238 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfxtp_4.gds
+-rw-r--r--   0        0        0     3586 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__diode_2.gds
+-rw-r--r--   0        0        0    10112 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlclkp_1.gds
+-rw-r--r--   0        0        0    10400 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlclkp_2.gds
+-rw-r--r--   0        0        0    12932 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlclkp_4.gds
+-rw-r--r--   0        0        0    13888 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrbn_1.gds
+-rw-r--r--   0        0        0    13486 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrbn_2.gds
+-rw-r--r--   0        0        0    13368 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrbp_1.gds
+-rw-r--r--   0        0        0    14986 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrbp_2.gds
+-rw-r--r--   0        0        0    11712 2023-11-18 19:15:28.748098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtn_1.gds
+-rw-r--r--   0        0        0    11538 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtn_2.gds
+-rw-r--r--   0        0        0    12858 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtn_4.gds
+-rw-r--r--   0        0        0    10882 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtp_1.gds
+-rw-r--r--   0        0        0    11326 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtp_2.gds
+-rw-r--r--   0        0        0    12854 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtp_4.gds
+-rw-r--r--   0        0        0    13134 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxbn_1.gds
+-rw-r--r--   0        0        0    13000 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxbn_2.gds
+-rw-r--r--   0        0        0    12630 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxbp_1.gds
+-rw-r--r--   0        0        0    10746 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxtn_1.gds
+-rw-r--r--   0        0        0    10216 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxtn_2.gds
+-rw-r--r--   0        0        0    11836 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxtn_4.gds
+-rw-r--r--   0        0        0    10294 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxtp_1.gds
+-rw-r--r--   0        0        0     5552 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd1_1.gds
+-rw-r--r--   0        0        0     6010 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd2_1.gds
+-rw-r--r--   0        0        0     6070 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd3_1.gds
+-rw-r--r--   0        0        0     7928 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s2s_1.gds
+-rw-r--r--   0        0        0     7928 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s4s_1.gds
+-rw-r--r--   0        0        0     7676 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s6s_1.gds
+-rw-r--r--   0        0        0     6962 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ebufn_1.gds
+-rw-r--r--   0        0        0     7340 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ebufn_2.gds
+-rw-r--r--   0        0        0     9578 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ebufn_4.gds
+-rw-r--r--   0        0        0    14044 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ebufn_8.gds
+-rw-r--r--   0        0        0    19118 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__edfxbp_1.gds
+-rw-r--r--   0        0        0    17568 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__edfxtp_1.gds
+-rw-r--r--   0        0        0     4386 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvn_0.gds
+-rw-r--r--   0        0        0     5210 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvn_1.gds
+-rw-r--r--   0        0        0     6430 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvn_2.gds
+-rw-r--r--   0        0        0     7922 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvn_4.gds
+-rw-r--r--   0        0        0    12408 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvn_8.gds
+-rw-r--r--   0        0        0     4656 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvp_1.gds
+-rw-r--r--   0        0        0     6332 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvp_2.gds
+-rw-r--r--   0        0        0     8108 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvp_4.gds
+-rw-r--r--   0        0        0    12766 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvp_8.gds
+-rw-r--r--   0        0        0    13092 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fa_1.gds
+-rw-r--r--   0        0        0    13746 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fa_2.gds
+-rw-r--r--   0        0        0    15828 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fa_4.gds
+-rw-r--r--   0        0        0    19582 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fah_1.gds
+-rw-r--r--   0        0        0    19430 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fahcin_1.gds
+-rw-r--r--   0        0        0    18950 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fahcon_1.gds
+-rw-r--r--   0        0        0     1384 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fill_1.gds
+-rw-r--r--   0        0        0     1512 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fill_2.gds
+-rw-r--r--   0        0        0     1768 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fill_4.gds
+-rw-r--r--   0        0        0     2280 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fill_8.gds
+-rw-r--r--   0        0        0     9028 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ha_1.gds
+-rw-r--r--   0        0        0     9718 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ha_2.gds
+-rw-r--r--   0        0        0    14160 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ha_4.gds
+-rw-r--r--   0        0        0     3636 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_1.gds
+-rw-r--r--   0        0        0    10452 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_12.gds
+-rw-r--r--   0        0        0    11632 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_16.gds
+-rw-r--r--   0        0        0     7652 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_2.gds
+-rw-r--r--   0        0        0     5132 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_4.gds
+-rw-r--r--   0        0        0     6092 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_6.gds
+-rw-r--r--   0        0        0     7642 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_8.gds
+-rw-r--r--   0        0        0     3134 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_bleeder_1.gds
+-rw-r--r--   0        0        0     4242 2023-11-18 19:15:28.752098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_1.gds
+-rw-r--r--   0        0        0    14752 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_16.gds
+-rw-r--r--   0        0        0     4934 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_2.gds
+-rw-r--r--   0        0        0     6080 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_4.gds
+-rw-r--r--   0        0        0     9014 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_8.gds
+-rw-r--r--   0        0        0     4284 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_1.gds
+-rw-r--r--   0        0        0    15400 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_16.gds
+-rw-r--r--   0        0        0     4862 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_2.gds
+-rw-r--r--   0        0        0     6778 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_4.gds
+-rw-r--r--   0        0        0    10626 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_8.gds
+-rw-r--r--   0        0        0     5274 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_12.gds
+-rw-r--r--   0        0        0     3224 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_3.gds
+-rw-r--r--   0        0        0     3416 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_4.gds
+-rw-r--r--   0        0        0     3896 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_6.gds
+-rw-r--r--   0        0        0     4408 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_8.gds
+-rw-r--r--   0        0        0     5018 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso0n_1.gds
+-rw-r--r--   0        0        0     5650 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso0p_1.gds
+-rw-r--r--   0        0        0     5062 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso1n_1.gds
+-rw-r--r--   0        0        0     4340 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso1p_1.gds
+-rw-r--r--   0        0        0     9080 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputisolatch_1.gds
+-rw-r--r--   0        0        0     4422 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_1.gds
+-rw-r--r--   0        0        0    23764 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_16.gds
+-rw-r--r--   0        0        0     6098 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_2.gds
+-rw-r--r--   0        0        0     8674 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_4.gds
+-rw-r--r--   0        0        0    13458 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_8.gds
+-rw-r--r--   0        0        0    22078 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrckapwr_16.gds
+-rw-r--r--   0        0        0    13400 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_1.gds
+-rw-r--r--   0        0        0    13432 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_2.gds
+-rw-r--r--   0        0        0    14664 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_4.gds
+-rw-r--r--   0        0        0    13068 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_4.gds
+-rw-r--r--   0        0        0    13396 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_1.gds
+-rw-r--r--   0        0        0    13428 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_2.gds
+-rw-r--r--   0        0        0    14660 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_4.gds
+-rw-r--r--   0        0        0     4066 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__macro_sparecell.gds
+-rw-r--r--   0        0        0     6268 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__maj3_1.gds
+-rw-r--r--   0        0        0     6592 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__maj3_2.gds
+-rw-r--r--   0        0        0     8014 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__maj3_4.gds
+-rw-r--r--   0        0        0     6972 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2_1.gds
+-rw-r--r--   0        0        0     7334 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2_2.gds
+-rw-r--r--   0        0        0     8478 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2_4.gds
+-rw-r--r--   0        0        0    12804 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2_8.gds
+-rw-r--r--   0        0        0     7040 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2i_1.gds
+-rw-r--r--   0        0        0     8158 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2i_2.gds
+-rw-r--r--   0        0        0    12286 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2i_4.gds
+-rw-r--r--   0        0        0    15620 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux4_1.gds
+-rw-r--r--   0        0        0    14382 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux4_2.gds
+-rw-r--r--   0        0        0    15752 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux4_4.gds
+-rw-r--r--   0        0        0     4036 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2_1.gds
+-rw-r--r--   0        0        0    10118 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2_2.gds
+-rw-r--r--   0        0        0     7726 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2_4.gds
+-rw-r--r--   0        0        0    12436 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2_8.gds
+-rw-r--r--   0        0        0     4676 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2b_1.gds
+-rw-r--r--   0        0        0     6708 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2b_2.gds
+-rw-r--r--   0        0        0     9202 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2b_4.gds
+-rw-r--r--   0        0        0     4486 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3_1.gds
+-rw-r--r--   0        0        0     7370 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3_2.gds
+-rw-r--r--   0        0        0    11280 2023-11-18 19:15:28.756098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3_4.gds
+-rw-r--r--   0        0        0     5680 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3b_1.gds
+-rw-r--r--   0        0        0     7094 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3b_2.gds
+-rw-r--r--   0        0        0    11932 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3b_4.gds
+-rw-r--r--   0        0        0     5348 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4_1.gds
+-rw-r--r--   0        0        0     8872 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4_2.gds
+-rw-r--r--   0        0        0    13550 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4_4.gds
+-rw-r--r--   0        0        0     5960 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4b_1.gds
+-rw-r--r--   0        0        0    10202 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4b_2.gds
+-rw-r--r--   0        0        0    15074 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4b_4.gds
+-rw-r--r--   0        0        0     7302 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4bb_1.gds
+-rw-r--r--   0        0        0    10534 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4bb_2.gds
+-rw-r--r--   0        0        0    15134 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4bb_4.gds
+-rw-r--r--   0        0        0     3750 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2_1.gds
+-rw-r--r--   0        0        0     9642 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2_2.gds
+-rw-r--r--   0        0        0     7190 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2_4.gds
+-rw-r--r--   0        0        0    11542 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2_8.gds
+-rw-r--r--   0        0        0     4398 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2b_1.gds
+-rw-r--r--   0        0        0     6074 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2b_2.gds
+-rw-r--r--   0        0        0     8650 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2b_4.gds
+-rw-r--r--   0        0        0     4324 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3_1.gds
+-rw-r--r--   0        0        0     6692 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3_2.gds
+-rw-r--r--   0        0        0     9460 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3_4.gds
+-rw-r--r--   0        0        0     4888 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3b_1.gds
+-rw-r--r--   0        0        0     7960 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3b_2.gds
+-rw-r--r--   0        0        0    10244 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3b_4.gds
+-rw-r--r--   0        0        0     4864 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4_1.gds
+-rw-r--r--   0        0        0     7794 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4_2.gds
+-rw-r--r--   0        0        0    12462 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4_4.gds
+-rw-r--r--   0        0        0     5350 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4b_1.gds
+-rw-r--r--   0        0        0     9414 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4b_2.gds
+-rw-r--r--   0        0        0    13638 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4b_4.gds
+-rw-r--r--   0        0        0     6506 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4bb_1.gds
+-rw-r--r--   0        0        0     9470 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4bb_2.gds
+-rw-r--r--   0        0        0    13670 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4bb_4.gds
+-rw-r--r--   0        0        0     8548 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111a_1.gds
+-rw-r--r--   0        0        0     8254 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111a_2.gds
+-rw-r--r--   0        0        0    11072 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111a_4.gds
+-rw-r--r--   0        0        0     6182 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111ai_1.gds
+-rw-r--r--   0        0        0     9610 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111ai_2.gds
+-rw-r--r--   0        0        0    15556 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111ai_4.gds
+-rw-r--r--   0        0        0     6928 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211a_1.gds
+-rw-r--r--   0        0        0     6468 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211a_2.gds
+-rw-r--r--   0        0        0     9140 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211a_4.gds
+-rw-r--r--   0        0        0     5542 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211ai_1.gds
+-rw-r--r--   0        0        0     7542 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211ai_2.gds
+-rw-r--r--   0        0        0    10166 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211ai_4.gds
+-rw-r--r--   0        0        0     5716 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21a_1.gds
+-rw-r--r--   0        0        0     5652 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21a_2.gds
+-rw-r--r--   0        0        0     8068 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21a_4.gds
+-rw-r--r--   0        0        0     4406 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ai_0.gds
+-rw-r--r--   0        0        0     4862 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ai_1.gds
+-rw-r--r--   0        0        0     6588 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ai_2.gds
+-rw-r--r--   0        0        0     8198 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ai_4.gds
+-rw-r--r--   0        0        0     6248 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ba_1.gds
+-rw-r--r--   0        0        0     6432 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ba_2.gds
+-rw-r--r--   0        0        0     9144 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ba_4.gds
+-rw-r--r--   0        0        0     5658 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21bai_1.gds
+-rw-r--r--   0        0        0     7202 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21bai_2.gds
+-rw-r--r--   0        0        0    10954 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21bai_4.gds
+-rw-r--r--   0        0        0     7374 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221a_1.gds
+-rw-r--r--   0        0        0     7620 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221a_2.gds
+-rw-r--r--   0        0        0    10954 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221a_4.gds
+-rw-r--r--   0        0        0     6552 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221ai_1.gds
+-rw-r--r--   0        0        0     8812 2023-11-18 19:15:28.760098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221ai_2.gds
+-rw-r--r--   0        0        0    13560 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221ai_4.gds
+-rw-r--r--   0        0        0     6162 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22a_1.gds
+-rw-r--r--   0        0        0     6738 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22a_2.gds
+-rw-r--r--   0        0        0     9770 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22a_4.gds
+-rw-r--r--   0        0        0     4980 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22ai_1.gds
+-rw-r--r--   0        0        0     8020 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22ai_2.gds
+-rw-r--r--   0        0        0    10748 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22ai_4.gds
+-rw-r--r--   0        0        0     6538 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_1.gds
+-rw-r--r--   0        0        0     7194 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_2.gds
+-rw-r--r--   0        0        0    11278 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_4.gds
+-rw-r--r--   0        0        0     6316 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_1.gds
+-rw-r--r--   0        0        0     8644 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_2.gds
+-rw-r--r--   0        0        0    14908 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_4.gds
+-rw-r--r--   0        0        0     7760 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311a_1.gds
+-rw-r--r--   0        0        0     8494 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311a_2.gds
+-rw-r--r--   0        0        0    12436 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311a_4.gds
+-rw-r--r--   0        0        0     7572 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311ai_0.gds
+-rw-r--r--   0        0        0     6994 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311ai_1.gds
+-rw-r--r--   0        0        0    10542 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311ai_2.gds
+-rw-r--r--   0        0        0    15998 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311ai_4.gds
+-rw-r--r--   0        0        0     6708 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31a_1.gds
+-rw-r--r--   0        0        0     7410 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31a_2.gds
+-rw-r--r--   0        0        0    11256 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31a_4.gds
+-rw-r--r--   0        0        0     6418 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31ai_1.gds
+-rw-r--r--   0        0        0     9072 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31ai_2.gds
+-rw-r--r--   0        0        0    14628 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31ai_4.gds
+-rw-r--r--   0        0        0     7188 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32a_1.gds
+-rw-r--r--   0        0        0     7878 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32a_2.gds
+-rw-r--r--   0        0        0    12392 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32a_4.gds
+-rw-r--r--   0        0        0     6820 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32ai_1.gds
+-rw-r--r--   0        0        0    10070 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32ai_2.gds
+-rw-r--r--   0        0        0    16122 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32ai_4.gds
+-rw-r--r--   0        0        0     8298 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41a_1.gds
+-rw-r--r--   0        0        0     9224 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41a_2.gds
+-rw-r--r--   0        0        0    13248 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41a_4.gds
+-rw-r--r--   0        0        0     7390 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41ai_1.gds
+-rw-r--r--   0        0        0    11188 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41ai_2.gds
+-rw-r--r--   0        0        0    18202 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41ai_4.gds
+-rw-r--r--   0        0        0     4036 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2_0.gds
+-rw-r--r--   0        0        0     4308 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2_1.gds
+-rw-r--r--   0        0        0     4500 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2_2.gds
+-rw-r--r--   0        0        0     5844 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2_4.gds
+-rw-r--r--   0        0        0     5032 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2b_1.gds
+-rw-r--r--   0        0        0     5608 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2b_2.gds
+-rw-r--r--   0        0        0     6920 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2b_4.gds
+-rw-r--r--   0        0        0     5212 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3_1.gds
+-rw-r--r--   0        0        0     5756 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3_2.gds
+-rw-r--r--   0        0        0     7200 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3_4.gds
+-rw-r--r--   0        0        0     6350 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3b_1.gds
+-rw-r--r--   0        0        0     5934 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3b_2.gds
+-rw-r--r--   0        0        0     6578 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3b_4.gds
+-rw-r--r--   0        0        0     6164 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4_1.gds
+-rw-r--r--   0        0        0     6692 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4_2.gds
+-rw-r--r--   0        0        0     7388 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4_4.gds
+-rw-r--r--   0        0        0     7368 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4b_1.gds
+-rw-r--r--   0        0        0     6638 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4b_2.gds
+-rw-r--r--   0        0        0     8576 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4b_4.gds
+-rw-r--r--   0        0        0     7192 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4bb_1.gds
+-rw-r--r--   0        0        0     7752 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4bb_2.gds
+-rw-r--r--   0        0        0     8902 2023-11-18 19:15:28.764098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4bb_4.gds
+-rw-r--r--   0        0        0    10154 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__probe_p_8.gds
+-rw-r--r--   0        0        0    12944 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__probec_p_8.gds
+-rw-r--r--   0        0        0    23076 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfbbn_1.gds
+-rw-r--r--   0        0        0    23508 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfbbn_2.gds
+-rw-r--r--   0        0        0    22448 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfbbp_1.gds
+-rw-r--r--   0        0        0    21054 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrbp_1.gds
+-rw-r--r--   0        0        0    20788 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrbp_2.gds
+-rw-r--r--   0        0        0    18978 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrtn_1.gds
+-rw-r--r--   0        0        0    18974 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_1.gds
+-rw-r--r--   0        0        0    19486 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_2.gds
+-rw-r--r--   0        0        0    20574 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_4.gds
+-rw-r--r--   0        0        0    21818 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfsbp_1.gds
+-rw-r--r--   0        0        0    22778 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfsbp_2.gds
+-rw-r--r--   0        0        0    19738 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfstp_1.gds
+-rw-r--r--   0        0        0    20650 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfstp_2.gds
+-rw-r--r--   0        0        0    21592 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfstp_4.gds
+-rw-r--r--   0        0        0    17148 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfxbp_1.gds
+-rw-r--r--   0        0        0    18028 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfxbp_2.gds
+-rw-r--r--   0        0        0    15352 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_1.gds
+-rw-r--r--   0        0        0    15944 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_2.gds
+-rw-r--r--   0        0        0    16604 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_4.gds
+-rw-r--r--   0        0        0    11122 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_1.gds
+-rw-r--r--   0        0        0    11746 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_2.gds
+-rw-r--r--   0        0        0    13554 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_4.gds
+-rw-r--r--   0        0        0    22832 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sedfxbp_1.gds
+-rw-r--r--   0        0        0    23984 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sedfxbp_2.gds
+-rw-r--r--   0        0        0    21282 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_1.gds
+-rw-r--r--   0        0        0    21858 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_2.gds
+-rw-r--r--   0        0        0    23010 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_4.gds
+-rw-r--r--   0        0        0     1958 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__tap_1.gds
+-rw-r--r--   0        0        0     2406 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__tap_2.gds
+-rw-r--r--   0        0        0     1968 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__tapvgnd2_1.gds
+-rw-r--r--   0        0        0     1966 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__tapvgnd_1.gds
+-rw-r--r--   0        0        0     1758 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__tapvpwrvgnd_1.gds
+-rw-r--r--   0        0        0     5448 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor2_1.gds
+-rw-r--r--   0        0        0     8824 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor2_2.gds
+-rw-r--r--   0        0        0    14184 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor2_4.gds
+-rw-r--r--   0        0        0    11750 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor3_1.gds
+-rw-r--r--   0        0        0    12322 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor3_2.gds
+-rw-r--r--   0        0        0    13330 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor3_4.gds
+-rw-r--r--   0        0        0     5526 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor2_1.gds
+-rw-r--r--   0        0        0     9222 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor2_2.gds
+-rw-r--r--   0        0        0    14550 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor2_4.gds
+-rw-r--r--   0        0        0    11956 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor3_1.gds
+-rw-r--r--   0        0        0    12450 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor3_2.gds
+-rw-r--r--   0        0        0    13442 2023-11-18 19:15:28.768098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor3_4.gds
+-rw-r--r--   0        0        0     9062 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111o_1.gds
+-rw-r--r--   0        0        0     9080 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111o_2.gds
+-rw-r--r--   0        0        0    13964 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111o_4.gds
+-rw-r--r--   0        0        0     6816 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111oi_1.gds
+-rw-r--r--   0        0        0    10046 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111oi_2.gds
+-rw-r--r--   0        0        0    16246 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111oi_4.gds
+-rw-r--r--   0        0        0     7314 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211o_1.gds
+-rw-r--r--   0        0        0     7536 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211o_2.gds
+-rw-r--r--   0        0        0    11728 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211o_4.gds
+-rw-r--r--   0        0        0     5798 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211oi_1.gds
+-rw-r--r--   0        0        0     9072 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211oi_2.gds
+-rw-r--r--   0        0        0    14822 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211oi_4.gds
+-rw-r--r--   0        0        0     7384 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21bo_1.gds
+-rw-r--r--   0        0        0     6860 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21bo_2.gds
+-rw-r--r--   0        0        0    10170 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21bo_4.gds
+-rw-r--r--   0        0        0     6936 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21boi_1.gds
+-rw-r--r--   0        0        0     8126 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21boi_2.gds
+-rw-r--r--   0        0        0    13102 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21boi_4.gds
+-rw-r--r--   0        0        0     6532 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21o_1.gds
+-rw-r--r--   0        0        0     7074 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21o_2.gds
+-rw-r--r--   0        0        0     9972 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21o_4.gds
+-rw-r--r--   0        0        0     5046 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21oi_1.gds
+-rw-r--r--   0        0        0     7058 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21oi_2.gds
+-rw-r--r--   0        0        0    10398 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21oi_4.gds
+-rw-r--r--   0        0        0     8604 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221o_1.gds
+-rw-r--r--   0        0        0     8450 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221o_2.gds
+-rw-r--r--   0        0        0    13584 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221o_4.gds
+-rw-r--r--   0        0        0     7992 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221oi_1.gds
+-rw-r--r--   0        0        0    10096 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221oi_2.gds
+-rw-r--r--   0        0        0    18014 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221oi_4.gds
+-rw-r--r--   0        0        0     9100 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a222o_1.gds
+-rw-r--r--   0        0        0     8818 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a222o_2.gds
+-rw-r--r--   0        0        0     8968 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a222oi_1.gds
+-rw-r--r--   0        0        0    11714 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a222oi_2.gds
+-rw-r--r--   0        0        0     7592 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22o_1.gds
+-rw-r--r--   0        0        0     7360 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22o_2.gds
+-rw-r--r--   0        0        0    11488 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22o_4.gds
+-rw-r--r--   0        0        0     5858 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22oi_1.gds
+-rw-r--r--   0        0        0     8374 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22oi_2.gds
+-rw-r--r--   0        0        0    13672 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22oi_4.gds
+-rw-r--r--   0        0        0     8276 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_1.gds
+-rw-r--r--   0        0        0     8708 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_2.gds
+-rw-r--r--   0        0        0    11684 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_4.gds
+-rw-r--r--   0        0        0     6766 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_1.gds
+-rw-r--r--   0        0        0     9084 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_2.gds
+-rw-r--r--   0        0        0    14706 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_4.gds
+-rw-r--r--   0        0        0     7712 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311o_1.gds
+-rw-r--r--   0        0        0     7348 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311o_2.gds
+-rw-r--r--   0        0        0    12498 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311o_4.gds
+-rw-r--r--   0        0        0     6622 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311oi_1.gds
+-rw-r--r--   0        0        0    10382 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311oi_2.gds
+-rw-r--r--   0        0        0    16532 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311oi_4.gds
+-rw-r--r--   0        0        0     7150 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31o_1.gds
+-rw-r--r--   0        0        0     7138 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31o_2.gds
+-rw-r--r--   0        0        0    12970 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31o_4.gds
+-rw-r--r--   0        0        0     6208 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31oi_1.gds
+-rw-r--r--   0        0        0     8372 2023-11-18 19:15:28.772098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31oi_2.gds
+-rw-r--r--   0        0        0    14192 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31oi_4.gds
+-rw-r--r--   0        0        0     7170 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32o_1.gds
+-rw-r--r--   0        0        0     7108 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32o_2.gds
+-rw-r--r--   0        0        0    13552 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32o_4.gds
+-rw-r--r--   0        0        0     6658 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32oi_1.gds
+-rw-r--r--   0        0        0    10626 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32oi_2.gds
+-rw-r--r--   0        0        0    17348 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32oi_4.gds
+-rw-r--r--   0        0        0     8176 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41o_1.gds
+-rw-r--r--   0        0        0     8876 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41o_2.gds
+-rw-r--r--   0        0        0    13542 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41o_4.gds
+-rw-r--r--   0        0        0     6118 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41oi_1.gds
+-rw-r--r--   0        0        0    10286 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41oi_2.gds
+-rw-r--r--   0        0        0    16672 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41oi_4.gds
+-rw-r--r--   0        0        0     5204 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2_1.gds
+-rw-r--r--   0        0        0     5334 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2_2.gds
+-rw-r--r--   0        0        0     7706 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2_4.gds
+-rw-r--r--   0        0        0     6250 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2b_1.gds
+-rw-r--r--   0        0        0     5582 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2b_2.gds
+-rw-r--r--   0        0        0     8556 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2b_4.gds
+-rw-r--r--   0        0        0     6146 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3_1.gds
+-rw-r--r--   0        0        0     6546 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3_2.gds
+-rw-r--r--   0        0        0    10552 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3_4.gds
+-rw-r--r--   0        0        0     7096 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3b_1.gds
+-rw-r--r--   0        0        0     7872 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3b_2.gds
+-rw-r--r--   0        0        0    10858 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3b_4.gds
+-rw-r--r--   0        0        0     7430 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4_1.gds
+-rw-r--r--   0        0        0     7336 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4_2.gds
+-rw-r--r--   0        0        0    11062 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4_4.gds
+-rw-r--r--   0        0        0     8018 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4b_1.gds
+-rw-r--r--   0        0        0     6730 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4b_2.gds
+-rw-r--r--   0        0        0    11374 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4b_4.gds
+-rw-r--r--   0        0        0     8078 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4bb_1.gds
+-rw-r--r--   0        0        0     8762 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4bb_2.gds
+-rw-r--r--   0        0        0    14658 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4bb_4.gds
+-rw-r--r--   0        0        0     4452 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__buf_1.gds
+-rw-r--r--   0        0        0    18612 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__buf_16.gds
+-rw-r--r--   0        0        0     4822 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__buf_2.gds
+-rw-r--r--   0        0        0     5850 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__buf_4.gds
+-rw-r--r--   0        0        0     9922 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__buf_8.gds
+-rw-r--r--   0        0        0    21314 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__bufbuf_16.gds
+-rw-r--r--   0        0        0    11088 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__bufbuf_8.gds
+-rw-r--r--   0        0        0    20254 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__bufinv_16.gds
+-rw-r--r--   0        0        0     9306 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__bufinv_8.gds
+-rw-r--r--   0        0        0     4930 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkbuf_1.gds
+-rw-r--r--   0        0        0    16060 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkbuf_16.gds
+-rw-r--r--   0        0        0     4300 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkbuf_2.gds
+-rw-r--r--   0        0        0     5630 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkbuf_4.gds
+-rw-r--r--   0        0        0     8876 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkbuf_8.gds
+-rw-r--r--   0        0        0     5952 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd1_1.gds
+-rw-r--r--   0        0        0     5952 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd2_1.gds
+-rw-r--r--   0        0        0     5936 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd3_1.gds
+-rw-r--r--   0        0        0     8112 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd1_1.gds
+-rw-r--r--   0        0        0     8112 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd2_1.gds
+-rw-r--r--   0        0        0     8064 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd3_1.gds
+-rw-r--r--   0        0        0     4134 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkinv_1.gds
+-rw-r--r--   0        0        0    18546 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkinv_16.gds
+-rw-r--r--   0        0        0     4236 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkinv_2.gds
+-rw-r--r--   0        0        0     6184 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkinv_4.gds
+-rw-r--r--   0        0        0    10004 2023-11-18 19:15:28.776098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkinv_8.gds
+-rw-r--r--   0        0        0     4476 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__conb_1.gds
+-rw-r--r--   0        0        0     2994 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__decap_4.gds
+-rw-r--r--   0        0        0     4082 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__decap_8.gds
+-rw-r--r--   0        0        0    20744 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfbbn_1.gds
+-rw-r--r--   0        0        0    21584 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfbbn_2.gds
+-rw-r--r--   0        0        0    20052 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfbbp_1.gds
+-rw-r--r--   0        0        0    17626 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrbp_1.gds
+-rw-r--r--   0        0        0    19776 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrbp_2.gds
+-rw-r--r--   0        0        0    16856 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrtn_1.gds
+-rw-r--r--   0        0        0    16474 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrtp_1.gds
+-rw-r--r--   0        0        0    17522 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrtp_2.gds
+-rw-r--r--   0        0        0    18906 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrtp_4.gds
+-rw-r--r--   0        0        0    18242 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfsbp_1.gds
+-rw-r--r--   0        0        0    19460 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfsbp_2.gds
+-rw-r--r--   0        0        0    17482 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfstp_1.gds
+-rw-r--r--   0        0        0    17252 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfstp_2.gds
+-rw-r--r--   0        0        0    18930 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfstp_4.gds
+-rw-r--r--   0        0        0    15130 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfxbp_1.gds
+-rw-r--r--   0        0        0    16412 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfxbp_2.gds
+-rw-r--r--   0        0        0    12764 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfxtp_1.gds
+-rw-r--r--   0        0        0    13500 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfxtp_2.gds
+-rw-r--r--   0        0        0    14984 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfxtp_4.gds
+-rw-r--r--   0        0        0     3950 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__diode_2.gds
+-rw-r--r--   0        0        0    10900 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlclkp_1.gds
+-rw-r--r--   0        0        0    12624 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlclkp_2.gds
+-rw-r--r--   0        0        0    13088 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlclkp_4.gds
+-rw-r--r--   0        0        0    13742 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrbn_1.gds
+-rw-r--r--   0        0        0    14132 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrbn_2.gds
+-rw-r--r--   0        0        0    12896 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrbp_1.gds
+-rw-r--r--   0        0        0    13922 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrbp_2.gds
+-rw-r--r--   0        0        0    11104 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtn_1.gds
+-rw-r--r--   0        0        0    11760 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtn_2.gds
+-rw-r--r--   0        0        0    14376 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtn_4.gds
+-rw-r--r--   0        0        0    10418 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtp_1.gds
+-rw-r--r--   0        0        0    11154 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtp_2.gds
+-rw-r--r--   0        0        0    13924 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtp_4.gds
+-rw-r--r--   0        0        0    13118 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxbn_1.gds
+-rw-r--r--   0        0        0    13966 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxbn_2.gds
+-rw-r--r--   0        0        0    13180 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxbp_1.gds
+-rw-r--r--   0        0        0    11300 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxtn_1.gds
+-rw-r--r--   0        0        0    11436 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxtn_2.gds
+-rw-r--r--   0        0        0    12508 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxtn_4.gds
+-rw-r--r--   0        0        0    11848 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxtp_1.gds
+-rw-r--r--   0        0        0     6620 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd1_1.gds
+-rw-r--r--   0        0        0     6620 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd2_1.gds
+-rw-r--r--   0        0        0     6588 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd3_1.gds
+-rw-r--r--   0        0        0     8188 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s2s_1.gds
+-rw-r--r--   0        0        0     8236 2023-11-18 19:15:28.780098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s4s_1.gds
+-rw-r--r--   0        0        0     8236 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s6s_1.gds
+-rw-r--r--   0        0        0     6522 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ebufn_1.gds
+-rw-r--r--   0        0        0     7324 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ebufn_2.gds
+-rw-r--r--   0        0        0     9612 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ebufn_4.gds
+-rw-r--r--   0        0        0    14906 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ebufn_8.gds
+-rw-r--r--   0        0        0    20468 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__edfxbp_1.gds
+-rw-r--r--   0        0        0    18594 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__edfxtp_1.gds
+-rw-r--r--   0        0        0     4956 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvn_1.gds
+-rw-r--r--   0        0        0     7078 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvn_2.gds
+-rw-r--r--   0        0        0     9292 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvn_4.gds
+-rw-r--r--   0        0        0    14230 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvn_8.gds
+-rw-r--r--   0        0        0     5128 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvp_1.gds
+-rw-r--r--   0        0        0     6854 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvp_2.gds
+-rw-r--r--   0        0        0     9576 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvp_4.gds
+-rw-r--r--   0        0        0    14452 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvp_8.gds
+-rw-r--r--   0        0        0    14168 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fa_1.gds
+-rw-r--r--   0        0        0    13544 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fa_2.gds
+-rw-r--r--   0        0        0    17172 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fa_4.gds
+-rw-r--r--   0        0        0    20584 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fah_1.gds
+-rw-r--r--   0        0        0    19798 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fah_2.gds
+-rw-r--r--   0        0        0    22438 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fah_4.gds
+-rw-r--r--   0        0        0    19264 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fahcin_1.gds
+-rw-r--r--   0        0        0    18432 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fahcon_1.gds
+-rw-r--r--   0        0        0     1424 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_1.gds
+-rw-r--r--   0        0        0     1552 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_2.gds
+-rw-r--r--   0        0        0     1808 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_4.gds
+-rw-r--r--   0        0        0     2320 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_8.gds
+-rw-r--r--   0        0        0     2088 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_diode_2.gds
+-rw-r--r--   0        0        0     2600 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_diode_4.gds
+-rw-r--r--   0        0        0     3880 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_diode_8.gds
+-rw-r--r--   0        0        0     9352 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ha_1.gds
+-rw-r--r--   0        0        0     9138 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ha_2.gds
+-rw-r--r--   0        0        0    15250 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ha_4.gds
+-rw-r--r--   0        0        0     4062 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__inv_1.gds
+-rw-r--r--   0        0        0    14252 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__inv_16.gds
+-rw-r--r--   0        0        0     4478 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__inv_2.gds
+-rw-r--r--   0        0        0     5284 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__inv_4.gds
+-rw-r--r--   0        0        0     7702 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__inv_8.gds
+-rw-r--r--   0        0        0     7028 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__maj3_1.gds
+-rw-r--r--   0        0        0     7956 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__maj3_2.gds
+-rw-r--r--   0        0        0    12438 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__maj3_4.gds
+-rw-r--r--   0        0        0     6994 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2_1.gds
+-rw-r--r--   0        0        0     8132 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2_2.gds
+-rw-r--r--   0        0        0    12544 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2_4.gds
+-rw-r--r--   0        0        0     7112 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2i_1.gds
+-rw-r--r--   0        0        0    10010 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2i_2.gds
+-rw-r--r--   0        0        0    14492 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2i_4.gds
+-rw-r--r--   0        0        0    14562 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux4_1.gds
+-rw-r--r--   0        0        0    15604 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux4_2.gds
+-rw-r--r--   0        0        0    25202 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux4_4.gds
+-rw-r--r--   0        0        0     4388 2023-11-18 19:15:28.784098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2_1.gds
+-rw-r--r--   0        0        0     5224 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2_2.gds
+-rw-r--r--   0        0        0     8050 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2_4.gds
+-rw-r--r--   0        0        0    12224 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2_8.gds
+-rw-r--r--   0        0        0     4846 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2b_1.gds
+-rw-r--r--   0        0        0     5982 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2b_2.gds
+-rw-r--r--   0        0        0     9482 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2b_4.gds
+-rw-r--r--   0        0        0     5456 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3_1.gds
+-rw-r--r--   0        0        0     6760 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3_2.gds
+-rw-r--r--   0        0        0    10832 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3_4.gds
+-rw-r--r--   0        0        0     5770 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3b_1.gds
+-rw-r--r--   0        0        0     8264 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3b_2.gds
+-rw-r--r--   0        0        0    10450 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3b_4.gds
+-rw-r--r--   0        0        0     5512 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4_1.gds
+-rw-r--r--   0        0        0     9054 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4_2.gds
+-rw-r--r--   0        0        0    14382 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4_4.gds
+-rw-r--r--   0        0        0     6140 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4b_1.gds
+-rw-r--r--   0        0        0    10308 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4b_2.gds
+-rw-r--r--   0        0        0    14142 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4b_4.gds
+-rw-r--r--   0        0        0     7662 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4bb_1.gds
+-rw-r--r--   0        0        0    10750 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4bb_2.gds
+-rw-r--r--   0        0        0    16040 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4bb_4.gds
+-rw-r--r--   0        0        0     3960 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2_1.gds
+-rw-r--r--   0        0        0     5380 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2_2.gds
+-rw-r--r--   0        0        0     8288 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2_4.gds
+-rw-r--r--   0        0        0    12336 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2_8.gds
+-rw-r--r--   0        0        0     4954 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2b_1.gds
+-rw-r--r--   0        0        0     6540 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2b_2.gds
+-rw-r--r--   0        0        0     8586 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2b_4.gds
+-rw-r--r--   0        0        0     4914 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3_1.gds
+-rw-r--r--   0        0        0     7010 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3_2.gds
+-rw-r--r--   0        0        0    10124 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3_4.gds
+-rw-r--r--   0        0        0     5338 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3b_1.gds
+-rw-r--r--   0        0        0     8854 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3b_2.gds
+-rw-r--r--   0        0        0    11926 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3b_4.gds
+-rw-r--r--   0        0        0     5742 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4_1.gds
+-rw-r--r--   0        0        0     8252 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4_2.gds
+-rw-r--r--   0        0        0    14130 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4_4.gds
+-rw-r--r--   0        0        0     6134 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4b_1.gds
+-rw-r--r--   0        0        0    10352 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4b_2.gds
+-rw-r--r--   0        0        0    16104 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4b_4.gds
+-rw-r--r--   0        0        0     7596 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4bb_1.gds
+-rw-r--r--   0        0        0    12042 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4bb_2.gds
+-rw-r--r--   0        0        0    16138 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4bb_4.gds
+-rw-r--r--   0        0        0     7934 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111a_1.gds
+-rw-r--r--   0        0        0     8436 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111a_2.gds
+-rw-r--r--   0        0        0    13056 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111a_4.gds
+-rw-r--r--   0        0        0     6994 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111ai_1.gds
+-rw-r--r--   0        0        0    11050 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111ai_2.gds
+-rw-r--r--   0        0        0    15894 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111ai_4.gds
+-rw-r--r--   0        0        0     8144 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211a_1.gds
+-rw-r--r--   0        0        0     7412 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211a_2.gds
+-rw-r--r--   0        0        0    11204 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211a_4.gds
+-rw-r--r--   0        0        0     6462 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211ai_1.gds
+-rw-r--r--   0        0        0     9316 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211ai_2.gds
+-rw-r--r--   0        0        0    13998 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211ai_4.gds
+-rw-r--r--   0        0        0     6732 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21a_1.gds
+-rw-r--r--   0        0        0     7120 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21a_2.gds
+-rw-r--r--   0        0        0     9846 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21a_4.gds
+-rw-r--r--   0        0        0     5158 2023-11-18 19:15:28.788098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ai_1.gds
+-rw-r--r--   0        0        0     6662 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ai_2.gds
+-rw-r--r--   0        0        0    10192 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ai_4.gds
+-rw-r--r--   0        0        0     7460 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ba_1.gds
+-rw-r--r--   0        0        0     6954 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ba_2.gds
+-rw-r--r--   0        0        0    10150 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ba_4.gds
+-rw-r--r--   0        0        0     6500 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21bai_1.gds
+-rw-r--r--   0        0        0     7722 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21bai_2.gds
+-rw-r--r--   0        0        0    12418 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21bai_4.gds
+-rw-r--r--   0        0        0     8082 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221a_1.gds
+-rw-r--r--   0        0        0     8466 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221a_2.gds
+-rw-r--r--   0        0        0    13182 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221a_4.gds
+-rw-r--r--   0        0        0     7598 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221ai_1.gds
+-rw-r--r--   0        0        0    10328 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221ai_2.gds
+-rw-r--r--   0        0        0    16248 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221ai_4.gds
+-rw-r--r--   0        0        0     7682 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22a_1.gds
+-rw-r--r--   0        0        0     7254 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22a_2.gds
+-rw-r--r--   0        0        0    11140 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22a_4.gds
+-rw-r--r--   0        0        0     5812 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22ai_1.gds
+-rw-r--r--   0        0        0     8818 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22ai_2.gds
+-rw-r--r--   0        0        0    12830 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22ai_4.gds
+-rw-r--r--   0        0        0     8008 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_1.gds
+-rw-r--r--   0        0        0     8186 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_2.gds
+-rw-r--r--   0        0        0    11528 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_4.gds
+-rw-r--r--   0        0        0     6734 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_1.gds
+-rw-r--r--   0        0        0     9994 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_2.gds
+-rw-r--r--   0        0        0    17300 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_4.gds
+-rw-r--r--   0        0        0     7984 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311a_1.gds
+-rw-r--r--   0        0        0     8108 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311a_2.gds
+-rw-r--r--   0        0        0    13778 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311a_4.gds
+-rw-r--r--   0        0        0     6910 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311ai_1.gds
+-rw-r--r--   0        0        0    10888 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311ai_2.gds
+-rw-r--r--   0        0        0    17046 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311ai_4.gds
+-rw-r--r--   0        0        0     6498 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31a_1.gds
+-rw-r--r--   0        0        0     6946 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31a_2.gds
+-rw-r--r--   0        0        0    12418 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31a_4.gds
+-rw-r--r--   0        0        0     6304 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31ai_1.gds
+-rw-r--r--   0        0        0     8912 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31ai_2.gds
+-rw-r--r--   0        0        0    13844 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31ai_4.gds
+-rw-r--r--   0        0        0     7216 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32a_1.gds
+-rw-r--r--   0        0        0     8472 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32a_2.gds
+-rw-r--r--   0        0        0    12894 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32a_4.gds
+-rw-r--r--   0        0        0     6812 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32ai_1.gds
+-rw-r--r--   0        0        0    11062 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32ai_2.gds
+-rw-r--r--   0        0        0    18084 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32ai_4.gds
+-rw-r--r--   0        0        0     8404 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41a_1.gds
+-rw-r--r--   0        0        0     8856 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41a_2.gds
+-rw-r--r--   0        0        0    13274 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41a_4.gds
+-rw-r--r--   0        0        0     6892 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41ai_1.gds
+-rw-r--r--   0        0        0    10848 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41ai_2.gds
+-rw-r--r--   0        0        0    16862 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41ai_4.gds
+-rw-r--r--   0        0        0     4900 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2_1.gds
+-rw-r--r--   0        0        0     5454 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2_2.gds
+-rw-r--r--   0        0        0     7446 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2_4.gds
+-rw-r--r--   0        0        0     6072 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2b_1.gds
+-rw-r--r--   0        0        0     5786 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2b_2.gds
+-rw-r--r--   0        0        0    10298 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2b_4.gds
+-rw-r--r--   0        0        0     5396 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3_1.gds
+-rw-r--r--   0        0        0     6622 2023-11-18 19:15:28.792098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3_2.gds
+-rw-r--r--   0        0        0     9566 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3_4.gds
+-rw-r--r--   0        0        0     7346 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3b_1.gds
+-rw-r--r--   0        0        0     6502 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3b_2.gds
+-rw-r--r--   0        0        0    10324 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3b_4.gds
+-rw-r--r--   0        0        0     6160 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4_1.gds
+-rw-r--r--   0        0        0     7558 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4_2.gds
+-rw-r--r--   0        0        0    11670 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4_4.gds
+-rw-r--r--   0        0        0     7616 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4b_1.gds
+-rw-r--r--   0        0        0     7568 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4b_2.gds
+-rw-r--r--   0        0        0    12512 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4b_4.gds
+-rw-r--r--   0        0        0     8468 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4bb_1.gds
+-rw-r--r--   0        0        0     8202 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4bb_2.gds
+-rw-r--r--   0        0        0    12948 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4bb_4.gds
+-rw-r--r--   0        0        0    24580 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfbbn_1.gds
+-rw-r--r--   0        0        0    26280 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfbbn_2.gds
+-rw-r--r--   0        0        0    23670 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfbbp_1.gds
+-rw-r--r--   0        0        0    21900 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrbp_1.gds
+-rw-r--r--   0        0        0    21876 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrbp_2.gds
+-rw-r--r--   0        0        0    20580 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrtn_1.gds
+-rw-r--r--   0        0        0    20632 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_1.gds
+-rw-r--r--   0        0        0    21136 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_2.gds
+-rw-r--r--   0        0        0    21380 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_4.gds
+-rw-r--r--   0        0        0    21582 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfsbp_1.gds
+-rw-r--r--   0        0        0    25042 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfsbp_2.gds
+-rw-r--r--   0        0        0    20846 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfstp_1.gds
+-rw-r--r--   0        0        0    21784 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfstp_2.gds
+-rw-r--r--   0        0        0    23098 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfstp_4.gds
+-rw-r--r--   0        0        0    19098 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfxbp_1.gds
+-rw-r--r--   0        0        0    19818 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfxbp_2.gds
+-rw-r--r--   0        0        0    16784 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_1.gds
+-rw-r--r--   0        0        0    17176 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_2.gds
+-rw-r--r--   0        0        0    17596 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_4.gds
+-rw-r--r--   0        0        0    11910 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_1.gds
+-rw-r--r--   0        0        0    12598 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_2.gds
+-rw-r--r--   0        0        0    13494 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_4.gds
+-rw-r--r--   0        0        0    22998 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sedfxbp_1.gds
+-rw-r--r--   0        0        0    24322 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sedfxbp_2.gds
+-rw-r--r--   0        0        0    22398 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_1.gds
+-rw-r--r--   0        0        0    22344 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_2.gds
+-rw-r--r--   0        0        0    23366 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_4.gds
+-rw-r--r--   0        0        0     2830 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tap_1.gds
+-rw-r--r--   0        0        0     3982 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tap_2.gds
+-rw-r--r--   0        0        0     2962 2023-11-18 19:15:28.796098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tapmet1_2.gds
+-rw-r--r--   0        0        0     2040 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tapvgnd2_1.gds
+-rw-r--r--   0        0        0     2038 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tapvgnd_1.gds
+-rw-r--r--   0        0        0     1758 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tapvpwrvgnd_1.gds
+-rw-r--r--   0        0        0     6092 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor2_1.gds
+-rw-r--r--   0        0        0     8426 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor2_2.gds
+-rw-r--r--   0        0        0    13058 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor2_4.gds
+-rw-r--r--   0        0        0    12680 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor3_1.gds
+-rw-r--r--   0        0        0    13416 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor3_2.gds
+-rw-r--r--   0        0        0    15998 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor3_4.gds
+-rw-r--r--   0        0        0     6424 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor2_1.gds
+-rw-r--r--   0        0        0     7828 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor2_2.gds
+-rw-r--r--   0        0        0    12988 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor2_4.gds
+-rw-r--r--   0        0        0    14044 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor3_1.gds
+-rw-r--r--   0        0        0    14716 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor3_2.gds
+-rw-r--r--   0        0        0    15794 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor3_4.gds
+-rw-r--r--   0        0        0    11766 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__a21o_1.gds
+-rw-r--r--   0        0        0     9658 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__a21oi_1.gds
+-rw-r--r--   0        0        0    13980 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__a22o_1.gds
+-rw-r--r--   0        0        0    10616 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__a22oi_1.gds
+-rw-r--r--   0        0        0     9098 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__and2_1.gds
+-rw-r--r--   0        0        0    10302 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__and3_1.gds
+-rw-r--r--   0        0        0     7688 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_1.gds
+-rw-r--r--   0        0        0    39408 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_16.gds
+-rw-r--r--   0        0        0     8694 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_2.gds
+-rw-r--r--   0        0        0    59888 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_32.gds
+-rw-r--r--   0        0        0    11338 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_4.gds
+-rw-r--r--   0        0        0    20202 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_8.gds
+-rw-r--r--   0        0        0     6942 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__conb_1.gds
+-rw-r--r--   0        0        0     4884 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__decap_4.gds
+-rw-r--r--   0        0        0     6964 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__decap_8.gds
+-rw-r--r--   0        0        0    31398 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfrbp_1.gds
+-rw-r--r--   0        0        0    29300 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfrtp_1.gds
+-rw-r--r--   0        0        0    33566 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfsbp_1.gds
+-rw-r--r--   0        0        0    29300 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfstp_1.gds
+-rw-r--r--   0        0        0    28546 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfxbp_1.gds
+-rw-r--r--   0        0        0    24170 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfxtp_1.gds
+-rw-r--r--   0        0        0     5168 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__diode_2.gds
+-rw-r--r--   0        0        0    24070 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dlclkp_1.gds
+-rw-r--r--   0        0        0    19870 2023-11-18 19:15:28.800098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dlrtp_1.gds
+-rw-r--r--   0        0        0    16574 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dlxtp_1.gds
+-rw-r--r--   0        0        0     9902 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__einvn_1.gds
+-rw-r--r--   0        0        0     9690 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__einvp_1.gds
+-rw-r--r--   0        0        0     2512 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__fill_1.gds
+-rw-r--r--   0        0        0     2896 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__fill_2.gds
+-rw-r--r--   0        0        0     3664 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__fill_4.gds
+-rw-r--r--   0        0        0     5200 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__fill_8.gds
+-rw-r--r--   0        0        0     5838 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__inv_1.gds
+-rw-r--r--   0        0        0    29772 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__inv_16.gds
+-rw-r--r--   0        0        0     7110 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__inv_2.gds
+-rw-r--r--   0        0        0    10288 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__inv_4.gds
+-rw-r--r--   0        0        0    17150 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__inv_8.gds
+-rw-r--r--   0        0        0    12836 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2hv_hl_1.gds
+-rw-r--r--   0        0        0    21610 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2hv_lh_1.gds
+-rw-r--r--   0        0        0    18828 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2lv_1.gds
+-rw-r--r--   0        0        0    13082 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2lv_simple_1.gds
+-rw-r--r--   0        0        0    23376 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_1.gds
+-rw-r--r--   0        0        0    53092 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_clkiso_hlkg_3.gds
+-rw-r--r--   0        0        0    29020 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_isosrchvaon_1.gds
+-rw-r--r--   0        0        0    23514 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_symmetric_1.gds
+-rw-r--r--   0        0        0    12504 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__mux2_1.gds
+-rw-r--r--   0        0        0    25182 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__mux4_1.gds
+-rw-r--r--   0        0        0     6892 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__nand2_1.gds
+-rw-r--r--   0        0        0     9498 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__nand3_1.gds
+-rw-r--r--   0        0        0     7454 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__nor2_1.gds
+-rw-r--r--   0        0        0     8292 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__nor3_1.gds
+-rw-r--r--   0        0        0    11886 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__o21a_1.gds
+-rw-r--r--   0        0        0     9088 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__o21ai_1.gds
+-rw-r--r--   0        0        0    12868 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__o22a_1.gds
+-rw-r--r--   0        0        0     9922 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__o22ai_1.gds
+-rw-r--r--   0        0        0     8814 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__or2_1.gds
+-rw-r--r--   0        0        0    10460 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__or3_1.gds
+-rw-r--r--   0        0        0    20954 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__probe_p_8.gds
+-rw-r--r--   0        0        0    23282 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__probec_p_8.gds
+-rw-r--r--   0        0        0    11536 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__schmittbuf_1.gds
+-rw-r--r--   0        0        0    34228 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfrbp_1.gds
+-rw-r--r--   0        0        0    36482 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfrtp_1.gds
+-rw-r--r--   0        0        0    38850 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfsbp_1.gds
+-rw-r--r--   0        0        0    35086 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfstp_1.gds
+-rw-r--r--   0        0        0    37804 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfxbp_1.gds
+-rw-r--r--   0        0        0    29122 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfxtp_1.gds
+-rw-r--r--   0        0        0    23000 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdlclkp_1.gds
+-rw-r--r--   0        0        0    24080 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdlxtp_1.gds
+-rw-r--r--   0        0        0    12322 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__xnor2_1.gds
+-rw-r--r--   0        0        0    12192 2023-11-18 19:15:28.804098 sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__xor2_1.gds
+-rw-r--r--   0        0        0     3411 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/klayout/grain.xml
+-rw-r--r--   0        0        0   231824 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/klayout/layers.lyp
+-rw-r--r--   0        0        0    75766 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/klayout/layers.yaml
+-rw-r--r--   0        0        0     5937 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/klayout/pymacros/klayout_Library.lym
+-rw-r--r--   0        0        0      697 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/klayout/pymacros/set_menus.lym
+-rw-r--r--   0        0        0     6801 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/klayout/sky130.lyt
+-rw-r--r--   0        0        0     7117 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/klayout/sky130.xs
+-rw-r--r--   0        0        0    13414 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/klayout/sky130_xs.lyp
+-rw-r--r--   0        0        0     2156 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/klayout/sky_x64.png
+-rw-r--r--   0        0        0     7646 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/klayout/tech.lyt
+-rw-r--r--   0        0        0    21395 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/layers.py
+-rw-r--r--   0        0        0     2419 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/nmos.py
+-rw-r--r--   0        0        0      705 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/__init__.py
+-rw-r--r--   0        0        0     4411 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/mimcap_1.py
+-rw-r--r--   0        0        0     3556 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/mimcap_2.py
+-rw-r--r--   0        0        0    15422 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/nmos.py
+-rw-r--r--   0        0        0    14299 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/nmos_5v.py
+-rw-r--r--   0        0        0    23719 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/npn_W1L1.py
+-rw-r--r--   0        0        0    24647 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/npn_W1L2.py
+-rw-r--r--   0        0        0     6875 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/p_n_poly.py
+-rw-r--r--   0        0        0     6878 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/p_p_poly.py
+-rw-r--r--   0        0        0    15208 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/pmos.py
+-rw-r--r--   0        0        0    13696 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/pmos_5v.py
+-rw-r--r--   0        0        0    23889 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/pnp.py
+-rw-r--r--   0        0        0     5207 2023-11-18 19:15:28.808098 sky130-0.9.0/sky130/pcells/via_generator.py
+-rw-r--r--   0        0        0   926242 2023-11-18 19:15:28.812098 sky130-0.9.0/sky130/spice/sky130_fd_sc_hd.spice
+-rwxr-xr-x   0        0        0   967549 2023-11-18 19:15:28.812098 sky130-0.9.0/sky130/spice/sky130_fd_sc_hs.spice
+-rw-r--r--   0        0        0   140107 2023-11-18 19:15:28.816098 sky130-0.9.0/sky130/spice/sky130_fd_sc_hvl.spice
+-rw-r--r--   0        0        0    72993 2023-11-18 19:15:28.816098 sky130-0.9.0/sky130/spice_models.py
+-rw-r--r--   0        0        0      471 2023-11-18 19:15:28.816098 sky130-0.9.0/sky130/tech.py
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 sky130-0.9.0/PKG-INFO
```

### Comparing `sky130-0.8.0/LICENSE` & `sky130-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/README.md` & `sky130-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# sky130 gdsfactory PDK 0.8.0
+# sky130 gdsfactory PDK 0.9.0
 
 [![pypi](https://img.shields.io/pypi/v/sky130)](https://pypi.org/project/sky130/)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 gdsfactory pdk based on [skywater130](https://github.com/google/skywater-pdk)
 
 ![logo](https://i.imgur.com/xvnfEtZ.png)
```

### Comparing `sky130-0.8.0/sky130/__init__.py` & `sky130-0.9.0/sky130/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from gdsfactory.pdk import Pdk
 
 from sky130 import components, pcells
 from sky130.config import PATH, module_path
 from sky130.layers import LAYER, LAYER_STACK, LAYER_VIEWS
 from sky130.tech import cross_sections
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 cells = get_cells([components, pcells])
 PDK = Pdk(
     name="sky130",
     cells=cells,
     cross_sections=cross_sections,
     layers=LAYER.dict(),
```

### Comparing `sky130-0.8.0/sky130/config.py` & `sky130-0.9.0/sky130/config.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111oi_0.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111oi_0.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2111oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2111oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a211oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a211oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21bo_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21bo_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21bo_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21bo_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21bo_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21bo_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21boi_0.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21boi_0.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21boi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21boi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21boi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21boi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21boi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21boi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a21oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a21oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a221oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a221oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a222oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a222oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a22oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a22oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a2bb2oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a311oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a311oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a31oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a31oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a32oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a32oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__a41oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__a41oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2_0.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2_0.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and2b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and2b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and3b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and3b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4bb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4bb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4bb_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4bb_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__and4bb_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__and4bb_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_12.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_12.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_6.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_6.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__buf_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__buf_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__bufbuf_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__bufbuf_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__bufbuf_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__bufbuf_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__bufinv_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__bufinv_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__bufinv_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__bufinv_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkbuf_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkbuf_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkbuf_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkbuf_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkbuf_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkbuf_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkbuf_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkbuf_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkbuf_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkbuf_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s15_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s15_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s15_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s15_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s18_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s18_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s18_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s18_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s25_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s25_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s25_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s25_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s50_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s50_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s50_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkdlybuf4s50_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinv_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinv_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinv_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinv_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinv_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinv_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinv_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinv_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinv_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinv_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinvlp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinvlp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__clkinvlp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__clkinvlp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__conb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__conb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__decap_12.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__decap_12.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__decap_3.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__decap_3.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__decap_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__decap_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__decap_6.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__decap_6.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__decap_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__decap_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfbbn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfbbn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfbbn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfbbn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfbbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfbbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrtn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrtn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfrtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfrtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfsbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfsbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfsbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfsbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfstp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfstp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfstp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfstp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfstp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfstp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfxbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfxbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfxtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfxtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dfxtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dfxtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__diode_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__diode_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlclkp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlclkp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlclkp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlclkp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlclkp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlclkp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrbn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrbn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrbn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrbn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtn_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtn_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlrtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlrtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxbn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxbn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxbn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxbn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxtn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxtn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxtn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxtn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxtn_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxtn_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd1_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd1_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlygate4sd3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s2s_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s2s_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s4s_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s4s_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s6s_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__dlymetal6s6s_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ebufn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ebufn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ebufn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ebufn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ebufn_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ebufn_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ebufn_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ebufn_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__edfxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__edfxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__edfxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__edfxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvn_0.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvn_0.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvn_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvn_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvn_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvn_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__einvp_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__einvp_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fa_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fa_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fa_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fa_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fa_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fa_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fah_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fah_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fahcin_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fahcin_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fahcon_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fahcon_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fill_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fill_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fill_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fill_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fill_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fill_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__fill_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__fill_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ha_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ha_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ha_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ha_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__ha_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__ha_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_12.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_12.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_6.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_6.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__inv_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__inv_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_bleeder_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_bleeder_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkbufkapwr_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_clkinvkapwr_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_12.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_12.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_3.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_3.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_6.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_6.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_decapkapwr_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso0n_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso0n_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso0p_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso0p_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso1n_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso1n_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso1p_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputiso1p_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputisolatch_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_inputisolatch_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrc_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrckapwr_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_isobufsrckapwr_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_hl_isowell_tap_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__lpflow_lsbuf_lh_isowell_tap_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__macro_sparecell.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__macro_sparecell.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__maj3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__maj3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__maj3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__maj3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__maj3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__maj3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2i_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2i_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2i_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2i_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux2i_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux2i_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux4_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux4_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__mux4_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__mux4_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand2b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand2b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand3b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand3b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4bb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4bb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4bb_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4bb_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nand4bb_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nand4bb_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor2b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor2b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor3b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor3b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4bb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4bb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4bb_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4bb_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__nor4bb_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__nor4bb_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2111ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2111ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o211ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o211ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ai_0.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ai_0.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ba_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ba_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ba_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ba_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21ba_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21ba_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21bai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21bai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21bai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21bai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o21bai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o21bai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o221ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o221ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o22ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o22ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o2bb2ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311ai_0.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311ai_0.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o311ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o311ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o31ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o31ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o32ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o32ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__o41ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__o41ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2_0.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2_0.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or2b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or2b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or3b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or3b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4bb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4bb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4bb_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4bb_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__or4bb_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__or4bb_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__probe_p_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__probe_p_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__probec_p_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__probec_p_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfbbn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfbbn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfbbn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfbbn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfbbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfbbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrtn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrtn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfrtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfsbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfsbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfsbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfsbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfstp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfstp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfstp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfstp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfstp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfstp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfxbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfxbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdfxtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sdlclkp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sedfxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sedfxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sedfxbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sedfxbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__sedfxtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__tap_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__tap_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__tap_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__tap_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__tapvgnd2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__tapvgnd2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__tapvgnd_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__tapvgnd_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__tapvpwrvgnd_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__tapvpwrvgnd_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xnor3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xnor3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hd__xor3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hd__xor3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2111oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2111oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a211oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a211oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21bo_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21bo_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21bo_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21bo_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21bo_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21bo_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21boi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21boi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21boi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21boi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21boi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21boi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a21oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a21oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a221oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a221oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a222o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a222o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a222o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a222o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a222oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a222oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a222oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a222oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a22oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a22oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a2bb2oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a311oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a311oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a31oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a31oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a32oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a32oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41o_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41o_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41o_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41o_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41oi_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41oi_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__a41oi_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__a41oi_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and2b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and2b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and3b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and3b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4bb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4bb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4bb_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4bb_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__and4bb_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__and4bb_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__buf_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__buf_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__buf_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__buf_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__buf_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__buf_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__buf_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__buf_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__buf_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__buf_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__bufbuf_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__bufbuf_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__bufbuf_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__bufbuf_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__bufinv_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__bufinv_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__bufinv_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__bufinv_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkbuf_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkbuf_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkbuf_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkbuf_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkbuf_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkbuf_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkbuf_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkbuf_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkbuf_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkbuf_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd1_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd1_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv3sd3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd1_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd1_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkdlyinv5sd3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkinv_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkinv_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkinv_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkinv_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkinv_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkinv_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkinv_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkinv_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__clkinv_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__clkinv_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__conb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__conb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__decap_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__decap_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__decap_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__decap_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfbbn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfbbn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfbbn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfbbn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfbbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfbbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrtn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrtn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfrtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfrtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfsbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfsbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfsbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfsbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfstp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfstp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfstp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfstp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfstp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfstp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfxbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfxbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfxtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfxtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dfxtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dfxtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__diode_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__diode_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlclkp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlclkp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlclkp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlclkp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlclkp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlclkp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrbn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrbn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrbn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrbn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtn_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtn_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlrtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlrtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxbn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxbn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxbn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxbn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxtn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxtn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxtn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxtn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxtn_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxtn_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd1_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd1_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlygate4sd3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s2s_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s2s_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s4s_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s4s_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s6s_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__dlymetal6s6s_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ebufn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ebufn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ebufn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ebufn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ebufn_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ebufn_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ebufn_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ebufn_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__edfxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__edfxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__edfxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__edfxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvn_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvn_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvn_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvn_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__einvp_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__einvp_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fa_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fa_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fa_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fa_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fa_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fa_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fah_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fah_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fah_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fah_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fah_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fah_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fahcin_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fahcin_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fahcon_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fahcon_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_diode_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_diode_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_diode_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_diode_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__fill_diode_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__fill_diode_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ha_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ha_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ha_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ha_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__ha_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__ha_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__inv_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__inv_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__inv_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__inv_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__inv_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__inv_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__inv_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__inv_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__inv_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__inv_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__maj3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__maj3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__maj3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__maj3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__maj3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__maj3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2i_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2i_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2i_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2i_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux2i_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux2i_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux4_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux4_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__mux4_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__mux4_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand2b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand2b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand3b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand3b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4bb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4bb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4bb_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4bb_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nand4bb_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nand4bb_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor2b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor2b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor3b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor3b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4bb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4bb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4bb_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4bb_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__nor4bb_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__nor4bb_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2111ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2111ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o211ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o211ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ba_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ba_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ba_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ba_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21ba_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21ba_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21bai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21bai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21bai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21bai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o21bai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o21bai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o221ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o221ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o22ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o22ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o2bb2ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o311ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o311ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o31ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o31ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o32ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o32ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41a_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41a_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41a_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41a_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41ai_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41ai_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__o41ai_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__o41ai_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or2b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or2b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or3b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or3b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4b_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4b_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4b_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4b_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4b_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4b_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4bb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4bb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4bb_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4bb_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__or4bb_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__or4bb_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfbbn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfbbn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfbbn_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfbbn_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfbbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfbbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrtn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrtn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfrtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfsbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfsbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfsbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfsbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfstp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfstp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfstp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfstp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfstp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfstp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfxbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfxbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdfxtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sdlclkp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sedfxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sedfxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sedfxbp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sedfxbp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__sedfxtp_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tap_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tap_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tap_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tap_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tapmet1_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tapmet1_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tapvgnd2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tapvgnd2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tapvgnd_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tapvgnd_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__tapvpwrvgnd_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__tapvpwrvgnd_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xnor3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xnor3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor2_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor2_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor2_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor2_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor3_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor3_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hs__xor3_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hs__xor3_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__a21o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__a21o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__a21oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__a21oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__a22o_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__a22o_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__a22oi_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__a22oi_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__and2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__and2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__and3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__and3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_32.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_32.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__buf_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__buf_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__conb_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__conb_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__decap_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__decap_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__decap_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__decap_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfrbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfrbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfrtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfrtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfsbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfsbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfstp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfstp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dfxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dfxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__diode_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__diode_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dlclkp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dlclkp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dlrtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dlrtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__dlxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__dlxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__einvn_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__einvn_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__einvp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__einvp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__fill_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__fill_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__fill_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__fill_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__fill_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__fill_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__fill_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__fill_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__inv_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__inv_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__inv_16.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__inv_16.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__inv_2.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__inv_2.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__inv_4.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__inv_4.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__inv_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__inv_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2hv_hl_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2hv_hl_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2hv_lh_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2hv_lh_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2lv_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2lv_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2lv_simple_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbufhv2lv_simple_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_clkiso_hlkg_3.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_clkiso_hlkg_3.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_isosrchvaon_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_isosrchvaon_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_symmetric_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__lsbuflv2hv_symmetric_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__mux2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__mux2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__mux4_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__mux4_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__nand2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__nand2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__nand3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__nand3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__nor2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__nor2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__nor3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__nor3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__o21a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__o21a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__o21ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__o21ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__o22a_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__o22a_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__o22ai_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__o22ai_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__or2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__or2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__or3_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__or3_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__probe_p_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__probe_p_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__probec_p_8.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__probec_p_8.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__schmittbuf_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__schmittbuf_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfrbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfrbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfrtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfrtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfsbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfsbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfstp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfstp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfxbp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfxbp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdfxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdfxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdlclkp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdlclkp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__sdlxtp_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__sdlxtp_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__xnor2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__xnor2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/gds/sky130_fd_sc_hvl__xor2_1.gds` & `sky130-0.9.0/sky130/gds/sky130_fd_sc_hvl__xor2_1.gds`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/klayout/grain.xml` & `sky130-0.9.0/sky130/klayout/grain.xml`

 * *Files 0% similar despite different names*

#### Comparing `sky130-0.8.0/sky130/klayout/grain.xml` & `sky130-0.9.0/sky130/klayout/grain.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <salt-grain>
   <name>sky130</name>
   <token/>
   <hidden>false</hidden>
-  <version>0.8.0</version>
+  <version>0.9.0</version>
   <api-version/>
   <title>sky130</title>
   <doc>Skywater 130nm libraries</doc>
   <doc-url>https://gdsfactory.github.io/skywater130/README.html</doc-url>
   <url>https://github.com/gdsfactory/skywater130</url>
   <license>Apache2</license>
   <author>GF</author>
```

### Comparing `sky130-0.8.0/sky130/klayout/layers.lyp` & `sky130-0.9.0/sky130/klayout/layers.lyp`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/klayout/layers.yaml` & `sky130-0.9.0/sky130/klayout/layers.yaml`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/klayout/pymacros/klayout_Library.lym` & `sky130-0.9.0/sky130/klayout/pymacros/klayout_Library.lym`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/klayout/pymacros/set_menus.lym` & `sky130-0.9.0/sky130/klayout/pymacros/set_menus.lym`

 * *Files 0% similar despite different names*

#### Comparing `sky130-0.8.0/sky130/klayout/pymacros/set_menus.lym` & `sky130-0.9.0/sky130/klayout/pymacros/set_menus.lym`

```diff
@@ -12,15 +12,15 @@
   <show-in-menu>false</show-in-menu>
   <group-name/>
   <menu-path>sky130.begin</menu-path>
   <interpreter>python</interpreter>
   <dsl-interpreter-name/>
   <text>import pya
 
-__version__ = &quot;0.8.0&quot;
+__version__ = &quot;0.9.0&quot;
 
 
 def set_menu():
     menu = pya.Application.instance().main_window().menu()
 
     s0 = &quot;sky130&quot;
     if not (menu.is_menu(s0)):
```

### Comparing `sky130-0.8.0/sky130/klayout/sky130.lyt` & `sky130-0.9.0/sky130/klayout/sky130.lyt`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/klayout/sky130.xs` & `sky130-0.9.0/sky130/klayout/sky130.xs`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/klayout/sky130_xs.lyp` & `sky130-0.9.0/sky130/klayout/sky130_xs.lyp`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/klayout/sky_x64.png` & `sky130-0.9.0/sky130/klayout/sky_x64.png`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/klayout/tech.lyt` & `sky130-0.9.0/sky130/klayout/tech.lyt`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/layers.py` & `sky130-0.9.0/sky130/layers.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/nmos.py` & `sky130-0.9.0/sky130/nmos.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/__init__.py` & `sky130-0.9.0/sky130/pcells/__init__.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/mimcap_1.py` & `sky130-0.9.0/sky130/pcells/mimcap_1.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/mimcap_2.py` & `sky130-0.9.0/sky130/pcells/mimcap_2.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/nmos.py` & `sky130-0.9.0/sky130/pcells/nmos.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/nmos_5v.py` & `sky130-0.9.0/sky130/pcells/nmos_5v.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/npn_W1L1.py` & `sky130-0.9.0/sky130/pcells/npn_W1L1.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/npn_W1L2.py` & `sky130-0.9.0/sky130/pcells/npn_W1L2.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/p_n_poly.py` & `sky130-0.9.0/sky130/pcells/p_n_poly.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/p_p_poly.py` & `sky130-0.9.0/sky130/pcells/p_p_poly.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/pmos.py` & `sky130-0.9.0/sky130/pcells/pmos.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/pmos_5v.py` & `sky130-0.9.0/sky130/pcells/pmos_5v.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/pnp.py` & `sky130-0.9.0/sky130/pcells/pnp.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/pcells/via_generator.py` & `sky130-0.9.0/sky130/pcells/via_generator.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/spice/sky130_fd_sc_hd.spice` & `sky130-0.9.0/sky130/spice/sky130_fd_sc_hd.spice`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/spice/sky130_fd_sc_hs.spice` & `sky130-0.9.0/sky130/spice/sky130_fd_sc_hs.spice`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/spice/sky130_fd_sc_hvl.spice` & `sky130-0.9.0/sky130/spice/sky130_fd_sc_hvl.spice`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/sky130/spice_models.py` & `sky130-0.9.0/sky130/spice_models.py`

 * *Files identical despite different names*

### Comparing `sky130-0.8.0/PKG-INFO` & `sky130-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: sky130
-Version: 0.8.0
+Version: 0.9.0
 Summary: skywater130 pdk
 Keywords: python
 Author-email: gdsfactory <contact@gdsfactory.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Dist: gdsfactory[cad]==7.3.0
+Requires-Dist: gdsfactory[cad]==7.8.17
 Requires-Dist: PySpice
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest_regressions ; extra == "dev"
-Requires-Dist: autodoc_pydantic ; extra == "docs"
+Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: jupytext ; extra == "docs"
 Requires-Dist: jupyter-book==0.15.1 ; extra == "docs"
 Provides-Extra: dev
 Provides-Extra: docs
 
-# sky130 gdsfactory PDK 0.8.0
+# sky130 gdsfactory PDK 0.9.0
 
 [![pypi](https://img.shields.io/pypi/v/sky130)](https://pypi.org/project/sky130/)
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 gdsfactory pdk based on [skywater130](https://github.com/google/skywater-pdk)
 
 ![logo](https://i.imgur.com/xvnfEtZ.png)
```

