# Comparing `tmp/deebot_client-7.1.0.tar.gz` & `tmp/deebot_client-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deebot_client-7.1.0.tar", last modified: Wed Apr 24 07:05:32 2024, max compression
+gzip compressed data, was "deebot_client-7.2.0.tar", last modified: Fri May 10 10:22:14 2024, max compression
```

## Comparing `deebot_client-7.1.0.tar` & `deebot_client-7.2.0.tar`

### file list

```diff
@@ -1,228 +1,229 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.015007 deebot_client-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:31.987007 deebot_client-7.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:31.987007 deebot_client-7.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:31.987007 deebot_client-7.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.prettierrc.js
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-24 07:05:22.000000 deebot_client-7.1.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-24 07:05:22.000000 deebot_client-7.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-24 07:05:32.015007 deebot_client-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-24 07:05:22.000000 deebot_client-7.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:31.987007 deebot_client-7.1.0/deebot_client/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14623 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:31.991007 deebot_client-7.1.0/deebot_client/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:31.995007 deebot_client-7.1.0/deebot_client/commands/json/
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/border_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/carpet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/child_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/clean_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/clean_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/clear_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/cross_map_border_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/efficiency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/life_span.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/map.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/moveup_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/multimap_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/ota.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/play_sound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/relocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/safe_protect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/sweep_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/true_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/voice_assistant_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/water_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/json/work_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:31.995007 deebot_client-7.1.0/deebot_client/commands/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/xml/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/xml/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/xml/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/xml/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/commands/xml/pos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/event_bus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:31.999007 deebot_client-7.1.0/deebot_client/events/
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/events/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/events/efficiency_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/events/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/events/map.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/events/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/events/water_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/events/work_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:31.999007 deebot_client-7.1.0/deebot_client/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.003008 deebot_client-7.1.0/deebot_client/hardware/deebot/
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/2o4lnm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/55aiho.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/5xu9h3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/626v6g.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/85nbtp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/9ku8nu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/clojes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/e6ofmn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/fallback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/itk04l.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/lf3bn4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/lx3j7m.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/p1jij8.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/p95mgv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/paeygf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/rss8xk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/umwv6z.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/vi829v.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/x5d34r.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/yna5xi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/hardware/deebot/zjavof.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23546 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.003008 deebot_client-7.1.0/deebot_client/messages/
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.003008 deebot_client-7.1.0/deebot_client/messages/json/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/messages/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/messages/json/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/messages/json/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/messages/json/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.003008 deebot_client-7.1.0/deebot_client/util/
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/util/continents.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 07:05:22.000000 deebot_client-7.1.0/deebot_client/util/countries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.015007 deebot_client-7.1.0/deebot_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-24 07:05:31.000000 deebot_client-7.1.0/deebot_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-04-24 07:05:31.000000 deebot_client-7.1.0/deebot_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:05:31.000000 deebot_client-7.1.0/deebot_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 07:05:31.000000 deebot_client-7.1.0/deebot_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 07:05:31.000000 deebot_client-7.1.0/deebot_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-24 07:05:22.000000 deebot_client-7.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-24 07:05:22.000000 deebot_client-7.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 07:05:22.000000 deebot_client-7.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 07:05:22.000000 deebot_client-7.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 07:05:22.000000 deebot_client-7.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 07:05:22.000000 deebot_client-7.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.003008 deebot_client-7.1.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-04-24 07:05:22.000000 deebot_client-7.1.0/scripts/check_getLogger.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-04-24 07:05:22.000000 deebot_client-7.1.0/scripts/run-in-env.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:05:32.015007 deebot_client-7.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.003008 deebot_client-7.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.003008 deebot_client-7.1.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.011007 deebot_client-7.1.0/tests/commands/json/
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_border_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_carpet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_child_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_clean_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_clean_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_cross_map_border_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_life_span.py
--rw-r--r--   0 runner    (1001) docker     (127)    11091 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_moveup_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_mulitmap_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_ota.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_safe_protect.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_sweep_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_true_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_voice_assistant_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_water_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/json/test_work_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.011007 deebot_client-7.1.0/tests/commands/xml/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/xml/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/xml/test_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/xml/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/commands/xml/test_pos.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.011007 deebot_client-7.1.0/tests/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.011007 deebot_client-7.1.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/fixtures/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/fixtures/mqtt_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.011007 deebot_client-7.1.0/tests/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/hardware/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.011007 deebot_client-7.1.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/helpers/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.011007 deebot_client-7.1.0/tests/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/messages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.011007 deebot_client-7.1.0/tests/messages/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/messages/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/messages/json/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/messages/json/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/messages/json/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/messages/test_get_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/messages/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/mqtt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/test_event_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/test_mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/test_mqtt_client_reconnect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:32.015007 deebot_client-7.1.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/util/test_continents.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/util/test_countries.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 07:05:22.000000 deebot_client-7.1.0/tests/util/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.081972 deebot_client-7.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.081972 deebot_client-7.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.081972 deebot_client-7.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.prettierrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-10 10:22:09.000000 deebot_client-7.2.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-10 10:22:09.000000 deebot_client-7.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-10 10:22:14.105971 deebot_client-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-10 10:22:09.000000 deebot_client-7.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.081972 deebot_client-7.2.0/deebot_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14623 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10781 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.085971 deebot_client-7.2.0/deebot_client/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.089971 deebot_client-7.2.0/deebot_client/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/border_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/carpet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/child_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/clean_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/clear_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/cross_map_border_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/life_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/moveup_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/multimap_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/ota.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/play_sound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/relocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/safe_protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/sweep_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/voice_assistant_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/json/work_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.089971 deebot_client-7.2.0/deebot_client/commands/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/commands/xml/pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/event_bus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.089971 deebot_client-7.2.0/deebot_client/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/efficiency_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/events/work_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.093971 deebot_client-7.2.0/deebot_client/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.093971 deebot_client-7.2.0/deebot_client/hardware/deebot/
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/2o4lnm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/55aiho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/5xu9h3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/626v6g.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/77atlz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/85nbtp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/9ku8nu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/clojes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/e6ofmn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/fallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/itk04l.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/lf3bn4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/lx3j7m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/p1jij8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/p95mgv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7176 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/paeygf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/rss8xk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/umwv6z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/vi829v.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/x5d34r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/yna5xi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7918 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/hardware/deebot/zjavof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23602 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.093971 deebot_client-7.2.0/deebot_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.097972 deebot_client-7.2.0/deebot_client/messages/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/messages/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/messages/json/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/messages/json/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/messages/json/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.097972 deebot_client-7.2.0/deebot_client/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/util/continents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-10 10:22:09.000000 deebot_client-7.2.0/deebot_client/util/countries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/deebot_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-10 10:22:14.000000 deebot_client-7.2.0/deebot_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-10 10:22:14.000000 deebot_client-7.2.0/deebot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:22:14.000000 deebot_client-7.2.0/deebot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 10:22:14.000000 deebot_client-7.2.0/deebot_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 10:22:14.000000 deebot_client-7.2.0/deebot_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-10 10:22:09.000000 deebot_client-7.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-10 10:22:09.000000 deebot_client-7.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-10 10:22:09.000000 deebot_client-7.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 10:22:09.000000 deebot_client-7.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-10 10:22:09.000000 deebot_client-7.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 10:22:09.000000 deebot_client-7.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.097972 deebot_client-7.2.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      561 2024-05-10 10:22:09.000000 deebot_client-7.2.0/scripts/check_getLogger.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      450 2024-05-10 10:22:09.000000 deebot_client-7.2.0/scripts/run-in-env.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:22:14.105971 deebot_client-7.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.097972 deebot_client-7.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.097972 deebot_client-7.2.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.101971 deebot_client-7.2.0/tests/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_border_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_carpet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_child_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_clean_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_cross_map_border_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_life_span.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14073 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_moveup_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_mulitmap_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_ota.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_safe_protect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_sweep_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_voice_assistant_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_water_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/json/test_work_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/commands/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/xml/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/xml/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/xml/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/commands/xml/test_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/fixtures/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/fixtures/mqtt_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/hardware/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/helpers/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/messages/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/json/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/json/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/json/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/test_get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/messages/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/mqtt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7482 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/test_mqtt_client_reconnect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:14.105971 deebot_client-7.2.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/util/test_continents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/util/test_countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 10:22:09.000000 deebot_client-7.2.0/tests/util/test_init.py
```

### Comparing `deebot_client-7.1.0/.devcontainer.json` & `deebot_client-7.2.0/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `deebot_client-7.2.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/.github/release-drafter.yml` & `deebot_client-7.2.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/.github/workflows/ci.yml` & `deebot_client-7.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/.github/workflows/codeql-analysis.yml` & `deebot_client-7.2.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/.github/workflows/python-publish.yml` & `deebot_client-7.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/.pre-commit-config.yaml` & `deebot_client-7.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     - verifyNoGetLogger
 
 default_language_version:
   python: python3.12
 
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.7
+    rev: v0.4.3
     hooks:
       - id: ruff
         args:
           - --fix
           # - --unsafe-fixes
       - id: ruff-format
   - repo: https://github.com/asottile/pyupgrade
@@ -42,15 +42,15 @@
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: detect-private-key
       - id: no-commit-to-branch
         args: [--branch, main, --branch, dev]
       - id: requirements-txt-fixer
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.1.0
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         additional_dependencies:
           - prettier@3.2.4
           - prettier-plugin-sort-json@3.1.0
         exclude_types:
           - python
```

