# Comparing `tmp/experimaestro-1.5.4.tar.gz` & `tmp/experimaestro-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experimaestro-1.5.4.tar", max compression
+gzip compressed data, was "experimaestro-1.5.5.tar", max compression
```

## Comparing `experimaestro-1.5.4.tar` & `experimaestro-1.5.5.tar`

### file list

```diff
@@ -1,147 +1,146 @@
--rw-r--r--   0        0        0    35149 2024-03-06 15:22:50.522841 experimaestro-1.5.4/LICENSE
--rw-r--r--   0        0        0     4047 2024-03-06 15:22:50.522841 experimaestro-1.5.4/README.md
--rw-r--r--   0        0        0     3536 2024-03-06 15:23:37.410740 experimaestro-1.5.4/pyproject.toml
--rw-r--r--   0        0        0     1548 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/__init__.py
--rw-r--r--   0        0        0    13528 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/__main__.py
--rw-r--r--   0        0        0     8450 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/annotations.py
--rw-r--r--   0        0        0      696 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/checkers.py
--rw-r--r--   0        0        0     2390 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/click.py
--rw-r--r--   0        0        0     9463 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/commandline.py
--rw-r--r--   0        0        0      171 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/compat.py
--rw-r--r--   0        0        0     5461 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/connectors/__init__.py
--rw-r--r--   0        0        0     5816 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/connectors/local.py
--rw-r--r--   0        0        0     8290 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/connectors/ssh.py
--rw-r--r--   0        0        0        0 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/core/__init__.py
--rw-r--r--   0        0        0     5620 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/core/arguments.py
--rw-r--r--   0        0        0     2638 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/core/context.py
--rw-r--r--   0        0        0    63989 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/core/objects.py
--rw-r--r--   0        0        0     7131 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/core/objects.pyi
--rw-r--r--   0        0        0     3836 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/core/serialization.py
--rw-r--r--   0        0        0     1197 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/core/serializers.py
--rw-r--r--   0        0        0    20176 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/core/types.py
--rw-r--r--   0        0        0      495 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/core/utils.py
--rw-r--r--   0        0        0       44 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/exceptions.py
--rw-r--r--   0        0        0      159 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/experiments/__init__.py
--rw-r--r--   0        0        0     7535 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/experiments/cli.py
--rw-r--r--   0        0        0     1150 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/experiments/configuration.py
--rw-r--r--   0        0        0     5794 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/filter.py
--rw-r--r--   0        0        0     1230 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/generators.py
--rw-r--r--   0        0        0     2956 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/huggingface.py
--rw-r--r--   0        0        0     1490 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/ipc.py
--rw-r--r--   0        0        0      294 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/launcherfinder/__init__.py
--rw-r--r--   0        0        0     1020 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/launcherfinder/base.py
--rw-r--r--   0        0        0     2279 2024-03-06 15:22:50.530840 experimaestro-1.5.4/src/experimaestro/launcherfinder/parser.py
--rw-r--r--   0        0        0     8925 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/launcherfinder/registry.py
--rw-r--r--   0        0        0     6448 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/launcherfinder/specs.py
--rw-r--r--   0        0        0     2525 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/launchers/__init__.py
--rw-r--r--   0        0        0     1967 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/launchers/direct.py
--rw-r--r--   0        0        0        0 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/launchers/oar.py
--rw-r--r--   0        0        0       41 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/launchers/slurm/__init__.py
--rw-r--r--   0        0        0    14135 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/launchers/slurm/base.py
--rw-r--r--   0        0        0      818 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/launchers/slurm/cli.py
--rw-r--r--   0        0        0    19357 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/launchers/slurm/configuration.py
--rw-r--r--   0        0        0     1477 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/locking.py
--rw-r--r--   0        0        0       34 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/mkdocs/__init__.py
--rw-r--r--   0        0        0      263 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/mkdocs/annotations.py
--rw-r--r--   0        0        0    16716 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/mkdocs/base.py
--rw-r--r--   0        0        0     1481 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/mkdocs/metaloader.py
--rw-r--r--   0        0        0       66 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/mkdocs/style.css
--rw-r--r--   0        0        0      285 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/mypy.py
--rw-r--r--   0        0        0     8710 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/notifications.py
--rw-r--r--   0        0        0        0 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/py.typed
--rw-r--r--   0        0        0     3605 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/rpyc.py
--rw-r--r--   0        0        0     4499 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/run.py
--rw-r--r--   0        0        0       20 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/scheduler/__init__.py
--rw-r--r--   0        0        0    31450 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/scheduler/base.py
--rw-r--r--   0        0        0     1994 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/scheduler/dependencies.py
--rw-r--r--   0        0        0     2393 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/scheduler/environment.py
--rw-r--r--   0        0        0     2189 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/scheduler/services.py
--rw-r--r--   0        0        0     1731 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/scheduler/workspace.py
--rw-r--r--   0        0        0     4357 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/scriptbuilder.py
--rw-r--r--   0        0        0    10854 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/server/__init__.py
--rw-r--r--   0        0        0   189684 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/016b4a6cdced82ab3aa1.ttf
--rw-r--r--   0        0        0   128352 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/0c35d18bf06992036b69.woff2
--rw-r--r--   0        0        0   135984 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2
--rw-r--r--   0        0        0   156236 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/3a4004a46a653d4b2166.woff
--rw-r--r--   0        0        0   339600 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/3baa5b8f3469222b822d.woff
--rw-r--r--   0        0        0   164912 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/4d73cb90e394b34b7670.woff
--rw-r--r--   0        0        0   215704 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2
--rw-r--r--   0        0        0    63348 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/50701fbb8177c2dde530.ttf
--rw-r--r--   0        0        0   206260 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/5d681e2edae8c60630db.woff
--rw-r--r--   0        0        0   155276 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2
--rw-r--r--   0        0        0   109808 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/878f31251d960bd6266f.woff2
--rw-r--r--   0        0        0    24488 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/b041b1fa4fe241b23445.woff2
--rw-r--r--   0        0        0   150020 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/b6879d41b0852f01ed5b.woff2
--rw-r--r--   0        0        0   173620 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/c380809fd3677d7d6903.woff2
--rw-r--r--   0        0        0   394668 2024-03-06 15:23:35.598743 experimaestro-1.5.4/src/experimaestro/server/data/d75e3fd1eb12e9bd6655.ttf
--rw-r--r--   0        0        0   182028 2024-03-06 15:23:35.566743 experimaestro-1.5.4/src/experimaestro/server/data/f882956fd323fd322f31.woff
--rw-r--r--   0        0        0     3870 2024-03-06 15:23:35.598743 experimaestro-1.5.4/src/experimaestro/server/data/favicon.ico
--rw-r--r--   0        0        0   418843 2024-03-06 15:23:35.598743 experimaestro-1.5.4/src/experimaestro/server/data/index.css
--rw-r--r--   0        0        0   576970 2024-03-06 15:23:35.598743 experimaestro-1.5.4/src/experimaestro/server/data/index.css.map
--rw-r--r--   0        0        0      706 2024-03-06 15:23:35.598743 experimaestro-1.5.4/src/experimaestro/server/data/index.html
--rw-r--r--   0        0        0  3734128 2024-03-06 15:23:35.598743 experimaestro-1.5.4/src/experimaestro/server/data/index.js
--rw-r--r--   0        0        0  3904832 2024-03-06 15:23:35.598743 experimaestro-1.5.4/src/experimaestro/server/data/index.js.map
--rw-r--r--   0        0        0      511 2024-03-06 15:23:35.598743 experimaestro-1.5.4/src/experimaestro/server/data/login.html
--rw-r--r--   0        0        0      318 2024-03-06 15:23:35.598743 experimaestro-1.5.4/src/experimaestro/server/data/manifest.json
--rw-r--r--   0        0        0     1807 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/settings.py
--rw-r--r--   0        0        0     9560 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/sphinx/__init__.py
--rw-r--r--   0        0        0      294 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/sphinx/static/experimaestro.css
--rw-r--r--   0        0        0      499 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/taskglobals.py
--rw-r--r--   0        0        0        0 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/__init__.py
--rw-r--r--   0        0        0      695 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/conftest.py
--rw-r--r--   0        0        0       21 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/connectors/bin/executable.py
--rw-r--r--   0        0        0     1204 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/connectors/test_local.py
--rw-r--r--   0        0        0      702 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/connectors/utils.py
--rw-r--r--   0        0        0      414 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/definitions_types.py
--rw-r--r--   0        0        0        0 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/launchers/__init__.py
--rwxr-xr-x   0        0        0      639 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/launchers/bin/sacct
--rwxr-xr-x   0        0        0     1177 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/launchers/bin/sbatch
--rw-r--r--   0        0        0      477 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/launchers/bin/test.py
--rw-r--r--   0        0        0     2468 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/launchers/common.py
--rw-r--r--   0        0        0        0 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/launchers/config_slurm/__init__.py
--rw-r--r--   0        0        0     2497 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/launchers/config_slurm/launchers.yaml
--rw-r--r--   0        0        0      717 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/launchers/test_local.py
--rw-r--r--   0        0        0     2534 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/launchers/test_slurm.py
--rw-r--r--   0        0        0     4016 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/restart.py
--rw-r--r--   0        0        0      295 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/restart_main.py
--rw-r--r--   0        0        0      407 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/scripts/notifyandwait.py
--rw-r--r--   0        0        0      120 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/scripts/waitforfile.py
--rw-r--r--   0        0        0      477 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/task_tokens.py
--rw-r--r--   0        0        0        0 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/tasks/__init__.py
--rw-r--r--   0        0        0     1851 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/tasks/all.py
--rw-r--r--   0        0        0      153 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/tasks/foreign.py
--rw-r--r--   0        0        0      403 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_checkers.py
--rw-r--r--   0        0        0     2005 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_dependencies.py
--rw-r--r--   0        0        0     2967 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_findlauncher.py
--rw-r--r--   0        0        0      780 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_forward.py
--rw-r--r--   0        0        0    13397 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_identifier.py
--rw-r--r--   0        0        0     1540 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_instance.py
--rw-r--r--   0        0        0     2037 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_objects.py
--rw-r--r--   0        0        0      781 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_outputs.py
--rw-r--r--   0        0        0     6405 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_param.py
--rw-r--r--   0        0        0     7580 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_progress.py
--rw-r--r--   0        0        0     2338 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_serializers.py
--rw-r--r--   0        0        0     3081 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_snippets.py
--rw-r--r--   0        0        0      979 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_ssh.py
--rw-r--r--   0        0        0     1975 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_tags.py
--rw-r--r--   0        0        0     9429 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_tasks.py
--rw-r--r--   0        0        0     7826 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_tokens.py
--rw-r--r--   0        0        0     1257 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_types.py
--rw-r--r--   0        0        0     4339 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/test_validation.py
--rw-r--r--   0        0        0     1701 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/token_reschedule.py
--rw-r--r--   0        0        0     3805 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tests/utils.py
--rw-r--r--   0        0        0    14681 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tokens.py
--rw-r--r--   0        0        0        0 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tools/__init__.py
--rw-r--r--   0        0        0     3436 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tools/diff.py
--rw-r--r--   0        0        0     9184 2024-03-06 15:22:50.534840 experimaestro-1.5.4/src/experimaestro/tools/documentation.py
--rw-r--r--   0        0        0     3516 2024-03-06 15:22:50.538841 experimaestro-1.5.4/src/experimaestro/tools/jobs.py
--rw-r--r--   0        0        0     3334 2024-03-06 15:22:50.538841 experimaestro-1.5.4/src/experimaestro/typingutils.py
--rw-r--r--   0        0        0     2434 2024-03-06 15:22:50.538841 experimaestro-1.5.4/src/experimaestro/utils/__init__.py
--rw-r--r--   0        0        0      601 2024-03-06 15:22:50.538841 experimaestro-1.5.4/src/experimaestro/utils/asyncio.py
--rw-r--r--   0        0        0     2394 2024-03-06 15:22:50.538841 experimaestro-1.5.4/src/experimaestro/utils/jobs.py
--rw-r--r--   0        0        0     2183 2024-03-06 15:22:50.538841 experimaestro-1.5.4/src/experimaestro/utils/jupyter.py
--rw-r--r--   0        0        0     1006 2024-03-06 15:22:50.538841 experimaestro-1.5.4/src/experimaestro/utils/resources.py
--rw-r--r--   0        0        0      793 2024-03-06 15:22:50.538841 experimaestro-1.5.4/src/experimaestro/utils/settings.py
--rw-r--r--   0        0        0     6766 2024-03-06 15:22:50.538841 experimaestro-1.5.4/src/experimaestro/utils/yaml.py
--rw-r--r--   0        0        0      638 2024-03-06 15:22:50.538841 experimaestro-1.5.4/src/experimaestro/xpmutils.py
--rw-r--r--   0        0        0     6265 1970-01-01 00:00:00.000000 experimaestro-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-10 07:30:50.073061 experimaestro-1.5.5/LICENSE
+-rw-r--r--   0        0        0     4047 2024-05-10 07:30:50.073061 experimaestro-1.5.5/README.md
+-rw-r--r--   0        0        0     3540 2024-05-10 07:31:21.760783 experimaestro-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1501 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/__init__.py
+-rw-r--r--   0        0        0    13528 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/__main__.py
+-rw-r--r--   0        0        0     8450 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/annotations.py
+-rw-r--r--   0        0        0      696 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/checkers.py
+-rw-r--r--   0        0        0     1377 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/click.py
+-rw-r--r--   0        0        0     9463 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/commandline.py
+-rw-r--r--   0        0        0      171 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/compat.py
+-rw-r--r--   0        0        0     5461 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/connectors/__init__.py
+-rw-r--r--   0        0        0     5816 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/connectors/local.py
+-rw-r--r--   0        0        0     8290 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/connectors/ssh.py
+-rw-r--r--   0        0        0        0 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/core/__init__.py
+-rw-r--r--   0        0        0     5620 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/core/arguments.py
+-rw-r--r--   0        0        0     2638 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/core/context.py
+-rw-r--r--   0        0        0    63989 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/core/objects.py
+-rw-r--r--   0        0        0     7131 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/core/objects.pyi
+-rw-r--r--   0        0        0     3836 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/core/serialization.py
+-rw-r--r--   0        0        0     1197 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/core/serializers.py
+-rw-r--r--   0        0        0    20176 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/core/types.py
+-rw-r--r--   0        0        0      495 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/core/utils.py
+-rw-r--r--   0        0        0       44 2024-05-10 07:30:50.081061 experimaestro-1.5.5/src/experimaestro/exceptions.py
+-rw-r--r--   0        0        0      159 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/experiments/__init__.py
+-rw-r--r--   0        0        0     7916 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/experiments/cli.py
+-rw-r--r--   0        0        0     1150 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/experiments/configuration.py
+-rw-r--r--   0        0        0     5794 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/filter.py
+-rw-r--r--   0        0        0     1230 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/generators.py
+-rw-r--r--   0        0        0     2956 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/huggingface.py
+-rw-r--r--   0        0        0     1490 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/ipc.py
+-rw-r--r--   0        0        0      294 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launcherfinder/__init__.py
+-rw-r--r--   0        0        0     1020 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launcherfinder/base.py
+-rw-r--r--   0        0        0     2279 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launcherfinder/parser.py
+-rw-r--r--   0        0        0     8925 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launcherfinder/registry.py
+-rw-r--r--   0        0        0     6448 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launcherfinder/specs.py
+-rw-r--r--   0        0        0     2525 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launchers/__init__.py
+-rw-r--r--   0        0        0     1967 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launchers/direct.py
+-rw-r--r--   0        0        0        0 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launchers/oar.py
+-rw-r--r--   0        0        0       41 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launchers/slurm/__init__.py
+-rw-r--r--   0        0        0    14135 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launchers/slurm/base.py
+-rw-r--r--   0        0        0      818 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launchers/slurm/cli.py
+-rw-r--r--   0        0        0    19357 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/launchers/slurm/configuration.py
+-rw-r--r--   0        0        0     1477 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/locking.py
+-rw-r--r--   0        0        0       34 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/mkdocs/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/mkdocs/annotations.py
+-rw-r--r--   0        0        0    16716 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/mkdocs/base.py
+-rw-r--r--   0        0        0     1481 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/mkdocs/metaloader.py
+-rw-r--r--   0        0        0       66 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/mkdocs/style.css
+-rw-r--r--   0        0        0      285 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/mypy.py
+-rw-r--r--   0        0        0     8710 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/notifications.py
+-rw-r--r--   0        0        0        0 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/py.typed
+-rw-r--r--   0        0        0     3605 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/rpyc.py
+-rw-r--r--   0        0        0     5294 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/run.py
+-rw-r--r--   0        0        0       20 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/scheduler/__init__.py
+-rw-r--r--   0        0        0    32132 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/scheduler/base.py
+-rw-r--r--   0        0        0     1994 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/scheduler/dependencies.py
+-rw-r--r--   0        0        0     2189 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/scheduler/services.py
+-rw-r--r--   0        0        0     2280 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/scheduler/workspace.py
+-rw-r--r--   0        0        0     4533 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/scriptbuilder.py
+-rw-r--r--   0        0        0    10854 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/server/__init__.py
+-rw-r--r--   0        0        0   189684 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/016b4a6cdced82ab3aa1.ttf
+-rw-r--r--   0        0        0   128352 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/0c35d18bf06992036b69.woff2
+-rw-r--r--   0        0        0   135984 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2
+-rw-r--r--   0        0        0   156236 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/3a4004a46a653d4b2166.woff
+-rw-r--r--   0        0        0   339600 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/3baa5b8f3469222b822d.woff
+-rw-r--r--   0        0        0   164912 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/4d73cb90e394b34b7670.woff
+-rw-r--r--   0        0        0   215704 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2
+-rw-r--r--   0        0        0    63348 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/50701fbb8177c2dde530.ttf
+-rw-r--r--   0        0        0   206260 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/5d681e2edae8c60630db.woff
+-rw-r--r--   0        0        0   155276 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2
+-rw-r--r--   0        0        0   109808 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/878f31251d960bd6266f.woff2
+-rw-r--r--   0        0        0    24488 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/b041b1fa4fe241b23445.woff2
+-rw-r--r--   0        0        0   150020 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/b6879d41b0852f01ed5b.woff2
+-rw-r--r--   0        0        0   173620 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/c380809fd3677d7d6903.woff2
+-rw-r--r--   0        0        0   394668 2024-05-10 07:31:20.612793 experimaestro-1.5.5/src/experimaestro/server/data/d75e3fd1eb12e9bd6655.ttf
+-rw-r--r--   0        0        0   182028 2024-05-10 07:31:20.584793 experimaestro-1.5.5/src/experimaestro/server/data/f882956fd323fd322f31.woff
+-rw-r--r--   0        0        0     3870 2024-05-10 07:31:20.612793 experimaestro-1.5.5/src/experimaestro/server/data/favicon.ico
+-rw-r--r--   0        0        0   418843 2024-05-10 07:31:20.612793 experimaestro-1.5.5/src/experimaestro/server/data/index.css
+-rw-r--r--   0        0        0   576970 2024-05-10 07:31:20.612793 experimaestro-1.5.5/src/experimaestro/server/data/index.css.map
+-rw-r--r--   0        0        0      706 2024-05-10 07:31:20.612793 experimaestro-1.5.5/src/experimaestro/server/data/index.html
+-rw-r--r--   0        0        0  3734128 2024-05-10 07:31:20.612793 experimaestro-1.5.5/src/experimaestro/server/data/index.js
+-rw-r--r--   0        0        0  3904832 2024-05-10 07:31:20.612793 experimaestro-1.5.5/src/experimaestro/server/data/index.js.map
+-rw-r--r--   0        0        0      511 2024-05-10 07:31:20.612793 experimaestro-1.5.5/src/experimaestro/server/data/login.html
+-rw-r--r--   0        0        0      318 2024-05-10 07:31:20.612793 experimaestro-1.5.5/src/experimaestro/server/data/manifest.json
+-rw-r--r--   0        0        0     2181 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/settings.py
+-rw-r--r--   0        0        0     9560 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/sphinx/__init__.py
+-rw-r--r--   0        0        0      294 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/sphinx/static/experimaestro.css
+-rw-r--r--   0        0        0      499 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/taskglobals.py
+-rw-r--r--   0        0        0        0 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/conftest.py
+-rw-r--r--   0        0        0       21 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/connectors/bin/executable.py
+-rw-r--r--   0        0        0     1204 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/connectors/test_local.py
+-rw-r--r--   0        0        0      702 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/connectors/utils.py
+-rw-r--r--   0        0        0      414 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/definitions_types.py
+-rw-r--r--   0        0        0        0 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/launchers/__init__.py
+-rwxr-xr-x   0        0        0      639 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/launchers/bin/sacct
+-rwxr-xr-x   0        0        0     1177 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/launchers/bin/sbatch
+-rw-r--r--   0        0        0      477 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/launchers/bin/test.py
+-rw-r--r--   0        0        0     2468 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/launchers/common.py
+-rw-r--r--   0        0        0        0 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/launchers/config_slurm/__init__.py
+-rw-r--r--   0        0        0     2497 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/launchers/config_slurm/launchers.yaml
+-rw-r--r--   0        0        0      717 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/launchers/test_local.py
+-rw-r--r--   0        0        0     2534 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/launchers/test_slurm.py
+-rw-r--r--   0        0        0     4016 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/restart.py
+-rw-r--r--   0        0        0      295 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/restart_main.py
+-rw-r--r--   0        0        0      407 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/scripts/notifyandwait.py
+-rw-r--r--   0        0        0      120 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/scripts/waitforfile.py
+-rw-r--r--   0        0        0      477 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/task_tokens.py
+-rw-r--r--   0        0        0        0 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/tasks/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/tasks/all.py
+-rw-r--r--   0        0        0      153 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/tasks/foreign.py
+-rw-r--r--   0        0        0      403 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_checkers.py
+-rw-r--r--   0        0        0     2005 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_dependencies.py
+-rw-r--r--   0        0        0     2967 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_findlauncher.py
+-rw-r--r--   0        0        0      780 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_forward.py
+-rw-r--r--   0        0        0    13397 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_identifier.py
+-rw-r--r--   0        0        0     1540 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_instance.py
+-rw-r--r--   0        0        0     2037 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_objects.py
+-rw-r--r--   0        0        0      781 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_outputs.py
+-rw-r--r--   0        0        0     6405 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_param.py
+-rw-r--r--   0        0        0     7580 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_progress.py
+-rw-r--r--   0        0        0     2338 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_serializers.py
+-rw-r--r--   0        0        0     3081 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_snippets.py
+-rw-r--r--   0        0        0      979 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_ssh.py
+-rw-r--r--   0        0        0     1975 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_tags.py
+-rw-r--r--   0        0        0     9429 2024-05-10 07:30:50.085061 experimaestro-1.5.5/src/experimaestro/tests/test_tasks.py
+-rw-r--r--   0        0        0     7826 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/tests/test_tokens.py
+-rw-r--r--   0        0        0     1257 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/tests/test_types.py
+-rw-r--r--   0        0        0     4339 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/tests/test_validation.py
+-rw-r--r--   0        0        0     1701 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/tests/token_reschedule.py
+-rw-r--r--   0        0        0     3805 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/tests/utils.py
+-rw-r--r--   0        0        0    14681 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/tokens.py
+-rw-r--r--   0        0        0        0 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/tools/__init__.py
+-rw-r--r--   0        0        0     3436 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/tools/diff.py
+-rw-r--r--   0        0        0     9184 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/tools/documentation.py
+-rw-r--r--   0        0        0     3516 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/tools/jobs.py
+-rw-r--r--   0        0        0     3334 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/typingutils.py
+-rw-r--r--   0        0        0     2434 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/utils/__init__.py
+-rw-r--r--   0        0        0      601 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/utils/asyncio.py
+-rw-r--r--   0        0        0     2394 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/utils/jobs.py
+-rw-r--r--   0        0        0     2183 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/utils/jupyter.py
+-rw-r--r--   0        0        0     1006 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/utils/resources.py
+-rw-r--r--   0        0        0      793 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/utils/settings.py
+-rw-r--r--   0        0        0     6766 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/utils/yaml.py
+-rw-r--r--   0        0        0      638 2024-05-10 07:30:50.089061 experimaestro-1.5.5/src/experimaestro/xpmutils.py
+-rw-r--r--   0        0        0     6265 1970-01-01 00:00:00.000000 experimaestro-1.5.5/PKG-INFO
```

### Comparing `experimaestro-1.5.4/LICENSE` & `experimaestro-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/README.md` & `experimaestro-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/pyproject.toml` & `experimaestro-1.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "src/experimaestro/server/data/*",
     "src/experimaestro/sphinx/static/experimaestro.css",
     "src/experimaestro/mkdocs/style.css"
 ]
