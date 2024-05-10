# Comparing `tmp/neon-skill-device_controls-1.1.0.tar.gz` & `tmp/neon-skill-device_controls-1.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-device_controls-1.1.0.tar", last modified: Tue Apr  2 00:54:21 2024, max compression
+gzip compressed data, was "neon-skill-device_controls-1.1.1a1.tar", last modified: Fri May 10 17:34:22 2024, max compression
```

## Comparing `neon-skill-device_controls-1.1.0.tar` & `neon-skill-device_controls-1.1.1a1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.908077 neon-skill-device_controls-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-02 00:54:21.908077 neon-skill-device_controls-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    14983 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.892076 neon-skill-device_controls-1.1.0/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.892076 neon-skill-device_controls-1.1.0/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.896077 neon-skill-device_controls-1.1.0/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/action_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/already_requiring.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/already_skipping.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/ask_disable_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/ask_exit_shutdown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/ask_start_requiring.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/ask_start_skipping.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_brain_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_brain_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_cancel.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_exiting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_listening_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_listening_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_require_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_restarting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_shutdown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_skip_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_ww_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_ww_changing.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/confirm_ww_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/error_invalid_ww_requested.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/error_no_ww_api.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/error_no_ww_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/error_ww_already_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/error_ww_change_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/dialog/not_doing_anything.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.896077 neon-skill-device_controls-1.1.0/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/intent/exit.intent
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/intent/restart.intent
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/intent/shutdown.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.900076 neon-skill-device_controls-1.1.0/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/regex/wakeword.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.900076 neon-skill-device_controls-1.1.0/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/debug.voc
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/disable.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/enable.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/exit.voc
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/listening.voc
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/mycroft.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/neon.voc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/no.voc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/request.voc
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/restart.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/shutdown.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/solo.voc
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/start.voc
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/start_sww.voc
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/stop.voc
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/stop_sww.voc
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/en-us/vocab/ww.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.892076 neon-skill-device_controls-1.1.0/locale/uk-ua/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.904077 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/action_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/already_requiring.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/already_skipping.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/ask_disable_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/ask_exit_shutdown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/ask_start_requiring.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/ask_start_skipping.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_brain_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_brain_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_cancel.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_exiting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_listening_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_listening_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_require_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_restarting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_shutdown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_skip_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_ww_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_ww_changing.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/confirm_ww_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/error_invalid_ww_requested.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/error_no_ww_api.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/error_no_ww_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/error_ww_already_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/error_ww_change_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/dialog/not_doing_anything.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.904077 neon-skill-device_controls-1.1.0/locale/uk-ua/intent/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/intent/exit.intent
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/intent/restart.intent
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/intent/shutdown.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.904077 neon-skill-device_controls-1.1.0/locale/uk-ua/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/regex/wakeword.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.908077 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/debug.voc
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/disable.voc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/enable.voc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/exit.voc
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/listening.voc
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/mycroft.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/neon.voc
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/no.voc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/request.voc
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/restart.voc
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/shutdown.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/solo.voc
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/start.voc
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/start_sww.voc
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/stop.voc
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/stop_sww.voc
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/locale/uk-ua/vocab/ww.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.908077 neon-skill-device_controls-1.1.0/neon_skill_device_controls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-02 00:54:21.000000 neon-skill-device_controls-1.1.0/neon_skill_device_controls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-02 00:54:21.000000 neon-skill-device_controls-1.1.0/neon_skill_device_controls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:54:21.000000 neon-skill-device_controls-1.1.0/neon_skill_device_controls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 00:54:21.000000 neon-skill-device_controls-1.1.0/neon_skill_device_controls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 00:54:21.000000 neon-skill-device_controls-1.1.0/neon_skill_device_controls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 00:54:21.000000 neon-skill-device_controls-1.1.0/neon_skill_device_controls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:54:21.908077 neon-skill-device_controls-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:54:21.908077 neon-skill-device_controls-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-02 00:54:17.000000 neon-skill-device_controls-1.1.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.759799 neon-skill-device_controls-1.1.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-10 17:34:22.759799 neon-skill-device_controls-1.1.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.743799 neon-skill-device_controls-1.1.1a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.743799 neon-skill-device_controls-1.1.1a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.747799 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/action_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/already_requiring.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/already_skipping.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/ask_disable_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/ask_exit_shutdown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/ask_start_requiring.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/ask_start_skipping.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_brain_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_brain_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_cancel.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_exiting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_listening_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_listening_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_require_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_restarting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_shutdown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_skip_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_ww_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_ww_changing.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/confirm_ww_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/error_invalid_ww_requested.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/error_no_ww_api.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/error_no_ww_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/error_ww_already_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/error_ww_change_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/dialog/not_doing_anything.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.747799 neon-skill-device_controls-1.1.1a1/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/intent/exit.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/intent/restart.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/intent/shutdown.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.747799 neon-skill-device_controls-1.1.1a1/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/regex/wakeword.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.751799 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/debug.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/disable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/enable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/exit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/listening.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/mycroft.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/no.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/request.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/restart.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/shutdown.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/solo.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/start.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/start_sww.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/stop.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/stop_sww.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/en-us/vocab/ww.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.743799 neon-skill-device_controls-1.1.1a1/locale/uk-ua/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.755799 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/action_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/already_requiring.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/already_skipping.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/ask_disable_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/ask_exit_shutdown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/ask_start_requiring.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/ask_start_skipping.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_brain_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_brain_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_cancel.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_exiting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_listening_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_listening_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_require_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_restarting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_shutdown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_skip_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_ww_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_ww_changing.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/confirm_ww_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/error_invalid_ww_requested.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/error_no_ww_api.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/error_no_ww_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/error_ww_already_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/error_ww_change_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/dialog/not_doing_anything.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.755799 neon-skill-device_controls-1.1.1a1/locale/uk-ua/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/intent/exit.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/intent/restart.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/intent/shutdown.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.755799 neon-skill-device_controls-1.1.1a1/locale/uk-ua/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/regex/wakeword.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.759799 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/debug.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/disable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/enable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/exit.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/listening.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/mycroft.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/no.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/request.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/restart.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/shutdown.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/solo.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/start.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/start_sww.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/stop.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/stop_sww.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/locale/uk-ua/vocab/ww.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.759799 neon-skill-device_controls-1.1.1a1/neon_skill_device_controls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-10 17:34:22.000000 neon-skill-device_controls-1.1.1a1/neon_skill_device_controls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-10 17:34:22.000000 neon-skill-device_controls-1.1.1a1/neon_skill_device_controls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:34:22.000000 neon-skill-device_controls-1.1.1a1/neon_skill_device_controls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-10 17:34:22.000000 neon-skill-device_controls-1.1.1a1/neon_skill_device_controls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-10 17:34:22.000000 neon-skill-device_controls-1.1.1a1/neon_skill_device_controls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:34:22.000000 neon-skill-device_controls-1.1.1a1/neon_skill_device_controls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:34:22.759799 neon-skill-device_controls-1.1.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:34:22.759799 neon-skill-device_controls-1.1.1a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-10 17:34:19.000000 neon-skill-device_controls-1.1.1a1/version.py
```

### Comparing `neon-skill-device_controls-1.1.0/LICENSE.md` & `neon-skill-device_controls-1.1.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.1.0/PKG-INFO` & `neon-skill-device_controls-1.1.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-device_controls
-Version: 1.1.0
+Version: 1.1.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-device_controls
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-device_controls-1.1.0/README.md` & `neon-skill-device_controls-1.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.1.0/__init__.py` & `neon-skill-device_controls-1.1.1a1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 from ovos_bus_client import Message
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from neon_utils.message_utils import dig_for_message
 from neon_utils.skills.neon_skill import NeonSkill
 from neon_utils.validator_utils import numeric_confirmation_validator