### Comparing `deebot_client-7.1.0/.yamllint` & `deebot_client-7.2.0/.yamllint`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/LICENSE.txt` & `deebot_client-7.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/PKG-INFO` & `deebot_client-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 7.1.0
+Version: 7.2.0
 Summary: Deebot client library in python 3
 Author-email: Robert Resch <robert@resch.dev>
 License: GPL-3.0
 Project-URL: Homepage, https://deebot.readthedocs.io/
 Project-URL: Source Code, https://github.com/DeebotUniverse/client.py
 Project-URL: Bug Reports, https://github.com/DeebotUniverse/client.py/issues
 Keywords: home,automation,homeassistant,vacuum,robot,deebot,ecovacs
```

### Comparing `deebot_client-7.1.0/README.md` & `deebot_client-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/api_client.py` & `deebot_client-7.2.0/deebot_client/api_client.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/authentication.py` & `deebot_client-7.2.0/deebot_client/authentication.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/capabilities.py` & `deebot_client-7.2.0/deebot_client/capabilities.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/command.py` & `deebot_client-7.2.0/deebot_client/command.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/__init__.py` & `deebot_client-7.2.0/deebot_client/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/__init__.py` & `deebot_client-7.2.0/deebot_client/commands/json/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/carpet.py` & `deebot_client-7.2.0/deebot_client/commands/json/carpet.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/charge.py` & `deebot_client-7.2.0/deebot_client/commands/json/charge.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/charge_state.py` & `deebot_client-7.2.0/deebot_client/commands/json/charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/clean.py` & `deebot_client-7.2.0/deebot_client/commands/json/clean.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/clean_count.py` & `deebot_client-7.2.0/deebot_client/commands/json/clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/clean_logs.py` & `deebot_client-7.2.0/deebot_client/commands/json/clean_logs.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/common.py` & `deebot_client-7.2.0/deebot_client/commands/json/common.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/continuous_cleaning.py` & `deebot_client-7.2.0/deebot_client/commands/json/continuous_cleaning.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/cross_map_border_warning.py` & `deebot_client-7.2.0/deebot_client/commands/json/cross_map_border_warning.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/custom.py` & `deebot_client-7.2.0/deebot_client/commands/json/custom.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/efficiency.py` & `deebot_client-7.2.0/deebot_client/commands/json/efficiency.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/error.py` & `deebot_client-7.2.0/deebot_client/commands/json/error.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/fan_speed.py` & `deebot_client-7.2.0/deebot_client/commands/json/fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/life_span.py` & `deebot_client-7.2.0/deebot_client/commands/json/life_span.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/map.py` & `deebot_client-7.2.0/deebot_client/commands/json/map.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,23 +12,27 @@
     MapSetEvent,
     MapSetType,
     MapSubsetEvent,
     MapTraceEvent,
     MinorMapEvent,
 )
 from deebot_client.events.map import CachedMapInfoEvent
