# Comparing `tmp/myokit-1.36.0.tar.gz` & `tmp/myokit-1.36.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myokit-1.36.0.tar", last modified: Fri Mar 22 18:40:41 2024, max compression
+gzip compressed data, was "myokit-1.36.1.tar", last modified: Fri May 10 10:35:17 2024, max compression
```

## Comparing `myokit-1.36.0.tar` & `myokit-1.36.1.tar`

### file list

```diff
@@ -1,463 +1,463 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.592880 myokit-1.36.0/
--rw-r--r--   0 michael   (1000) michael   (1000)     1833 2024-02-01 16:26:05.000000 myokit-1.36.0/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-07 13:48:23.000000 myokit-1.36.0/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     5735 2024-03-22 18:40:41.591880 myokit-1.36.0/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     4496 2024-02-01 16:26:05.000000 myokit-1.36.0/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.549880 myokit-1.36.0/myokit/
--rw-r--r--   0 michael   (1000) michael   (1000)    14272 2024-03-12 11:54:33.000000 myokit-1.36.0/myokit/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    53688 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23743 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_aux.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.549880 myokit-1.36.0/myokit/_bin/
--rw-r--r--   0 michael   (1000) michael   (1000)     6226 2023-10-13 08:52:06.000000 myokit-1.36.0/myokit/_bin/example.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.553880 myokit-1.36.0/myokit/_bin/gui/
--rw-r--r--   0 michael   (1000) michael   (1000)      784 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/find.png
--rw-r--r--   0 michael   (1000) michael   (1000)    96412 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-128.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     3528 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-16.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-24.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   233500 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-256.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    12232 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-32.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    23817 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-48.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    36761 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-64.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    65257 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-96.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer.ico
--rw-r--r--   0 michael   (1000) michael   (1000)    30396 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer.png
--rw-r--r--   0 michael   (1000) michael   (1000)    47406 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-ide-128.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     2987 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-ide-16.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     4971 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-ide-24.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   152751 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-ide-256.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     7355 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-ide-32.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     9835 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-ide-48.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    16235 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-ide-64.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    30683 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-ide-96.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-ide.ico
--rw-r--r--   0 michael   (1000) michael   (1000)    15096 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/icon-ide.png
--rw-r--r--   0 michael   (1000) michael   (1000)      571 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/new.png
--rw-r--r--   0 michael   (1000) michael   (1000)      544 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/open.png
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/redo.png
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/run.png
--rw-r--r--   0 michael   (1000) michael   (1000)      565 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/save.png
--rw-r--r--   0 michael   (1000) michael   (1000)      284 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/_bin/gui/undo.png
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.554880 myokit-1.36.0/myokit/_bin/install-lin/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      254 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/_bin/install-lin/myokit-datablock-viewer.desktop
--rwxr-xr-x   0 michael   (1000) michael   (1000)      266 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/_bin/install-lin/myokit-datalog-viewer.desktop
--rwxr-xr-x   0 michael   (1000) michael   (1000)      264 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/install-lin/myokit-ide.desktop
--rw-r--r--   0 michael   (1000) michael   (1000)     4338 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/_bin/install-lin/myokit.lang
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-07 13:47:50.000000 myokit-1.36.0/myokit/_bin/install-lin/x-abf.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      246 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/install-lin/x-cellml.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/_bin/install-lin/x-myokit.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      275 2023-06-07 13:47:50.000000 myokit-1.36.0/myokit/_bin/install-lin/x-wcp.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.554880 myokit-1.36.0/myokit/_bin/install-win/
--rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_bin/install-win/menu.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.554880 myokit-1.36.0/myokit/_bin/sundials-win-vs/
--rw-r--r--   0 michael   (1000) michael   (1000)     1758 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/LICENSE
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.543880 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.554880 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/cvodes/
--rw-r--r--   0 michael   (1000) michael   (1000)    27506 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h
--rw-r--r--   0 michael   (1000) michael   (1000)     2427 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h
--rw-r--r--   0 michael   (1000) michael   (1000)    12344 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.554880 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/nvector/
--rw-r--r--   0 michael   (1000) michael   (1000)     8934 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.556880 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/
--rw-r--r--   0 michael   (1000) michael   (1000)     5785 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h
--rw-r--r--   0 michael   (1000) michael   (1000)     8997 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h
--rw-r--r--   0 michael   (1000) michael   (1000)    13330 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h
--rw-r--r--   0 michael   (1000) michael   (1000)     1024 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h
--rw-r--r--   0 michael   (1000) michael   (1000)    10283 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h
--rw-r--r--   0 michael   (1000) michael   (1000)     9385 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5420 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h
--rw-r--r--   0 michael   (1000) michael   (1000)     9190 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h
--rw-r--r--   0 michael   (1000) michael   (1000)    12559 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5165 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h
--rw-r--r--   0 michael   (1000) michael   (1000)     1266 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.556880 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sunlinsol/
--rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.556880 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sunmatrix/
--rw-r--r--   0 michael   (1000) michael   (1000)     3647 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.557880 myokit-1.36.0/myokit/_bin/sundials-win-vs/lib/
--rw-r--r--   0 michael   (1000) michael   (1000)   677888 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll
--rw-r--r--   0 michael   (1000) michael   (1000)   169196 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib
--rw-r--r--   0 michael   (1000) michael   (1000)   160768 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll
--rw-r--r--   0 michael   (1000) michael   (1000)    59576 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib
--rw-r--r--   0 michael   (1000) michael   (1000)    11989 2024-03-08 14:23:00.000000 myokit-1.36.0/myokit/_config.py
--rw-r--r--   0 michael   (1000) michael   (1000)    89061 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_datablock.py
--rw-r--r--   0 michael   (1000) michael   (1000)    75852 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_datalog.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11060 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_err.py
--rw-r--r--   0 michael   (1000) michael   (1000)   103902 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/_expressions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8948 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_io.py
--rw-r--r--   0 michael   (1000) michael   (1000)   194214 2024-03-13 12:21:41.000000 myokit-1.36.0/myokit/_model_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)      726 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/_myokit_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)    74065 2023-11-21 18:38:30.000000 myokit-1.36.0/myokit/_parsing.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4410 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_progress.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30756 2024-02-01 16:26:05.000000 myokit-1.36.0/myokit/_protocol.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.560880 myokit-1.36.0/myokit/_sim/
--rw-r--r--   0 michael   (1000) michael   (1000)    13488 2024-03-13 14:18:16.000000 myokit-1.36.0/myokit/_sim/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19156 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)    18908 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/cable.py
--rw-r--r--   0 michael   (1000) michael   (1000)    38795 2023-11-21 18:38:30.000000 myokit-1.36.0/myokit/_sim/cmodel.h
--rw-r--r--   0 michael   (1000) michael   (1000)    15775 2023-11-21 18:38:30.000000 myokit-1.36.0/myokit/_sim/cmodel.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4047 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_sim/compiler.c
--rw-r--r--   0 michael   (1000) michael   (1000)     2664 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/compiler.py
--rw-r--r--   0 michael   (1000) michael   (1000)    75604 2024-03-12 11:54:33.000000 myokit-1.36.0/myokit/_sim/cvodessim.c
--rw-r--r--   0 michael   (1000) michael   (1000)    46122 2024-03-12 11:54:33.000000 myokit-1.36.0/myokit/_sim/cvodessim.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15446 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/differential.hpp
--rw-r--r--   0 michael   (1000) michael   (1000)    47444 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/fiber_tissue.c
--rw-r--r--   0 michael   (1000) michael   (1000)    50780 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/fiber_tissue.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8012 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/jacobian.cpp
--rw-r--r--   0 michael   (1000) michael   (1000)    12957 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/jacobian.py
--rw-r--r--   0 michael   (1000) michael   (1000)    32352 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/mcl.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5037 2023-10-13 08:52:06.000000 myokit-1.36.0/myokit/_sim/opencl.c
--rw-r--r--   0 michael   (1000) michael   (1000)    16446 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/opencl.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46541 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/openclsim.c
--rw-r--r--   0 michael   (1000) michael   (1000)    19360 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/openclsim.cl
--rw-r--r--   0 michael   (1000) michael   (1000)    69159 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/openclsim.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29888 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/pacing.h
--rw-r--r--   0 michael   (1000) michael   (1000)    10914 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/rhs.c
--rw-r--r--   0 michael   (1000) michael   (1000)     7392 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/rhs.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1720 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/_sim/sundials.c
--rw-r--r--   0 michael   (1000) michael   (1000)     2972 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_sim/sundials.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4602 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_system.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29849 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/_unit.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3066 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/float.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.560880 myokit-1.36.0/myokit/formats/
--rw-r--r--   0 michael   (1000) michael   (1000)    29248 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.560880 myokit-1.36.0/myokit/formats/ansic/
--rw-r--r--   0 michael   (1000) michael   (1000)     3424 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/ansic/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7360 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/ansic/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5361 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/ansic/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.560880 myokit-1.36.0/myokit/formats/ansic/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    11965 2023-10-13 08:52:06.000000 myokit-1.36.0/myokit/formats/ansic/template/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)     6044 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/ansic/template/euler.c
--rw-r--r--   0 michael   (1000) michael   (1000)    14244 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/ansic/template/sim.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.561880 myokit-1.36.0/myokit/formats/axon/
--rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/axon/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    75937 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/axon/_abf.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10543 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/axon/_atf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      826 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/axon/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.561880 myokit-1.36.0/myokit/formats/cellml/
--rw-r--r--   0 michael   (1000) michael   (1000)     1466 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2719 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2283 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2229 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.562880 myokit-1.36.0/myokit/formats/cellml/v1/
--rw-r--r--   0 michael   (1000) michael   (1000)      608 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/v1/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59011 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/v1/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)    43554 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/v1/_parser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15055 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/v1/_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.562880 myokit-1.36.0/myokit/formats/cellml/v2/
--rw-r--r--   0 michael   (1000) michael   (1000)      598 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/v2/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59012 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/v2/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29536 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/v2/_parser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11994 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cellml/v2/_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.562880 myokit-1.36.0/myokit/formats/channelml/
--rw-r--r--   0 michael   (1000) michael   (1000)      443 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/channelml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    14605 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/channelml/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.562880 myokit-1.36.0/myokit/formats/cpp/
--rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cpp/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      930 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/cpp/_ewriter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.563880 myokit-1.36.0/myokit/formats/cuda/
--rw-r--r--   0 michael   (1000) michael   (1000)      816 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cuda/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3102 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/cuda/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2059 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cuda/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.563880 myokit-1.36.0/myokit/formats/cuda/template/
--rw-r--r--   0 michael   (1000) michael   (1000)     8863 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/cuda/template/kernel.cu
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.563880 myokit-1.36.0/myokit/formats/easyml/
--rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/easyml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2597 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/easyml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15771 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/easyml/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.563880 myokit-1.36.0/myokit/formats/heka/
--rw-r--r--   0 michael   (1000) michael   (1000)      847 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/heka/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1154 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/heka/_importer.py
--rw-r--r--   0 michael   (1000) michael   (1000)   106500 2024-02-01 17:37:11.000000 myokit-1.36.0/myokit/formats/heka/_patchmaster.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.564880 myokit-1.36.0/myokit/formats/html/
--rw-r--r--   0 michael   (1000) michael   (1000)      457 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/html/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2343 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/html/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6606 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/html/_flatten.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.564880 myokit-1.36.0/myokit/formats/latex/
--rw-r--r--   0 michael   (1000) michael   (1000)      682 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/latex/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7904 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/latex/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5118 2024-03-08 14:23:00.000000 myokit-1.36.0/myokit/formats/latex/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.564880 myokit-1.36.0/myokit/formats/mathml/
--rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/mathml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    12194 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/mathml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)    34289 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/mathml/_parser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.565880 myokit-1.36.0/myokit/formats/matlab/
--rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/matlab/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4096 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/matlab/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2868 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/matlab/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.565880 myokit-1.36.0/myokit/formats/matlab/template/
--rw-r--r--   0 michael   (1000) michael   (1000)      528 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/formats/matlab/template/constants.m
--rw-r--r--   0 michael   (1000) michael   (1000)      374 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/formats/matlab/template/ifthenelse.m
--rw-r--r--   0 michael   (1000) michael   (1000)     2095 2023-10-13 08:52:06.000000 myokit-1.36.0/myokit/formats/matlab/template/main.m
--rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/formats/matlab/template/model.m
--rw-r--r--   0 michael   (1000) michael   (1000)      461 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/formats/matlab/template/model_wrapper.m
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.566880 myokit-1.36.0/myokit/formats/opencl/
--rw-r--r--   0 michael   (1000) michael   (1000)     6962 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/opencl/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4944 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/opencl/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3903 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/opencl/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.566880 myokit-1.36.0/myokit/formats/opencl/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    11633 2023-10-13 08:52:06.000000 myokit-1.36.0/myokit/formats/opencl/template/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)     8158 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/opencl/template/kernel.cl
--rw-r--r--   0 michael   (1000) michael   (1000)     9018 2023-10-13 08:52:06.000000 myokit-1.36.0/myokit/formats/opencl/template/minilog.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1042 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/formats/opencl/template/plot.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      162 2023-10-13 08:52:06.000000 myokit-1.36.0/myokit/formats/opencl/template/test.sh
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.566880 myokit-1.36.0/myokit/formats/python/
--rw-r--r--   0 michael   (1000) michael   (1000)     1049 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/python/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8251 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/python/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/python/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.566880 myokit-1.36.0/myokit/formats/python/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    10311 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/python/template/sim.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.567880 myokit-1.36.0/myokit/formats/sbml/
--rw-r--r--   0 michael   (1000) michael   (1000)      653 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/sbml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59396 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/sbml/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)      987 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/sbml/_importer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29181 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/sbml/_parser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.567880 myokit-1.36.0/myokit/formats/stan/
--rw-r--r--   0 michael   (1000) michael   (1000)     2877 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/stan/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2998 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/formats/stan/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3745 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/stan/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.567880 myokit-1.36.0/myokit/formats/stan/template/
--rw-r--r--   0 michael   (1000) michael   (1000)     5305 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/stan/template/cell.stan
--rwxr-xr-x   0 michael   (1000) michael   (1000)       92 2023-02-05 15:45:10.000000 myokit-1.36.0/myokit/formats/stan/template/run.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.568880 myokit-1.36.0/myokit/formats/sympy/
--rw-r--r--   0 michael   (1000) michael   (1000)     1638 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/sympy/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6758 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/sympy/_ereader.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4875 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/sympy/_ewriter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.568880 myokit-1.36.0/myokit/formats/wcp/
--rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/wcp/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    17751 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/wcp/_wcp.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.568880 myokit-1.36.0/myokit/formats/xml/
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/xml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1494 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/xml/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)      393 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/formats/xml/_split.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.569880 myokit-1.36.0/myokit/gui/
--rw-r--r--   0 michael   (1000) michael   (1000)     6426 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/gui/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    49529 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/gui/datablock_viewer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    32774 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/gui/datalog_viewer.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8676 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/gui/explorer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)   108238 2024-01-10 18:28:46.000000 myokit-1.36.0/myokit/gui/ide.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2157 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/gui/progress.py
--rw-r--r--   0 michael   (1000) michael   (1000)    52367 2024-03-08 14:23:00.000000 myokit-1.36.0/myokit/gui/source.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6072 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/gui/vargrapher.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.570880 myokit-1.36.0/myokit/lib/
--rw-r--r--   0 michael   (1000) michael   (1000)      216 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/lib/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23859 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/lib/deps.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28056 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/lib/guess.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46678 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/lib/hh.py
--rw-r--r--   0 michael   (1000) michael   (1000)    67940 2024-02-01 17:37:08.000000 myokit-1.36.0/myokit/lib/markov.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4408 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/lib/multi.py
--rw-r--r--   0 michael   (1000) michael   (1000)    13875 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/lib/plots.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4552 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/pacing.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8230 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/pype.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.579880 myokit-1.36.0/myokit/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)    10233 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2738 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/ansic_event_based_pacing.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1250 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/ansic_time_series_pacing.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.581880 myokit-1.36.0/myokit/tests/data/
--rw-r--r--   0 michael   (1000) michael   (1000)     3022 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/tests/data/beeler-1977-model-compare-a.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     2889 2023-10-13 08:52:06.000000 myokit-1.36.0/myokit/tests/data/beeler-1977-model-compare-b.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3137 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/tests/data/beeler-1977-model.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/beeler-1977-protocol.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/beeler-1977-script.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3287 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/tests/data/beeler-1977-units.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     5091 2023-10-13 08:52:06.000000 myokit-1.36.0/myokit/tests/data/clancy-1999-fitting.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3128 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/conditional.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6067 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/tests/data/cv1d.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/cv1d.zip
--rw-r--r--   0 michael   (1000) michael   (1000)    23916 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/decker-2009.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)    18227 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/data/decker.model
--rw-r--r--   0 michael   (1000) michael   (1000)    10416 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/dn-1985-normalised.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      800 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/dom-markov.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.581880 myokit-1.36.0/myokit/tests/data/formats/
--rw-r--r--   0 michael   (1000) michael   (1000)     8192 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/abf-protocol.pro
--rw-r--r--   0 michael   (1000) michael   (1000)    98376 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/abf-v1.abf
--rw-r--r--   0 michael   (1000) michael   (1000)    44544 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/data/formats/abf-v2.abf
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.582880 myokit-1.36.0/myokit/tests/data/formats/cellml/
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/cellml/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)    59093 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/cellml/br-1977-dot.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    58593 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/cellml/br-1977.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)   117223 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/cellml/corrias.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)   221953 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/cellml/decker-2009.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)     1595 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/cellml/documentation.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/cellml/invalid-file.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    44837 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    44947 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.584880 myokit-1.36.0/myokit/tests/data/formats/channelml/
--rw-r--r--   0 michael   (1000) michael   (1000)     2648 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      557 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     2702 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     2369 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1258 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1539 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1290 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1374 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1373 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      675 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1398 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1317 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.585880 myokit-1.36.0/myokit/tests/data/formats/sbml/
--rw-r--r--   0 michael   (1000) michael   (1000)     8719 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     9801 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml
--rw-r--r--   0 michael   (1000) michael   (1000)    31408 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/sbml/HodgkinHuxley.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/sbml/LICENSE
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.585880 myokit-1.36.0/myokit/tests/data/formats/sbml/model/
--rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     2952 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     1226 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.585880 myokit-1.36.0/myokit/tests/data/formats/sbml/result/
--rw-r--r--   0 michael   (1000) michael   (1000)     2457 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/sbml/result/00001-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     2206 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/sbml/result/00004-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/sbml/result/01103-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)    25600 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/formats/wcp-file.wcp
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.591880 myokit-1.36.0/myokit/tests/data/io/
--rw-r--r--   0 michael   (1000) michael   (1000)      735 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad1d-1-not-enough-files.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109429 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad1d-2-no-header.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   104768 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad1d-3-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad1d-4-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109458 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad1d-5-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1549 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad1d-6-time-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad1d-7-0d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad1d-8-1d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)      739 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad2d-1-not-enough-files.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346240 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad2d-2-no-header.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   333091 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad2d-3-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad2d-4-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346257 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad2d-5-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1553 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad2d-6-time-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1588 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad2d-7-0d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/bad2d-8-2d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)      623 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/badlog-1-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1281 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/badlog-2-no-structure.zip
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/badlog-3-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/badlog-4-invalid-n-fields.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/badlog-5-invalid-data-size.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1457 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/badlog-6-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/badlog-7-not-enough-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     6031 2023-06-07 13:48:59.000000 myokit-1.36.0/myokit/tests/data/io/block2d.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/block2d.zip
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-1-empty.csv
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-10-just-spaces.csv
--rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-11-just-a-semicolon.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-12-bad-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-13-header-with-empty-1.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-14-header-with-empty-2.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-15-header-with-empty-3.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-16-wrong-columns-in-data.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-17-non-float-data.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      112 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-2-windows.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-3-old-mac.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-4-empty-lines.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-5-semicolons.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-6-open-string.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-7-empty-lines-2.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-8-unquoted-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      114 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog-9-double-quoted-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/datalog.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     1421 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/io/goodlog.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     4992 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/lr-1991-dep.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     2315 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/lr-1991-fitting.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     4571 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/lr-1991-testing.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6136 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/data/lr-1991.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.591880 myokit-1.36.0/myokit/tests/data/multi/
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/multi/beeler-1977-protocol.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/multi/beeler-1977-script.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/multi/beeler-no-name.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6013 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/multi/lr-1991.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/multi/not-a-model.csv
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.591880 myokit-1.36.0/myokit/tests/data/multi/subdir/
--rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/multi/subdir/beeler-no-name.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3754 2023-06-07 13:48:23.000000 myokit-1.36.0/myokit/tests/data/noble-1962.mmt
--rwxr-xr-x   0 michael   (1000) michael   (1000)    22536 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_aux.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    56981 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_cellml_v1_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    41869 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_cellml_v1_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12532 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_cellml_v1_writer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    73319 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_cellml_v2_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    26345 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_cellml_v2_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10977 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_cellml_v2_writer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4058 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_cmodel.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      476 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_compiler_detection.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14096 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_component.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11511 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_config.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    52565 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_datablock.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    91575 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_datalog.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    60654 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_dependency_checking.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)   138508 2023-11-21 18:38:30.000000 myokit-1.36.0/myokit/tests/test_expressions.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4882 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_float.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8085 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    13260 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_ansic.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    33181 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_axon.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    19078 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_formats_cellml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6703 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_formats_channelml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3762 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_cpp.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8695 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_cuda.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    13211 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_easyml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6647 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_exporters_run.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3520 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_html.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8546 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_latex.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    38093 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_mathml_content.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     9076 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_mathml_presentation.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8021 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_matlab.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8844 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_opencl.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    22761 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_python.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4672 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_formats_sbml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6310 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_stan.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10709 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_formats_sympy.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7658 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_formats_wcp.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14334 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_io.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1821 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_jacobian_calculator.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1767 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_jacobian_tracer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7476 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_lib_deps.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    42333 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_lib_guess.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    31014 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_lib_hh.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    39983 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_lib_markov.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5145 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_lib_multi.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5754 2024-03-22 18:39:02.000000 myokit-1.36.0/myokit/tests/test_lib_plots.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2829 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_meta.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    87008 2024-03-10 14:01:18.000000 myokit-1.36.0/myokit/tests/test_model.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    16716 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_model_building.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3834 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_opencl_info.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8193 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_pacing_factory.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6504 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_pacing_system_c.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3637 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_pacing_system_py.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    50865 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_parsing.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2762 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_progress_reporters.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    15092 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_protocol.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12565 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_protocol_floating_point.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2318 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_protocol_time_series.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2402 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_pype.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7353 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_quantity.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3452 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_rhs_benchmarker.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    71633 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_sbml_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    54542 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_sbml_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    19281 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_simulation_1d.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    48408 2024-03-10 14:01:18.000000 myokit-1.36.0/myokit/tests/test_simulation_cvodes.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1853 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_simulation_cvodes_from_disk.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    36596 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_simulation_fiber_tissue.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14033 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_simulation_log_interval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    60162 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_simulation_opencl.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3005 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_simulation_opencl_log_interval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    20114 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_simulation_opencl_vs_cvode.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5216 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_simulation_opencl_vs_sim1d.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      562 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_system_info.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10358 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_tools.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    13635 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_unit.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_user_functions.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    33331 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/tests/test_variable.py
--rw-r--r--   0 michael   (1000) michael   (1000)    16942 2024-02-01 16:26:05.000000 myokit-1.36.0/myokit/tools.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8503 2023-10-30 14:08:26.000000 myokit-1.36.0/myokit/units.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-22 18:40:41.549880 myokit-1.36.0/myokit.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     5735 2024-03-22 18:40:41.000000 myokit-1.36.0/myokit.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)    15269 2024-03-22 18:40:41.000000 myokit-1.36.0/myokit.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2024-03-22 18:40:41.000000 myokit-1.36.0/myokit.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       48 2024-03-22 18:40:41.000000 myokit-1.36.0/myokit.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-01-04 14:18:38.000000 myokit-1.36.0/myokit.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      176 2024-03-22 18:40:41.000000 myokit-1.36.0/myokit.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        7 2024-03-22 18:40:41.000000 myokit-1.36.0/myokit.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-03-22 18:40:41.592880 myokit-1.36.0/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     3206 2023-10-30 14:08:26.000000 myokit-1.36.0/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.058497 myokit-1.36.1/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1833 2024-02-01 16:26:05.000000 myokit-1.36.1/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-07 13:48:23.000000 myokit-1.36.1/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     5735 2024-05-10 10:35:17.058497 myokit-1.36.1/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     4496 2024-02-01 16:26:05.000000 myokit-1.36.1/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.950497 myokit-1.36.1/myokit/
+-rw-r--r--   0 michael   (1000) michael   (1000)    14272 2024-03-12 11:54:33.000000 myokit-1.36.1/myokit/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    53688 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23743 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_aux.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.951497 myokit-1.36.1/myokit/_bin/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6226 2023-10-13 08:52:06.000000 myokit-1.36.1/myokit/_bin/example.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.960497 myokit-1.36.1/myokit/_bin/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)      784 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/find.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    96412 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-128.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     3528 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-16.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-24.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   233500 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-256.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    12232 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-32.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    23817 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-48.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    36761 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-64.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    65257 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-96.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)    30396 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    47406 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-ide-128.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     2987 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-ide-16.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     4971 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-ide-24.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   152751 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-ide-256.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     7355 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-ide-32.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     9835 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-ide-48.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    16235 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-ide-64.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    30683 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-ide-96.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-ide.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)    15096 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/icon-ide.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      571 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/new.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      544 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/open.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/redo.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/run.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      565 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/save.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      284 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/_bin/gui/undo.png
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.962497 myokit-1.36.1/myokit/_bin/install-lin/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      254 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/_bin/install-lin/myokit-datablock-viewer.desktop
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      266 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/_bin/install-lin/myokit-datalog-viewer.desktop
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      264 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/install-lin/myokit-ide.desktop
+-rw-r--r--   0 michael   (1000) michael   (1000)     4338 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/_bin/install-lin/myokit.lang
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-07 13:47:50.000000 myokit-1.36.1/myokit/_bin/install-lin/x-abf.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      246 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/install-lin/x-cellml.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/_bin/install-lin/x-myokit.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      275 2023-06-07 13:47:50.000000 myokit-1.36.1/myokit/_bin/install-lin/x-wcp.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.962497 myokit-1.36.1/myokit/_bin/install-win/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_bin/install-win/menu.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.962497 myokit-1.36.1/myokit/_bin/sundials-win-vs/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1758 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/LICENSE
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.940497 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.963497 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/cvodes/
+-rw-r--r--   0 michael   (1000) michael   (1000)    27506 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     2427 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    12344 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.964497 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/nvector/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8934 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.969497 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5785 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     8997 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    13330 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     1024 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    10283 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     9385 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5420 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     9190 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    12559 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5165 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     1266 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.969497 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sunlinsol/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.969497 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sunmatrix/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3647 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.977497 myokit-1.36.1/myokit/_bin/sundials-win-vs/lib/
+-rw-r--r--   0 michael   (1000) michael   (1000)   677888 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll
+-rw-r--r--   0 michael   (1000) michael   (1000)   169196 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib
+-rw-r--r--   0 michael   (1000) michael   (1000)   160768 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll
+-rw-r--r--   0 michael   (1000) michael   (1000)    59576 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib
+-rw-r--r--   0 michael   (1000) michael   (1000)    11989 2024-03-08 14:23:00.000000 myokit-1.36.1/myokit/_config.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    89061 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_datablock.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    75852 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_datalog.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11060 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_err.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   103902 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/_expressions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8948 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_io.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   194214 2024-03-13 12:21:41.000000 myokit-1.36.1/myokit/_model_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      726 2024-05-10 10:33:43.000000 myokit-1.36.1/myokit/_myokit_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    74065 2023-11-21 18:38:30.000000 myokit-1.36.1/myokit/_parsing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4410 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_progress.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30756 2024-02-01 16:26:05.000000 myokit-1.36.1/myokit/_protocol.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.983497 myokit-1.36.1/myokit/_sim/
+-rw-r--r--   0 michael   (1000) michael   (1000)    13488 2024-03-13 14:18:16.000000 myokit-1.36.1/myokit/_sim/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19156 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    18908 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/cable.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    38795 2023-11-21 18:38:30.000000 myokit-1.36.1/myokit/_sim/cmodel.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    15775 2023-11-21 18:38:30.000000 myokit-1.36.1/myokit/_sim/cmodel.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4047 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_sim/compiler.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     2664 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/compiler.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    78062 2024-05-09 14:25:03.000000 myokit-1.36.1/myokit/_sim/cvodessim.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    46122 2024-03-12 11:54:33.000000 myokit-1.36.1/myokit/_sim/cvodessim.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15446 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/differential.hpp
+-rw-r--r--   0 michael   (1000) michael   (1000)    47444 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/fiber_tissue.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    50780 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/fiber_tissue.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8012 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/jacobian.cpp
+-rw-r--r--   0 michael   (1000) michael   (1000)    12957 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/jacobian.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    34114 2024-05-10 10:31:35.000000 myokit-1.36.1/myokit/_sim/mcl.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5037 2023-10-13 08:52:06.000000 myokit-1.36.1/myokit/_sim/opencl.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    16446 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/opencl.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46541 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/openclsim.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    19360 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/openclsim.cl
+-rw-r--r--   0 michael   (1000) michael   (1000)    69159 2024-04-30 09:34:35.000000 myokit-1.36.1/myokit/_sim/openclsim.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29888 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/pacing.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    10914 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/rhs.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     7392 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/rhs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1720 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/_sim/sundials.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     2972 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_sim/sundials.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4602 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_system.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29849 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/_unit.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3066 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/float.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.983497 myokit-1.36.1/myokit/formats/
+-rw-r--r--   0 michael   (1000) michael   (1000)    29248 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.984497 myokit-1.36.1/myokit/formats/ansic/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3424 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/ansic/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7360 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/ansic/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5361 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/ansic/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.985497 myokit-1.36.1/myokit/formats/ansic/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11965 2023-10-13 08:52:06.000000 myokit-1.36.1/myokit/formats/ansic/template/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     6044 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/ansic/template/euler.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    14244 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/ansic/template/sim.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.987497 myokit-1.36.1/myokit/formats/axon/
+-rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/axon/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    75937 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/axon/_abf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10543 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/axon/_atf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      826 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/axon/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.988497 myokit-1.36.1/myokit/formats/cellml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1466 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2719 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2283 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2229 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.990497 myokit-1.36.1/myokit/formats/cellml/v1/
+-rw-r--r--   0 michael   (1000) michael   (1000)      608 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/v1/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59011 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/v1/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    43554 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/v1/_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15055 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/v1/_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.992497 myokit-1.36.1/myokit/formats/cellml/v2/
+-rw-r--r--   0 michael   (1000) michael   (1000)      598 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/v2/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59012 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/v2/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29536 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/v2/_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11994 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cellml/v2/_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.992497 myokit-1.36.1/myokit/formats/channelml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      443 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/channelml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    14605 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/channelml/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.992497 myokit-1.36.1/myokit/formats/cpp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cpp/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      930 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/cpp/_ewriter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.993497 myokit-1.36.1/myokit/formats/cuda/
+-rw-r--r--   0 michael   (1000) michael   (1000)      816 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cuda/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3102 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/cuda/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2059 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cuda/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.993497 myokit-1.36.1/myokit/formats/cuda/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8863 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/cuda/template/kernel.cu
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.994497 myokit-1.36.1/myokit/formats/easyml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/easyml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2597 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/easyml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15771 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/easyml/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.994497 myokit-1.36.1/myokit/formats/heka/
+-rw-r--r--   0 michael   (1000) michael   (1000)      847 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/heka/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1154 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/heka/_importer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   106500 2024-02-01 17:37:11.000000 myokit-1.36.1/myokit/formats/heka/_patchmaster.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.996497 myokit-1.36.1/myokit/formats/html/
+-rw-r--r--   0 michael   (1000) michael   (1000)      457 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/html/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2343 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/html/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6606 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/html/_flatten.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.997497 myokit-1.36.1/myokit/formats/latex/
+-rw-r--r--   0 michael   (1000) michael   (1000)      682 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/latex/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7904 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/latex/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5118 2024-03-08 14:23:00.000000 myokit-1.36.1/myokit/formats/latex/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.998497 myokit-1.36.1/myokit/formats/mathml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/mathml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    12194 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/mathml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    34289 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/mathml/_parser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.999497 myokit-1.36.1/myokit/formats/matlab/
+-rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/matlab/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4096 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/matlab/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2868 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/matlab/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.999497 myokit-1.36.1/myokit/formats/matlab/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)      528 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/formats/matlab/template/constants.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      374 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/formats/matlab/template/ifthenelse.m
+-rw-r--r--   0 michael   (1000) michael   (1000)     2095 2023-10-13 08:52:06.000000 myokit-1.36.1/myokit/formats/matlab/template/main.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/formats/matlab/template/model.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      461 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/formats/matlab/template/model_wrapper.m
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.000497 myokit-1.36.1/myokit/formats/opencl/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6962 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/opencl/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4944 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/opencl/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3903 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/opencl/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.001497 myokit-1.36.1/myokit/formats/opencl/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11633 2023-10-13 08:52:06.000000 myokit-1.36.1/myokit/formats/opencl/template/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     8158 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/opencl/template/kernel.cl
+-rw-r--r--   0 michael   (1000) michael   (1000)     9018 2023-10-13 08:52:06.000000 myokit-1.36.1/myokit/formats/opencl/template/minilog.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1042 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/formats/opencl/template/plot.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      162 2023-10-13 08:52:06.000000 myokit-1.36.1/myokit/formats/opencl/template/test.sh
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.002497 myokit-1.36.1/myokit/formats/python/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1049 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/python/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8251 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/python/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/python/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.002497 myokit-1.36.1/myokit/formats/python/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    10311 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/python/template/sim.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.003497 myokit-1.36.1/myokit/formats/sbml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      653 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/sbml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59396 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/sbml/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      987 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/sbml/_importer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29181 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/sbml/_parser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.004497 myokit-1.36.1/myokit/formats/stan/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2877 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/stan/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2998 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/formats/stan/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3745 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/stan/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.004497 myokit-1.36.1/myokit/formats/stan/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5305 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/stan/template/cell.stan
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       92 2023-02-05 15:45:10.000000 myokit-1.36.1/myokit/formats/stan/template/run.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.005497 myokit-1.36.1/myokit/formats/sympy/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1638 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/sympy/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6758 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/sympy/_ereader.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4875 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/sympy/_ewriter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.005497 myokit-1.36.1/myokit/formats/wcp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/wcp/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    17751 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/wcp/_wcp.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.006497 myokit-1.36.1/myokit/formats/xml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/xml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1494 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/xml/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      393 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/formats/xml/_split.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.008497 myokit-1.36.1/myokit/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6426 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/gui/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    49529 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/gui/datablock_viewer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    32774 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/gui/datalog_viewer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8676 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/gui/explorer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)   108238 2024-01-10 18:28:46.000000 myokit-1.36.1/myokit/gui/ide.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2157 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/gui/progress.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    52367 2024-03-08 14:23:00.000000 myokit-1.36.1/myokit/gui/source.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6072 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/gui/vargrapher.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.010497 myokit-1.36.1/myokit/lib/
+-rw-r--r--   0 michael   (1000) michael   (1000)      216 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/lib/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23859 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/lib/deps.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28056 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/lib/guess.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46813 2024-05-10 10:31:35.000000 myokit-1.36.1/myokit/lib/hh.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    67940 2024-02-01 17:37:08.000000 myokit-1.36.1/myokit/lib/markov.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4408 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/lib/multi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    13875 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/lib/plots.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4552 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/pacing.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8230 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/pype.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.032497 myokit-1.36.1/myokit/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)    10233 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2738 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/ansic_event_based_pacing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1250 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/ansic_time_series_pacing.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.037497 myokit-1.36.1/myokit/tests/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3022 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/tests/data/beeler-1977-model-compare-a.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2889 2023-10-13 08:52:06.000000 myokit-1.36.1/myokit/tests/data/beeler-1977-model-compare-b.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3137 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/tests/data/beeler-1977-model.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/beeler-1977-protocol.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/beeler-1977-script.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3287 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/tests/data/beeler-1977-units.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     5091 2023-10-13 08:52:06.000000 myokit-1.36.1/myokit/tests/data/clancy-1999-fitting.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3128 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/conditional.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6067 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/tests/data/cv1d.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/cv1d.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)    23916 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/decker-2009.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)    18227 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/data/decker.model
+-rw-r--r--   0 michael   (1000) michael   (1000)    10416 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/dn-1985-normalised.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      800 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/dom-markov.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.038497 myokit-1.36.1/myokit/tests/data/formats/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8192 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/abf-protocol.pro
+-rw-r--r--   0 michael   (1000) michael   (1000)    98376 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/abf-v1.abf
+-rw-r--r--   0 michael   (1000) michael   (1000)    44544 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/data/formats/abf-v2.abf
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.041497 myokit-1.36.1/myokit/tests/data/formats/cellml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/cellml/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)    59093 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/cellml/br-1977-dot.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    58593 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/cellml/br-1977.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)   117223 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/cellml/corrias.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)   221953 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/cellml/decker-2009.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1595 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/cellml/documentation.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/cellml/invalid-file.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    44837 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    44947 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.044497 myokit-1.36.1/myokit/tests/data/formats/channelml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2648 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      557 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2702 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2369 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1258 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1539 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1290 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1374 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1373 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      675 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1398 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1317 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.044497 myokit-1.36.1/myokit/tests/data/formats/sbml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8719 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     9801 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)    31408 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/sbml/HodgkinHuxley.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/sbml/LICENSE
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.045497 myokit-1.36.1/myokit/tests/data/formats/sbml/model/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2952 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1226 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.045497 myokit-1.36.1/myokit/tests/data/formats/sbml/result/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2457 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/sbml/result/00001-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     2206 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/sbml/result/00004-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/sbml/result/01103-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)    25600 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/formats/wcp-file.wcp
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.057497 myokit-1.36.1/myokit/tests/data/io/
+-rw-r--r--   0 michael   (1000) michael   (1000)      735 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad1d-1-not-enough-files.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109429 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad1d-2-no-header.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   104768 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad1d-3-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad1d-4-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109458 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad1d-5-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1549 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad1d-6-time-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad1d-7-0d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad1d-8-1d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)      739 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad2d-1-not-enough-files.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346240 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad2d-2-no-header.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   333091 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad2d-3-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad2d-4-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346257 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad2d-5-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1553 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad2d-6-time-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1588 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad2d-7-0d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/bad2d-8-2d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)      623 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/badlog-1-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1281 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/badlog-2-no-structure.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/badlog-3-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/badlog-4-invalid-n-fields.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/badlog-5-invalid-data-size.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1457 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/badlog-6-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/badlog-7-not-enough-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     6031 2023-06-07 13:48:59.000000 myokit-1.36.1/myokit/tests/data/io/block2d.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/block2d.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-1-empty.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-10-just-spaces.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-11-just-a-semicolon.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-12-bad-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-13-header-with-empty-1.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-14-header-with-empty-2.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-15-header-with-empty-3.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-16-wrong-columns-in-data.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-17-non-float-data.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      112 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-2-windows.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-3-old-mac.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-4-empty-lines.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-5-semicolons.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-6-open-string.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-7-empty-lines-2.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-8-unquoted-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      114 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog-9-double-quoted-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/datalog.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     1421 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/io/goodlog.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     4992 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/lr-1991-dep.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2315 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/lr-1991-fitting.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4571 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/lr-1991-testing.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6136 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/data/lr-1991.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.058497 myokit-1.36.1/myokit/tests/data/multi/
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/multi/beeler-1977-protocol.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/multi/beeler-1977-script.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/multi/beeler-no-name.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6013 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/multi/lr-1991.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/multi/not-a-model.csv
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:17.058497 myokit-1.36.1/myokit/tests/data/multi/subdir/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/multi/subdir/beeler-no-name.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3754 2023-06-07 13:48:23.000000 myokit-1.36.1/myokit/tests/data/noble-1962.mmt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    22536 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_aux.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    56981 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_cellml_v1_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    41869 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_cellml_v1_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12532 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_cellml_v1_writer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    73319 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_cellml_v2_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    26345 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_cellml_v2_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10977 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_cellml_v2_writer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4058 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_cmodel.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      476 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_compiler_detection.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14096 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_component.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11511 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_config.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    52565 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_datablock.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    91575 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_datalog.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    60654 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_dependency_checking.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)   138508 2023-11-21 18:38:30.000000 myokit-1.36.1/myokit/tests/test_expressions.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4882 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_float.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8085 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    13260 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_ansic.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    33181 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_axon.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    19078 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_formats_cellml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6703 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_formats_channelml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3762 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_cpp.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8695 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_cuda.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    13211 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_easyml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6647 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_exporters_run.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3520 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_html.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8546 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_latex.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    38093 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_mathml_content.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     9076 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_mathml_presentation.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8021 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_matlab.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8844 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_opencl.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    22761 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_python.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4672 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_formats_sbml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6310 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_stan.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10709 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_formats_sympy.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7658 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_formats_wcp.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14334 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_io.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1821 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_jacobian_calculator.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1767 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_jacobian_tracer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7476 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_lib_deps.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    42333 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_lib_guess.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    32591 2024-05-10 10:31:35.000000 myokit-1.36.1/myokit/tests/test_lib_hh.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    39983 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_lib_markov.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5145 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_lib_multi.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5754 2024-03-22 18:39:02.000000 myokit-1.36.1/myokit/tests/test_lib_plots.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2829 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_meta.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    87008 2024-03-10 14:01:18.000000 myokit-1.36.1/myokit/tests/test_model.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    16716 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_model_building.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3834 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_opencl_info.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8193 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_pacing_factory.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6504 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_pacing_system_c.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3637 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_pacing_system_py.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    50865 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_parsing.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2762 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_progress_reporters.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    15092 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_protocol.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12565 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_protocol_floating_point.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2318 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_protocol_time_series.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2402 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_pype.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7353 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_quantity.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3452 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_rhs_benchmarker.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    71633 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_sbml_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    54542 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_sbml_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    19281 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_simulation_1d.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    48408 2024-03-10 14:01:18.000000 myokit-1.36.1/myokit/tests/test_simulation_cvodes.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1853 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_simulation_cvodes_from_disk.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    36596 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_simulation_fiber_tissue.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14033 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_simulation_log_interval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    60162 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_simulation_opencl.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3005 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_simulation_opencl_log_interval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    20114 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_simulation_opencl_vs_cvode.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5216 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_simulation_opencl_vs_sim1d.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      562 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_system_info.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10358 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_tools.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    13635 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_unit.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_user_functions.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    33331 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/tests/test_variable.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16942 2024-02-01 16:26:05.000000 myokit-1.36.1/myokit/tools.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8503 2023-10-30 14:08:26.000000 myokit-1.36.1/myokit/units.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-05-10 10:35:16.951497 myokit-1.36.1/myokit.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5735 2024-05-10 10:35:16.000000 myokit-1.36.1/myokit.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15269 2024-05-10 10:35:16.000000 myokit-1.36.1/myokit.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2024-05-10 10:35:16.000000 myokit-1.36.1/myokit.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       48 2024-05-10 10:35:16.000000 myokit-1.36.1/myokit.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-01-04 14:18:38.000000 myokit-1.36.1/myokit.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      176 2024-05-10 10:35:16.000000 myokit-1.36.1/myokit.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        7 2024-05-10 10:35:16.000000 myokit-1.36.1/myokit.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-05-10 10:35:17.058497 myokit-1.36.1/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     3206 2023-10-30 14:08:26.000000 myokit-1.36.1/setup.py
```

### Comparing `myokit-1.36.0/LICENSE.txt` & `myokit-1.36.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/PKG-INFO` & `myokit-1.36.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myokit
-Version: 1.36.0
+Version: 1.36.1
 Summary: A modeling and simulation tool for cardiac cellular electrophysiology
 Home-page: http://myokit.org
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/myokit/myokit/issues
 Project-URL: Documentation, http://docs.myokit.org