-version = "1.5.4"
+version = "1.5.5"
 repository = "https://github.com/experimaestro/experimaestro-python"
 documentation = "https://experimaestro-python.readthedocs.io/"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
@@ -57,15 +57,15 @@
 flask = "^2.3"
 flask-socketio = "^5.3"
 arpeggio = "^2"
 watchdog = "^2"
 marshmallow = "^3.20"
 fabric = "^3"
 decorator = "^5"
-rpyc = "^5"
+rpyc = ">=5,<7"
 
 [tool.poetry.group.ssh]
 optional = true
 
 [tool.poetry.group.ssh.dependencies]
 paramiko = "^3.3"
 
@@ -119,11 +119,11 @@
 
 [tool.mypy]
 python_version = "3.9"
 warn_unused_ignores = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.5.4"
+version = "1.5.5"
 changelog_start_rev = "0.15.0"
 tag_format = "v$version"
 update_changelog_on_bump = true
```

### Comparing `experimaestro-1.5.4/src/experimaestro/__init__.py` & `experimaestro-1.5.5/src/experimaestro/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     LightweightTask,
     ObjectStore,
 )
 from .core.context import SerializationContext
 from .core.serializers import SerializationLWTask, PathSerializationLWTask
 from .core.types import Any, SubmitHook
 from .launchers import Launcher