+from deebot_client.logging_filter import get_logger
 from deebot_client.message import HandlingResult, HandlingState, MessageBodyDataDict
 from deebot_client.util import decompress_7z_base64_data
 
 from .common import JsonCommandWithMessageHandling
 
 if TYPE_CHECKING:
     from deebot_client.event_bus import EventBus
 
 
+_LOGGER = get_logger(__name__)
+
+
 class GetCachedMapInfo(JsonCommandWithMessageHandling, MessageBodyDataDict):
     """Get cached map info command."""
 
     name = "getCachedMapInfo"
     # version definition for using type of getMapSet v1 or v2
     _map_set_command: type[GetMapSet | GetMapSetV2]
 
@@ -195,29 +199,29 @@
 
 
 class GetMapSubSet(JsonCommandWithMessageHandling, MessageBodyDataDict):
     """Get map subset command."""
 
     _ROOM_NUM_TO_NAME = MappingProxyType(
         {
-            "0": "Default",
-            "1": "Living Room",
-            "2": "Dining Room",
-            "3": "Bedroom",
-            "4": "Study",
-            "5": "Kitchen",
-            "6": "Bathroom",
-            "7": "Laundry",
-            "8": "Lounge",
-            "9": "Storeroom",
-            "10": "Kids room",
-            "11": "Sunroom",
-            "12": "Corridor",
-            "13": "Balcony",
-            "14": "Gym",
+            0: "Default",
+            1: "Living Room",
+            2: "Dining Room",
+            3: "Bedroom",
+            4: "Study",
+            5: "Kitchen",
+            6: "Bathroom",
+            7: "Laundry",
+            8: "Lounge",
+            9: "Storeroom",
+            10: "Kids room",
+            11: "Sunroom",
+            12: "Corridor",
+            13: "Balcony",
+            14: "Gym",
             # 15 custom; get name from name attribute
         }
     )
 
     name = "getMapSubSet"
 
     def __init__(
@@ -250,33 +254,40 @@
         cls, event_bus: EventBus, data: dict[str, Any]
     ) -> HandlingResult:
         """Handle message->body->data and notify the correct event subscribers.
 
         :return: A message response
         """
         if MapSetType.has_value(data["type"]):
-            subtype = data.get("subtype", data.get("subType"))
-            name = None
-            if subtype == "15":
-                name = data.get("name")
-            elif subtype:
-                name = cls._ROOM_NUM_TO_NAME.get(subtype, None)
+            name = data.get("name", "").strip()
+
+            if not name and (subtype := data.get("subtype", data.get("subType"))):
+                try:
+                    name = cls._ROOM_NUM_TO_NAME.get(int(subtype), None)
+                except ValueError:
+                    _LOGGER.warning("Subtype is not a number", exc_info=True)
+                    return HandlingResult.analyse()
+
+            _type = MapSetType(data["type"])
+            if _type == MapSetType.ROOMS and not name:
+                _LOGGER.warning("Got room without a name")
+                return HandlingResult.analyse()
 
             # This command is used by new and old bots
             if data.get("compress", 0) == 1:
                 # Newer bot's return coordinates as base64 decoded string
                 coordinates = decompress_7z_base64_data(data["value"]).decode()
             else:
                 # Older bot's return coordinates direct as comma/semicolon separated list
                 coordinates = data["value"]
 
             event_bus.notify(
                 MapSubsetEvent(
                     id=int(data["mssid"]),
-                    type=MapSetType(data["type"]),
+                    type=_type,
                     coordinates=coordinates,
                     name=name,
                 )
             )
 
             return HandlingResult.success()