```

### Comparing `myokit-1.36.0/README.md` & `myokit-1.36.1/README.md`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/__init__.py` & `myokit-1.36.1/myokit/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/__main__.py` & `myokit-1.36.1/myokit/__main__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_aux.py` & `myokit-1.36.1/myokit/_aux.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/example.mmt` & `myokit-1.36.1/myokit/_bin/example.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/find.png` & `myokit-1.36.1/myokit/_bin/gui/find.png`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-128.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-128.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-16.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-16.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-24.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-24.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-256.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-256.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-32.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-32.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-48.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-48.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-64.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-64.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer-96.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer-96.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer.ico` & `myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer.ico`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-datablock-viewer.png` & `myokit-1.36.1/myokit/_bin/gui/icon-datablock-viewer.png`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-ide-128.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-ide-128.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-ide-16.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-ide-16.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-ide-24.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-ide-24.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-ide-256.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-ide-256.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-ide-32.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-ide-32.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-ide-48.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-ide-48.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-ide-64.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-ide-64.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-ide-96.xpm` & `myokit-1.36.1/myokit/_bin/gui/icon-ide-96.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-ide.ico` & `myokit-1.36.1/myokit/_bin/gui/icon-ide.ico`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/icon-ide.png` & `myokit-1.36.1/myokit/_bin/gui/icon-ide.png`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/new.png` & `myokit-1.36.1/myokit/_bin/gui/new.png`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/open.png` & `myokit-1.36.1/myokit/_bin/gui/open.png`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/gui/save.png` & `myokit-1.36.1/myokit/_bin/gui/save.png`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/install-lin/myokit.lang` & `myokit-1.36.1/myokit/_bin/install-lin/myokit.lang`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/install-win/menu.json` & `myokit-1.36.1/myokit/_bin/install-win/menu.json`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/LICENSE` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/LICENSE`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib` & `myokit-1.36.1/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_config.py` & `myokit-1.36.1/myokit/_config.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_datablock.py` & `myokit-1.36.1/myokit/_datablock.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_datalog.py` & `myokit-1.36.1/myokit/_datalog.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_err.py` & `myokit-1.36.1/myokit/_err.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_expressions.py` & `myokit-1.36.1/myokit/_expressions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_io.py` & `myokit-1.36.1/myokit/_io.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_model_api.py` & `myokit-1.36.1/myokit/_model_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_myokit_version.py` & `myokit-1.36.1/myokit/_myokit_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Version as a tuple (major, minor, revision)
 #  - Changes to major are rare
 #  - Changes to minor indicate new features, possible slight backwards
 #    incompatibility
 #  - Changes to revision indicate bugfixes, tiny new features
 #  - There is no significance to odd/even numbers
-__version_tuple__ = 1, 36, 0
+__version_tuple__ = 1, 36, 1
 
 # String version of the version number
 __version__ = '.'.join([str(x) for x in __version_tuple__])
 if not __release__:  # pragma: no cover
     __version_tuple__ += ('dev', )
     __version__ += '.dev'
```