-from .scheduler.environment import Environment
 from .scheduler.workspace import Workspace, RunMode
 from .scheduler import Scheduler, experiment, FailedExperiment
 from .notifications import progress, tqdm
 from .checkers import Choices
 from .xpmutils import DirectoryContext
 from .mkdocs.annotations import documentation
 from .scheduler.base import Job
```

### Comparing `experimaestro-1.5.4/src/experimaestro/__main__.py` & `experimaestro-1.5.5/src/experimaestro/__main__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/annotations.py` & `experimaestro-1.5.5/src/experimaestro/annotations.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/checkers.py` & `experimaestro-1.5.5/src/experimaestro/checkers.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/commandline.py` & `experimaestro-1.5.5/src/experimaestro/commandline.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/connectors/__init__.py` & `experimaestro-1.5.5/src/experimaestro/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/connectors/local.py` & `experimaestro-1.5.5/src/experimaestro/connectors/local.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/connectors/ssh.py` & `experimaestro-1.5.5/src/experimaestro/connectors/ssh.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/core/arguments.py` & `experimaestro-1.5.5/src/experimaestro/core/arguments.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/core/context.py` & `experimaestro-1.5.5/src/experimaestro/core/context.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/core/objects.py` & `experimaestro-1.5.5/src/experimaestro/core/objects.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/core/objects.pyi` & `experimaestro-1.5.5/src/experimaestro/core/objects.pyi`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/core/serialization.py` & `experimaestro-1.5.5/src/experimaestro/core/serialization.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/core/serializers.py` & `experimaestro-1.5.5/src/experimaestro/core/serializers.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/core/types.py` & `experimaestro-1.5.5/src/experimaestro/core/types.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/experiments/cli.py` & `experimaestro-1.5.5/src/experimaestro/experiments/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import inspect
-import itertools
 import json
 import logging
 import sys
 from pathlib import Path
 from typing import Any, List, Optional, Protocol, Tuple, Dict
 
 import click
 import omegaconf
 import yaml
 from experimaestro import LauncherRegistry, RunMode, experiment
 from experimaestro.experiments.configuration import ConfigurationBase
 from experimaestro.exceptions import HandledException
-from experimaestro.settings import get_settings, get_workspace
+from experimaestro.settings import get_workspace
 from omegaconf import OmegaConf, SCMode
 from termcolor import cprint
 
 
 class ExperimentHelper:
     """Helper for experiments"""
 
@@ -102,18 +101,24 @@
     default=None,
     help="Port for monitoring (can be defined in the settings.yaml file)",
 )
 @click.option(
     "--file", "xp_file", help="The file containing the main experimental code"
 )
 @click.option(
+    "--workspace",
+    type=str,
+    default=None,
+    help="Workspace ID (reads from settings.yaml in experimaestro config)",
+)
+@click.option(
     "--workdir",
     type=str,
     default=None,
-    help="Working directory - if None, uses the default XPM " "working directory",
+    help="Working environment",
 )
 @click.option("--conf", "-c", "extra_conf", type=str, multiple=True)
 @click.option(
     "--pre-yaml", type=str, multiple=True, help="Add YAML file after the main one"
 )
 @click.option(
     "--post-yaml", type=str, multiple=True, help="Add YAML file before the main one"
@@ -124,14 +129,15 @@
 def experiments_cli(  # noqa: C901
     yaml_file: str,
     xp_file: str,
     host: str,
     port: int,
     xpm_config_dir: Path,
     workdir: Optional[Path],
+    workspace: Optional[str],
     env: List[Tuple[str, str]],
     run_mode: RunMode,
     extra_conf: List[str],
     pre_yaml: List[str],
     post_yaml: List[str],
     args: List[str],
     show: bool,
@@ -220,34 +226,46 @@
         sys.exit(0)
 
     # Move to an object container
     configuration = OmegaConf.to_container(
         configuration, structured_config_mode=SCMode.INSTANTIATE
     )
 
-    # Get the working directory
-    settings = get_settings()
-    ws_env = {}
+    # Define the workspace
     workdir = Path(workdir) if workdir else None
-    if (workdir is None) or (not workdir.is_dir()):
-        logging.info("Searching for workspace %s", workdir)
-        ws_settings = get_workspace(str(workdir))
-        workdir = ws_settings.path.expanduser()
-        ws_env = ws_settings.env
+
+    if workspace:
+        ws_env = get_workspace(workspace)
+        if ws_env is None:
+            raise RuntimeError("No workspace named %s", workspace)
+
+        logging.info("Using workspace %s", ws_env.id)
+        if workdir:
+            # Overrides working directory
+            logging.info(" override working directory: %s", workdir)
+            ws_env.path = workdir
+        else:
+            workdir = ws_env.path
+    elif workdir:
+        logging.info("Using workdir %s", workdir)
+        ws_env = workdir
+    else:
+        ws_env = get_workspace()
+        assert ws_env is not None, "No workdir or workspace defined, and no default"
+        logging.info("Using default workspace %s", ws_env.id)
 
     logging.info("Using working directory %s", str(workdir.resolve()))
 
     # --- Runs the experiment
     with experiment(
-        workdir, configuration.id, host=host, port=port, run_mode=run_mode
+        ws_env, configuration.id, host=host, port=port, run_mode=run_mode
     ) as xp:
         # Set up the environment
         # (1) global settings (2) workspace settings and (3) command line settings
-        for key, value in itertools.chain(settings.env.items(), ws_env.items(), env):
-            logging.info("Setting environment: %s=%s", key, value)
+        for key, value in env:
             xp.setenv(key, value)
 
         try:
             # Run the experiment
             helper.xp = xp
             helper.run(list(args), configuration)
```