```

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/network.py` & `deebot_client-7.2.0/deebot_client/commands/json/network.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/ota.py` & `deebot_client-7.2.0/deebot_client/commands/json/ota.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/pos.py` & `deebot_client-7.2.0/deebot_client/commands/json/pos.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/stats.py` & `deebot_client-7.2.0/deebot_client/commands/json/stats.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/voice_assistant_state.py` & `deebot_client-7.2.0/deebot_client/commands/json/voice_assistant_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/volume.py` & `deebot_client-7.2.0/deebot_client/commands/json/volume.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/water_info.py` & `deebot_client-7.2.0/deebot_client/commands/json/water_info.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/json/work_mode.py` & `deebot_client-7.2.0/deebot_client/commands/json/work_mode.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/xml/__init__.py` & `deebot_client-7.2.0/deebot_client/commands/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/xml/charge_state.py` & `deebot_client-7.2.0/deebot_client/commands/xml/charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/xml/common.py` & `deebot_client-7.2.0/deebot_client/commands/xml/common.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/xml/error.py` & `deebot_client-7.2.0/deebot_client/commands/xml/error.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/xml/fan_speed.py` & `deebot_client-7.2.0/deebot_client/commands/xml/fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/commands/xml/pos.py` & `deebot_client-7.2.0/deebot_client/commands/xml/pos.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/const.py` & `deebot_client-7.2.0/deebot_client/const.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/device.py` & `deebot_client-7.2.0/deebot_client/device.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/event_bus.py` & `deebot_client-7.2.0/deebot_client/event_bus.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/events/__init__.py` & `deebot_client-7.2.0/deebot_client/events/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/events/map.py` & `deebot_client-7.2.0/deebot_client/events/map.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/events/water_info.py` & `deebot_client-7.2.0/deebot_client/events/water_info.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/exceptions.py` & `deebot_client-7.2.0/deebot_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/2o4lnm.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/2o4lnm.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/55aiho.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/55aiho.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/5xu9h3.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/5xu9h3.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/626v6g.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/626v6g.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/85nbtp.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/85nbtp.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/9ku8nu.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/9ku8nu.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/__init__.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/clojes.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/clojes.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/e6ofmn.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/e6ofmn.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/fallback.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/fallback.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/itk04l.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/77atlz.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/lf3bn4.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/lf3bn4.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/lx3j7m.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/lx3j7m.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/p1jij8.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/p1jij8.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/p95mgv.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/p95mgv.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/paeygf.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/paeygf.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/rss8xk.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/rss8xk.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/umwv6z.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/umwv6z.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/vi829v.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/vi829v.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/x5d34r.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/x5d34r.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/yna5xi.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/yna5xi.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/hardware/deebot/zjavof.py` & `deebot_client-7.2.0/deebot_client/hardware/deebot/zjavof.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/logging_filter.py` & `deebot_client-7.2.0/deebot_client/logging_filter.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/map.py` & `deebot_client-7.2.0/deebot_client/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,16 +308,17 @@
     return svg_positions
 
 
 def _get_svg_subset(
     subset: MapSubsetEvent,
     map_manipulation: MapManipulation,
 ) -> Path | svg.Polygon:
-    subset_coordinates: list[int] = ast.literal_eval(subset.coordinates)
+    _LOGGER.debug("Creating svg subset for %s", subset)
 
+    subset_coordinates: list[int] = ast.literal_eval(subset.coordinates)
     points = [
         _calc_point(
             subset_coordinates[i],
             subset_coordinates[i + 1],
             map_manipulation,
         )
         for i in range(0, len(subset_coordinates), 2)
```

### Comparing `deebot_client-7.1.0/deebot_client/message.py` & `deebot_client-7.2.0/deebot_client/message.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/messages/__init__.py` & `deebot_client-7.2.0/deebot_client/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/messages/json/__init__.py` & `deebot_client-7.2.0/deebot_client/messages/json/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/messages/json/battery.py` & `deebot_client-7.2.0/deebot_client/messages/json/battery.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/messages/json/map.py` & `deebot_client-7.2.0/deebot_client/messages/json/map.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/messages/json/stats.py` & `deebot_client-7.2.0/deebot_client/messages/json/stats.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/models.py` & `deebot_client-7.2.0/deebot_client/models.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/mqtt_client.py` & `deebot_client-7.2.0/deebot_client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/util/__init__.py` & `deebot_client-7.2.0/deebot_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client/util/continents.py` & `deebot_client-7.2.0/deebot_client/util/continents.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/deebot_client.egg-info/PKG-INFO` & `deebot_client-7.2.0/deebot_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 7.1.0
+Version: 7.2.0
 Summary: Deebot client library in python 3
 Author-email: Robert Resch <robert@resch.dev>
 License: GPL-3.0
 Project-URL: Homepage, https://deebot.readthedocs.io/
 Project-URL: Source Code, https://github.com/DeebotUniverse/client.py
 Project-URL: Bug Reports, https://github.com/DeebotUniverse/client.py/issues
 Keywords: home,automation,homeassistant,vacuum,robot,deebot,ecovacs
```

### Comparing `deebot_client-7.1.0/deebot_client.egg-info/SOURCES.txt` & `deebot_client-7.2.0/deebot_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 deebot_client/events/water_info.py
 deebot_client/events/work_mode.py
 deebot_client/hardware/__init__.py
 deebot_client/hardware/deebot/2o4lnm.py
 deebot_client/hardware/deebot/55aiho.py
 deebot_client/hardware/deebot/5xu9h3.py
 deebot_client/hardware/deebot/626v6g.py
+deebot_client/hardware/deebot/77atlz.py
 deebot_client/hardware/deebot/85nbtp.py
 deebot_client/hardware/deebot/9ku8nu.py
 deebot_client/hardware/deebot/__init__.py
 deebot_client/hardware/deebot/clojes.py
 deebot_client/hardware/deebot/e6ofmn.py
 deebot_client/hardware/deebot/fallback.py
 deebot_client/hardware/deebot/itk04l.py