-
-from mycroft.skills import intent_handler, intent_file_handler
+from ovos_workshop.decorators import intent_handler
 
 
 class SystemCommand(Enum):
     SHUTDOWN = "shut down this device"
     RESTART = "restart Neon"
     EXIT = "stop Neon"
 
@@ -107,25 +106,25 @@
                                       "number": confirm_number},
                                      validator, "action_not_confirmed")
         if not response:
             self.speak_dialog("confirm_cancel", private=True)
         elif response:
             self._do_exit_shutdown(action)
 
-    @intent_file_handler("exit.intent")
+    @intent_handler("exit.intent")
     def handle_exit_intent(self, message):
         message.data['exit'] = True
         self.handle_exit_shutdown_intent(message)
 
-    @intent_file_handler("restart.intent")
+    @intent_handler("restart.intent")
     def handle_restart_intent(self, message):
         message.data['restart'] = True
         self.handle_exit_shutdown_intent(message)
 
-    @intent_file_handler("shutdown.intent")
+    @intent_handler("shutdown.intent")
     def handle_shutdown_intent(self, message):
         message.data['shutdown'] = True
         self.handle_exit_shutdown_intent(message)
 
     @intent_handler(IntentBuilder("SkipWWIntent").require("ww")
                     .require("start_sww"))
     @intent_handler(IntentBuilder("SoloModeIntent").one_of("start", "enable")
```

### Comparing `neon-skill-device_controls-1.1.0/neon_skill_device_controls.egg-info/PKG-INFO` & `neon-skill-device_controls-1.1.1a1/neon_skill_device_controls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-device-controls
-Version: 1.1.0
+Version: 1.1.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-device_controls
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-device_controls-1.1.0/neon_skill_device_controls.egg-info/SOURCES.txt` & `neon-skill-device_controls-1.1.1a1/neon_skill_device_controls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.1.0/setup.py` & `neon-skill-device_controls-1.1.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.1.0/skill.json` & `neon-skill-device_controls-1.1.1a1/skill.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984848484848485%*

 * *Differences: {"'requirements'": "{'python': {insert: [(0, 'adapt-parser<2.0,>=0.5'), (4, "*

 * *                   "'ovos-workshop~=0.0.15')]}}"}*

```diff
@@ -29,17 +29,19 @@
         "x86_64",
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
+            "adapt-parser<2.0,>=0.5",
             "neon-utils~=1.0",
             "ovos-bus-client~=0.0.3",
-            "ovos-utils~=0.0, >=0.0.28"
+            "ovos-utils~=0.0, >=0.0.28",
+            "ovos-workshop~=0.0.15"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Handles system-wide settings and controls.",
     "skillname": "skill-device_controls",
     "summary": "Handles system-wide settings and controls.",
```

### Comparing `neon-skill-device_controls-1.1.0/test/test_skill.py` & `neon-skill-device_controls-1.1.1a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-1.1.0/version.py` & `neon-skill-device_controls-1.1.1a1/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.1.0"
+__version__ = "1.1.1a1"
```

