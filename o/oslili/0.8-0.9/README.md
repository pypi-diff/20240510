# Comparing `tmp/oslili-0.8.tar.gz` & `tmp/oslili-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslili-0.8.tar", last modified: Sun Apr 14 22:51:10 2024, max compression
+gzip compressed data, was "oslili-0.9.tar", last modified: Sun Apr 14 23:07:32 2024, max compression
```

## Comparing `oslili-0.8.tar` & `oslili-0.9.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-14 22:51:10.953038 oslili-0.8/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-12 06:16:56.000000 oslili-0.8/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-04-12 06:16:56.000000 oslili-0.8/NOTICE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3022 2024-04-14 22:51:10.952981 oslili-0.8/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2451 2024-04-12 06:16:56.000000 oslili-0.8/README.md
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-14 22:51:10.885949 oslili-0.8/oslili/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       77 2024-04-12 06:16:56.000000 oslili-0.8/oslili/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5481 2024-04-14 22:50:51.000000 oslili-0.8/oslili/identifier.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-14 22:51:10.952581 oslili-0.8/oslili/spdx/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      643 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/0BSD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1931 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/389-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2529 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AAL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      488 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ADSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4676 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AFL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4950 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AFL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8987 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AFL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8948 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AFL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10334 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AFL-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15839 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AGPL-1.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15839 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AGPL-1.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    34020 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AGPL-3.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    34020 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AGPL-3.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5642 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AMDPLPA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2358 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AML.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2192 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AMPAS.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1261 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ANTLR-PD-fallback.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      987 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ANTLR-PD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      617 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/APAFML.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    46103 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/APL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19644 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/APSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20151 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/APSL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19800 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/APSL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20285 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/APSL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      731 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Abstyles.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      236 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/AdaCore-doc.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1776 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Adobe-2006.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1608 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Adobe-Glyph.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      893 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Afmparse.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11604 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Aladdin.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2507 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Apache-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2514 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Apache-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10280 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Apache-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      224 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/App-s2p.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6901 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Arphic-1999.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6060 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Artistic-1.0-Perl.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5184 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Artistic-1.0-cl8.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4854 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Artistic-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8764 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Artistic-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1573 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Autoconf-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1818 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Autoconf-exception-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      266 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Autoconf-exception-generic.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      768 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Autoconf-exception-macro.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1086 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-1-Clause.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2569 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-2-Clause-Patent.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1519 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-2-Clause-Views.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1267 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-2-Clause.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1646 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-3-Clause-Attribution.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1676 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-3-Clause-Clear.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2388 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-3-Clause-LBNL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1624 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-3-Clause-Modification.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1647 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-3-Clause-No-Military-License.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1709 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-3-Clause-No-Nuclear-License-2014.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1693 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-3-Clause-No-Nuclear-License.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1699 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-3-Clause-No-Nuclear-Warranty.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1820 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-3-Clause-Open-MPI.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1460 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-3-Clause.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1048 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-4-Clause-Shortened.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1771 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-4-Clause-UC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1618 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-4-Clause.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      476 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-4.3RENO.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      781 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-4.3TAHOE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1626 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-Advertising-Acknowledgement.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1679 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-Attribution-HPND-disclaimer.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6244 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-Protection.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1301 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSD-Source-Code.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1338 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3424 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BUSL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      479 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Baekmuk.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1377 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Bahyph.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      603 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Barr.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      266 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Beerware.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      673 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Bison-exception-2.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    24219 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BitTorrent-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    27782 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BitTorrent-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      572 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Bitstream-Charter.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2318 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Bitstream-Vera.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1552 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/BlueOak-1.0.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      523 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Bootloader-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      647 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Borceux.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1096 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Brian-Gladman-3-Clause.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3451 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/C-UDA-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16125 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CAL-1.0-Combined-Work-Exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16125 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CAL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19046 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CATOSL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11405 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12572 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17126 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-2.5-AU.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12781 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19189 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-3.0-AT.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19218 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17572 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-3.0-IGO.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18371 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-3.0-NL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14654 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-3.0-US.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18666 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17023 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11902 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13585 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13790 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20434 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19607 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17649 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11032 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-ND-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12711 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-ND-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12936 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-ND-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19469 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-ND-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17672 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-ND-3.0-IGO.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17860 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-ND-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17452 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-ND-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13065 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-SA-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15676 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-SA-2.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18798 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-SA-2.0-FR.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11347 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-SA-2.0-UK.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15177 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-SA-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15386 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-SA-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22414 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-SA-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20330 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-SA-3.0-IGO.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21351 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-SA-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19018 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-NC-SA-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10488 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-ND-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11696 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-ND-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11921 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-ND-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18246 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-ND-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16930 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-ND-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16830 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-ND-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12523 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-SA-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10810 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-SA-2.0-UK.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14122 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-SA-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16303 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-SA-2.1-JP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14331 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-SA-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22343 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-SA-3.0-AT.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22421 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-SA-3.0-DE.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21305 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-SA-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18375 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-BY-SA-4.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1593 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC-PDDC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     7048 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CC0-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16514 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CDDL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17390 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CDDL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8592 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CDL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10462 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CDLA-Permissive-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2354 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CDLA-Permissive-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11233 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CDLA-Sharing-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21842 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CECILL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21219 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CECILL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21097 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CECILL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21778 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CECILL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21393 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CECILL-B.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21863 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CECILL-C.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8114 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CERN-OHL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9168 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CERN-OHL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8855 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CERN-OHL-P-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13419 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CERN-OHL-S-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14529 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CERN-OHL-W-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1408 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CFITSIO.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2698 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CLISP-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      938 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CMU-Mach.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3923 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CNRI-Jython.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4004 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CNRI-Python-GPL-Compatible.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3381 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CNRI-Python.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1657 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/COIL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    28319 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CPAL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11653 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11649 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CPOL-1.02.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    23381 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CUA-OPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2577 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Caldera.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6389 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ClArtistic.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Classpath-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      938 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Clips.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15885 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Community-Spec-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6056 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Condor-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      971 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Cornell-Lossless-JPEG.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      480 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Crossword.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      982 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/CrystalStacker.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1078 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Cube.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15238 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/D-FSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2518 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/DL-DE-BY-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4472 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/DOC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1512 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/DRL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2280 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/DSDP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3131 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/DigiRule-FOSS-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      261 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Dotseqn.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2425 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ECL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11111 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ECL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/EFL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      924 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/EFL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3439 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/EPICS.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11345 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/EPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14020 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/EPL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3199 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/EUDatagrid.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13005 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/EUPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13231 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/EUPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13792 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/EUPL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3860 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Elastic-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2277 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Entessa.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13958 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ErlPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1367 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Eurosym.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4447 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/FDK-AAC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1470 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/FLTK-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      225 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/FSFAP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      198 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/FSFUL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      234 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/FSFULLR.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      544 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/FSFULLRWD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5979 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/FTL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      245 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Fair.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1344 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Fawkes-Runtime-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      582 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Font-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9771 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Frameworx-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2781 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/FreeBSD-DOC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17656 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/FreeImage.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      482 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GCC-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3390 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GCC-exception-3.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2983 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.1-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.1-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.1-no-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.1-no-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.1-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.1-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.2-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.2-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.2-no-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.2-no-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.2-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.2-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.3-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.3-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.3-no-invariants-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.3-no-invariants-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.3-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GFDL-1.3-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      896 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GL2PS.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      959 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GLWTPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      379 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GNAT-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12235 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GPL-1.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12235 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GPL-1.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17337 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GPL-2.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    17337 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GPL-2.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      359 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GPL-3.0-linking-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      531 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GPL-3.0-linking-source-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    34670 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GPL-3.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    34670 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GPL-3.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2092 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GPL-CC-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      246 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GStreamer-exception-2005.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      462 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/GStreamer-exception-2008.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1352 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Giftware.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12253 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Glide.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      462 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Glulxe.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      707 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Graphics-Gems.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      617 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/HP-1986.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      179 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/HPND-Markus-Kuhn.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      944 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/HPND-export-US.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      891 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/HPND-sell-variant-MIT-disclaimer.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1102 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/HPND-sell-variant.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1173 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/HPND.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1460 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/HTMLTIDY.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      602 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/HaskellReport.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8422 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Hippocratic-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      855 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/IBM-pibs.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1597 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ICU.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2330 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/IEC-Code-Components-EULA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1640 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/IJG-short.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4244 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/IJG.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9093 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/IPA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11409 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/IPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      823 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ISC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12506 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ImageMagick.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2002 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Imlib2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3171 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Info-ZIP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6132 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Intel-ACPI.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2084 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Intel.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    24344 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Interbase-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3158 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/JPL-image.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2086 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/JPNIC.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1114 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/JSON.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      195 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Jam.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2741 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/JasPer-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      683 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Kazlib.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      299 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/KiCad-libraries-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      296 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Knuth-CTAN.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6972 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LAL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8264 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LAL-1.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    24842 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LGPL-2.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    24842 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LGPL-2.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    25967 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LGPL-2.1-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    25967 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LGPL-2.1-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1033 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LGPL-3.0-linking-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    42098 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LGPL-3.0-only.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    42098 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LGPL-3.0-or-later.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14556 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LGPLLR.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LLVM-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2054 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LOOP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11948 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11824 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LPL-1.02.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8929 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LPPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14026 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LPPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14115 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LPPL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18012 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LPPL-1.3a.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18575 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LPPL-1.3c.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      240 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LZMA-SDK-9.11-to-9.20.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      582 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LZMA-SDK-9.22.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      522 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LZMA-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      704 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Latex2e.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      734 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Leptonica.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6590 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LiLiQ-P-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8694 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LiLiQ-R-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8338 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/LiLiQ-Rplus-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4218 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Libpng.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      254 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Libtool-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      939 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Linux-OpenIB.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1019 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Linux-man-pages-copyleft.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      638 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Linux-syscall-note.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      915 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MIT-0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1150 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MIT-CMU.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      917 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MIT-Modern-Variant.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1295 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MIT-Wu.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1270 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MIT-advertising.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1668 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MIT-enna.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1105 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MIT-feh.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1121 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MIT-open-group.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1078 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MIT.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1531 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MITNFA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    18272 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    23669 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16727 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MPL-2.0-no-copyleft-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16727 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MPL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2870 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MS-LPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2663 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MS-PL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3058 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MS-RL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3239 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MTLL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1974 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MakeIndex.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      407 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Martin-Birgmeier.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2193 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Minpack.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      887 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MirOS.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20187 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Motosoto.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8908 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MulanPSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9233 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/MulanPSL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2040 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Multics.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1459 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Mup.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3792 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NAIST-2003.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13778 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NASA-1.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5425 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NBPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5540 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NCGL-UK-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1700 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NCSA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4703 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NGPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2977 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NICTA-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1644 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NIST-PD-fallback.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      890 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NIST-PD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8712 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NLOD-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8810 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NLOD-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      268 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NLPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    24490 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NOSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21051 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    28018 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11800 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NPOSL-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3298 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NRL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      528 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NTP-0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      714 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NTP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1953 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Naumen.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14237 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Net-SNMP.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1881 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/NetCDF.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      510 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Newsletr.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1177 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Nokia-Qt-exception-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21003 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Nokia.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1126 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Noweb.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3434 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/O-UDA-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14012 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OCCT-PL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      663 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OCCT-exception-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11124 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OCLC-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      881 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OCaml-LGPL-linking-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19808 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ODC-By-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    25289 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ODbL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1007 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OFFIS.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OFL-1.0-RFN.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OFL-1.0-no-RFN.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OFL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OFL-1.1-RFN.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OFL-1.1-no-RFN.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OFL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2179 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OGC-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11606 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OGDL-Taiwan-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3679 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OGL-Canada-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6080 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OGL-UK-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5980 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OGL-UK-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6220 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OGL-UK-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5277 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OGTSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5393 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5396 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5795 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-1.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5873 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-1.4.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1977 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.0.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1981 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2220 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2241 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2267 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.2.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2228 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2265 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2124 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.4.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2171 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2109 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.6.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2197 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.7.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2195 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OLDAP-2.8.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1689 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OML.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20309 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6148 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OPUBL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    19967 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OSET-PL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8921 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9663 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OSL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9880 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OSL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9872 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OSL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10319 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OSL-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1447 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OpenJDK-assembly-exception-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3962 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OpenPBS-2.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     5309 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/OpenSSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    15485 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/PDDL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2846 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/PHP-3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2855 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/PHP-3.01.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      439 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/PS-or-PDF-font-exception-20170817.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2427 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/PSF-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1704 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Parity-6.0.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3524 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Parity-7.0.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1849 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Plexus.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4563 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/PolyForm-Noncommercial-1.0.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4389 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/PolyForm-Small-Business-1.0.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1195 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/PostgreSQL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9916 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Python-2.0.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9411 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Python-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      334 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/QPL-1.0-INRIA-2004-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4641 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/QPL-1.0-INRIA-2004.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4364 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/QPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1304 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Qhull.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      964 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Qt-GPL-exception-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1195 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Qt-LGPL-exception-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1199 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Qwt-exception-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21641 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/RHeCos-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    33931 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/RPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    32009 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/RPL-1.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    30271 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/RPSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      869 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/RSA-MD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21050 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/RSCPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1107 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Rdisc.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2137 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Ruby.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2315 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SAX-PD.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6638 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SCEA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13553 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SGI-B-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14556 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SGI-B-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1503 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SGI-B-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11386 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SHL-0.5.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11399 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SHL-0.51.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2776 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SHL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4485 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SHL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    12474 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SISSL-1.2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    14496 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SISSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1122 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SMLNJ.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3177 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SMPPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    21717 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SNIA.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    23398 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3399 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SSH-OpenSSH.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      326 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SSH-short.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    30609 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SSPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      382 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SWI-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2129 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SWL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2133 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Saxpath.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      290 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SchemeReport.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4020 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Sendmail-8.23.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3948 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Sendmail.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2529 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SimPL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4995 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Sleepycat.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      628 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Spencer-86.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      935 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Spencer-94.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1376 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Spencer-99.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    22087 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SugarCRM-1.1.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      246 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/SunPro.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      355 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Swift-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      515 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Symlinks.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    13932 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TAPR-OHL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2251 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TCL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      648 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TCP-wrappers.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2537 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TMate.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3998 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TORQUE-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2074 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TOSL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      233 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TPDL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    23787 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      406 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TTWL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      678 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TU-Berlin-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1369 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/TU-Berlin-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1948 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/UCAR.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10566 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/UCL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1837 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/UPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2873 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Unicode-DFS-2015.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2858 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Unicode-DFS-2016.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     6261 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Unicode-TOU.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3154 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Universal-FOSS-exception-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1211 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Unlicense.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3058 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/VOSTROM.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2065 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/VSL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4525 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Vim.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3116 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/W3C-19980720.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1807 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/W3C-20150513.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2701 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/W3C.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      432 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/WTFPL.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20972 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Watcom-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      529 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Wsuipa.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1267 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/WxWindows-exception-3.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1314 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/X11-distribute-modifications-variant.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1338 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/X11.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2398 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/XFree86-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      535 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/XSkat.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      963 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Xerox.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1186 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Xnet.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     9010 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/YPL-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8988 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/YPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2924 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ZPL-1.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2275 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ZPL-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2100 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/ZPL-2.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      259 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Zed.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2490 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Zend-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8994 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Zimbra-1.3.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8947 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Zimbra-1.4.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      838 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/Zlib.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      244 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/blessing.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1739 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/bzip2-1.0.6.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      435 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/checkmk.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10571 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/copyleft-next-0.3.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    10634 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/copyleft-next-0.3.1.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1043 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/curl.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       88 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/diffmark.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      210 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/dvipdfm.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      575 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/eCos-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     4235 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/eGenix.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     8198 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/etalab-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1687 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/freertos-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    20362 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/gSOAP-1.3b.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      341 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/gnu-javamail-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1407 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/gnuplot.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      605 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/i2p-gpl-java-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3473 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/iMatix.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1550 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/libpng-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1034 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/libselinux-1.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1139 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/libtiff.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      915 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/libutil-David-Nugent.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      529 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/mif-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      583 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/mpi-permissive.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1424 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/mpich2.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      226 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/mplus.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      629 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/openvpn-openssl-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      480 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/psfrag.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1961 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/psutils.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      209 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/snprintf.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      629 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/u-boot-exception-2.0.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      568 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/w3m.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      591 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/x11vnc-openssl-exception.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2030 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/xinetd.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      734 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/xlock.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2482 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/xpp.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1133 2024-04-12 06:16:56.000000 oslili-0.8/oslili/spdx/zlib-acknowledgement.txt
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-14 22:51:10.952733 oslili-0.8/oslili.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3022 2024-04-14 22:51:10.000000 oslili-0.8/oslili.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    16059 2024-04-14 22:51:10.000000 oslili-0.8/oslili.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-04-14 22:51:10.000000 oslili-0.8/oslili.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       20 2024-04-14 22:51:10.000000 oslili-0.8/oslili.egg-info/requires.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        7 2024-04-14 22:51:10.000000 oslili-0.8/oslili.egg-info/top_level.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       79 2024-04-14 22:51:10.953247 oslili-0.8/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1062 2024-04-12 06:16:56.000000 oslili-0.8/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-14 23:07:32.974284 oslili-0.9/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-12 06:16:56.000000 oslili-0.9/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-04-12 06:16:56.000000 oslili-0.9/NOTICE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3022 2024-04-14 23:07:32.974227 oslili-0.9/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2451 2024-04-12 06:16:56.000000 oslili-0.9/README.md
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-14 23:07:32.852554 oslili-0.9/oslili/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       77 2024-04-12 06:16:56.000000 oslili-0.9/oslili/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5294 2024-04-14 23:07:10.000000 oslili-0.9/oslili/identifier.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-14 23:07:32.973775 oslili-0.9/oslili/spdx/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      643 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/0BSD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1931 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/389-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2529 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AAL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      488 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ADSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4676 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AFL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4950 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AFL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8987 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AFL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8948 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AFL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10334 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AFL-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15839 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AGPL-1.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15839 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AGPL-1.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    34020 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AGPL-3.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    34020 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AGPL-3.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5642 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AMDPLPA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2358 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AML.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2192 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AMPAS.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1261 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ANTLR-PD-fallback.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      987 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ANTLR-PD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      617 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/APAFML.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    46103 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/APL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19644 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/APSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20151 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/APSL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19800 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/APSL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20285 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/APSL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      731 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Abstyles.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      236 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/AdaCore-doc.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1776 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Adobe-2006.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1608 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Adobe-Glyph.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      893 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Afmparse.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11604 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Aladdin.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2507 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Apache-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2514 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Apache-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10280 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Apache-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      224 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/App-s2p.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6901 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Arphic-1999.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6060 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Artistic-1.0-Perl.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5184 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Artistic-1.0-cl8.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4854 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Artistic-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8764 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Artistic-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1573 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Autoconf-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1818 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Autoconf-exception-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      266 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Autoconf-exception-generic.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      768 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Autoconf-exception-macro.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1086 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-1-Clause.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2569 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-2-Clause-Patent.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1519 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-2-Clause-Views.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1267 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-2-Clause.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1646 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-3-Clause-Attribution.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1676 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-3-Clause-Clear.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2388 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-3-Clause-LBNL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1624 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-3-Clause-Modification.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1647 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-3-Clause-No-Military-License.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1709 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-3-Clause-No-Nuclear-License-2014.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1693 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-3-Clause-No-Nuclear-License.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1699 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-3-Clause-No-Nuclear-Warranty.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1820 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-3-Clause-Open-MPI.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1460 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-3-Clause.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1048 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-4-Clause-Shortened.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1771 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-4-Clause-UC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1618 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-4-Clause.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      476 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-4.3RENO.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      781 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-4.3TAHOE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1626 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-Advertising-Acknowledgement.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1679 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-Attribution-HPND-disclaimer.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6244 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-Protection.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1301 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSD-Source-Code.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1338 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3424 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BUSL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      479 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Baekmuk.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1377 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Bahyph.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      603 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Barr.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      266 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Beerware.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      673 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Bison-exception-2.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    24219 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BitTorrent-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    27782 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BitTorrent-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      572 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Bitstream-Charter.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2318 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Bitstream-Vera.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1552 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/BlueOak-1.0.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      523 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Bootloader-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      647 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Borceux.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1096 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Brian-Gladman-3-Clause.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3451 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/C-UDA-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16125 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CAL-1.0-Combined-Work-Exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16125 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CAL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19046 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CATOSL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11405 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12572 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17126 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-2.5-AU.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12781 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19189 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-3.0-AT.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19218 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17572 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-3.0-IGO.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18371 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-3.0-NL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14654 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-3.0-US.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18666 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17023 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11902 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13585 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13790 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20434 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19607 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17649 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11032 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-ND-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12711 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-ND-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12936 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-ND-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19469 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-ND-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17672 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-ND-3.0-IGO.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17860 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-ND-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17452 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-ND-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13065 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-SA-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15676 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-SA-2.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18798 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-SA-2.0-FR.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11347 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-SA-2.0-UK.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15177 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-SA-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15386 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-SA-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22414 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-SA-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20330 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-SA-3.0-IGO.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21351 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-SA-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19018 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-NC-SA-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10488 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-ND-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11696 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-ND-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11921 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-ND-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18246 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-ND-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16930 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-ND-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16830 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-ND-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12523 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-SA-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10810 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-SA-2.0-UK.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14122 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-SA-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16303 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-SA-2.1-JP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14331 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-SA-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22343 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-SA-3.0-AT.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22421 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-SA-3.0-DE.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21305 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-SA-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18375 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-BY-SA-4.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1593 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC-PDDC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     7048 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CC0-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16514 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CDDL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17390 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CDDL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8592 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CDL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10462 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CDLA-Permissive-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2354 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CDLA-Permissive-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11233 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CDLA-Sharing-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21842 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CECILL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21219 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CECILL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21097 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CECILL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21778 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CECILL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21393 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CECILL-B.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21863 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CECILL-C.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8114 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CERN-OHL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9168 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CERN-OHL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8855 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CERN-OHL-P-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13419 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CERN-OHL-S-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14529 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CERN-OHL-W-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1408 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CFITSIO.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2698 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CLISP-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      938 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CMU-Mach.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3923 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CNRI-Jython.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4004 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CNRI-Python-GPL-Compatible.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3381 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CNRI-Python.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1657 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/COIL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    28319 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CPAL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11653 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11649 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CPOL-1.02.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    23381 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CUA-OPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2577 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Caldera.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6389 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ClArtistic.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Classpath-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      938 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Clips.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15885 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Community-Spec-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6056 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Condor-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      971 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Cornell-Lossless-JPEG.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      480 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Crossword.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      982 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/CrystalStacker.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1078 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Cube.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15238 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/D-FSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2518 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/DL-DE-BY-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4472 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/DOC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1512 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/DRL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2280 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/DSDP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3131 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/DigiRule-FOSS-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      261 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Dotseqn.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2425 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ECL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11111 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ECL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/EFL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      924 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/EFL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3439 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/EPICS.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11345 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/EPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14020 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/EPL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3199 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/EUDatagrid.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13005 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/EUPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13231 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/EUPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13792 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/EUPL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3860 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Elastic-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2277 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Entessa.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13958 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ErlPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1367 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Eurosym.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4447 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/FDK-AAC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1470 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/FLTK-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      225 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/FSFAP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      198 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/FSFUL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      234 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/FSFULLR.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      544 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/FSFULLRWD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5979 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/FTL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      245 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Fair.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1344 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Fawkes-Runtime-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      582 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Font-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9771 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Frameworx-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2781 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/FreeBSD-DOC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17656 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/FreeImage.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      482 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GCC-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3390 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GCC-exception-3.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2983 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.1-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.1-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.1-no-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.1-no-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.1-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17970 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.1-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.2-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.2-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.2-no-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.2-no-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.2-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20272 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.2-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.3-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.3-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.3-no-invariants-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.3-no-invariants-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.3-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22791 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GFDL-1.3-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      896 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GL2PS.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      959 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GLWTPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      379 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GNAT-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12235 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GPL-1.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12235 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GPL-1.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17337 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GPL-2.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    17337 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GPL-2.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      359 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GPL-3.0-linking-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      531 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GPL-3.0-linking-source-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    34670 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GPL-3.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    34670 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GPL-3.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2092 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GPL-CC-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      246 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GStreamer-exception-2005.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      462 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/GStreamer-exception-2008.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1352 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Giftware.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12253 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Glide.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      462 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Glulxe.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      707 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Graphics-Gems.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      617 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/HP-1986.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      179 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/HPND-Markus-Kuhn.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      944 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/HPND-export-US.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      891 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/HPND-sell-variant-MIT-disclaimer.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1102 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/HPND-sell-variant.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1173 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/HPND.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1460 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/HTMLTIDY.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      602 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/HaskellReport.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8422 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Hippocratic-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      855 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/IBM-pibs.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1597 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ICU.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2330 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/IEC-Code-Components-EULA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1640 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/IJG-short.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4244 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/IJG.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9093 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/IPA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11409 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/IPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      823 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ISC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12506 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ImageMagick.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2002 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Imlib2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3171 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Info-ZIP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6132 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Intel-ACPI.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2084 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Intel.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    24344 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Interbase-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3158 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/JPL-image.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2086 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/JPNIC.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1114 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/JSON.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      195 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Jam.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2741 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/JasPer-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      683 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Kazlib.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      299 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/KiCad-libraries-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      296 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Knuth-CTAN.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6972 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LAL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8264 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LAL-1.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    24842 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LGPL-2.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    24842 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LGPL-2.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    25967 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LGPL-2.1-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    25967 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LGPL-2.1-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1033 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LGPL-3.0-linking-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    42098 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LGPL-3.0-only.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    42098 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LGPL-3.0-or-later.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14556 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LGPLLR.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      919 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LLVM-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2054 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LOOP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11948 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11824 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LPL-1.02.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8929 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LPPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14026 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LPPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14115 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LPPL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18012 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LPPL-1.3a.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18575 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LPPL-1.3c.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      240 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LZMA-SDK-9.11-to-9.20.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      582 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LZMA-SDK-9.22.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      522 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LZMA-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      704 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Latex2e.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      734 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Leptonica.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6590 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LiLiQ-P-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8694 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LiLiQ-R-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8338 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/LiLiQ-Rplus-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4218 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Libpng.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      254 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Libtool-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      939 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Linux-OpenIB.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1019 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Linux-man-pages-copyleft.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      638 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Linux-syscall-note.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      915 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MIT-0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1150 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MIT-CMU.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      917 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MIT-Modern-Variant.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1295 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MIT-Wu.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1270 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MIT-advertising.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1668 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MIT-enna.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1105 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MIT-feh.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1121 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MIT-open-group.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1078 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MIT.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1531 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MITNFA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    18272 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    23669 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16727 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MPL-2.0-no-copyleft-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16727 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MPL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2870 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MS-LPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2663 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MS-PL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3058 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MS-RL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3239 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MTLL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1974 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MakeIndex.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      407 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Martin-Birgmeier.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2193 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Minpack.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      887 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MirOS.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20187 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Motosoto.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8908 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MulanPSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9233 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/MulanPSL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2040 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Multics.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1459 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Mup.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3792 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NAIST-2003.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13778 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NASA-1.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5425 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NBPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5540 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NCGL-UK-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1700 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NCSA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4703 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NGPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2977 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NICTA-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1644 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NIST-PD-fallback.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      890 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NIST-PD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8712 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NLOD-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8810 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NLOD-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      268 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NLPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    24490 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NOSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21051 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    28018 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11800 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NPOSL-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3298 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NRL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      528 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NTP-0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      714 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NTP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1953 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Naumen.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14237 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Net-SNMP.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1881 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/NetCDF.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      510 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Newsletr.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1177 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Nokia-Qt-exception-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21003 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Nokia.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1126 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Noweb.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3434 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/O-UDA-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14012 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OCCT-PL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      663 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OCCT-exception-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11124 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OCLC-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      881 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OCaml-LGPL-linking-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19808 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ODC-By-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    25289 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ODbL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1007 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OFFIS.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OFL-1.0-RFN.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OFL-1.0-no-RFN.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3858 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OFL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OFL-1.1-RFN.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OFL-1.1-no-RFN.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4016 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OFL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2179 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OGC-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11606 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OGDL-Taiwan-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3679 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OGL-Canada-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6080 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OGL-UK-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5980 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OGL-UK-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6220 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OGL-UK-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5277 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OGTSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5393 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5396 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5795 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-1.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5873 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-1.4.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1977 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.0.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1981 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2220 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2241 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2267 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.2.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2228 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2265 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2124 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.4.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2171 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2109 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.6.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2197 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.7.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2195 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OLDAP-2.8.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1689 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OML.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20309 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6148 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OPUBL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    19967 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OSET-PL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8921 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9663 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OSL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9880 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OSL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9872 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OSL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10319 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OSL-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1447 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OpenJDK-assembly-exception-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3962 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OpenPBS-2.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     5309 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/OpenSSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    15485 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/PDDL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2846 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/PHP-3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2855 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/PHP-3.01.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      439 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/PS-or-PDF-font-exception-20170817.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2427 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/PSF-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1704 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Parity-6.0.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3524 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Parity-7.0.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1849 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Plexus.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4563 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/PolyForm-Noncommercial-1.0.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4389 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/PolyForm-Small-Business-1.0.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1195 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/PostgreSQL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9916 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Python-2.0.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9411 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Python-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      334 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/QPL-1.0-INRIA-2004-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4641 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/QPL-1.0-INRIA-2004.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4364 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/QPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1304 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Qhull.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      964 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Qt-GPL-exception-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1195 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Qt-LGPL-exception-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1199 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Qwt-exception-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21641 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/RHeCos-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    33931 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/RPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    32009 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/RPL-1.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    30271 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/RPSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      869 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/RSA-MD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21050 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/RSCPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1107 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Rdisc.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2137 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Ruby.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2315 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SAX-PD.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6638 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SCEA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13553 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SGI-B-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14556 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SGI-B-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1503 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SGI-B-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11386 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SHL-0.5.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11399 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SHL-0.51.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2776 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SHL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4485 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SHL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    12474 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SISSL-1.2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    14496 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SISSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1122 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SMLNJ.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3177 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SMPPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    21717 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SNIA.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    23398 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3399 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SSH-OpenSSH.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      326 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SSH-short.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    30609 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SSPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      382 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SWI-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2129 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SWL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2133 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Saxpath.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      290 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SchemeReport.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4020 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Sendmail-8.23.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3948 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Sendmail.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2529 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SimPL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4995 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Sleepycat.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      628 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Spencer-86.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      935 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Spencer-94.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1376 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Spencer-99.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    22087 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SugarCRM-1.1.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      246 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/SunPro.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      355 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Swift-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      515 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Symlinks.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    13932 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TAPR-OHL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2251 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TCL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      648 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TCP-wrappers.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2537 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TMate.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3998 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TORQUE-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2074 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TOSL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      233 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TPDL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    23787 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      406 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TTWL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      678 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TU-Berlin-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1369 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/TU-Berlin-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1948 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/UCAR.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10566 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/UCL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1837 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/UPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2873 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Unicode-DFS-2015.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2858 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Unicode-DFS-2016.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     6261 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Unicode-TOU.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3154 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Universal-FOSS-exception-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1211 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Unlicense.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3058 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/VOSTROM.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2065 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/VSL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4525 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Vim.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3116 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/W3C-19980720.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1807 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/W3C-20150513.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2701 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/W3C.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      432 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/WTFPL.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20972 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Watcom-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      529 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Wsuipa.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1267 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/WxWindows-exception-3.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1314 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/X11-distribute-modifications-variant.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1338 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/X11.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2398 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/XFree86-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      535 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/XSkat.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      963 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Xerox.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1186 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Xnet.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     9010 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/YPL-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8988 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/YPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2924 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ZPL-1.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2275 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ZPL-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2100 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/ZPL-2.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      259 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Zed.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2490 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Zend-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8994 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Zimbra-1.3.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8947 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Zimbra-1.4.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      838 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/Zlib.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      244 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/blessing.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1739 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/bzip2-1.0.6.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      435 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/checkmk.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10571 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/copyleft-next-0.3.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    10634 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/copyleft-next-0.3.1.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1043 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/curl.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       88 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/diffmark.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      210 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/dvipdfm.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      575 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/eCos-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4235 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/eGenix.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     8198 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/etalab-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1687 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/freertos-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    20362 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/gSOAP-1.3b.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      341 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/gnu-javamail-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1407 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/gnuplot.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      605 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/i2p-gpl-java-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3473 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/iMatix.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1550 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/libpng-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1034 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/libselinux-1.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1139 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/libtiff.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      915 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/libutil-David-Nugent.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      529 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/mif-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      583 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/mpi-permissive.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1424 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/mpich2.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      226 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/mplus.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      629 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/openvpn-openssl-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      480 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/psfrag.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1961 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/psutils.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      209 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/snprintf.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      629 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/u-boot-exception-2.0.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      568 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/w3m.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      591 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/x11vnc-openssl-exception.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2030 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/xinetd.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      734 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/xlock.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2482 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/xpp.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1133 2024-04-12 06:16:56.000000 oslili-0.9/oslili/spdx/zlib-acknowledgement.txt
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-14 23:07:32.973956 oslili-0.9/oslili.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3022 2024-04-14 23:07:32.000000 oslili-0.9/oslili.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    16059 2024-04-14 23:07:32.000000 oslili-0.9/oslili.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-04-14 23:07:32.000000 oslili-0.9/oslili.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       20 2024-04-14 23:07:32.000000 oslili-0.9/oslili.egg-info/requires.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        7 2024-04-14 23:07:32.000000 oslili-0.9/oslili.egg-info/top_level.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       79 2024-04-14 23:07:32.974495 oslili-0.9/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1062 2024-04-14 22:58:28.000000 oslili-0.9/setup.py
```

### Comparing `oslili-0.8/LICENSE` & `oslili-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oslili-0.8/PKG-INFO` & `oslili-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslili
-Version: 0.8
+Version: 0.9
 Summary: Open Source License Identification Library
 Home-page: https://github.com/oscarvalenzuelab/oslili
 Author: Oscar Valenzuela B.
 Author-email: alkamod@gmail.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `oslili-0.8/README.md` & `oslili-0.9/README.md`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/identifier.py` & `oslili-0.9/oslili/identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,44 +52,42 @@
             self.classifier.fit(X, y)
 
             with open(self.cache_file, 'wb') as f:
                 pickle.dump((self.vectorizer, self.classifier), f)
 
     def normilize_text(self, text):
         # remove copyright