```

### Comparing `deebot_client-7.1.0/mypy.ini` & `deebot_client-7.2.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/pyproject.toml` & `deebot_client-7.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/scripts/check_getLogger.sh` & `deebot_client-7.2.0/scripts/check_getLogger.sh`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/__init__.py` & `deebot_client-7.2.0/tests/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,26 +35,29 @@
 
     command._execute = _execute.__get__(command)  # type: ignore[method-assign]
     return (command, verify_result)
 
 
 async def assert_command(
     command: Command,
-    json_api_response: dict[str, Any],
+    json_api_response: dict[str, Any] | tuple[dict[str, Any], ...],
     expected_events: Event | None | Sequence[Event],
     *,
     command_result: CommandResult | None = None,
 ) -> None:
     command_result = command_result or CommandResult.success()
     event_bus = Mock(spec_set=EventBus)
     authenticator = Mock(spec_set=Authenticator)
     authenticator.authenticate = AsyncMock(
         return_value=Credentials("token", "user_id", 9999)
     )
-    authenticator.post_authenticated = AsyncMock(return_value=json_api_response)
+    if isinstance(json_api_response, tuple):
+        authenticator.post_authenticated = AsyncMock(side_effect=json_api_response)
+    else:
+        authenticator.post_authenticated = AsyncMock(return_value=json_api_response)
     device_info = ApiDeviceInfo(
         {
             "company": "company",
             "did": "did",
             "name": "name",
             "nick": "nick",
             "resource": "resource",
```

### Comparing `deebot_client-7.1.0/tests/commands/json/__init__.py` & `deebot_client-7.2.0/tests/commands/json/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_advanced_mode.py` & `deebot_client-7.2.0/tests/commands/json/test_advanced_mode.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_battery.py` & `deebot_client-7.2.0/tests/commands/json/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_border_switch.py` & `deebot_client-7.2.0/tests/commands/json/test_border_switch.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_carpet.py` & `deebot_client-7.2.0/tests/commands/json/test_carpet.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_charge.py` & `deebot_client-7.2.0/tests/commands/json/test_charge.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_charge_state.py` & `deebot_client-7.2.0/tests/commands/json/test_charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_child_lock.py` & `deebot_client-7.2.0/tests/commands/json/test_child_lock.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_clean.py` & `deebot_client-7.2.0/tests/commands/json/test_clean.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_clean_count.py` & `deebot_client-7.2.0/tests/commands/json/test_clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_clean_log.py` & `deebot_client-7.2.0/tests/commands/json/test_clean_log.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_clean_preference.py` & `deebot_client-7.2.0/tests/commands/json/test_clean_preference.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_common.py` & `deebot_client-7.2.0/tests/commands/json/test_common.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_continuous_cleaning.py` & `deebot_client-7.2.0/tests/commands/json/test_continuous_cleaning.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_cross_map_border_warning.py` & `deebot_client-7.2.0/tests/commands/json/test_cross_map_border_warning.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_custom.py` & `deebot_client-7.2.0/tests/commands/json/test_custom.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_efficiency.py` & `deebot_client-7.2.0/tests/commands/json/test_efficiency.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_error.py` & `deebot_client-7.2.0/tests/commands/json/test_error.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_fan_speed.py` & `deebot_client-7.2.0/tests/commands/json/test_fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_life_span.py` & `deebot_client-7.2.0/tests/commands/json/test_life_span.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_map.py` & `deebot_client-7.2.0/tests/commands/json/test_map.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
 
+from typing import Any
+
 import pytest