### Comparing `myokit-1.36.0/myokit/_parsing.py` & `myokit-1.36.1/myokit/_parsing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_progress.py` & `myokit-1.36.1/myokit/_progress.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_protocol.py` & `myokit-1.36.1/myokit/_protocol.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/__init__.py` & `myokit-1.36.1/myokit/_sim/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/cable.c` & `myokit-1.36.1/myokit/_sim/cable.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/cable.py` & `myokit-1.36.1/myokit/_sim/cable.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/cmodel.h` & `myokit-1.36.1/myokit/_sim/cmodel.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/cmodel.py` & `myokit-1.36.1/myokit/_sim/cmodel.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/compiler.c` & `myokit-1.36.1/myokit/_sim/compiler.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/compiler.py` & `myokit-1.36.1/myokit/_sim/compiler.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/cvodessim.c` & `myokit-1.36.1/myokit/_sim/cvodessim.c`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,34 @@
 #
 import myokit
 ?>
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 #include <stdio.h>
 
-#include <cvodes/cvodes.h>
-#include <nvector/nvector_serial.h>
-#include <sundials/sundials_types.h>
 #include <sundials/sundials_config.h>
 #ifndef SUNDIALS_VERSION_MAJOR
     #define SUNDIALS_VERSION_MAJOR 2
 #endif