-        pattern = re.compile(r'(?i)copyright\s+\d{4}(\s*-\s*\d{4})?', re.MULTILINE)
+        pattern = re.compile(
+            r'(?i)copyright\s+\d{4}(\s*-\s*\d{4})?', re.MULTILINE
+        )
         text = re.sub(pattern, '', text)
         text = text.lower().strip()
         # Remove non-alpha
         text = re.sub('[^0-9a-zA-Z]+', ' ', text)
         # collapse_whitespace
         text = re.sub(' +', ' ', text)
         return text
 
     def store_hashes(self, hashfile, idxstr, hashstr):
         str_hash = idxstr + "|" + hashstr
         with open(hashfile, 'a+') as file:
-                file.seek(0)
-                if str_hash + '\n' not in file.readlines():
-                    file.write(str_hash + '\n')
+            file.seek(0)
+            if str_hash + '\n' not in file.readlines():
+                file.write(str_hash + '\n')
 
     def identify_license(self, text):
         text = self.normilize_text(text)
         X = self.vectorizer.transform([text])
-        predicted_class = self.classifier.predict(X)
+        predicted_class = self.classifier.predict(X)[0]
         predicted_proba = self.classifier.predict_proba(X)[0]
-
-        # Getting the index of the predicted class in the list of classes
-        class_index = self.classifier.classes_.tolist().index(predicted_class[0])
-
-        # Check if the highest probability is less than 50%
+        class_index = self.classifier.classes_.tolist().index(predicted_class)
         if predicted_proba[class_index] < 0.5:
-            return '', 0.0  # Return empty string and 0 probability if less than 50%
+            return '', 0.0
         else:
-            return predicted_class[0], predicted_proba[class_index]
+            return predicted_class, predicted_proba[class_index]
 
 
 class CopyrightIdentifier:
     def __init__(self):
         self.year_range_pattern = re.compile(
                                     r'(\d{4}\s*(?:-|\s+to\s+)\s*\d{4}|\d{4})')
```

### Comparing `oslili-0.8/oslili/spdx/0BSD.txt` & `oslili-0.9/oslili/spdx/0BSD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/389-exception.txt` & `oslili-0.9/oslili/spdx/389-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AAL.txt` & `oslili-0.9/oslili/spdx/AAL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AFL-1.1.txt` & `oslili-0.9/oslili/spdx/AFL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AFL-1.2.txt` & `oslili-0.9/oslili/spdx/AFL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AFL-2.0.txt` & `oslili-0.9/oslili/spdx/AFL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AFL-2.1.txt` & `oslili-0.9/oslili/spdx/AFL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AFL-3.0.txt` & `oslili-0.9/oslili/spdx/AFL-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AGPL-1.0-only.txt` & `oslili-0.9/oslili/spdx/AGPL-1.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AGPL-1.0-or-later.txt` & `oslili-0.9/oslili/spdx/AGPL-1.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AGPL-3.0-only.txt` & `oslili-0.9/oslili/spdx/AGPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AGPL-3.0-or-later.txt` & `oslili-0.9/oslili/spdx/AGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AMDPLPA.txt` & `oslili-0.9/oslili/spdx/AMDPLPA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AML.txt` & `oslili-0.9/oslili/spdx/AML.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/AMPAS.txt` & `oslili-0.9/oslili/spdx/AMPAS.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ANTLR-PD-fallback.txt` & `oslili-0.9/oslili/spdx/ANTLR-PD-fallback.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ANTLR-PD.txt` & `oslili-0.9/oslili/spdx/ANTLR-PD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/APAFML.txt` & `oslili-0.9/oslili/spdx/APAFML.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/APL-1.0.txt` & `oslili-0.9/oslili/spdx/APL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/APSL-1.0.txt` & `oslili-0.9/oslili/spdx/APSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/APSL-1.1.txt` & `oslili-0.9/oslili/spdx/APSL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/APSL-1.2.txt` & `oslili-0.9/oslili/spdx/APSL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/APSL-2.0.txt` & `oslili-0.9/oslili/spdx/APSL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Abstyles.txt` & `oslili-0.9/oslili/spdx/Abstyles.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Adobe-2006.txt` & `oslili-0.9/oslili/spdx/Adobe-2006.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Adobe-Glyph.txt` & `oslili-0.9/oslili/spdx/Adobe-Glyph.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Afmparse.txt` & `oslili-0.9/oslili/spdx/Afmparse.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Aladdin.txt` & `oslili-0.9/oslili/spdx/Aladdin.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Apache-1.0.txt` & `oslili-0.9/oslili/spdx/Apache-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Apache-1.1.txt` & `oslili-0.9/oslili/spdx/Apache-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Apache-2.0.txt` & `oslili-0.9/oslili/spdx/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Arphic-1999.txt` & `oslili-0.9/oslili/spdx/Arphic-1999.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Artistic-1.0-Perl.txt` & `oslili-0.9/oslili/spdx/Artistic-1.0-Perl.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Artistic-1.0-cl8.txt` & `oslili-0.9/oslili/spdx/Artistic-1.0-cl8.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Artistic-1.0.txt` & `oslili-0.9/oslili/spdx/Artistic-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Artistic-2.0.txt` & `oslili-0.9/oslili/spdx/Artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Autoconf-exception-2.0.txt` & `oslili-0.9/oslili/spdx/Autoconf-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Autoconf-exception-3.0.txt` & `oslili-0.9/oslili/spdx/Autoconf-exception-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Autoconf-exception-macro.txt` & `oslili-0.9/oslili/spdx/Autoconf-exception-macro.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-1-Clause.txt` & `oslili-0.9/oslili/spdx/BSD-1-Clause.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-2-Clause-Patent.txt` & `oslili-0.9/oslili/spdx/BSD-2-Clause-Patent.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-2-Clause-Views.txt` & `oslili-0.9/oslili/spdx/BSD-2-Clause-Views.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-2-Clause.txt` & `oslili-0.9/oslili/spdx/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-3-Clause-Attribution.txt` & `oslili-0.9/oslili/spdx/BSD-3-Clause-Attribution.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-3-Clause-Clear.txt` & `oslili-0.9/oslili/spdx/BSD-3-Clause-Clear.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-3-Clause-LBNL.txt` & `oslili-0.9/oslili/spdx/BSD-3-Clause-LBNL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-3-Clause-Modification.txt` & `oslili-0.9/oslili/spdx/BSD-3-Clause-Modification.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-3-Clause-No-Military-License.txt` & `oslili-0.9/oslili/spdx/BSD-3-Clause-No-Military-License.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-3-Clause-No-Nuclear-License-2014.txt` & `oslili-0.9/oslili/spdx/BSD-3-Clause-No-Nuclear-License-2014.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-3-Clause-No-Nuclear-License.txt` & `oslili-0.9/oslili/spdx/BSD-3-Clause-No-Nuclear-License.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-3-Clause-No-Nuclear-Warranty.txt` & `oslili-0.9/oslili/spdx/BSD-3-Clause-No-Nuclear-Warranty.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-3-Clause-Open-MPI.txt` & `oslili-0.9/oslili/spdx/BSD-3-Clause-Open-MPI.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-3-Clause.txt` & `oslili-0.9/oslili/spdx/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-4-Clause-Shortened.txt` & `oslili-0.9/oslili/spdx/BSD-4-Clause-Shortened.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-4-Clause-UC.txt` & `oslili-0.9/oslili/spdx/BSD-4-Clause-UC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-4-Clause.txt` & `oslili-0.9/oslili/spdx/BSD-4-Clause.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-4.3TAHOE.txt` & `oslili-0.9/oslili/spdx/BSD-4.3TAHOE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-Advertising-Acknowledgement.txt` & `oslili-0.9/oslili/spdx/BSD-Advertising-Acknowledgement.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-Attribution-HPND-disclaimer.txt` & `oslili-0.9/oslili/spdx/BSD-Attribution-HPND-disclaimer.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-Protection.txt` & `oslili-0.9/oslili/spdx/BSD-Protection.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSD-Source-Code.txt` & `oslili-0.9/oslili/spdx/BSD-Source-Code.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BSL-1.0.txt` & `oslili-0.9/oslili/spdx/BSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BUSL-1.1.txt` & `oslili-0.9/oslili/spdx/BUSL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Bahyph.txt` & `oslili-0.9/oslili/spdx/Bahyph.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Barr.txt` & `oslili-0.9/oslili/spdx/Barr.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Bison-exception-2.2.txt` & `oslili-0.9/oslili/spdx/Bison-exception-2.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BitTorrent-1.0.txt` & `oslili-0.9/oslili/spdx/BitTorrent-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BitTorrent-1.1.txt` & `oslili-0.9/oslili/spdx/BitTorrent-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Bitstream-Charter.txt` & `oslili-0.9/oslili/spdx/Bitstream-Charter.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Bitstream-Vera.txt` & `oslili-0.9/oslili/spdx/Bitstream-Vera.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/BlueOak-1.0.0.txt` & `oslili-0.9/oslili/spdx/BlueOak-1.0.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Bootloader-exception.txt` & `oslili-0.9/oslili/spdx/Bootloader-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Borceux.txt` & `oslili-0.9/oslili/spdx/Borceux.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Brian-Gladman-3-Clause.txt` & `oslili-0.9/oslili/spdx/Brian-Gladman-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/C-UDA-1.0.txt` & `oslili-0.9/oslili/spdx/C-UDA-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CAL-1.0-Combined-Work-Exception.txt` & `oslili-0.9/oslili/spdx/CAL-1.0-Combined-Work-Exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CAL-1.0.txt` & `oslili-0.9/oslili/spdx/CAL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CATOSL-1.1.txt` & `oslili-0.9/oslili/spdx/CATOSL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-1.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-2.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-2.5-AU.txt` & `oslili-0.9/oslili/spdx/CC-BY-2.5-AU.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-2.5.txt` & `oslili-0.9/oslili/spdx/CC-BY-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-3.0-AT.txt` & `oslili-0.9/oslili/spdx/CC-BY-3.0-AT.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-3.0-DE.txt` & `oslili-0.9/oslili/spdx/CC-BY-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-3.0-IGO.txt` & `oslili-0.9/oslili/spdx/CC-BY-3.0-IGO.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-3.0-NL.txt` & `oslili-0.9/oslili/spdx/CC-BY-3.0-NL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-3.0-US.txt` & `oslili-0.9/oslili/spdx/CC-BY-3.0-US.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-3.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-4.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-1.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-2.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-2.5.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-3.0-DE.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-3.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-4.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-ND-1.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-ND-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-ND-2.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-ND-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-ND-2.5.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-ND-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-ND-3.0-DE.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-ND-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-ND-3.0-IGO.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-ND-3.0-IGO.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-ND-3.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-ND-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-ND-4.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-ND-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-SA-1.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-SA-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-SA-2.0-DE.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-SA-2.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-SA-2.0-FR.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-SA-2.0-FR.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-SA-2.0-UK.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-SA-2.0-UK.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-SA-2.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-SA-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-SA-2.5.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-SA-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-SA-3.0-DE.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-SA-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-SA-3.0-IGO.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-SA-3.0-IGO.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-SA-3.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-SA-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-NC-SA-4.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-NC-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-ND-1.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-ND-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-ND-2.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-ND-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-ND-2.5.txt` & `oslili-0.9/oslili/spdx/CC-BY-ND-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-ND-3.0-DE.txt` & `oslili-0.9/oslili/spdx/CC-BY-ND-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-ND-3.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-ND-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-ND-4.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-ND-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-SA-1.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-SA-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-SA-2.0-UK.txt` & `oslili-0.9/oslili/spdx/CC-BY-SA-2.0-UK.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-SA-2.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-SA-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-SA-2.1-JP.txt` & `oslili-0.9/oslili/spdx/CC-BY-SA-2.1-JP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-SA-2.5.txt` & `oslili-0.9/oslili/spdx/CC-BY-SA-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-SA-3.0-AT.txt` & `oslili-0.9/oslili/spdx/CC-BY-SA-3.0-AT.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-SA-3.0-DE.txt` & `oslili-0.9/oslili/spdx/CC-BY-SA-3.0-DE.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-SA-3.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-SA-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-BY-SA-4.0.txt` & `oslili-0.9/oslili/spdx/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC-PDDC.txt` & `oslili-0.9/oslili/spdx/CC-PDDC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CC0-1.0.txt` & `oslili-0.9/oslili/spdx/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CDDL-1.0.txt` & `oslili-0.9/oslili/spdx/CDDL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CDDL-1.1.txt` & `oslili-0.9/oslili/spdx/CDDL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CDL-1.0.txt` & `oslili-0.9/oslili/spdx/CDL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CDLA-Permissive-1.0.txt` & `oslili-0.9/oslili/spdx/CDLA-Permissive-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CDLA-Permissive-2.0.txt` & `oslili-0.9/oslili/spdx/CDLA-Permissive-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CDLA-Sharing-1.0.txt` & `oslili-0.9/oslili/spdx/CDLA-Sharing-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CECILL-1.0.txt` & `oslili-0.9/oslili/spdx/CECILL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CECILL-1.1.txt` & `oslili-0.9/oslili/spdx/CECILL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CECILL-2.0.txt` & `oslili-0.9/oslili/spdx/CECILL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CECILL-2.1.txt` & `oslili-0.9/oslili/spdx/CECILL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CECILL-B.txt` & `oslili-0.9/oslili/spdx/CECILL-B.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CECILL-C.txt` & `oslili-0.9/oslili/spdx/CECILL-C.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CERN-OHL-1.1.txt` & `oslili-0.9/oslili/spdx/CERN-OHL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CERN-OHL-1.2.txt` & `oslili-0.9/oslili/spdx/CERN-OHL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CERN-OHL-P-2.0.txt` & `oslili-0.9/oslili/spdx/CERN-OHL-P-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CERN-OHL-S-2.0.txt` & `oslili-0.9/oslili/spdx/CERN-OHL-S-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CERN-OHL-W-2.0.txt` & `oslili-0.9/oslili/spdx/CERN-OHL-W-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CFITSIO.txt` & `oslili-0.9/oslili/spdx/CFITSIO.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CLISP-exception-2.0.txt` & `oslili-0.9/oslili/spdx/CLISP-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CMU-Mach.txt` & `oslili-0.9/oslili/spdx/CMU-Mach.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CNRI-Jython.txt` & `oslili-0.9/oslili/spdx/CNRI-Jython.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CNRI-Python-GPL-Compatible.txt` & `oslili-0.9/oslili/spdx/CNRI-Python-GPL-Compatible.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CNRI-Python.txt` & `oslili-0.9/oslili/spdx/CNRI-Python.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/COIL-1.0.txt` & `oslili-0.9/oslili/spdx/COIL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CPAL-1.0.txt` & `oslili-0.9/oslili/spdx/CPAL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CPL-1.0.txt` & `oslili-0.9/oslili/spdx/CPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CPOL-1.02.txt` & `oslili-0.9/oslili/spdx/CPOL-1.02.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CUA-OPL-1.0.txt` & `oslili-0.9/oslili/spdx/CUA-OPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Caldera.txt` & `oslili-0.9/oslili/spdx/Caldera.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ClArtistic.txt` & `oslili-0.9/oslili/spdx/ClArtistic.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Classpath-exception-2.0.txt` & `oslili-0.9/oslili/spdx/Classpath-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Clips.txt` & `oslili-0.9/oslili/spdx/Clips.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Community-Spec-1.0.txt` & `oslili-0.9/oslili/spdx/Community-Spec-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Condor-1.1.txt` & `oslili-0.9/oslili/spdx/Condor-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Cornell-Lossless-JPEG.txt` & `oslili-0.9/oslili/spdx/Cornell-Lossless-JPEG.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/CrystalStacker.txt` & `oslili-0.9/oslili/spdx/CrystalStacker.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Cube.txt` & `oslili-0.9/oslili/spdx/Cube.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/D-FSL-1.0.txt` & `oslili-0.9/oslili/spdx/D-FSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/DL-DE-BY-2.0.txt` & `oslili-0.9/oslili/spdx/DL-DE-BY-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/DOC.txt` & `oslili-0.9/oslili/spdx/DOC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/DRL-1.0.txt` & `oslili-0.9/oslili/spdx/DRL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/DSDP.txt` & `oslili-0.9/oslili/spdx/DSDP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/DigiRule-FOSS-exception.txt` & `oslili-0.9/oslili/spdx/DigiRule-FOSS-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ECL-1.0.txt` & `oslili-0.9/oslili/spdx/ECL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ECL-2.0.txt` & `oslili-0.9/oslili/spdx/ECL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/EFL-1.0.txt` & `oslili-0.9/oslili/spdx/EFL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/EFL-2.0.txt` & `oslili-0.9/oslili/spdx/EFL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/EPICS.txt` & `oslili-0.9/oslili/spdx/EPICS.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/EPL-1.0.txt` & `oslili-0.9/oslili/spdx/EPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/EPL-2.0.txt` & `oslili-0.9/oslili/spdx/EPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/EUDatagrid.txt` & `oslili-0.9/oslili/spdx/EUDatagrid.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/EUPL-1.0.txt` & `oslili-0.9/oslili/spdx/EUPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/EUPL-1.1.txt` & `oslili-0.9/oslili/spdx/EUPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/EUPL-1.2.txt` & `oslili-0.9/oslili/spdx/EUPL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Elastic-2.0.txt` & `oslili-0.9/oslili/spdx/Elastic-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Entessa.txt` & `oslili-0.9/oslili/spdx/Entessa.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ErlPL-1.1.txt` & `oslili-0.9/oslili/spdx/ErlPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Eurosym.txt` & `oslili-0.9/oslili/spdx/Eurosym.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/FDK-AAC.txt` & `oslili-0.9/oslili/spdx/FDK-AAC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/FLTK-exception.txt` & `oslili-0.9/oslili/spdx/FLTK-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/FSFULLRWD.txt` & `oslili-0.9/oslili/spdx/FSFULLRWD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/FTL.txt` & `oslili-0.9/oslili/spdx/FTL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Fawkes-Runtime-exception.txt` & `oslili-0.9/oslili/spdx/Fawkes-Runtime-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Font-exception-2.0.txt` & `oslili-0.9/oslili/spdx/Font-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Frameworx-1.0.txt` & `oslili-0.9/oslili/spdx/Frameworx-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/FreeBSD-DOC.txt` & `oslili-0.9/oslili/spdx/FreeBSD-DOC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/FreeImage.txt` & `oslili-0.9/oslili/spdx/FreeImage.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GCC-exception-3.1.txt` & `oslili-0.9/oslili/spdx/GCC-exception-3.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GD.txt` & `oslili-0.9/oslili/spdx/GD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.1-invariants-only.txt` & `oslili-0.9/oslili/spdx/GFDL-1.1-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.1-invariants-or-later.txt` & `oslili-0.9/oslili/spdx/GFDL-1.1-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.1-no-invariants-only.txt` & `oslili-0.9/oslili/spdx/GFDL-1.1-no-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.1-no-invariants-or-later.txt` & `oslili-0.9/oslili/spdx/GFDL-1.1-no-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.1-only.txt` & `oslili-0.9/oslili/spdx/GFDL-1.1-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.1-or-later.txt` & `oslili-0.9/oslili/spdx/GFDL-1.1-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.2-invariants-only.txt` & `oslili-0.9/oslili/spdx/GFDL-1.2-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.2-invariants-or-later.txt` & `oslili-0.9/oslili/spdx/GFDL-1.2-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.2-no-invariants-only.txt` & `oslili-0.9/oslili/spdx/GFDL-1.2-no-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.2-no-invariants-or-later.txt` & `oslili-0.9/oslili/spdx/GFDL-1.2-no-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.2-only.txt` & `oslili-0.9/oslili/spdx/GFDL-1.2-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.2-or-later.txt` & `oslili-0.9/oslili/spdx/GFDL-1.2-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.3-invariants-only.txt` & `oslili-0.9/oslili/spdx/GFDL-1.3-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.3-invariants-or-later.txt` & `oslili-0.9/oslili/spdx/GFDL-1.3-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.3-no-invariants-only.txt` & `oslili-0.9/oslili/spdx/GFDL-1.3-no-invariants-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.3-no-invariants-or-later.txt` & `oslili-0.9/oslili/spdx/GFDL-1.3-no-invariants-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.3-only.txt` & `oslili-0.9/oslili/spdx/GFDL-1.3-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GFDL-1.3-or-later.txt` & `oslili-0.9/oslili/spdx/GFDL-1.3-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GL2PS.txt` & `oslili-0.9/oslili/spdx/GL2PS.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GLWTPL.txt` & `oslili-0.9/oslili/spdx/GLWTPL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GPL-1.0-only.txt` & `oslili-0.9/oslili/spdx/GPL-1.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GPL-1.0-or-later.txt` & `oslili-0.9/oslili/spdx/GPL-1.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GPL-2.0-only.txt` & `oslili-0.9/oslili/spdx/GPL-2.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GPL-2.0-or-later.txt` & `oslili-0.9/oslili/spdx/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GPL-3.0-linking-source-exception.txt` & `oslili-0.9/oslili/spdx/GPL-3.0-linking-source-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GPL-3.0-only.txt` & `oslili-0.9/oslili/spdx/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GPL-3.0-or-later.txt` & `oslili-0.9/oslili/spdx/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/GPL-CC-1.0.txt` & `oslili-0.9/oslili/spdx/GPL-CC-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Giftware.txt` & `oslili-0.9/oslili/spdx/Giftware.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Glide.txt` & `oslili-0.9/oslili/spdx/Glide.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Graphics-Gems.txt` & `oslili-0.9/oslili/spdx/Graphics-Gems.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/HP-1986.txt` & `oslili-0.9/oslili/spdx/HP-1986.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/HPND-export-US.txt` & `oslili-0.9/oslili/spdx/HPND-export-US.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/HPND-sell-variant-MIT-disclaimer.txt` & `oslili-0.9/oslili/spdx/HPND-sell-variant-MIT-disclaimer.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/HPND-sell-variant.txt` & `oslili-0.9/oslili/spdx/HPND-sell-variant.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/HPND.txt` & `oslili-0.9/oslili/spdx/HPND.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/HTMLTIDY.txt` & `oslili-0.9/oslili/spdx/HTMLTIDY.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/HaskellReport.txt` & `oslili-0.9/oslili/spdx/HaskellReport.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Hippocratic-2.1.txt` & `oslili-0.9/oslili/spdx/Hippocratic-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/IBM-pibs.txt` & `oslili-0.9/oslili/spdx/IBM-pibs.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ICU.txt` & `oslili-0.9/oslili/spdx/ICU.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/IEC-Code-Components-EULA.txt` & `oslili-0.9/oslili/spdx/IEC-Code-Components-EULA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/IJG-short.txt` & `oslili-0.9/oslili/spdx/IJG-short.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/IJG.txt` & `oslili-0.9/oslili/spdx/IJG.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/IPA.txt` & `oslili-0.9/oslili/spdx/IPA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/IPL-1.0.txt` & `oslili-0.9/oslili/spdx/IPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ISC.txt` & `oslili-0.9/oslili/spdx/ISC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ImageMagick.txt` & `oslili-0.9/oslili/spdx/ImageMagick.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Imlib2.txt` & `oslili-0.9/oslili/spdx/Imlib2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Info-ZIP.txt` & `oslili-0.9/oslili/spdx/Info-ZIP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Intel-ACPI.txt` & `oslili-0.9/oslili/spdx/Intel-ACPI.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Intel.txt` & `oslili-0.9/oslili/spdx/Intel.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Interbase-1.0.txt` & `oslili-0.9/oslili/spdx/Interbase-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/JPL-image.txt` & `oslili-0.9/oslili/spdx/JPL-image.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/JPNIC.txt` & `oslili-0.9/oslili/spdx/JPNIC.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/JSON.txt` & `oslili-0.9/oslili/spdx/JSON.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/JasPer-2.0.txt` & `oslili-0.9/oslili/spdx/JasPer-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Kazlib.txt` & `oslili-0.9/oslili/spdx/Kazlib.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LAL-1.2.txt` & `oslili-0.9/oslili/spdx/LAL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LAL-1.3.txt` & `oslili-0.9/oslili/spdx/LAL-1.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LGPL-2.0-only.txt` & `oslili-0.9/oslili/spdx/LGPL-2.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LGPL-2.0-or-later.txt` & `oslili-0.9/oslili/spdx/LGPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LGPL-2.1-only.txt` & `oslili-0.9/oslili/spdx/LGPL-2.1-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LGPL-2.1-or-later.txt` & `oslili-0.9/oslili/spdx/LGPL-2.1-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LGPL-3.0-linking-exception.txt` & `oslili-0.9/oslili/spdx/LGPL-3.0-linking-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LGPL-3.0-only.txt` & `oslili-0.9/oslili/spdx/LGPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LGPL-3.0-or-later.txt` & `oslili-0.9/oslili/spdx/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LGPLLR.txt` & `oslili-0.9/oslili/spdx/LGPLLR.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LLVM-exception.txt` & `oslili-0.9/oslili/spdx/LLVM-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LOOP.txt` & `oslili-0.9/oslili/spdx/LOOP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LPL-1.0.txt` & `oslili-0.9/oslili/spdx/LPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LPL-1.02.txt` & `oslili-0.9/oslili/spdx/LPL-1.02.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LPPL-1.0.txt` & `oslili-0.9/oslili/spdx/LPPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LPPL-1.1.txt` & `oslili-0.9/oslili/spdx/LPPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LPPL-1.2.txt` & `oslili-0.9/oslili/spdx/LPPL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LPPL-1.3a.txt` & `oslili-0.9/oslili/spdx/LPPL-1.3a.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LPPL-1.3c.txt` & `oslili-0.9/oslili/spdx/LPPL-1.3c.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LZMA-SDK-9.22.txt` & `oslili-0.9/oslili/spdx/LZMA-SDK-9.22.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LZMA-exception.txt` & `oslili-0.9/oslili/spdx/LZMA-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Latex2e.txt` & `oslili-0.9/oslili/spdx/Latex2e.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Leptonica.txt` & `oslili-0.9/oslili/spdx/Leptonica.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LiLiQ-P-1.1.txt` & `oslili-0.9/oslili/spdx/LiLiQ-P-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LiLiQ-R-1.1.txt` & `oslili-0.9/oslili/spdx/LiLiQ-R-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/LiLiQ-Rplus-1.1.txt` & `oslili-0.9/oslili/spdx/LiLiQ-Rplus-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Libpng.txt` & `oslili-0.9/oslili/spdx/Libpng.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Linux-OpenIB.txt` & `oslili-0.9/oslili/spdx/Linux-OpenIB.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Linux-man-pages-copyleft.txt` & `oslili-0.9/oslili/spdx/Linux-man-pages-copyleft.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Linux-syscall-note.txt` & `oslili-0.9/oslili/spdx/Linux-syscall-note.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MIT-0.txt` & `oslili-0.9/oslili/spdx/MIT-0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MIT-CMU.txt` & `oslili-0.9/oslili/spdx/MIT-CMU.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MIT-Modern-Variant.txt` & `oslili-0.9/oslili/spdx/MIT-Modern-Variant.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MIT-Wu.txt` & `oslili-0.9/oslili/spdx/MIT-Wu.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MIT-advertising.txt` & `oslili-0.9/oslili/spdx/MIT-advertising.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MIT-enna.txt` & `oslili-0.9/oslili/spdx/MIT-enna.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MIT-feh.txt` & `oslili-0.9/oslili/spdx/MIT-feh.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MIT-open-group.txt` & `oslili-0.9/oslili/spdx/MIT-open-group.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MIT.txt` & `oslili-0.9/oslili/spdx/MIT.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MITNFA.txt` & `oslili-0.9/oslili/spdx/MITNFA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MPL-1.0.txt` & `oslili-0.9/oslili/spdx/MPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MPL-1.1.txt` & `oslili-0.9/oslili/spdx/MPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MPL-2.0-no-copyleft-exception.txt` & `oslili-0.9/oslili/spdx/MPL-2.0-no-copyleft-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MPL-2.0.txt` & `oslili-0.9/oslili/spdx/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MS-LPL.txt` & `oslili-0.9/oslili/spdx/MS-LPL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MS-PL.txt` & `oslili-0.9/oslili/spdx/MS-PL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MS-RL.txt` & `oslili-0.9/oslili/spdx/MS-RL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MTLL.txt` & `oslili-0.9/oslili/spdx/MTLL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MakeIndex.txt` & `oslili-0.9/oslili/spdx/MakeIndex.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Minpack.txt` & `oslili-0.9/oslili/spdx/Minpack.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MirOS.txt` & `oslili-0.9/oslili/spdx/MirOS.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Motosoto.txt` & `oslili-0.9/oslili/spdx/Motosoto.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MulanPSL-1.0.txt` & `oslili-0.9/oslili/spdx/MulanPSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/MulanPSL-2.0.txt` & `oslili-0.9/oslili/spdx/MulanPSL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Multics.txt` & `oslili-0.9/oslili/spdx/Multics.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Mup.txt` & `oslili-0.9/oslili/spdx/Mup.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NAIST-2003.txt` & `oslili-0.9/oslili/spdx/NAIST-2003.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NASA-1.3.txt` & `oslili-0.9/oslili/spdx/NASA-1.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NBPL-1.0.txt` & `oslili-0.9/oslili/spdx/NBPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NCGL-UK-2.0.txt` & `oslili-0.9/oslili/spdx/NCGL-UK-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NCSA.txt` & `oslili-0.9/oslili/spdx/NCSA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NGPL.txt` & `oslili-0.9/oslili/spdx/NGPL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NICTA-1.0.txt` & `oslili-0.9/oslili/spdx/NICTA-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NIST-PD-fallback.txt` & `oslili-0.9/oslili/spdx/NIST-PD-fallback.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NIST-PD.txt` & `oslili-0.9/oslili/spdx/NIST-PD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NLOD-1.0.txt` & `oslili-0.9/oslili/spdx/NLOD-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NLOD-2.0.txt` & `oslili-0.9/oslili/spdx/NLOD-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NOSL.txt` & `oslili-0.9/oslili/spdx/NOSL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NPL-1.0.txt` & `oslili-0.9/oslili/spdx/NPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NPL-1.1.txt` & `oslili-0.9/oslili/spdx/NPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NPOSL-3.0.txt` & `oslili-0.9/oslili/spdx/NPOSL-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NRL.txt` & `oslili-0.9/oslili/spdx/NRL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NTP-0.txt` & `oslili-0.9/oslili/spdx/NTP-0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NTP.txt` & `oslili-0.9/oslili/spdx/NTP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Naumen.txt` & `oslili-0.9/oslili/spdx/Naumen.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Net-SNMP.txt` & `oslili-0.9/oslili/spdx/Net-SNMP.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/NetCDF.txt` & `oslili-0.9/oslili/spdx/NetCDF.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Nokia-Qt-exception-1.1.txt` & `oslili-0.9/oslili/spdx/Nokia-Qt-exception-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Nokia.txt` & `oslili-0.9/oslili/spdx/Nokia.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Noweb.txt` & `oslili-0.9/oslili/spdx/Noweb.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/O-UDA-1.0.txt` & `oslili-0.9/oslili/spdx/O-UDA-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OCCT-PL.txt` & `oslili-0.9/oslili/spdx/OCCT-PL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OCCT-exception-1.0.txt` & `oslili-0.9/oslili/spdx/OCCT-exception-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OCLC-2.0.txt` & `oslili-0.9/oslili/spdx/OCLC-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OCaml-LGPL-linking-exception.txt` & `oslili-0.9/oslili/spdx/OCaml-LGPL-linking-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ODC-By-1.0.txt` & `oslili-0.9/oslili/spdx/ODC-By-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ODbL-1.0.txt` & `oslili-0.9/oslili/spdx/ODbL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OFFIS.txt` & `oslili-0.9/oslili/spdx/OFFIS.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OFL-1.0-RFN.txt` & `oslili-0.9/oslili/spdx/OFL-1.0-RFN.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OFL-1.0-no-RFN.txt` & `oslili-0.9/oslili/spdx/OFL-1.0-no-RFN.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OFL-1.0.txt` & `oslili-0.9/oslili/spdx/OFL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OFL-1.1-RFN.txt` & `oslili-0.9/oslili/spdx/OFL-1.1-RFN.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OFL-1.1-no-RFN.txt` & `oslili-0.9/oslili/spdx/OFL-1.1-no-RFN.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OFL-1.1.txt` & `oslili-0.9/oslili/spdx/OFL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OGC-1.0.txt` & `oslili-0.9/oslili/spdx/OGC-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OGDL-Taiwan-1.0.txt` & `oslili-0.9/oslili/spdx/OGDL-Taiwan-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OGL-Canada-2.0.txt` & `oslili-0.9/oslili/spdx/OGL-Canada-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OGL-UK-1.0.txt` & `oslili-0.9/oslili/spdx/OGL-UK-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OGL-UK-2.0.txt` & `oslili-0.9/oslili/spdx/OGL-UK-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OGL-UK-3.0.txt` & `oslili-0.9/oslili/spdx/OGL-UK-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OGTSL.txt` & `oslili-0.9/oslili/spdx/OGTSL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-1.1.txt` & `oslili-0.9/oslili/spdx/OLDAP-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-1.2.txt` & `oslili-0.9/oslili/spdx/OLDAP-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-1.3.txt` & `oslili-0.9/oslili/spdx/OLDAP-1.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-1.4.txt` & `oslili-0.9/oslili/spdx/OLDAP-1.4.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.0.1.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.0.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.0.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.1.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.2.1.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.2.2.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.2.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.2.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.3.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.4.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.4.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.5.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.6.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.6.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.7.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.7.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OLDAP-2.8.txt` & `oslili-0.9/oslili/spdx/OLDAP-2.8.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OML.txt` & `oslili-0.9/oslili/spdx/OML.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OPL-1.0.txt` & `oslili-0.9/oslili/spdx/OPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OPUBL-1.0.txt` & `oslili-0.9/oslili/spdx/OPUBL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OSET-PL-2.1.txt` & `oslili-0.9/oslili/spdx/OSET-PL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OSL-1.0.txt` & `oslili-0.9/oslili/spdx/OSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OSL-1.1.txt` & `oslili-0.9/oslili/spdx/OSL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OSL-2.0.txt` & `oslili-0.9/oslili/spdx/OSL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OSL-2.1.txt` & `oslili-0.9/oslili/spdx/OSL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OSL-3.0.txt` & `oslili-0.9/oslili/spdx/OSL-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OpenJDK-assembly-exception-1.0.txt` & `oslili-0.9/oslili/spdx/OpenJDK-assembly-exception-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OpenPBS-2.3.txt` & `oslili-0.9/oslili/spdx/OpenPBS-2.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/OpenSSL.txt` & `oslili-0.9/oslili/spdx/OpenSSL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/PDDL-1.0.txt` & `oslili-0.9/oslili/spdx/PDDL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/PHP-3.0.txt` & `oslili-0.9/oslili/spdx/PHP-3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/PHP-3.01.txt` & `oslili-0.9/oslili/spdx/PHP-3.01.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/PSF-2.0.txt` & `oslili-0.9/oslili/spdx/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Parity-6.0.0.txt` & `oslili-0.9/oslili/spdx/Parity-6.0.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Parity-7.0.0.txt` & `oslili-0.9/oslili/spdx/Parity-7.0.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Plexus.txt` & `oslili-0.9/oslili/spdx/Plexus.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/PolyForm-Noncommercial-1.0.0.txt` & `oslili-0.9/oslili/spdx/PolyForm-Noncommercial-1.0.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/PolyForm-Small-Business-1.0.0.txt` & `oslili-0.9/oslili/spdx/PolyForm-Small-Business-1.0.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/PostgreSQL.txt` & `oslili-0.9/oslili/spdx/PostgreSQL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Python-2.0.1.txt` & `oslili-0.9/oslili/spdx/Python-2.0.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Python-2.0.txt` & `oslili-0.9/oslili/spdx/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/QPL-1.0-INRIA-2004.txt` & `oslili-0.9/oslili/spdx/QPL-1.0-INRIA-2004.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/QPL-1.0.txt` & `oslili-0.9/oslili/spdx/QPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Qhull.txt` & `oslili-0.9/oslili/spdx/Qhull.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Qt-GPL-exception-1.0.txt` & `oslili-0.9/oslili/spdx/Qt-GPL-exception-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Qt-LGPL-exception-1.1.txt` & `oslili-0.9/oslili/spdx/Qt-LGPL-exception-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Qwt-exception-1.0.txt` & `oslili-0.9/oslili/spdx/Qwt-exception-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/RHeCos-1.1.txt` & `oslili-0.9/oslili/spdx/RHeCos-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/RPL-1.1.txt` & `oslili-0.9/oslili/spdx/RPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/RPL-1.5.txt` & `oslili-0.9/oslili/spdx/RPL-1.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/RPSL-1.0.txt` & `oslili-0.9/oslili/spdx/RPSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/RSA-MD.txt` & `oslili-0.9/oslili/spdx/RSA-MD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/RSCPL.txt` & `oslili-0.9/oslili/spdx/RSCPL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Rdisc.txt` & `oslili-0.9/oslili/spdx/Rdisc.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Ruby.txt` & `oslili-0.9/oslili/spdx/Ruby.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SAX-PD.txt` & `oslili-0.9/oslili/spdx/SAX-PD.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SCEA.txt` & `oslili-0.9/oslili/spdx/SCEA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SGI-B-1.0.txt` & `oslili-0.9/oslili/spdx/SGI-B-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SGI-B-1.1.txt` & `oslili-0.9/oslili/spdx/SGI-B-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SGI-B-2.0.txt` & `oslili-0.9/oslili/spdx/SGI-B-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SHL-0.5.txt` & `oslili-0.9/oslili/spdx/SHL-0.5.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SHL-0.51.txt` & `oslili-0.9/oslili/spdx/SHL-0.51.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SHL-2.0.txt` & `oslili-0.9/oslili/spdx/SHL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SHL-2.1.txt` & `oslili-0.9/oslili/spdx/SHL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SISSL-1.2.txt` & `oslili-0.9/oslili/spdx/SISSL-1.2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SISSL.txt` & `oslili-0.9/oslili/spdx/SISSL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SMLNJ.txt` & `oslili-0.9/oslili/spdx/SMLNJ.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SMPPL.txt` & `oslili-0.9/oslili/spdx/SMPPL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SNIA.txt` & `oslili-0.9/oslili/spdx/SNIA.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SPL-1.0.txt` & `oslili-0.9/oslili/spdx/SPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SSH-OpenSSH.txt` & `oslili-0.9/oslili/spdx/SSH-OpenSSH.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SSPL-1.0.txt` & `oslili-0.9/oslili/spdx/SSPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SWL.txt` & `oslili-0.9/oslili/spdx/SWL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Saxpath.txt` & `oslili-0.9/oslili/spdx/Saxpath.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Sendmail-8.23.txt` & `oslili-0.9/oslili/spdx/Sendmail-8.23.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Sendmail.txt` & `oslili-0.9/oslili/spdx/Sendmail.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SimPL-2.0.txt` & `oslili-0.9/oslili/spdx/SimPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Sleepycat.txt` & `oslili-0.9/oslili/spdx/Sleepycat.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Spencer-86.txt` & `oslili-0.9/oslili/spdx/Spencer-86.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Spencer-94.txt` & `oslili-0.9/oslili/spdx/Spencer-94.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Spencer-99.txt` & `oslili-0.9/oslili/spdx/Spencer-99.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/SugarCRM-1.1.3.txt` & `oslili-0.9/oslili/spdx/SugarCRM-1.1.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Symlinks.txt` & `oslili-0.9/oslili/spdx/Symlinks.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/TAPR-OHL-1.0.txt` & `oslili-0.9/oslili/spdx/TAPR-OHL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/TCL.txt` & `oslili-0.9/oslili/spdx/TCL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/TCP-wrappers.txt` & `oslili-0.9/oslili/spdx/TCP-wrappers.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/TMate.txt` & `oslili-0.9/oslili/spdx/TMate.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/TORQUE-1.1.txt` & `oslili-0.9/oslili/spdx/TORQUE-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/TOSL.txt` & `oslili-0.9/oslili/spdx/TOSL.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/TPL-1.0.txt` & `oslili-0.9/oslili/spdx/TPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/TU-Berlin-1.0.txt` & `oslili-0.9/oslili/spdx/TU-Berlin-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/TU-Berlin-2.0.txt` & `oslili-0.9/oslili/spdx/TU-Berlin-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/UCAR.txt` & `oslili-0.9/oslili/spdx/UCAR.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/UCL-1.0.txt` & `oslili-0.9/oslili/spdx/UCL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/UPL-1.0.txt` & `oslili-0.9/oslili/spdx/UPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Unicode-DFS-2015.txt` & `oslili-0.9/oslili/spdx/Unicode-DFS-2015.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Unicode-DFS-2016.txt` & `oslili-0.9/oslili/spdx/Unicode-DFS-2016.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Unicode-TOU.txt` & `oslili-0.9/oslili/spdx/Unicode-TOU.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Universal-FOSS-exception-1.0.txt` & `oslili-0.9/oslili/spdx/Universal-FOSS-exception-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Unlicense.txt` & `oslili-0.9/oslili/spdx/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/VOSTROM.txt` & `oslili-0.9/oslili/spdx/VOSTROM.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/VSL-1.0.txt` & `oslili-0.9/oslili/spdx/VSL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Vim.txt` & `oslili-0.9/oslili/spdx/Vim.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/W3C-19980720.txt` & `oslili-0.9/oslili/spdx/W3C-19980720.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/W3C-20150513.txt` & `oslili-0.9/oslili/spdx/W3C-20150513.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/W3C.txt` & `oslili-0.9/oslili/spdx/W3C.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Watcom-1.0.txt` & `oslili-0.9/oslili/spdx/Watcom-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Wsuipa.txt` & `oslili-0.9/oslili/spdx/Wsuipa.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/WxWindows-exception-3.1.txt` & `oslili-0.9/oslili/spdx/WxWindows-exception-3.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/X11-distribute-modifications-variant.txt` & `oslili-0.9/oslili/spdx/X11-distribute-modifications-variant.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/X11.txt` & `oslili-0.9/oslili/spdx/X11.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/XFree86-1.1.txt` & `oslili-0.9/oslili/spdx/XFree86-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/XSkat.txt` & `oslili-0.9/oslili/spdx/XSkat.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Xerox.txt` & `oslili-0.9/oslili/spdx/Xerox.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Xnet.txt` & `oslili-0.9/oslili/spdx/Xnet.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/YPL-1.0.txt` & `oslili-0.9/oslili/spdx/YPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/YPL-1.1.txt` & `oslili-0.9/oslili/spdx/YPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ZPL-1.1.txt` & `oslili-0.9/oslili/spdx/ZPL-1.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ZPL-2.0.txt` & `oslili-0.9/oslili/spdx/ZPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/ZPL-2.1.txt` & `oslili-0.9/oslili/spdx/ZPL-2.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Zend-2.0.txt` & `oslili-0.9/oslili/spdx/Zend-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Zimbra-1.3.txt` & `oslili-0.9/oslili/spdx/Zimbra-1.3.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Zimbra-1.4.txt` & `oslili-0.9/oslili/spdx/Zimbra-1.4.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/Zlib.txt` & `oslili-0.9/oslili/spdx/Zlib.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/bzip2-1.0.6.txt` & `oslili-0.9/oslili/spdx/bzip2-1.0.6.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/copyleft-next-0.3.0.txt` & `oslili-0.9/oslili/spdx/copyleft-next-0.3.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/copyleft-next-0.3.1.txt` & `oslili-0.9/oslili/spdx/copyleft-next-0.3.1.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/curl.txt` & `oslili-0.9/oslili/spdx/curl.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/eCos-exception-2.0.txt` & `oslili-0.9/oslili/spdx/eCos-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/eGenix.txt` & `oslili-0.9/oslili/spdx/eGenix.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/etalab-2.0.txt` & `oslili-0.9/oslili/spdx/etalab-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/freertos-exception-2.0.txt` & `oslili-0.9/oslili/spdx/freertos-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/gSOAP-1.3b.txt` & `oslili-0.9/oslili/spdx/gSOAP-1.3b.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/gnuplot.txt` & `oslili-0.9/oslili/spdx/gnuplot.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/i2p-gpl-java-exception.txt` & `oslili-0.9/oslili/spdx/i2p-gpl-java-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/iMatix.txt` & `oslili-0.9/oslili/spdx/iMatix.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/libpng-2.0.txt` & `oslili-0.9/oslili/spdx/libpng-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/libselinux-1.0.txt` & `oslili-0.9/oslili/spdx/libselinux-1.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/libtiff.txt` & `oslili-0.9/oslili/spdx/libtiff.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/libutil-David-Nugent.txt` & `oslili-0.9/oslili/spdx/libutil-David-Nugent.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/mif-exception.txt` & `oslili-0.9/oslili/spdx/mif-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/mpi-permissive.txt` & `oslili-0.9/oslili/spdx/mpi-permissive.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/mpich2.txt` & `oslili-0.9/oslili/spdx/mpich2.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/openvpn-openssl-exception.txt` & `oslili-0.9/oslili/spdx/openvpn-openssl-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/psutils.txt` & `oslili-0.9/oslili/spdx/psutils.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/u-boot-exception-2.0.txt` & `oslili-0.9/oslili/spdx/u-boot-exception-2.0.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/w3m.txt` & `oslili-0.9/oslili/spdx/w3m.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/x11vnc-openssl-exception.txt` & `oslili-0.9/oslili/spdx/x11vnc-openssl-exception.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/xinetd.txt` & `oslili-0.9/oslili/spdx/xinetd.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/xlock.txt` & `oslili-0.9/oslili/spdx/xlock.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/xpp.txt` & `oslili-0.9/oslili/spdx/xpp.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili/spdx/zlib-acknowledgement.txt` & `oslili-0.9/oslili/spdx/zlib-acknowledgement.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/oslili.egg-info/PKG-INFO` & `oslili-0.9/oslili.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslili
-Version: 0.8
+Version: 0.9
 Summary: Open Source License Identification Library
 Home-page: https://github.com/oscarvalenzuelab/oslili
 Author: Oscar Valenzuela B.
 Author-email: alkamod@gmail.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `oslili-0.8/oslili.egg-info/SOURCES.txt` & `oslili-0.9/oslili.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oslili-0.8/setup.py` & `oslili-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 import sys
 from setuptools import setup, find_packages
 
 
 HERE = pathlib.Path(__file__).parent
-VERSION = '0.8'
+VERSION = '0.9'
 PACKAGE_NAME = 'oslili'
 AUTHOR = 'Oscar Valenzuela B.'
 AUTHOR_EMAIL = 'alkamod@gmail.com'
 URL = 'https://github.com/oscarvalenzuelab/oslili'
 LICENSE = 'Apache-2.0'
 DESCRIPTION = 'Open Source License Identification Library'
 LONG_DESCRIPTION = (HERE / "README.md").read_text()
```