### Comparing `experimaestro-1.5.4/src/experimaestro/experiments/configuration.py` & `experimaestro-1.5.5/src/experimaestro/experiments/configuration.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/filter.py` & `experimaestro-1.5.5/src/experimaestro/filter.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/generators.py` & `experimaestro-1.5.5/src/experimaestro/generators.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/huggingface.py` & `experimaestro-1.5.5/src/experimaestro/huggingface.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/ipc.py` & `experimaestro-1.5.5/src/experimaestro/ipc.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/launcherfinder/base.py` & `experimaestro-1.5.5/src/experimaestro/launcherfinder/base.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/launcherfinder/parser.py` & `experimaestro-1.5.5/src/experimaestro/launcherfinder/parser.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/launcherfinder/registry.py` & `experimaestro-1.5.5/src/experimaestro/launcherfinder/registry.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/launcherfinder/specs.py` & `experimaestro-1.5.5/src/experimaestro/launcherfinder/specs.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/launchers/__init__.py` & `experimaestro-1.5.5/src/experimaestro/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/launchers/direct.py` & `experimaestro-1.5.5/src/experimaestro/launchers/direct.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/launchers/slurm/base.py` & `experimaestro-1.5.5/src/experimaestro/launchers/slurm/base.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/launchers/slurm/cli.py` & `experimaestro-1.5.5/src/experimaestro/launchers/slurm/cli.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/launchers/slurm/configuration.py` & `experimaestro-1.5.5/src/experimaestro/launchers/slurm/configuration.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/locking.py` & `experimaestro-1.5.5/src/experimaestro/locking.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/mkdocs/base.py` & `experimaestro-1.5.5/src/experimaestro/mkdocs/base.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/mkdocs/metaloader.py` & `experimaestro-1.5.5/src/experimaestro/mkdocs/metaloader.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/notifications.py` & `experimaestro-1.5.5/src/experimaestro/notifications.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/rpyc.py` & `experimaestro-1.5.5/src/experimaestro/rpyc.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/run.py` & `experimaestro-1.5.5/src/experimaestro/run.py`

 * *Files 20% similar despite different names*