+#include <sundials/sundials_types.h>
+#if SUNDIALS_VERSION_MAJOR >= 7
+    #define realtype sunrealtype
+    #define RCONST SUN_RCONST
+#endif
+#include <nvector/nvector_serial.h>
+#include <cvodes/cvodes.h>
 #if SUNDIALS_VERSION_MAJOR >= 3
     #include <sunmatrix/sunmatrix_dense.h>
     #include <sunlinsol/sunlinsol_dense.h>
-    #include <cvodes/cvodes_direct.h>
 #else
     #include <cvodes/cvodes_dense.h>
 #endif
+#if SUNDIALS_VERSION_MAJOR < 6
+    #include <cvodes/cvodes_direct.h>
+#endif
 
 <?
 if myokit.DEBUG_SM:
     print('// Show debug output')
     print('#ifndef MYOKIT_DEBUG_MESSAGES')
     print('#define MYOKIT_DEBUG_MESSAGES')
     print('#endif')
@@ -72,122 +78,196 @@
  * sensitivity analysis.
  */
 typedef struct {
     realtype *p;
 } *UserData;
 
 /*
+ * Check flags set by a generic sundials function, set python error.
+ *  sundials_flag: The value to check
+ *  funcname: The name of the function that returned the flag
+ */
+int
+check_sundials_flag(int flag, const char *funcname)
+{
+    /* Check if flag < 0 */
+    if (flag < 0) {
+        PyErr_Format(PyExc_Exception, "Function %s failed with flag = %d", funcname, flag);
+        return 1;
+    }
+    return 0;
+}
+
+/*
+ * Check flags set by any cvode-related function except cvode(), set python error.
+ *  sundials_flag: The value to check
+ *  funcname: The name of the function that returned the flag
+ */
+int
+check_cvode_related_flag(int flag, const char *funcname)
+{
+    /* Check if flag < 0 */
+    if (flag < 0) {
+        switch (flag) {
+        case CV_MEM_NULL:
+            PyErr_Format(PyExc_Exception, "Function %s failed with flag CV_MEM_NULL: The cvode memory block was not initialized.", funcname);
+            break;
+        case CV_MEM_FAIL:
+            PyErr_Format(PyExc_Exception, "Function %s failed with flag CV_MEM_FAIL: A memory allocation failed.", funcname);
+            break;
+        case CV_NO_MALLOC:
+            PyErr_Format(PyExc_Exception, "Function %s failed with flag CV_NO_MALLOC: A memory allocation function returned NULL.", funcname);
+            break;
+        case CV_ILL_INPUT:
+            PyErr_Format(PyExc_Exception, "Function %s failed with flag CV_ILL_INPUT: Invalid input arguments.", funcname);
+            break;
+        case CV_NO_SENS:
+            PyErr_Format(PyExc_Exception, "Function %s failed with flag CV_NO_SENS: Forward sensitivity analysis was not initialized.", funcname);
+            break;
+        case CV_BAD_K:
+            PyErr_Format(PyExc_Exception, "Function %s failed with flag CV_BAD_K: Argument k is not in range.", funcname);
+            break;
+        case CV_BAD_T:
+            PyErr_Format(PyExc_Exception, "Function %s failed with flag CV_BAD_T: Argument t is not in range.", funcname);
+            break;
+        case CV_BAD_DKY:
+            PyErr_Format(PyExc_Exception, "Function %s failed with flag CV_BAD_DKY: The argument DKY was NULL.", funcname);
+            break;
+        default:
+            PyErr_Format(PyExc_Exception, "Function %s failed with unhandled flag = %d", funcname, flag);
+        }
+        return 1;
+    }
+    return 0;
+}
+
+/*
  * Check sundials flags, set python error.
- *  flagvalue : The value to check
+ *  flag: The value to check
+ *  funcname: The name of the function that returned the flag
+ */
+int
+check_cvode_flag(int flag)
+{
+    /* Check if flag < 0 */
+    if (flag < 0) {
+        switch (flag) {
+        case CV_TOO_MUCH_WORK:
+            PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag CV_TOO_MUCH_WORK: The solver took mxstep internal steps but could not reach tout.");
+            break;
+        case CV_TOO_MUCH_ACC:
+            PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag CV_TOO_MUCH_ACC: The solver could not satisfy the accuracy demanded by the user for some internal step.");
+            break;
+        case CV_ERR_FAILURE:
+            PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag CV_ERR_FAILURE: Error test failures occurred too many times during one internal time step or minimum step size was reached.");
+            break;
+        case CV_CONV_FAILURE:
+            PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag CV_CONV_FAILURE: Convergence test failures occurred too many times during one internal time step or minimum step size was reached.");
+            break;
+        case CV_LINIT_FAIL:
+            PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag CV_LINIT_FAIL: The linear solver's initialization function failed.");
+            break;
+        case -6:
+            PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -6 CV_LSETUP_FAIL: The linear solver's setup function failed in an unrecoverable manner.");
+            break;
+        case -7:
+            PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -7 CV_LSOLVE_FAIL: The linear solver's solve function failed in an unrecoverable manner.");
+            break;
+        case -8:
+            PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -8 CV_RHSFUNC_FAIL: The right-hand side function failed in an unrecoverable manner.");
+            break;
+        case -9:
+            PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -9 CV_FIRST_RHSFUNC_ERR: The right-hand side function failed at the first call.");
+            break;
+        case -10:
+            PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -10 CV_REPTD_RHSFUNC_ERR: The right-hand side function had repeated recoverable errors.");
+            break;
+        case -11:
+            PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -11 CV_UNREC_RHSFUNC_ERR: The right-hand side function had a recoverable error, but no recovery is possible.");
+            break;
+        case -12:
+            PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -12 CV_RTFUNC_FAIL: The root finding function failed in an unrecoverable manner.");
+            break;
+        case -20:
+            PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -20 CV_MEM_FAIL: A memory allocation failed.");
+            break;
+        case -21:
+            PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -21 CV_MEM_NULL: The cvode mem argument was NULL.");
+            break;
+        case -22:
+            PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -22 CV_ILL_INPUT: One of the function inputs is illegal.");
+            break;
+        case -23:
+            PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -23 CV_NO_MALLOC: The cvode memory block was not allocated by a call to CVodeMalloc.");
+            break;
+        case -24:
+            PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -24 CV_BAD_K: The derivative order k is larger than the order used.");
+            break;
+        case -25:
+            PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -25 CV_BAD_T: The time t is outside the last step taken.");
+            break;
+        case -26:
+            PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -26 CV_BAD_DKY: The output derivative vector is NULL.");
+            break;
+        case -27:
+            PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -27 CV_TOO_CLOSE: The output and initial times are too close to each other.");
+            break;
+        default:
+            PyErr_Format(PyExc_Exception, "Function CVode() failed with unhandled flag = %d", flag);
+        }
+        return 1;
+    }
+    return 0;
+}
+
+#if SUNDIALS_VERSION_MAJOR >= 7
+/*
+ * Check sundials error code (Sundials 7 and above)
+ *  sunerr   : The SunErroCode to check
  *  funcname : The name of the function that returned the flag
- *  opt : Mode selector
- *         0 : Error if the flag is null
- *         1 : Error if the flag is < 0
- *         2 : Errir
  */
 int