+from testfixtures import LogCapture
 
 from deebot_client.command import CommandResult
 from deebot_client.commands.json import (
     GetCachedMapInfo,
     GetMajorMap,
     GetMapSet,
     GetMapSubSet,
@@ -22,83 +25,154 @@
 from deebot_client.message import HandlingState
 from tests.helpers import get_request_json, get_success_body
 
 from . import assert_command
 
 
 @pytest.mark.parametrize(
-    ("compress", "value", "expected"),
+    ("compress", "value", "expected_coordinates"),
     [
         (
             1,
             "XQAABACZAAAAABaOQmW9Bsibxz42rKUpGlV7Rr4D1S/9x9mDa60v4J1BKrEsnk34EAt6X5gKkxwYzfOu3T8GAPpmIy5o4A==",
             "-9125,3225;-9025,3225;-8975,3175;-8975,2475;-8925,2425;-8925,2375;-8325,2375;-8275,2425;-8225,2375;-8225,2425;-8174,2475;-8024,2475;-8024,4375;-9125,4375",
         ),
         (
             0,
             "1400,1800;1400,3250;3000,3250;3000,2700;2900,2850;2750,2700;2800,1250;2700,1050;2700,850;1450,850;1400,1800",
             "1400,1800;1400,3250;3000,3250;3000,2700;2900,2850;2750,2700;2800,1250;2700,1050;2700,850;1450,850;1400,1800",
         ),
     ],
+    ids=["Compressed", "Plain"],
+)
+@pytest.mark.parametrize(
+    ("additional_data", "expected_name"),
+    [
+        (
+            {"subtype": "15", "name": "Levin"},
+            "Levin",
+        ),
+        (
+            {"subtype": "1", "name": "Custom"},
+            "Custom",
+        ),
+        (
+            {"subtype": "1", "name": ""},
+            "Living Room",
+        ),
+    ],
+    ids=["Custom subtype", "Override default name", "Default name"],
 )
 async def test_getMapSubSet_customName(
-    compress: int, value: str, expected: str
+    compress: int,
+    value: str,
+    expected_coordinates: str,
+    additional_data: dict[str, Any],
+    expected_name: str,
 ) -> None:
-    type = MapSetType.ROOMS
-    name = "Levin"
+    _type = MapSetType.ROOMS
     mid = "98100521"
     mssid = "8"
     json = get_request_json(
         get_success_body(
             {
-                "type": type.value,
-                "subtype": "15",
+                "type": _type.value,
                 "connections": "7,",
-                "name": name,
                 "seqIndex": 0,
                 "seq": 0,
                 "count": 0,
                 "totalCount": 50,
                 "index": 0,
                 "cleanset": "1,0,2",
                 "valueSize": 633,
                 "compress": compress,
                 "center": "-6775,-9225",
                 "mssid": mssid,
                 "value": value,
                 "mid": mid,
+                **additional_data,
             }
         )
     )
     await assert_command(
         GetMapSubSet(mid=mid, mssid=mssid, msid="1"),
         json,
-        MapSubsetEvent(8, type, expected, name),
+        MapSubsetEvent(8, _type, expected_coordinates, expected_name),
     )
 
 
-async def test_getMapSubSet_living_room() -> None:
-    type = MapSetType.ROOMS
-    value = "-1400,-1600;-1400,-1350;-950,-1100;-900,-150;-550,100;200,950;500,950;650,800;800,950;1850,950;1950,800;1950,-200;2050,-300;2300,-300;2550,-650;2700,-650;2700,-1600;2400,-1750;2700,-1900;2700,-2950;2450,-2950;2300,-3100;2400,-3200;2650,-3200;2700,-3500;2300,-3500;2200,-3250;2050,-3550;1200,-3550;1200,-3300;1050,-3200;950,-3300;950,-3550;600,-3550;550,-2850;850,-2800;950,-2700;850,-2600;950,-2400;900,-2350;800,-2300;550,-2500;550,-2350;400,-2250;200,-2650;-800,-2650;-950,-2550;-950,-2150;-650,-2000;-450,-2000;-400,-1950;-450,-1850;-750,-1800;-950,-1900;-1350,-1900;-1400,-1600"
-    json = get_request_json(
+@pytest.mark.parametrize(
+    ("additional_data", "expected_log_message"),
+    [
+        ({"subtype": "15"}, "Got room without a name"),
+        ({}, "Got room without a name"),
+        ({"subType": "bla"}, "Subtype is not a number"),
+    ],
+    ids=["No custom name", "No subtype", "Subtype not int"],
+)
+async def test_getMapSubSet_invalid(
+    additional_data: dict[str, Any], expected_log_message: str
+) -> None:
+    mid = "199390082"
+    mssid = "1"
+    data = {
+        "type": MapSetType.ROOMS,
+        "mssid": mssid,
+        "value": "-442,2910;-442,982;1214,982;1214,2910",
+        "connections": "12",
+        "mid": mid,
+        **additional_data,
+    }
+    json = get_request_json(get_success_body(data))
+    with LogCapture() as log:
+        await assert_command(
+            GetMapSubSet(mid=mid, mssid=mssid, msid="1"),
+            json,
+            None,
+            command_result=CommandResult(HandlingState.ANALYSE_LOGGED),
+        )
+
+        log.check_present(
+            (
+                "deebot_client.commands.json.map",
+                "WARNING",
+                expected_log_message,
+            )
+        )
+        log.check_present(
+            (
+                "deebot_client.message",
+                "DEBUG",
+                f"Could not handle getMapSubSet message: {data}",
+            )
+        )
+
+
+def _getMapSubSet_room_valid_response(value: str, id: int) -> dict[str, Any]:
+    return get_request_json(
         get_success_body(
             {
-                "type": type.value,
-                "mssid": "7",
+                "type": MapSetType.ROOMS.value,
+                "mssid": str(id),
                 "value": value,
                 "subtype": "1",
                 "connections": "12",
                 "mid": "199390082",
             }
         )
     )
+
+
+async def test_getMapSubSet_living_room() -> None:
+    value = "-1400,-1600;-1400,-1350;-950,-1100;-900,-150;-550,100;200,950;500,950;650,800;800,950;1850,950;1950,800;1950,-200;2050,-300;2300,-300;2550,-650;2700,-650;2700,-1600;2400,-1750;2700,-1900;2700,-2950;2450,-2950;2300,-3100;2400,-3200;2650,-3200;2700,-3500;2300,-3500;2200,-3250;2050,-3550;1200,-3550;1200,-3300;1050,-3200;950,-3300;950,-3550;600,-3550;550,-2850;850,-2800;950,-2700;850,-2600;950,-2400;900,-2350;800,-2300;550,-2500;550,-2350;400,-2250;200,-2650;-800,-2650;-950,-2550;-950,-2150;-650,-2000;-450,-2000;-400,-1950;-450,-1850;-750,-1800;-950,-1900;-1350,-1900;-1400,-1600"
+    json = _getMapSubSet_room_valid_response(value, 7)
     await assert_command(
         GetMapSubSet(mid="199390082", mssid="7", msid="1"),
         json,
-        MapSubsetEvent(7, type, value, "Living Room"),
+        MapSubsetEvent(7, MapSetType.ROOMS, value, "Living Room"),
     )
 
 
 @pytest.mark.parametrize(
     ("command", "map_set_type"),
     [
         (GetCachedMapInfo(), GetMapSet),
@@ -170,38 +244,50 @@
         MajorMapEvent(expected_mid, value.split(","), requested=True),
     )
 
 
 async def test_getMapSet() -> None:
     mid = "199390082"
     msid = "8"
-    json = get_request_json(
-        get_success_body(
-            {
-                "type": "ar",
-                "count": 7,
-                "mid": mid,
-                "msid": msid,
-                "subsets": [
-                    {"mssid": "7"},
-                    {"mssid": "12"},
-                    {"mssid": "17"},
-                    {"mssid": "14"},
-                    {"mssid": "10"},
-                    {"mssid": "11"},
-                    {"mssid": "13"},
-                ],
-            }
-        )
-    )
+    room_value = "-442,2910;-442,982;1214,982;1214,2910"
     subsets = [7, 12, 17, 14, 10, 11, 13]
+    json = (
+        # getMapSet response
+        get_request_json(
+            get_success_body(
+                {
+                    "type": "ar",
+                    "count": 7,
+                    "mid": mid,
+                    "msid": msid,
+                    "subsets": [
+                        {"mssid": "7"},
+                        {"mssid": "12"},
+                        {"mssid": "17"},
+                        {"mssid": "14"},
+                        {"mssid": "10"},
+                        {"mssid": "11"},
+                        {"mssid": "13"},
+                    ],
+                }
+            )
+        ),
+        # getMapSubSet response
+        *(_getMapSubSet_room_valid_response(room_value, subset) for subset in subsets),
+    )
     await assert_command(
         GetMapSet(mid),
         json,
-        MapSetEvent(MapSetType.ROOMS, subsets),
+        (
+            MapSetEvent(MapSetType.ROOMS, subsets),
+            *(
+                MapSubsetEvent(subset, MapSetType.ROOMS, room_value, "Living Room")
+                for subset in subsets
+            ),
+        ),
         command_result=CommandResult(
             HandlingState.SUCCESS,
             {"id": mid, "set_id": msid, "type": MapSetType.ROOMS, "subsets": subsets},
             [
                 GetMapSubSet(mid=mid, msid=msid, type=MapSetType.ROOMS, mssid=s)
                 for s in subsets
             ],
@@ -242,34 +328,46 @@
     mid = "199390082"
     msid = "8"
     type = MapSetType.ROOMS
     subsets_comp = (
         "XQAABADnAQAAAC2WwEHwYhHYFuLu9964T0CAIjkOBSGKBW+PcTQDCjKFThR86eaw4bFiV2BKLAP+0lTYd1ADOkmjNPrfSqBeHZLY4JNCaEMc2H245BSG143miuQm6X6"
         "KeTCnXV7Er028XLcnN9q/immzxeoPpkdhnbhuL9f8jW5kgVLGPJnfv2V2a79W4PjkSR4b4Px632ID+UKVwGL1mYiwNnMO35XA41W+pPsgW12ZRnsMDvGMAlv4VLhDJFAy4AA="
     )
-    json = get_request_json(
-        get_success_body(
-            {
-                "type": type,
-                "mid": mid,
-                "msid": msid,
-                "batid": "gheijg",
-                "serial": 1,
-                "index": 1,
-                "subsets": subsets_comp,
-                "infoSize": 199,
-            }
-        )
-    )
     subsets = [0, 1, 6, 2, 7, 3, 5]
+    room_value = "-442,2910;-442,982;1214,982;1214,2910"
+    json = (
+        # GetMapSetV2 response
+        get_request_json(
+            get_success_body(
+                {
+                    "type": type,
+                    "mid": mid,
+                    "msid": msid,
+                    "batid": "gheijg",
+                    "serial": 1,
+                    "index": 1,
+                    "subsets": subsets_comp,
+                    "infoSize": 199,
+                }
+            )
+        ),
+        # getMapSubSet response
+        *(_getMapSubSet_room_valid_response(room_value, subset) for subset in subsets),
+    )
 
     await assert_command(
         GetMapSetV2(mid, type),
         json,
-        MapSetEvent(MapSetType(type), subsets),
+        (
+            MapSetEvent(MapSetType(type), subsets),
+            *(
+                MapSubsetEvent(subset, MapSetType.ROOMS, room_value, "Living Room")
+                for subset in subsets
+            ),
+        ),
         command_result=CommandResult(
             HandlingState.SUCCESS,
             {"id": mid, "set_id": msid, "type": MapSetType(type), "subsets": subsets},
             [GetMapSubSet(mid=mid, msid=msid, type=type, mssid=s) for s in subsets],
         ),
     )
```

### Comparing `deebot_client-7.1.0/tests/commands/json/test_moveup_warning.py` & `deebot_client-7.2.0/tests/commands/json/test_moveup_warning.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_mulitmap_state.py` & `deebot_client-7.2.0/tests/commands/json/test_mulitmap_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_network.py` & `deebot_client-7.2.0/tests/commands/json/test_network.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_ota.py` & `deebot_client-7.2.0/tests/commands/json/test_ota.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_safe_protect.py` & `deebot_client-7.2.0/tests/commands/json/test_safe_protect.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_sweep_mode.py` & `deebot_client-7.2.0/tests/commands/json/test_sweep_mode.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_true_detect.py` & `deebot_client-7.2.0/tests/commands/json/test_true_detect.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_voice_assistant_state.py` & `deebot_client-7.2.0/tests/commands/json/test_voice_assistant_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_volume.py` & `deebot_client-7.2.0/tests/commands/json/test_volume.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_water_info.py` & `deebot_client-7.2.0/tests/commands/json/test_water_info.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/json/test_work_mode.py` & `deebot_client-7.2.0/tests/commands/json/test_work_mode.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/xml/test_charge_state.py` & `deebot_client-7.2.0/tests/commands/xml/test_charge_state.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/xml/test_error.py` & `deebot_client-7.2.0/tests/commands/xml/test_error.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/xml/test_fan_speed.py` & `deebot_client-7.2.0/tests/commands/xml/test_fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/commands/xml/test_pos.py` & `deebot_client-7.2.0/tests/commands/xml/test_pos.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/conftest.py` & `deebot_client-7.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/fixtures/base.py` & `deebot_client-7.2.0/tests/fixtures/base.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/fixtures/mqtt_server.py` & `deebot_client-7.2.0/tests/fixtures/mqtt_server.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/hardware/test_init.py` & `deebot_client-7.2.0/tests/hardware/test_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,14 +279,15 @@
     """Test that all models are loaded."""
     _load()
     assert list(DEVICES) == [
         "2o4lnm",
         "55aiho",
         "5xu9h3",
         "626v6g",
+        "77atlz",
         "85nbtp",
         "9ku8nu",
         "clojes",
         "e6ofmn",
         "fallback",
         "itk04l",
         "lf3bn4",
```

### Comparing `deebot_client-7.1.0/tests/helpers/__init__.py` & `deebot_client-7.2.0/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/helpers/tasks.py` & `deebot_client-7.2.0/tests/helpers/tasks.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/messages/__init__.py` & `deebot_client-7.2.0/tests/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/messages/json/test_battery.py` & `deebot_client-7.2.0/tests/messages/json/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/messages/json/test_map.py` & `deebot_client-7.2.0/tests/messages/json/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/messages/json/test_stats.py` & `deebot_client-7.2.0/tests/messages/json/test_stats.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/messages/test_get_messages.py` & `deebot_client-7.2.0/tests/messages/test_get_messages.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/mqtt_util.py` & `deebot_client-7.2.0/tests/mqtt_util.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/test_authentication.py` & `deebot_client-7.2.0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/test_command.py` & `deebot_client-7.2.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/test_device.py` & `deebot_client-7.2.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/test_event_bus.py` & `deebot_client-7.2.0/tests/test_event_bus.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/test_map.py` & `deebot_client-7.2.0/tests/test_map.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,24 @@
     ClosePath,
     CubicBezier,
     HorizontalLineToRel,
     LineToRel,
     MoveTo,
     MoveToRel,
     PathData,
+    Polygon,
     SmoothCubicBezierRel,
     VerticalLineToRel,
 )
 
 from deebot_client.events.map import (
     MajorMapEvent,
     MapChangedEvent,
     MapSetEvent,
+    MapSetType,
     MapSubsetEvent,
     MapTraceEvent,
     MinorMapEvent,
     Position,
     PositionsEvent,
     PositionType,
 )
@@ -34,14 +36,15 @@
     Map,
     MapData,
     MapManipulation,
     Path,
     Point,
     TracePoint,
     _calc_point,
+    _get_svg_subset,
     _points_to_svg_path,
 )
 from deebot_client.models import Room
 
 from .common import block_till_done
 
 if TYPE_CHECKING:
@@ -215,7 +218,53 @@
         ),
     ],
 )
 def test_points_to_svg_path(
     points: Sequence[Point | TracePoint], expected: list[PathData]
 ) -> None:
     assert _points_to_svg_path(points) == expected
+
+
+@pytest.mark.parametrize(
+    ("subset", "expected"),
+    [
+        (
+            MapSubsetEvent(
+                id=0, type=MapSetType.VIRTUAL_WALLS, coordinates="[-3900,668,-2133,668]"
+            ),
+            Path(
+                stroke="#f00000",
+                stroke_width=1.5,
+                stroke_dasharray=[4],
+                vector_effect="non-scaling-stroke",
+                d=[MoveTo(x=322.0, y=413.36), HorizontalLineToRel(dx=35.34)],
+            ),
+        ),
+        (
+            MapSubsetEvent(
+                id=1,
+                type=MapSetType.NO_MOP_ZONES,
+                coordinates="[-442,2910,-442,982,1214,982,1214,2910]",
+            ),
+            Polygon(
+                fill="#ffa50030",
+                stroke="#ffa500",
+                stroke_width=1.5,
+                stroke_dasharray=[4],
+                vector_effect="non-scaling-stroke",
+                points=[391.16, 458.2, 391.16, 419.64, 424.28, 419.64, 424.28, 458.2],
+            ),
+        ),
+    ],
+)
+def test_get_svg_subset(subset: MapSubsetEvent, expected: Path | Polygon) -> None:
+    manipulation = MapManipulation(
+        AxisManipulation(
+            map_shift=0,
+            svg_max=1000,
+        ),
+        AxisManipulation(
+            map_shift=0,
+            svg_max=1000,
+        ),
+    )
+    assert _get_svg_subset(subset, manipulation) == expected
```

### Comparing `deebot_client-7.1.0/tests/test_mqtt_client.py` & `deebot_client-7.2.0/tests/test_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/test_mqtt_client_reconnect.py` & `deebot_client-7.2.0/tests/test_mqtt_client_reconnect.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/util/test_continents.py` & `deebot_client-7.2.0/tests/util/test_continents.py`

 * *Files identical despite different names*

### Comparing `deebot_client-7.1.0/tests/util/test_init.py` & `deebot_client-7.2.0/tests/util/test_init.py`

 * *Files identical despite different names*