```diff
@@ -88,24 +88,34 @@
                     logger.error("Error while releasing lock %s", lock)
 
             if self.started:
                 report_eoj()
             logger.info("Finished cleanup")
 
     def handle_error(self, code, frame_type):
-        logger.info("Finished with code %d", code)
+        logger.info("Error handler: finished with code %d", code)
         self.failedpath.write_text(str(code))
         self.cleanup()
         logger.info("Exiting")
         sys.exit(1)
 
     def run(self):
         atexit.register(self.cleanup)
-        signal.signal(signal.SIGTERM, self.handle_error)
-        signal.signal(signal.SIGINT, self.handle_error)
+        sigterm_handler = signal.signal(signal.SIGTERM, self.handle_error)
+        sigint_handler = signal.signal(signal.SIGINT, self.handle_error)
+
+        def remove_signal_handlers(remove_cleanup=True):
+            """Removes cleanup in forked processes"""
+            signal.signal(signal.SIGTERM, sigterm_handler)
+            signal.signal(signal.SIGINT, sigint_handler)
+            atexit.unregister(self.cleanup)
+
+        if sys.platform != "win32":
+            os.register_at_fork(after_in_child=remove_signal_handlers)
+
         try:
             workdir = self.scriptpath.parent
             os.chdir(workdir)
             os.getpid()
             logger.info("Working in directory %s", workdir)
 
             for lockfile in self.lockfiles:
@@ -125,18 +135,27 @@
                 logger.info("Job already completed")
             else:
                 logger.info("Running task")
                 rmfile(self.failedpath)
                 self.started = True
                 run(workdir / "params.json")
 
+                # ... remove the handlers
+                logger.info("Task ended successfully")
+                remove_signal_handlers(remove_cleanup=False)
+
                 # Everything went OK
                 sys.exit(0)
         except Exception:
             logger.exception("Got exception while running")
             self.handle_error(1, None)
 
         except SystemExit as e:
             if e.code == 0:
+                # Normal exit, just create the ".done" file
                 self.donepath.touch()
+
+                # ... and finish the exit process
+                logger.info("This is the end (TODO: remove this line)")
+                raise
             else:
                 self.handle_error(e.code, None)
```