-check_cvode_flag(void *flagvalue, char *funcname, int opt)
+check_sundials_error(SUNErrCode code, const char *funcname)
 {
-    if (opt == 0 && flagvalue == NULL) {
-        /* Check if sundials function returned null pointer */
-        PyErr_Format(PyExc_Exception, "%s() failed - returned NULL pointer", funcname);
+    const char* msg;
+    if (code) {
+        msg = SUNGetErrMsg(code);
+        PyErr_Format(PyExc_Exception, "%s() failed with message = %s", funcname, msg);
         return 1;
-    } else if (opt == 1) {
-        /* Check if flag < 0 */
-        int flag = *((int*)flagvalue);
-        if (flag < 0) {
-            if (strcmp(funcname, "CVode") == 0) {
-                switch (flag) {
-                case -1:
-                    PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -1 CV_TOO_MUCH_WORK: The solver took mxstep internal steps but could not reach tout.");
-                    break;
-                case -2:
-                    PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -2 CV_TOO_MUCH_ACC: The solver could not satisfy the accuracy demanded by the user for some internal step.");
-                    break;
-                case -3:
-                    PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -3 CV_ERR_FAILURE: Error test failures occurred too many times during one internal time step or minimum step size was reached.");
-                    break;
-                case -4:
-                    PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -4 CV_CONV_FAILURE: Convergence test failures occurred too many times during one internal time step or minimum step size was reached.");
-                    break;
-                case -5:
-                    PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -5 CV_LINIT_FAIL: The linear solver's initialization function failed.");
-                    break;
-                case -6:
-                    PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -6 CV_LSETUP_FAIL: The linear solver's setup function failed in an unrecoverable manner.");
-                    break;
-                case -7:
-                    PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -7 CV_LSOLVE_FAIL: The linear solver's solve function failed in an unrecoverable manner.");
-                    break;
-                case -8:
-                    PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -8 CV_RHSFUNC_FAIL: The right-hand side function failed in an unrecoverable manner.");
-                    break;
-                case -9:
-                    PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -9 CV_FIRST_RHSFUNC_ERR: The right-hand side function failed at the first call.");
-                    break;
-                case -10:
-                    PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -10 CV_REPTD_RHSFUNC_ERR: The right-hand side function had repeated recoverable errors.");
-                    break;
-                case -11:
-                    PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -11 CV_UNREC_RHSFUNC_ERR: The right-hand side function had a recoverable error, but no recovery is possible.");
-                    break;
-                case -12:
-                    PyErr_SetString(PyExc_ArithmeticError, "Function CVode() failed with flag -12 CV_RTFUNC_FAIL: The root finding function failed in an unrecoverable manner.");
-                    break;
-                case -20:
-                    PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -20 CV_MEM_FAIL: A memory allocation failed.");
-                    break;
-                case -21:
-                    PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -21 CV_MEM_NULL: The cvode mem argument was NULL.");
-                    break;
-                case -22:
-                    PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -22 CV_ILL_INPUT: One of the function inputs is illegal.");
-                    break;
-                case -23:
-                    PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -23 CV_NO_MALLOC: The cvode memory block was not allocated by a call to CVodeMalloc.");
-                    break;
-                case -24:
-                    PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -24 CV_BAD_K: The derivative order k is larger than the order used.");
-                    break;
-                case -25:
-                    PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -25 CV_BAD_T: The time t is outside the last step taken.");
-                    break;
-                case -26:
-                    PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -26 CV_BAD_DKY: The output derivative vector is NULL.");
-                    break;
-                case -27:
-                    PyErr_SetString(PyExc_Exception, "Function CVode() failed with flag -27 CV_TOO_CLOSE: The output and initial times are too close to each other.");
-                    break;
-                default:
-                    PyErr_Format(PyExc_Exception, "Function CVode() failed with unknown flag = %d", flag);
-                }
-            } else {
-                PyErr_Format(PyExc_Exception, "%s() failed with flag = %d", funcname, flag);
-            }
-            return 1;
-        }
     }
     return 0;
 }
+#endif
 
 /*
  * Error and warning message handler for CVODES.
- * Error messages are already set via check_cvode_flag, so this method
+ * Error messages are already set via check_cvode_flag & co, so this method
  * suppresses error messages.
  * Warnings are passed to Python's warning system, where they can be
  * caught or suppressed using the warnings module.
  */
+#if SUNDIALS_VERSION_MAJOR >= 7
+void
+ErrorHandler(int line, const char* function, const char* file, const char* msg,
+             SUNErrCode error_code, void* err_user_data, SUNContext context)
+{
+    if (error_code) {
+        PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "CVODES: %s", msg);
+    }
+}
+#else
 void
 ErrorHandler(int error_code, const char *module, const char *function,
              char *msg, void *eh_data)
 {
     if (error_code > 0) {
         PyErr_WarnFormat(PyExc_RuntimeWarning, 1, "CVODES: %s", msg);
     }
 }
+#endif
 
 /*
  * Initialisation status.
  * Proper sequence is init(), repeated step() calls till finished, then clean.
  */
 int initialized = 0; /* Has the simulation been initialized */
 
@@ -565,14 +645,18 @@
     #endif
 
     /* Error checking flags */
     int flag_cvode;
     Model_Flag flag_model;
     ESys_Flag flag_epacing;
     TSys_Flag flag_fpacing;
+    /* Error handling in >=7 */
+    #if SUNDIALS_VERSION_MAJOR >= 7
+    SUNErrCode sunerr;
+    #endif
 
     /* Pacing systems */
     ESys epacing;
     TSys fpacing;
     const char* protocol_type_name;
 
     /* General purpose ints for iterating */
@@ -743,19 +827,20 @@
     #ifdef MYOKIT_DEBUG_PROFILING
     benchmarker_print("CP Created C model struct.");
     #endif
 
     /*
      * Create sundials context
      */
-    #if SUNDIALS_VERSION_MAJOR >= 6
+    #if SUNDIALS_VERSION_MAJOR >= 7
+    sunerr = SUNContext_Create(SUN_COMM_NULL, &sundials_context);
+    if (check_sundials_error(sunerr, "SUNContext_Create")) return sim_clean();
+    #elif SUNDIALS_VERSION_MAJOR >= 6
     flag_cvode = SUNContext_Create(NULL, &sundials_context);
-    if (check_cvode_flag(&flag_cvode, "SUNContext_Create", 1)) {
-        return sim_cleanx(PyExc_Exception, "Failed to create Sundials context.");
-    }
+    if (check_sundials_flag(flag_cvode, "SUNContext_Create")) return sim_clean();
     #ifdef MYOKIT_DEBUG_PROFILING
     benchmarker_print("CP Created sundials context.");
     #endif
     #endif
 
     /*
      * Create state vectors
@@ -763,34 +848,28 @@
 
     /* Create state vector */
     #if SUNDIALS_VERSION_MAJOR >= 6
     y = N_VNew_Serial(model->n_states, sundials_context);
     #else
     y = N_VNew_Serial(model->n_states);
     #endif