### Comparing `experimaestro-1.5.4/src/experimaestro/scheduler/base.py` & `experimaestro-1.5.5/src/experimaestro/scheduler/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from collections import ChainMap
 from functools import cached_property
+import logging
 import os
 from pathlib import Path
 from shutil import rmtree
 import threading
 import time
 from typing import Any, List, Optional, Set, TypeVar, Union, TYPE_CHECKING
 import enum
 import signal
 import asyncio
 from experimaestro.exceptions import HandledException
 from experimaestro.notifications import LevelInformation, Reporter
 from typing import Dict
 from experimaestro.scheduler.services import Service
-from experimaestro.settings import get_settings
+from experimaestro.settings import WorkspaceSettings, get_settings
 
 
 from experimaestro.core.objects import Config, ConfigWalkContext
 from experimaestro.utils import logger
 from experimaestro.locking import Locks, LockError, Lock
-from .environment import Environment
 from .workspace import RunMode, Workspace
 from .dependencies import Dependency, DependencyStatus, Resource
 import concurrent.futures
 
 
 if TYPE_CHECKING:
     from experimaestro.connectors import Process
@@ -176,15 +176,15 @@
         1. The launcher environment
         1. The workspace environment
 
         """
         return ChainMap(
             {},
             self.launcher.environ if self.launcher else {},
-            self.workspace.environment.environ if self.workspace else {},
+            self.workspace.env if self.workspace else {},
         )
 
     @property
     def progress(self):
         return self._progress
 
     def set_progress(self, level: int, value: float, desc: Optional[str]):
@@ -504,14 +504,20 @@
         """
         logger.info("Submitting job %s", job)
         job._readyEvent = asyncio.Event()
         job.submittime = time.time()
         job.scheduler = self
         self.waitingjobs.add(job)
 
+        # Check that we don't have a completed job in
+        # alternate directories
+        for jobspath in experiment.current().alt_jobspaths:
+            # FIXME: check if done
+            pass
+
         # Creates a link into the experiment folder
         path = experiment.current().jobspath / job.relpath
         path.parent.mkdir(parents=True, exist_ok=True)
         if path.is_symlink():
             path.unlink()
         path.symlink_to(job.path)
 
@@ -715,29 +721,29 @@
 
     ```py
         with experiment(...) as xp:
             ...
     ```
     """
 
-    # Current experiment
+    #: Current experiment
     CURRENT: Optional["experiment"] = None
 
     @staticmethod
     def current() -> "experiment":
         """Returns the current experiment, but checking first if set
 
         If there is no current experiment, raises an AssertError
         """
         assert experiment.CURRENT is not None, "No current experiment defined"
         return experiment.CURRENT
 
     def __init__(
         self,
-        env: Union[Path, str, Environment],
+        env: Union[Path, str, WorkspaceSettings],
         name: str,
         *,
         host: Optional[str] = None,
         port: Optional[int] = None,
         token: Optional[str] = None,
         run_mode: Optional[RunMode] = None,
         launcher=None,
@@ -757,34 +763,31 @@
 
         :param run_mode: The run mode for the experiment (normal, generate run
             files, dry run)
         """
 
         from experimaestro.server import Server
 
-        if isinstance(env, Environment):
-            self.environment = env
-        else:
-            self.environment = Environment(workdir=env)
+        settings = get_settings()
+        if not isinstance(env, WorkspaceSettings):
+            env = WorkspaceSettings(id=None, path=Path(env))
 
         # Creates the workspace
         run_mode = run_mode or RunMode.NORMAL