-    if (check_cvode_flag((void*)y, "N_VNew_Serial", 0)) {
-        return sim_cleanx(PyExc_Exception, "Failed to create state vector.");
-    }
+    if (y == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for state vector.");
 
     /* Create state vector copy for error handling */
     #if SUNDIALS_VERSION_MAJOR >= 6
     ylast = N_VNew_Serial(model->n_states, sundials_context);
     #else
     ylast = N_VNew_Serial(model->n_states);
     #endif
-    if (check_cvode_flag((void*)ylast, "N_VNew_Serial", 0)) {
-        return sim_cleanx(PyExc_Exception, "Failed to create last-state vector.");
-    }
+    if (ylast == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for last-state vector.");
 
     /* Create sensitivity vector array */
     if (model->has_sensitivities) {
         sy = N_VCloneVectorArray(model->ns_independents, y);
-        if (check_cvode_flag((void*)sy, "N_VCloneVectorArray", 0)) {
-            return sim_cleanx(PyExc_Exception, "Failed to allocate space to store sensitivities.");
-        }
+        if (sy == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for sensitivity vector array.");
     }
 
     /*
      * Create state vectors for logging
      */
 
     /* Determine if dynamic logging is being used (or if it's periodic/point-list logging) */
@@ -805,22 +884,18 @@
         sz = sy;
     } else {
         #if SUNDIALS_VERSION_MAJOR >= 6
         z = N_VNew_Serial(model->n_states, sundials_context);
         #else
         z = N_VNew_Serial(model->n_states);
         #endif
-        if (check_cvode_flag((void*)z, "N_VNew_Serial", 0)) {
-            return sim_cleanx(PyExc_Exception, "Failed to create state vector for logging.");
-        }
+        if (z == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for state vector for logging.");
         if (model->has_sensitivities) {
             sz = N_VCloneVectorArray(model->ns_independents, y);
-            if (check_cvode_flag((void*)sz, "N_VCloneVectorArray", 0)) {
-                return sim_cleanx(PyExc_Exception, "Failed to create state sensitivity vector array for logging.");
-            }
+            if (sz == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for sensitivity vector array for logging.");
         }
     }
 
     #ifdef MYOKIT_DEBUG_PROFILING
     benchmarker_print("CP Created sundials state vectors.");
     #endif
 
@@ -960,17 +1035,15 @@
         for (i=0; i<model->ns_independents; i++) {
             udata->p[i] = *model->s_independents[i];
         }
 
         /* Create parameter scaling vector, for error control */
         /* TODO: Get this from the Python code ? */
         pbar = (realtype*)malloc((size_t)model->ns_independents * sizeof(realtype));
-        if (pbar == NULL) {
-            return sim_cleanx(PyExc_Exception, "Unable to allocate space to store parameter scales.");
-        }
+        if (pbar == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for parameter scale array.");
         for (i=0; i<model->ns_independents; i++) {
             pbar[i] = (udata->p[i] == 0.0 ? 1.0 : fabs(udata->p[i]));
         }
 
         #ifdef MYOKIT_DEBUG_PROFILING
         benchmarker_print("CP Created UserData for sensitivities.");
         #endif
@@ -986,25 +1059,19 @@
         #endif
         if (!PyList_Check(protocols)) {
             return sim_cleanx(PyExc_TypeError, "'protocols' must be a list.");
         }
         n_pace = (int)PyList_Size(protocols);
     }
     pacing_systems = (union PSys*)malloc((size_t)n_pace * sizeof(union PSys));
-    if (pacing_systems == NULL) {
-        return sim_cleanx(PyExc_Exception, "Unable to allocate space to store pacing systems.");
-    }
+    if (pacing_systems == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for pacing systems.");
     pacing_types = (enum PSysType *)malloc((size_t)n_pace * sizeof(enum PSysType));
-    if (pacing_types == NULL) {
-        return sim_cleanx(PyExc_Exception, "Unable to allocate space to store pacing types.");
-    }
+    if (pacing_types == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for pacing types.");
     pacing = (realtype*)malloc((size_t)n_pace * sizeof(realtype));
-    if (pacing == NULL) {
-        return sim_cleanx(PyExc_Exception, "Unable to allocate space to store pacing values.");
-    }
+    if (pacing == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for pacing values.");
     Model_SetupPacing(model, n_pace);
 
     /*
      *  Unless set by pacing, tnext is set to tmax
      */
     tnext = tmax;
 
@@ -1077,101 +1144,106 @@
         #if SUNDIALS_VERSION_MAJOR >= 6
         cvode_mem = CVodeCreate(CV_BDF, sundials_context);
         #elif SUNDIALS_VERSION_MAJOR >= 4
         cvode_mem = CVodeCreate(CV_BDF);  /* Newton is still default */
         #else
         cvode_mem = CVodeCreate(CV_BDF, CV_NEWTON);
         #endif
-        if (check_cvode_flag((void*)cvode_mem, "CVodeCreate", 0)) return sim_clean();
+        if (cvode_mem == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate CVODE memory.");
 
         /* Set error and warning-message handler */
+        #if SUNDIALS_VERSION_MAJOR >= 7
+        sunerr = SUNContext_PushErrHandler(sundials_context, ErrorHandler, NULL);
+        if (check_sundials_error(sunerr, "SUNContext_PushErrHandler")) return sim_clean();
+        #else
         flag_cvode = CVodeSetErrHandlerFn(cvode_mem, ErrorHandler, NULL);
-        if (check_cvode_flag(&flag_cvode, "CVodeInit", 1)) return sim_clean();
+        if (check_cvode_related_flag(flag_cvode, "CVodeSetErrHandlerFn")) return sim_clean();
+        #endif
 
         /* Initialize solver memory, specify the rhs */
         flag_cvode = CVodeInit(cvode_mem, rhs, t, y);
-        if (check_cvode_flag(&flag_cvode, "CVodeInit", 1)) return sim_clean();
+        if (check_cvode_related_flag(flag_cvode, "CVodeInit")) return sim_clean();
 
         /* Set absolute and relative tolerances */
         flag_cvode = CVodeSStolerances(cvode_mem, RCONST(rel_tol), RCONST(abs_tol));
-        if (check_cvode_flag(&flag_cvode, "CVodeSStolerances", 1)) return sim_clean();
+        if (check_cvode_related_flag(flag_cvode, "CVodeSStolerances")) return sim_clean();
 
         /* Set a maximum step size (or 0.0 for none) */
         flag_cvode = CVodeSetMaxStep(cvode_mem, dt_max < 0 ? 0.0 : dt_max);
-        if (check_cvode_flag(&flag_cvode, "CVodeSetmaxStep", 1)) return sim_clean();
+        if (check_cvode_related_flag(flag_cvode, "CVodeSetmaxStep")) return sim_clean();
 
         /* Set a minimum step size (or 0.0 for none) */
         flag_cvode = CVodeSetMinStep(cvode_mem, dt_min < 0 ? 0.0 : dt_min);
-        if (check_cvode_flag(&flag_cvode, "CVodeSetminStep", 1)) return sim_clean();
+        if (check_cvode_related_flag(flag_cvode, "CVodeSetminStep")) return sim_clean();
 
         #if SUNDIALS_VERSION_MAJOR >= 6
             /* Create dense matrix for use in linear solves */
             sundense_matrix = SUNDenseMatrix(model->n_states, model->n_states, sundials_context);
-            if (check_cvode_flag((void *)sundense_matrix, "SUNDenseMatrix", 0)) return sim_clean();
+            if (sundense_matrix == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for dense matrix.");
 
             /* Create dense linear solver object with matrix */
             sundense_solver = SUNLinSol_Dense(y, sundense_matrix, sundials_context);
-            if (check_cvode_flag((void *)sundense_solver, "SUNLinSol_Dense", 0)) return sim_clean();
+            if (sundense_solver == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for dense solver.");
 
             /* Attach the matrix and solver to cvode */
             flag_cvode = CVodeSetLinearSolver(cvode_mem, sundense_solver, sundense_matrix);
-            if (check_cvode_flag(&flag_cvode, "CVodeSetLinearSolver", 1)) return sim_clean();
+            if (check_sundials_flag(flag_cvode, "CVodeSetLinearSolver")) return sim_clean();
         #elif SUNDIALS_VERSION_MAJOR >= 4
             /* Create dense matrix for use in linear solves */
             sundense_matrix = SUNDenseMatrix(model->n_states, model->n_states);
-            if (check_cvode_flag((void *)sundense_matrix, "SUNDenseMatrix", 0)) return sim_clean();
+            if (sundense_matrix == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for dense matrix.");
 
             /* Create dense linear solver object with matrix */
             sundense_solver = SUNLinSol_Dense(y, sundense_matrix);
-            if (check_cvode_flag((void *)sundense_solver, "SUNLinSol_Dense", 0)) return sim_clean();
+            if (sundense_solver == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for dense solver.");
 
             /* Attach the matrix and solver to cvode */
             flag_cvode = CVodeSetLinearSolver(cvode_mem, sundense_solver, sundense_matrix);
-            if (check_cvode_flag(&flag_cvode, "CVodeSetLinearSolver", 1)) return sim_clean();
+            if (check_sundials_flag(flag_cvode, "CVodeSetLinearSolver")) return sim_clean();
         #elif SUNDIALS_VERSION_MAJOR >= 3
             /* Create dense matrix for use in linear solves */
             sundense_matrix = SUNDenseMatrix(model->n_states, model->n_states);
-            if (check_cvode_flag((void *)sundense_matrix, "SUNDenseMatrix", 0)) return sim_clean();
+            if (sundense_matrix == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for dense matrix.");
 
             /* Create dense linear solver object with matrix */
             sundense_solver = SUNDenseLinearSolver(y, sundense_matrix);
-            if (check_cvode_flag((void *)sundense_solver, "SUNDenseLinearSolver", 0)) return sim_clean();
+            if (sundense_solver == NULL) return sim_cleanx(PyExc_Exception, "Unable to allocate space for dense solver.");
 
             /* Attach the matrix and solver to cvode */
             flag_cvode = CVDlsSetLinearSolver(cvode_mem, sundense_solver, sundense_matrix);
-            if (check_cvode_flag(&flag_cvode, "CVDlsSetLinearSolver", 1)) return sim_clean();
+            if (check_sundials_flag(flag_cvode, "CVDlsSetLinearSolver")) return sim_clean();
         #else
             /* Create dense matrix for use in linear solves */
             flag_cvode = CVDense(cvode_mem, model->n_states);
-            if (check_cvode_flag(&flag_cvode, "CVDense", 1)) return sim_clean();
+            if (check_sundials_flag(flag_cvode, "CVDense")) return sim_clean();
         #endif
 
         #ifdef MYOKIT_DEBUG_PROFILING
         benchmarker_print("CP CVODES solver initialized.");
         #endif
 
         /* Activate forward sensitivity computations */
         if (model->has_sensitivities) {
             /* TODO: NULL here is the place to insert a user function to calculate the
                RHS of the sensitivity ODE */
             /*flag_cvode = CVodeSensInit(cvode_mem, model->ns_independents, CV_SIMULTANEOUS, rhs1, sy);*/
             flag_cvode = CVodeSensInit(cvode_mem, model->ns_independents, CV_SIMULTANEOUS, NULL, sy);
-            if (check_cvode_flag(&flag_cvode, "CVodeSensInit", 1)) return sim_clean();
+            if (check_cvode_related_flag(flag_cvode, "CVodeSensInit")) return sim_clean();
 
             /* Attach user data */
             flag_cvode = CVodeSetUserData(cvode_mem, udata);
-            if (check_cvode_flag(&flag_cvode, "CVodeSetUserData", 1)) return sim_clean();
+            if (check_cvode_related_flag(flag_cvode, "CVodeSetUserData")) return sim_clean();
 
             /* Set parameter scales used in tolerances */
             flag_cvode = CVodeSetSensParams(cvode_mem, udata->p, pbar, NULL);
-            if (check_cvode_flag(&flag_cvode, "CVodeSetSensParams", 1)) return sim_clean();
+            if (check_cvode_related_flag(flag_cvode, "CVodeSetSensParams")) return sim_clean();
 
             /* Set sensitivity tolerances calculating method (using pbar) */
             flag_cvode = CVodeSensEEtolerances(cvode_mem);
-            if (check_cvode_flag(&flag_cvode, "CVodeSensEEtolerances", 1)) return sim_clean();
+            if (check_cvode_related_flag(flag_cvode, "CVodeSensEEtolerances")) return sim_clean();
 
             #ifdef MYOKIT_DEBUG_PROFILING
             benchmarker_print("CP CVODES sensitivity methods initialized.");
             #endif
         }
     }
 
@@ -1180,15 +1252,15 @@
      * Enabled if rf_list is a PyList
      */
     rf_direction = NULL;
 
     if (model->is_ode && PyList_Check(rf_list)) {
         /* Initialize root function with 1 component */
         flag_cvode = CVodeRootInit(cvode_mem, 1, rf_function);
-        if (check_cvode_flag(&flag_cvode, "CVodeRootInit", 1)) return sim_clean();
+        if (check_cvode_related_flag(flag_cvode, "CVodeRootInit")) return sim_clean();
 
         /* Direction of root crossings, one entry per root function, but we only use 1. */
         rf_direction = (int*)malloc(sizeof(int));
 
         #ifdef MYOKIT_DEBUG_PROFILING
         benchmarker_print("CP CVODES root-finding initialized.");
         #endif
@@ -1412,15 +1484,15 @@
             printf("%ld,\t%ld,\t%ld,\t%ld,\t%d,\t%d,\t%g,\t%g,\t%g,\t%g\n",
                    cv_nsteps, cv_nfevals, cv_nlinsetups, cv_netfails,
                    cv_qlast, cv_qcur,
                    cv_hinused, cv_hlast, cv_hcur, cv_tcur);
             #endif
 
             /* Check for errors */
-            if (check_cvode_flag(&flag_cvode, "CVode", 1)) {
+            if (check_cvode_flag(flag_cvode)) {
                 #ifdef MYOKIT_DEBUG_MESSAGES
                 printf("\nCM CVODE flag %d. Setting error output and returning.\n", flag_cvode);
                 #endif
 
                 /* Something went wrong... Set outputs and return */
                 for (i=0; i<model->n_states; i++) {
                     PyList_SetItem(state_py, i, PyFloat_FromDouble(NV_Ith_S(ylast, i)));
@@ -1483,37 +1555,37 @@
                 if (t > tnext) {
                     #ifdef MYOKIT_DEBUG_MESSAGES
                     printf("CM Event time exceeded, rewinding to %g.\n", tnext);
                     #endif
 
                     /* Go back to time=tnext */
                     flag_cvode = CVodeGetDky(cvode_mem, tnext, 0, y);
-                    if (check_cvode_flag(&flag_cvode, "CVodeGetDky", 1)) return sim_clean();
+                    if (check_cvode_related_flag(flag_cvode, "CVodeGetDky")) return sim_clean();
                     if (model->has_sensitivities) {
                         flag_cvode = CVodeGetSensDky(cvode_mem, tnext, 0, sy);
-                        if (check_cvode_flag(&flag_cvode, "CVodeGetSensDky", 1)) return sim_clean();
+                        if (check_cvode_related_flag(flag_cvode, "CVodeGetSensDky")) return sim_clean();
                     }
                     t = tnext;
                     /* Require reinit (after logging) */
                     flag_reinit = 1;
 
                 } else {
 
                     /* Get current sensitivity vector */
                     if (model->has_sensitivities) {
                         flag_cvode = CVodeGetSens(cvode_mem, &t, sy);
-                        if (check_cvode_flag(&flag_cvode, "CVodeGetSens", 1)) return sim_clean();
+                        if (check_cvode_related_flag(flag_cvode, "CVodeGetSens")) return sim_clean();
                     }
 
                     /* Root found */
                     if (flag_cvode == CV_ROOT_RETURN) {
 
                         /* Get directions of root crossings (1 per root function) */
                         flag_root = CVodeGetRootInfo(cvode_mem, rf_direction);
-                        if (check_cvode_flag(&flag_root, "CVodeGetRootInfo", 1)) return sim_clean();
+                        if (check_cvode_related_flag(flag_root, "CVodeGetRootInfo")) return sim_clean();
                         /* We only have one root function, so we know that rf_direction[0] is non-zero at this point. */
 
                         /* Store tuple (time, direction) for the found root */
                         val = PyTuple_New(2);
                         PyTuple_SetItem(val, 0, PyFloat_FromDouble(t)); /* Steals reference, so this is ok */
                         PyTuple_SetItem(val, 1, PyLong_FromLong(rf_direction[0]));
                         if (PyList_Append(rf_list, val)) {    /* Doesn't steal, need to decref */
@@ -1545,18 +1617,18 @@
                         realtime = benchmarker_realtime();
                         if (realtime < 0) return sim_cleanx(PyExc_Exception, "Failed to set realtime during interpolation logging.");
                     }
 
                     /* Get interpolated y(tlog) */
                     if (model->is_ode) {
                         flag_cvode = CVodeGetDky(cvode_mem, tlog, 0, z);
-                        if (check_cvode_flag(&flag_cvode, "CVodeGetDky", 1)) return sim_clean();
+                        if (check_cvode_related_flag(flag_cvode, "CVodeGetDky")) return sim_clean();
                         if (model->has_sensitivities) {
                             flag_cvode = CVodeGetSensDky(cvode_mem, tlog, 0, sz);
-                            if (check_cvode_flag(&flag_cvode, "CVodeGetSensDky", 1)) return sim_clean();
+                            if (check_cvode_related_flag(flag_cvode, "CVodeGetSensDky")) return sim_clean();
                         }
                     }
                     /* If cvode-free mode, the states can't change so we don't
                        need to do anything here */
 
                     /* Calculate intermediate variables & derivatives */
                     rhs(tlog, z, NULL, udata);
@@ -1674,18 +1746,18 @@
             }
 
             /*
              * Reinitialize CVODE if needed
              */
             if (model->is_ode && flag_reinit) {
                 flag_cvode = CVodeReInit(cvode_mem, t, y);
-                if (check_cvode_flag(&flag_cvode, "CVodeReInit", 1)) return sim_clean();
+                if (check_cvode_related_flag(flag_cvode, "CVodeReInit")) return sim_clean();
                 if (model->has_sensitivities) {
                     flag_cvode = CVodeSensReInit(cvode_mem, CV_SIMULTANEOUS, sy);
-                    if (check_cvode_flag(&flag_cvode, "CVodeSensReInit", 1)) return sim_clean();
+                    if (check_cvode_related_flag(flag_cvode, "CVodeSensReInit")) return sim_clean();
                 }
                 flag_reinit = 0;
             }
         }
 
         /*
          * Check if we're finished
```

### Comparing `myokit-1.36.0/myokit/_sim/cvodessim.py` & `myokit-1.36.1/myokit/_sim/cvodessim.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/differential.hpp` & `myokit-1.36.1/myokit/_sim/differential.hpp`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/fiber_tissue.c` & `myokit-1.36.1/myokit/_sim/fiber_tissue.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/fiber_tissue.py` & `myokit-1.36.1/myokit/_sim/fiber_tissue.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/jacobian.cpp` & `myokit-1.36.1/myokit/_sim/jacobian.cpp`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/jacobian.py` & `myokit-1.36.1/myokit/_sim/jacobian.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/mcl.h` & `myokit-1.36.1/myokit/_sim/mcl.h`

 * *Files 4% similar despite different names*

```diff
@@ -647,84 +647,117 @@
     device = PyDict_New();
     if(device == NULL) {
         PyErr_SetString(PyExc_Exception, "Unable to create dict for device info.");
         return NULL;
     }
 
     // Name
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying name\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_NAME, bufsize, buffer, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyUnicode_FromString(buffer);
     PyDict_SetItemString(device, "name", val);
     Py_CLEAR(val);
 
     // Vendor
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying vendor\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_VENDOR, bufsize, buffer, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyUnicode_FromString(buffer);
     PyDict_SetItemString(device, "vendor", val);
     Py_CLEAR(val);
 
     // Device version
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying device version\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_VERSION, bufsize, buffer, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyUnicode_FromString(buffer);
     PyDict_SetItemString(device, "version", val);
     Py_CLEAR(val);
 
     // Driver version
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying driver version\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DRIVER_VERSION, bufsize, buffer, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyUnicode_FromString(buffer);
     PyDict_SetItemString(device, "driver", val);
     Py_CLEAR(val);
 
     // Clock speed (MHz)
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying clock speed\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_MAX_CLOCK_FREQUENCY, sizeof(buf_uint), &buf_uint, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyLong_FromUnsignedLong(buf_uint);
     PyDict_SetItemString(device, "clock", val);
     Py_CLEAR(val);
 
     // Global memory (bytes)
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying global memory size\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_GLOBAL_MEM_SIZE, sizeof(buf_ulong), &buf_ulong, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyLong_FromUnsignedLongLong(buf_ulong);
     PyDict_SetItemString(device, "global", val);
     Py_CLEAR(val);
 
     // Local memory (bytes)
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying local memory size\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_LOCAL_MEM_SIZE, sizeof(buf_ulong), &buf_ulong, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyLong_FromUnsignedLongLong(buf_ulong);
     PyDict_SetItemString(device, "local", val);
     Py_CLEAR(val);
 
     // Const memory (bytes)
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying max buffer size\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_MAX_CONSTANT_BUFFER_SIZE, sizeof(buf_ulong), &buf_ulong, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyLong_FromUnsignedLongLong(buf_ulong);
     PyDict_SetItemString(device, "const", val);
     Py_CLEAR(val);
 
     // Computing units
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying max computing units\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_MAX_COMPUTE_UNITS, sizeof(buf_uint), &buf_uint, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyLong_FromUnsignedLong(buf_uint);
     PyDict_SetItemString(device, "units", val);
     Py_CLEAR(val);
 
     // Max workgroup size
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying max work group size\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_MAX_WORK_GROUP_SIZE, sizeof(buf_size_t), &buf_size_t, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyLong_FromSize_t(buf_size_t);
     PyDict_SetItemString(device, "groups", val);
     Py_CLEAR(val);
 
     // Max workitem sizes
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying max work item sizes\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_MAX_WORK_ITEM_DIMENSIONS, sizeof(buf_uint), &buf_uint, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyLong_FromUnsignedLong(buf_uint);
     PyDict_SetItemString(device, "dimensions", val);
     Py_CLEAR(val);
 
     work_item_sizes = (size_t*)malloc(buf_uint * sizeof(size_t));
@@ -735,14 +768,17 @@
         PyTuple_SetItem(items_sizes_tuple, i, PyLong_FromSize_t(work_item_sizes[i]));
     }
     free(work_item_sizes); work_item_sizes = NULL;
     PyDict_SetItemString(device, "items", items_sizes_tuple);
     Py_CLEAR(items_sizes_tuple);
 
     // Maximum size of a kernel parameter
+    #ifdef MYOKIT_DEBUG_MESSAGES
+    printf("  Querying maximum kernel parameter size\n");
+    #endif
     flag = clGetDeviceInfo(device_id, CL_DEVICE_MAX_PARAMETER_SIZE, sizeof(buf_size_t), &buf_size_t, NULL);
     if(mcl_flag(flag)) { Py_DECREF(device); return NULL; }
     val = PyLong_FromSize_t(buf_size_t);
     PyDict_SetItemString(device, "param", val);
     Py_CLEAR(val);
 
     // Done!
@@ -830,37 +866,55 @@
     // No platforms found
     if (n_platforms == 0) {
         return platforms;
     }
 
     // Check all platforms
     for (i=0; i<n_platforms; i++) {
+        #ifdef MYOKIT_DEBUG_MESSAGES
+        printf("Checking platform %u\n", (unsigned int)i);
+        #endif
 
         // Create platform dict
         platform = mcl_info_platform_dict(platform_ids[i], sizeof(buffer), buffer);
         if (platform == NULL) { Py_DECREF(platforms); return NULL; }
+        #ifdef MYOKIT_DEBUG_MESSAGES
+        printf("  Obtained platform info dict.\n");
+        #endif
 
         // Count devices
         flag = clGetDeviceIDs(platform_ids[i], CL_DEVICE_TYPE_ALL, MCL_MAX_DEVICES, device_ids, &n_devices);
         if (flag == CL_DEVICE_NOT_FOUND) {
             n_devices = 0;
+        } else if (flag == CL_INVALID_VALUE) {
+            // This seems to happen on Mac OS 14.4.1
+            n_devices = 0;
         } else if (mcl_flag(flag)) {
             Py_DECREF(platforms);
             return NULL;
         }
+        #ifdef MYOKIT_DEBUG_MESSAGES
+        printf("  Found %u devices.\n", (unsigned int)n_devices);
+        #endif
 
         // Create devices tuple, must decref on exception
         devices = PyTuple_New((size_t)n_devices);
 
         // Add devices
         for (j=0; j<n_devices; j++) {
+            #ifdef MYOKIT_DEBUG_MESSAGES
+            printf("    Checking device %u\n", (unsigned int)j);
+            #endif
 
             // Create device dict, must decref on exception
             device = mcl_info_device_dict(device_ids[j], sizeof(buffer), buffer);
             if (device == NULL) { Py_DECREF(platforms); Py_DECREF(devices); return NULL; }
+            #ifdef MYOKIT_DEBUG_MESSAGES
+            printf("    Obtained device info dict.\n");
+            #endif
 
             // Add device to devices tuple (steals reference)
             PyTuple_SetItem(devices, j, device);
             device = NULL;
         }
 
         // Add devices entry to platform dict
```

### Comparing `myokit-1.36.0/myokit/_sim/opencl.c` & `myokit-1.36.1/myokit/_sim/opencl.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/opencl.py` & `myokit-1.36.1/myokit/_sim/opencl.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/openclsim.c` & `myokit-1.36.1/myokit/_sim/openclsim.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/openclsim.cl` & `myokit-1.36.1/myokit/_sim/openclsim.cl`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/openclsim.py` & `myokit-1.36.1/myokit/_sim/openclsim.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/pacing.h` & `myokit-1.36.1/myokit/_sim/pacing.h`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/rhs.c` & `myokit-1.36.1/myokit/_sim/rhs.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/rhs.py` & `myokit-1.36.1/myokit/_sim/rhs.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/sundials.c` & `myokit-1.36.1/myokit/_sim/sundials.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_sim/sundials.py` & `myokit-1.36.1/myokit/_sim/sundials.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_system.py` & `myokit-1.36.1/myokit/_system.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/_unit.py` & `myokit-1.36.1/myokit/_unit.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/float.py` & `myokit-1.36.1/myokit/float.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/__init__.py` & `myokit-1.36.1/myokit/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/ansic/__init__.py` & `myokit-1.36.1/myokit/formats/ansic/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/ansic/_ewriter.py` & `myokit-1.36.1/myokit/formats/ansic/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/ansic/_exporter.py` & `myokit-1.36.1/myokit/formats/ansic/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/ansic/template/cable.c` & `myokit-1.36.1/myokit/formats/ansic/template/cable.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/ansic/template/euler.c` & `myokit-1.36.1/myokit/formats/ansic/template/euler.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/ansic/template/sim.c` & `myokit-1.36.1/myokit/formats/ansic/template/sim.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/axon/__init__.py` & `myokit-1.36.1/myokit/formats/axon/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/axon/_abf.py` & `myokit-1.36.1/myokit/formats/axon/_abf.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/axon/_atf.py` & `myokit-1.36.1/myokit/formats/axon/_atf.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/axon/_importer.py` & `myokit-1.36.1/myokit/formats/axon/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/__init__.py` & `myokit-1.36.1/myokit/formats/cellml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/_ewriter.py` & `myokit-1.36.1/myokit/formats/cellml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/_exporter.py` & `myokit-1.36.1/myokit/formats/cellml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/_importer.py` & `myokit-1.36.1/myokit/formats/cellml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/v1/__init__.py` & `myokit-1.36.1/myokit/formats/cellml/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/v1/_api.py` & `myokit-1.36.1/myokit/formats/cellml/v1/_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/v1/_parser.py` & `myokit-1.36.1/myokit/formats/cellml/v1/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/v1/_writer.py` & `myokit-1.36.1/myokit/formats/cellml/v1/_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/v2/__init__.py` & `myokit-1.36.1/myokit/formats/cellml/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/v2/_api.py` & `myokit-1.36.1/myokit/formats/cellml/v2/_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/v2/_parser.py` & `myokit-1.36.1/myokit/formats/cellml/v2/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cellml/v2/_writer.py` & `myokit-1.36.1/myokit/formats/cellml/v2/_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/channelml/_importer.py` & `myokit-1.36.1/myokit/formats/channelml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cpp/__init__.py` & `myokit-1.36.1/myokit/formats/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cpp/_ewriter.py` & `myokit-1.36.1/myokit/formats/cpp/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cuda/__init__.py` & `myokit-1.36.1/myokit/formats/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cuda/_ewriter.py` & `myokit-1.36.1/myokit/formats/cuda/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cuda/_exporter.py` & `myokit-1.36.1/myokit/formats/cuda/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/cuda/template/kernel.cu` & `myokit-1.36.1/myokit/formats/cuda/template/kernel.cu`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/easyml/__init__.py` & `myokit-1.36.1/myokit/formats/easyml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/easyml/_ewriter.py` & `myokit-1.36.1/myokit/formats/easyml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/easyml/_exporter.py` & `myokit-1.36.1/myokit/formats/easyml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/heka/__init__.py` & `myokit-1.36.1/myokit/formats/heka/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/heka/_importer.py` & `myokit-1.36.1/myokit/formats/heka/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/heka/_patchmaster.py` & `myokit-1.36.1/myokit/formats/heka/_patchmaster.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/html/_exporter.py` & `myokit-1.36.1/myokit/formats/html/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/html/_flatten.py` & `myokit-1.36.1/myokit/formats/html/_flatten.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/latex/__init__.py` & `myokit-1.36.1/myokit/formats/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/latex/_ewriter.py` & `myokit-1.36.1/myokit/formats/latex/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/latex/_exporter.py` & `myokit-1.36.1/myokit/formats/latex/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/mathml/__init__.py` & `myokit-1.36.1/myokit/formats/mathml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/mathml/_ewriter.py` & `myokit-1.36.1/myokit/formats/mathml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/mathml/_parser.py` & `myokit-1.36.1/myokit/formats/mathml/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/matlab/__init__.py` & `myokit-1.36.1/myokit/formats/matlab/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/matlab/_ewriter.py` & `myokit-1.36.1/myokit/formats/matlab/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/matlab/_exporter.py` & `myokit-1.36.1/myokit/formats/matlab/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/matlab/template/constants.m` & `myokit-1.36.1/myokit/formats/matlab/template/constants.m`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/matlab/template/main.m` & `myokit-1.36.1/myokit/formats/matlab/template/main.m`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/matlab/template/model.m` & `myokit-1.36.1/myokit/formats/matlab/template/model.m`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/opencl/__init__.py` & `myokit-1.36.1/myokit/formats/opencl/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/opencl/_ewriter.py` & `myokit-1.36.1/myokit/formats/opencl/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/opencl/_exporter.py` & `myokit-1.36.1/myokit/formats/opencl/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/opencl/template/cable.c` & `myokit-1.36.1/myokit/formats/opencl/template/cable.c`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/opencl/template/kernel.cl` & `myokit-1.36.1/myokit/formats/opencl/template/kernel.cl`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/opencl/template/minilog.py` & `myokit-1.36.1/myokit/formats/opencl/template/minilog.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/opencl/template/plot.py` & `myokit-1.36.1/myokit/formats/opencl/template/plot.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/python/__init__.py` & `myokit-1.36.1/myokit/formats/python/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/python/_ewriter.py` & `myokit-1.36.1/myokit/formats/python/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/python/_exporter.py` & `myokit-1.36.1/myokit/formats/python/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/python/template/sim.py` & `myokit-1.36.1/myokit/formats/python/template/sim.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/sbml/__init__.py` & `myokit-1.36.1/myokit/formats/sbml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/sbml/_api.py` & `myokit-1.36.1/myokit/formats/sbml/_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/sbml/_importer.py` & `myokit-1.36.1/myokit/formats/sbml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/sbml/_parser.py` & `myokit-1.36.1/myokit/formats/sbml/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/stan/__init__.py` & `myokit-1.36.1/myokit/formats/stan/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/stan/_ewriter.py` & `myokit-1.36.1/myokit/formats/stan/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/stan/_exporter.py` & `myokit-1.36.1/myokit/formats/stan/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/stan/template/cell.stan` & `myokit-1.36.1/myokit/formats/stan/template/cell.stan`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/sympy/__init__.py` & `myokit-1.36.1/myokit/formats/sympy/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/sympy/_ereader.py` & `myokit-1.36.1/myokit/formats/sympy/_ereader.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/sympy/_ewriter.py` & `myokit-1.36.1/myokit/formats/sympy/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/wcp/_wcp.py` & `myokit-1.36.1/myokit/formats/wcp/_wcp.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/formats/xml/_exporter.py` & `myokit-1.36.1/myokit/formats/xml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/gui/__init__.py` & `myokit-1.36.1/myokit/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/gui/datablock_viewer.py` & `myokit-1.36.1/myokit/gui/datablock_viewer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/gui/datalog_viewer.py` & `myokit-1.36.1/myokit/gui/datalog_viewer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/gui/explorer.py` & `myokit-1.36.1/myokit/gui/explorer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/gui/ide.py` & `myokit-1.36.1/myokit/gui/ide.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/gui/progress.py` & `myokit-1.36.1/myokit/gui/progress.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/gui/source.py` & `myokit-1.36.1/myokit/gui/source.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/gui/vargrapher.py` & `myokit-1.36.1/myokit/gui/vargrapher.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/lib/deps.py` & `myokit-1.36.1/myokit/lib/deps.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/lib/guess.py` & `myokit-1.36.1/myokit/lib/guess.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/lib/hh.py` & `myokit-1.36.1/myokit/lib/hh.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,14 +294,17 @@
             inf = w.ex(myokit.Name(inf))
             tau = w.ex(myokit.Name(tau))
             k = str(k)
             f.append(
                 '_y[' + k + '] = ' + state.uname() + ' = '
                 + inf + ' + (_y0[' + k + '] - ' + inf
                 + ') * numpy.exp(-_t / ' + tau + ')')
+            f.append(
+                '_y[' + k + '][_t == 0] = ' + state.uname() + '[_t == 0] = '
+                + '_y0[' + k + ']')
 
         # Add current calculation
         if self._current is not None:
             f.append('_i = ' + w.ex(self._current.rhs()))
         else:
             f.append('_i = None')
```

### Comparing `myokit-1.36.0/myokit/lib/markov.py` & `myokit-1.36.1/myokit/lib/markov.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/lib/multi.py` & `myokit-1.36.1/myokit/lib/multi.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/lib/plots.py` & `myokit-1.36.1/myokit/lib/plots.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/pacing.py` & `myokit-1.36.1/myokit/pacing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/pype.py` & `myokit-1.36.1/myokit/pype.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/__init__.py` & `myokit-1.36.1/myokit/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/ansic_event_based_pacing.py` & `myokit-1.36.1/myokit/tests/ansic_event_based_pacing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/ansic_time_series_pacing.py` & `myokit-1.36.1/myokit/tests/ansic_time_series_pacing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/beeler-1977-model-compare-a.mmt` & `myokit-1.36.1/myokit/tests/data/beeler-1977-model-compare-a.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/beeler-1977-model-compare-b.mmt` & `myokit-1.36.1/myokit/tests/data/beeler-1977-model-compare-b.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/beeler-1977-model.mmt` & `myokit-1.36.1/myokit/tests/data/beeler-1977-model.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/beeler-1977-units.mmt` & `myokit-1.36.1/myokit/tests/data/beeler-1977-units.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/clancy-1999-fitting.mmt` & `myokit-1.36.1/myokit/tests/data/clancy-1999-fitting.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/conditional.mmt` & `myokit-1.36.1/myokit/tests/data/conditional.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/cv1d.mmt` & `myokit-1.36.1/myokit/tests/data/cv1d.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/cv1d.zip` & `myokit-1.36.1/myokit/tests/data/cv1d.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/decker-2009.mmt` & `myokit-1.36.1/myokit/tests/data/decker-2009.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/decker.model` & `myokit-1.36.1/myokit/tests/data/decker.model`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/dn-1985-normalised.mmt` & `myokit-1.36.1/myokit/tests/data/dn-1985-normalised.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/dom-markov.mmt` & `myokit-1.36.1/myokit/tests/data/dom-markov.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/abf-protocol.pro` & `myokit-1.36.1/myokit/tests/data/formats/abf-protocol.pro`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/abf-v1.abf` & `myokit-1.36.1/myokit/tests/data/formats/abf-v1.abf`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/abf-v2.abf` & `myokit-1.36.1/myokit/tests/data/formats/abf-v2.abf`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/cellml/br-1977-dot.cellml` & `myokit-1.36.1/myokit/tests/data/formats/cellml/br-1977-dot.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/cellml/br-1977.cellml` & `myokit-1.36.1/myokit/tests/data/formats/cellml/br-1977.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/cellml/corrias.cellml` & `myokit-1.36.1/myokit/tests/data/formats/cellml/corrias.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/cellml/decker-2009.cellml` & `myokit-1.36.1/myokit/tests/data/formats/cellml/decker-2009.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/cellml/documentation.cellml` & `myokit-1.36.1/myokit/tests/data/formats/cellml/documentation.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml` & `myokit-1.36.1/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml` & `myokit-1.36.1/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml` & `myokit-1.36.1/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml` & `myokit-1.36.1/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml` & `myokit-1.36.1/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/sbml/HodgkinHuxley.xml` & `myokit-1.36.1/myokit/tests/data/formats/sbml/HodgkinHuxley.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml` & `myokit-1.36.1/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml` & `myokit-1.36.1/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml` & `myokit-1.36.1/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/sbml/result/00001-results.csv` & `myokit-1.36.1/myokit/tests/data/formats/sbml/result/00001-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/sbml/result/00004-results.csv` & `myokit-1.36.1/myokit/tests/data/formats/sbml/result/00004-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/sbml/result/01103-results.csv` & `myokit-1.36.1/myokit/tests/data/formats/sbml/result/01103-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/formats/wcp-file.wcp` & `myokit-1.36.1/myokit/tests/data/formats/wcp-file.wcp`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad1d-1-not-enough-files.zip` & `myokit-1.36.1/myokit/tests/data/io/bad1d-1-not-enough-files.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad1d-2-no-header.zip` & `myokit-1.36.1/myokit/tests/data/io/bad1d-2-no-header.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad1d-3-no-data.zip` & `myokit-1.36.1/myokit/tests/data/io/bad1d-3-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad1d-4-not-a-zip.zip` & `myokit-1.36.1/myokit/tests/data/io/bad1d-4-not-a-zip.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad1d-5-bad-data-type.zip` & `myokit-1.36.1/myokit/tests/data/io/bad1d-5-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad1d-6-time-too-short.zip` & `myokit-1.36.1/myokit/tests/data/io/bad1d-6-time-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad1d-7-0d-too-short.zip` & `myokit-1.36.1/myokit/tests/data/io/bad1d-7-0d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad1d-8-1d-too-short.zip` & `myokit-1.36.1/myokit/tests/data/io/bad1d-8-1d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad2d-1-not-enough-files.zip` & `myokit-1.36.1/myokit/tests/data/io/bad2d-1-not-enough-files.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad2d-2-no-header.zip` & `myokit-1.36.1/myokit/tests/data/io/bad2d-2-no-header.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad2d-3-no-data.zip` & `myokit-1.36.1/myokit/tests/data/io/bad2d-3-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad2d-4-not-a-zip.zip` & `myokit-1.36.1/myokit/tests/data/io/bad2d-4-not-a-zip.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad2d-5-bad-data-type.zip` & `myokit-1.36.1/myokit/tests/data/io/bad2d-5-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad2d-6-time-too-short.zip` & `myokit-1.36.1/myokit/tests/data/io/bad2d-6-time-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad2d-7-0d-too-short.zip` & `myokit-1.36.1/myokit/tests/data/io/bad2d-7-0d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/bad2d-8-2d-too-short.zip` & `myokit-1.36.1/myokit/tests/data/io/bad2d-8-2d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/badlog-1-no-data.zip` & `myokit-1.36.1/myokit/tests/data/io/badlog-1-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/badlog-2-no-structure.zip` & `myokit-1.36.1/myokit/tests/data/io/badlog-2-no-structure.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/badlog-4-invalid-n-fields.zip` & `myokit-1.36.1/myokit/tests/data/io/badlog-4-invalid-n-fields.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/badlog-5-invalid-data-size.zip` & `myokit-1.36.1/myokit/tests/data/io/badlog-5-invalid-data-size.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/badlog-6-bad-data-type.zip` & `myokit-1.36.1/myokit/tests/data/io/badlog-6-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/badlog-7-not-enough-data.zip` & `myokit-1.36.1/myokit/tests/data/io/badlog-7-not-enough-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/block2d.mmt` & `myokit-1.36.1/myokit/tests/data/io/block2d.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/block2d.zip` & `myokit-1.36.1/myokit/tests/data/io/block2d.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/io/goodlog.zip` & `myokit-1.36.1/myokit/tests/data/io/goodlog.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/lr-1991-dep.mmt` & `myokit-1.36.1/myokit/tests/data/lr-1991-dep.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/lr-1991-fitting.mmt` & `myokit-1.36.1/myokit/tests/data/lr-1991-fitting.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/lr-1991-testing.mmt` & `myokit-1.36.1/myokit/tests/data/lr-1991-testing.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/lr-1991.mmt` & `myokit-1.36.1/myokit/tests/data/lr-1991.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/multi/beeler-no-name.mmt` & `myokit-1.36.1/myokit/tests/data/multi/beeler-no-name.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/multi/lr-1991.mmt` & `myokit-1.36.1/myokit/tests/data/multi/lr-1991.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/multi/subdir/beeler-no-name.mmt` & `myokit-1.36.1/myokit/tests/data/multi/subdir/beeler-no-name.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/data/noble-1962.mmt` & `myokit-1.36.1/myokit/tests/data/noble-1962.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_aux.py` & `myokit-1.36.1/myokit/tests/test_aux.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_cellml_v1_api.py` & `myokit-1.36.1/myokit/tests/test_cellml_v1_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_cellml_v1_parser.py` & `myokit-1.36.1/myokit/tests/test_cellml_v1_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_cellml_v1_writer.py` & `myokit-1.36.1/myokit/tests/test_cellml_v1_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_cellml_v2_api.py` & `myokit-1.36.1/myokit/tests/test_cellml_v2_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_cellml_v2_parser.py` & `myokit-1.36.1/myokit/tests/test_cellml_v2_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_cellml_v2_writer.py` & `myokit-1.36.1/myokit/tests/test_cellml_v2_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_cmodel.py` & `myokit-1.36.1/myokit/tests/test_cmodel.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_component.py` & `myokit-1.36.1/myokit/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_config.py` & `myokit-1.36.1/myokit/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_datablock.py` & `myokit-1.36.1/myokit/tests/test_datablock.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_datalog.py` & `myokit-1.36.1/myokit/tests/test_datalog.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_dependency_checking.py` & `myokit-1.36.1/myokit/tests/test_dependency_checking.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_expressions.py` & `myokit-1.36.1/myokit/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_float.py` & `myokit-1.36.1/myokit/tests/test_float.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats.py` & `myokit-1.36.1/myokit/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_ansic.py` & `myokit-1.36.1/myokit/tests/test_formats_ansic.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_axon.py` & `myokit-1.36.1/myokit/tests/test_formats_axon.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_cellml.py` & `myokit-1.36.1/myokit/tests/test_formats_cellml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_channelml.py` & `myokit-1.36.1/myokit/tests/test_formats_channelml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_cpp.py` & `myokit-1.36.1/myokit/tests/test_formats_cpp.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_cuda.py` & `myokit-1.36.1/myokit/tests/test_formats_cuda.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_easyml.py` & `myokit-1.36.1/myokit/tests/test_formats_easyml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_exporters_run.py` & `myokit-1.36.1/myokit/tests/test_formats_exporters_run.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_html.py` & `myokit-1.36.1/myokit/tests/test_formats_html.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_latex.py` & `myokit-1.36.1/myokit/tests/test_formats_latex.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_mathml_content.py` & `myokit-1.36.1/myokit/tests/test_formats_mathml_content.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_mathml_presentation.py` & `myokit-1.36.1/myokit/tests/test_formats_mathml_presentation.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_matlab.py` & `myokit-1.36.1/myokit/tests/test_formats_matlab.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_opencl.py` & `myokit-1.36.1/myokit/tests/test_formats_opencl.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_python.py` & `myokit-1.36.1/myokit/tests/test_formats_python.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_sbml.py` & `myokit-1.36.1/myokit/tests/test_formats_sbml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_stan.py` & `myokit-1.36.1/myokit/tests/test_formats_stan.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_sympy.py` & `myokit-1.36.1/myokit/tests/test_formats_sympy.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_formats_wcp.py` & `myokit-1.36.1/myokit/tests/test_formats_wcp.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_io.py` & `myokit-1.36.1/myokit/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_jacobian_calculator.py` & `myokit-1.36.1/myokit/tests/test_jacobian_calculator.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_jacobian_tracer.py` & `myokit-1.36.1/myokit/tests/test_jacobian_tracer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_lib_deps.py` & `myokit-1.36.1/myokit/tests/test_lib_deps.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_lib_guess.py` & `myokit-1.36.1/myokit/tests/test_lib_guess.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_lib_hh.py` & `myokit-1.36.1/myokit/tests/test_lib_hh.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import numpy as np
 
 import myokit
 import myokit.lib.hh as hh
 
 from myokit.tests import DIR_DATA
 
+from myokit.tests import WarningCollector
+
 
 MODEL = """
 [[model]]
 membrane.V = -80
 ikr.a = 4.5e-4
 ikr.r = 0.15
 ina.r = 0.15
@@ -910,10 +912,44 @@
         e = np.abs(d1['membrane.V'] - d2['membrane.V'])
         self.assertEqual(np.max(e), 0)
 
         # Test current output is very similar
         e = np.abs(d1['binding.I'] - d2['binding.I'])
         self.assertLess(np.max(e), 2e-4)
 
+    def test_tau_overflow(self):
+        # Overflows leading to tau=0 should still report current
+        # https://github.com/myokit/myokit/issues/1059
+
+        # Load model and convert to inf-tau form
+        fname = os.path.join(DIR_DATA, 'lr-1991-fitting.mmt')
+        model = hh.convert_hh_states_to_inf_tau_form(myokit.load_model(fname))
+
+        # Get initial state and set steady state
+        initial_state = model.get('ina.m').initial_value(as_float=True)
+        steady_state = 0.75
+        model.get('ina.m.inf').set_rhs(steady_state)
+
+        # Create an analytical simulation
+        model = hh.HHModel(model, states=['ina.m', 'ina.h', 'ina.j'],
+                           parameters=['ina.p5'], current='ina.INa')
+        p = myokit.pacing.steptrain_linear(20, 40, 10, -80, 10, 10)
+        s = hh.AnalyticalSimulation(model, protocol=p)
+
+        # Setting p5=0.001 will trigger an overflow in ina.m.beta
+        s.set_parameters([0.001])
+        with WarningCollector() as wc:
+            # Log times chosen so that s._function varies length of _t
+            log = s.run(41, log_times=np.array([0, 1, 2, 10, 11, 12, 20, 40]))
+        self.assertIn('overflow', wc.text())
+
+        # Should be no NaNs in log
+        self.assertFalse(np.any(np.isnan(log['ina.INa'])))
+        self.assertFalse(np.any(np.isnan(log['ina.m'])))
+
+        # Should immediately jump from initial state to steady state
+        self.assertTrue(log['ina.m'][0] == initial_state)
+        self.assertTrue(np.all(log['ina.m'][1:] == steady_state))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `myokit-1.36.0/myokit/tests/test_lib_markov.py` & `myokit-1.36.1/myokit/tests/test_lib_markov.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_lib_multi.py` & `myokit-1.36.1/myokit/tests/test_lib_multi.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_lib_plots.py` & `myokit-1.36.1/myokit/tests/test_lib_plots.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_meta.py` & `myokit-1.36.1/myokit/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_model.py` & `myokit-1.36.1/myokit/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_model_building.py` & `myokit-1.36.1/myokit/tests/test_model_building.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_opencl_info.py` & `myokit-1.36.1/myokit/tests/test_opencl_info.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_pacing_factory.py` & `myokit-1.36.1/myokit/tests/test_pacing_factory.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_pacing_system_c.py` & `myokit-1.36.1/myokit/tests/test_pacing_system_c.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_pacing_system_py.py` & `myokit-1.36.1/myokit/tests/test_pacing_system_py.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_parsing.py` & `myokit-1.36.1/myokit/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_progress_reporters.py` & `myokit-1.36.1/myokit/tests/test_progress_reporters.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_protocol.py` & `myokit-1.36.1/myokit/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_protocol_floating_point.py` & `myokit-1.36.1/myokit/tests/test_protocol_floating_point.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_protocol_time_series.py` & `myokit-1.36.1/myokit/tests/test_protocol_time_series.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_pype.py` & `myokit-1.36.1/myokit/tests/test_pype.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_quantity.py` & `myokit-1.36.1/myokit/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_rhs_benchmarker.py` & `myokit-1.36.1/myokit/tests/test_rhs_benchmarker.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_sbml_api.py` & `myokit-1.36.1/myokit/tests/test_sbml_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_sbml_parser.py` & `myokit-1.36.1/myokit/tests/test_sbml_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_simulation_1d.py` & `myokit-1.36.1/myokit/tests/test_simulation_1d.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_simulation_cvodes.py` & `myokit-1.36.1/myokit/tests/test_simulation_cvodes.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_simulation_cvodes_from_disk.py` & `myokit-1.36.1/myokit/tests/test_simulation_cvodes_from_disk.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_simulation_fiber_tissue.py` & `myokit-1.36.1/myokit/tests/test_simulation_fiber_tissue.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_simulation_log_interval.py` & `myokit-1.36.1/myokit/tests/test_simulation_log_interval.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_simulation_opencl.py` & `myokit-1.36.1/myokit/tests/test_simulation_opencl.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_simulation_opencl_log_interval.py` & `myokit-1.36.1/myokit/tests/test_simulation_opencl_log_interval.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_simulation_opencl_vs_cvode.py` & `myokit-1.36.1/myokit/tests/test_simulation_opencl_vs_cvode.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_simulation_opencl_vs_sim1d.py` & `myokit-1.36.1/myokit/tests/test_simulation_opencl_vs_sim1d.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_system_info.py` & `myokit-1.36.1/myokit/tests/test_system_info.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_tools.py` & `myokit-1.36.1/myokit/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_unit.py` & `myokit-1.36.1/myokit/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_user_functions.py` & `myokit-1.36.1/myokit/tests/test_user_functions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tests/test_variable.py` & `myokit-1.36.1/myokit/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/tools.py` & `myokit-1.36.1/myokit/tools.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit/units.py` & `myokit-1.36.1/myokit/units.py`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/myokit.egg-info/PKG-INFO` & `myokit-1.36.1/myokit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myokit
-Version: 1.36.0
+Version: 1.36.1
 Summary: A modeling and simulation tool for cardiac cellular electrophysiology
 Home-page: http://myokit.org
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/myokit/myokit/issues
 Project-URL: Documentation, http://docs.myokit.org
```

### Comparing `myokit-1.36.0/myokit.egg-info/SOURCES.txt` & `myokit-1.36.1/myokit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myokit-1.36.0/setup.py` & `myokit-1.36.1/setup.py`

 * *Files identical despite different names*