-        self.workspace = Workspace(
-            self.environment, launcher=launcher, run_mode=run_mode
-        )
+        self.workspace = Workspace(settings, env, launcher=launcher, run_mode=run_mode)
 
         # Mark the directory has an experimaestro folder
         self.workdir = self.workspace.experimentspath / name
         self.workdir.mkdir(parents=True, exist_ok=True)
         self.xplockpath = self.workdir / "lock"
         self.xplock = None
         self.old_experiment = None
         self.services: Dict[str, Service] = {}
 
-        settings = get_settings()
+        # Get configuration settings
 
         if host is not None:
             settings.server.host = host
 
         if port is not None:
             settings.server.port = port
 
@@ -796,14 +799,19 @@
         self.server = (
             Server(self.scheduler, settings.server)
             if (settings.server.port is not None and settings.server.port >= 0)
             and self.workspace.run_mode == RunMode.NORMAL
             else None
         )
 
+        # Copy environment variable from main (but do not
+        # override)
+        for key, value in settings.env.items():
+            self.environment.setenv(key, value, override=False)
+
         if os.environ.get("XPM_ENABLEFAULTHANDLER", "0") == "1":
             import faulthandler
 
             logger.info("Enabling fault handler")
             faulthandler.enable(all_threads=True)
 
     def submit(self, job: Job):
@@ -829,14 +837,20 @@
 
     @property
     def jobspath(self):
         """Return the directory in which results can be stored for this experiment"""
         return self.workdir / "jobs"
 
     @property
+    def alt_jobspaths(self):
+        """Return potential other directories"""
+        for alt_workdir in self.workspace.alt_workdirs:
+            yield alt_workdir / "jobs"
+
+    @property
     def jobsbakpath(self):
         """Return the directory in which results can be stored for this experiment"""
         return self.workdir / "jobs.bak"
 
     def stop(self):
         """Stop the experiment as soon as possible"""
 
@@ -872,17 +886,19 @@
                                 job.stderr,
                             )
                     raise FailedExperiment(f"{count} failed jobs")
 
         future = asyncio.run_coroutine_threadsafe(awaitcompletion(), self.loop)
         return future.result()
 
-    def setenv(self, name, value):
+    def setenv(self, name, value, override=True):
         """Shortcut to set the environment value"""
-        self.environment.setenv(name, value)
+        if override or name not in self.workspace.env:
+            logging.info("Setting environment: %s=%s", name, value)
+            self.worskpace.env[name] = value
 
     def token(self, name: str, count: int):
         """Returns a token for this experiment
 
         The token is the default token of the workspace connector"""
         return self.workspace.connector.createtoken(name, count)
```

### Comparing `experimaestro-1.5.4/src/experimaestro/scheduler/dependencies.py` & `experimaestro-1.5.5/src/experimaestro/scheduler/dependencies.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/scheduler/services.py` & `experimaestro-1.5.5/src/experimaestro/scheduler/services.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/scriptbuilder.py` & `experimaestro-1.5.5/src/experimaestro/scriptbuilder.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,15 +88,19 @@
             self.command.output(context, fpnull)
         scriptpath = job.jobpath / ("%s.py" % job.name)
 
         logger.debug("Writing script %s", scriptpath)
         with scriptpath.open("wt") as out:
             out.write("#!{}\n".format(self.pythonpath))
             out.write("# Experimaestro generated task\n\n")
-            out.write("""import logging\nlogging.basicConfig(level=logging.INFO)\n\n""")
+            out.write(
+                """import logging\n"""
+                """logging.basicConfig(level=logging.INFO, """
+                """format='%(levelname)s:%(process)d:%(asctime)s [%(name)s] %(message)s', datefmt='%y-%m-%d %H:%M:%S')\n\n"""
+            )
 
             out.write("\nif __name__ == '__main__':\n\n" "")
 
             # --- Checks locks right away
 
             out.write(
                 """    from experimaestro.run import TaskRunner\n    import os\n\n"""
```

### Comparing `experimaestro-1.5.4/src/experimaestro/server/__init__.py` & `experimaestro-1.5.5/src/experimaestro/server/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/016b4a6cdced82ab3aa1.ttf` & `experimaestro-1.5.5/src/experimaestro/server/data/016b4a6cdced82ab3aa1.ttf`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/0c35d18bf06992036b69.woff2` & `experimaestro-1.5.5/src/experimaestro/server/data/0c35d18bf06992036b69.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2` & `experimaestro-1.5.5/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/3a4004a46a653d4b2166.woff` & `experimaestro-1.5.5/src/experimaestro/server/data/3a4004a46a653d4b2166.woff`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/3baa5b8f3469222b822d.woff` & `experimaestro-1.5.5/src/experimaestro/server/data/3baa5b8f3469222b822d.woff`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/4d73cb90e394b34b7670.woff` & `experimaestro-1.5.5/src/experimaestro/server/data/4d73cb90e394b34b7670.woff`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2` & `experimaestro-1.5.5/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/50701fbb8177c2dde530.ttf` & `experimaestro-1.5.5/src/experimaestro/server/data/50701fbb8177c2dde530.ttf`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/5d681e2edae8c60630db.woff` & `experimaestro-1.5.5/src/experimaestro/server/data/5d681e2edae8c60630db.woff`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2` & `experimaestro-1.5.5/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/878f31251d960bd6266f.woff2` & `experimaestro-1.5.5/src/experimaestro/server/data/878f31251d960bd6266f.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/b041b1fa4fe241b23445.woff2` & `experimaestro-1.5.5/src/experimaestro/server/data/b041b1fa4fe241b23445.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/b6879d41b0852f01ed5b.woff2` & `experimaestro-1.5.5/src/experimaestro/server/data/b6879d41b0852f01ed5b.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/c380809fd3677d7d6903.woff2` & `experimaestro-1.5.5/src/experimaestro/server/data/c380809fd3677d7d6903.woff2`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/d75e3fd1eb12e9bd6655.ttf` & `experimaestro-1.5.5/src/experimaestro/server/data/d75e3fd1eb12e9bd6655.ttf`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/f882956fd323fd322f31.woff` & `experimaestro-1.5.5/src/experimaestro/server/data/f882956fd323fd322f31.woff`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/favicon.ico` & `experimaestro-1.5.5/src/experimaestro/server/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/index.css` & `experimaestro-1.5.5/src/experimaestro/server/data/index.css`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/index.css.map` & `experimaestro-1.5.5/src/experimaestro/server/data/index.css.map`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/index.html` & `experimaestro-1.5.5/src/experimaestro/server/data/index.html`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/index.js` & `experimaestro-1.5.5/src/experimaestro/server/data/index.js`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/server/data/index.js.map` & `experimaestro-1.5.5/src/experimaestro/server/data/index.js.map`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/settings.py` & `experimaestro-1.5.5/src/experimaestro/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from omegaconf import OmegaConf
+from omegaconf import OmegaConf, SCMode
 from dataclasses import field, dataclass
 from functools import lru_cache
 from pathlib import Path
 from typing import Dict, Optional, List
 
 
 @dataclass
@@ -19,23 +19,31 @@
 
     token: Optional[str] = None
     """Token for the server"""
 
 
 @dataclass
 class WorkspaceSettings:
+    """Defines the workspace"""
+
     id: str
     """The workspace identifier"""
 
-    path: Path
+    path: Path = field()
     """The workspace path"""
 
     env: Dict[str, str] = field(default_factory=dict)
     """Workspace specific environment variables"""
 
+    alt_workspaces: List[str] = field(default_factory=list)
+    """Alternative workspaces to find jobs or experiments"""
+
+    def __post_init__(self):
+        self.path = self.path.expanduser().resolve()
+
 
 @dataclass
 class Settings:
     server: ServerSettings = field(default_factory=ServerSettings)
     workspaces: List[WorkspaceSettings] = field(default_factory=list)
 
     env: Dict[str, str] = field(default_factory=dict)
@@ -47,21 +55,23 @@
     if "PYTEST_CURRENT_TEST" in os.environ:
         return Settings()
     else:
         schema = OmegaConf.structured(Settings)
 
         path = path or Path("~/.config/experimaestro/settings.yaml").expanduser()
         if not path.is_file():
-            return schema
+            return schema.to_object()
 
         conf = OmegaConf.load(path)
-        return OmegaConf.merge(schema, conf)
+        return OmegaConf.to_container(
+            OmegaConf.merge(schema, conf), structured_config_mode=SCMode.INSTANTIATE
+        )
 
 
-def get_workspace(id: Optional[str]) -> WorkspaceSettings:
+def get_workspace(id: Optional[str] = None) -> Optional[WorkspaceSettings]:
     """Return the workspace settings given an id (or None for the default one)"""
     workspaces = get_settings().workspaces
     if workspaces:
         if id is None:
             return workspaces[0]
         for workspace in workspaces:
             if id == workspace.id:
```

### Comparing `experimaestro-1.5.4/src/experimaestro/sphinx/__init__.py` & `experimaestro-1.5.5/src/experimaestro/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/conftest.py` & `experimaestro-1.5.5/src/experimaestro/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/connectors/test_local.py` & `experimaestro-1.5.5/src/experimaestro/tests/connectors/test_local.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/connectors/utils.py` & `experimaestro-1.5.5/src/experimaestro/tests/connectors/utils.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/launchers/bin/sacct` & `experimaestro-1.5.5/src/experimaestro/tests/launchers/bin/sacct`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/launchers/bin/sbatch` & `experimaestro-1.5.5/src/experimaestro/tests/launchers/bin/sbatch`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/launchers/common.py` & `experimaestro-1.5.5/src/experimaestro/tests/launchers/common.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/launchers/config_slurm/launchers.yaml` & `experimaestro-1.5.5/src/experimaestro/tests/launchers/config_slurm/launchers.yaml`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/launchers/test_local.py` & `experimaestro-1.5.5/src/experimaestro/tests/launchers/test_local.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/launchers/test_slurm.py` & `experimaestro-1.5.5/src/experimaestro/tests/launchers/test_slurm.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/restart.py` & `experimaestro-1.5.5/src/experimaestro/tests/restart.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/tasks/all.py` & `experimaestro-1.5.5/src/experimaestro/tests/tasks/all.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_dependencies.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_findlauncher.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_findlauncher.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_forward.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_forward.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_identifier.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_instance.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_objects.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_outputs.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_outputs.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_param.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_progress.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_serializers.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_snippets.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_snippets.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_ssh.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_ssh.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_tags.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_tasks.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_tokens.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_types.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/test_validation.py` & `experimaestro-1.5.5/src/experimaestro/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/token_reschedule.py` & `experimaestro-1.5.5/src/experimaestro/tests/token_reschedule.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tests/utils.py` & `experimaestro-1.5.5/src/experimaestro/tests/utils.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tokens.py` & `experimaestro-1.5.5/src/experimaestro/tokens.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tools/diff.py` & `experimaestro-1.5.5/src/experimaestro/tools/diff.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tools/documentation.py` & `experimaestro-1.5.5/src/experimaestro/tools/documentation.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/tools/jobs.py` & `experimaestro-1.5.5/src/experimaestro/tools/jobs.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/typingutils.py` & `experimaestro-1.5.5/src/experimaestro/typingutils.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/utils/__init__.py` & `experimaestro-1.5.5/src/experimaestro/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/utils/asyncio.py` & `experimaestro-1.5.5/src/experimaestro/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/utils/jobs.py` & `experimaestro-1.5.5/src/experimaestro/utils/jobs.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/utils/jupyter.py` & `experimaestro-1.5.5/src/experimaestro/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/utils/resources.py` & `experimaestro-1.5.5/src/experimaestro/utils/resources.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/utils/settings.py` & `experimaestro-1.5.5/src/experimaestro/utils/settings.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/utils/yaml.py` & `experimaestro-1.5.5/src/experimaestro/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/src/experimaestro/xpmutils.py` & `experimaestro-1.5.5/src/experimaestro/xpmutils.py`

 * *Files identical despite different names*

### Comparing `experimaestro-1.5.4/PKG-INFO` & `experimaestro-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimaestro
-Version: 1.5.4
+Version: 1.5.5
 Summary: "Experimaestro is a computer science experiment manager"
 Home-page: https://github.com/experimaestro/experimaestro-python
 License: GPL-3
 Keywords: experiment manager
 Author: Benjamin Piwowarski
 Author-email: benjamin@piwowarski.fr
 Requires-Python: >=3.8,<4.0
@@ -37,15 +37,15 @@
 Requires-Dist: marshmallow (>=3.20,<4.0)
 Requires-Dist: omegaconf (>=2.3,<3.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: pyparsing (>=3.1,<4.0)
 Requires-Dist: pytools (>=2023.1.1,<2024.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31,<3.0)
-Requires-Dist: rpyc (>=5,<6)
+Requires-Dist: rpyc (>=5,<7)
 Requires-Dist: sortedcontainers (>=2.4,<3.0)
 Requires-Dist: termcolor (>=2.3)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: typing-extensions (>=4.2) ; python_version < "3.12"
 Requires-Dist: watchdog (>=2,<3)
 Project-URL: Documentation, https://experimaestro-python.readthedocs.io/
 Project-URL: Repository, https://github.com/experimaestro/experimaestro-python
```

