# Comparing `tmp/pyinsteon-1.5.3.tar.gz` & `tmp/pyinsteon-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinsteon-1.5.3.tar", last modified: Mon Dec 11 23:19:17 2023, max compression
+gzip compressed data, was "pyinsteon-1.6.0.tar", last modified: Fri May 10 12:54:50 2024, max compression
```

## Comparing `pyinsteon-1.5.3.tar` & `pyinsteon-1.6.0.tar`

### file list

```diff
@@ -1,246 +1,249 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1547 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/DESCRIPTION.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/LICENSE.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       53 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2652 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2144 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/README.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.815653 pyinsteon-1.5.3/pyinsteon/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3731 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      126 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/__main__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2917 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/address.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.815653 pyinsteon-1.5.3/pyinsteon/aldb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      183 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/aldb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5205 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/aldb/aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    19535 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/aldb/aldb_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1841 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/aldb/aldb_battery.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9046 2023-12-11 23:18:04.000000 pyinsteon-1.5.3/pyinsteon/aldb/aldb_record.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4042 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/aldb/mock_modem_aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3920 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/aldb/modem_aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4255 2023-12-11 23:18:04.000000 pyinsteon-1.5.3/pyinsteon/aldb/no_aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    22245 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/commands.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.815653 pyinsteon-1.5.3/pyinsteon/config/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5540 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/config/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1130 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/config/derived_property.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3686 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/config/device_flag.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      603 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/config/extended_property.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1813 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/config/load_button.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      418 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/config/modem_config.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2150 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/config/momentary_delay.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1794 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/config/op_flag_property.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3502 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/config/op_flag_property_byte.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/config/operating_flag.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5374 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/config/radio_button.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1692 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/config/ramp_rate.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3635 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/config/relay_mode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3493 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/config/toggle_button.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10950 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/constants.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.815653 pyinsteon-1.5.3/pyinsteon/data_types/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       32 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/data_types/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5126 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/data_types/all_link_record_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4242 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/data_types/im_config_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3663 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/data_types/io_sensor_config_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8465 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/data_types/message_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5551 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/data_types/user_data.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      226 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/default_link.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.815653 pyinsteon-1.5.3/pyinsteon/device_types/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1283 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/access_control.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6666 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/battery_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20054 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/climate_control.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10924 2023-12-11 23:18:04.000000 pyinsteon-1.5.3/pyinsteon/device_types/device_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1216 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/device_types/device_commands.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    53500 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/device_types/dimmable_lighting_control.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2469 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/energy_management.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4964 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/general_controller.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      486 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/hub.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23861 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/device_types/i3_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    41968 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/device_types/ipdb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      517 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/mock_modem.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8007 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/modem_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5226 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/on_off_controller_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4225 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/on_off_responder_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5172 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/open_close_controller_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4092 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/open_close_responder_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      646 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/plm.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26941 2023-12-11 23:18:04.000000 pyinsteon-1.5.3/pyinsteon/device_types/security_health_safety.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14495 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/sensors_actuators.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26255 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/device_types/switched_lighting_control.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      137 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/unknown_device.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4446 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/variable_controller_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4143 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/variable_responder_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2294 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/window_coverings.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7184 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/device_types/x10.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4838 2023-12-11 23:18:04.000000 pyinsteon-1.5.3/pyinsteon/device_types/x10_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3364 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/events.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.815653 pyinsteon-1.5.3/pyinsteon/groups/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1450 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/groups/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      921 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/groups/fan.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2240 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/groups/group_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1429 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/groups/on_level.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1438 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/groups/on_off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1146 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/groups/open_close.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4513 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/groups/thermostat.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      935 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/groups/wet_dry.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.815653 pyinsteon-1.5.3/pyinsteon/handlers/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4317 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/all_link_cleanup_failure_report.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      756 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/all_link_cleanup_status_report.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      998 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/all_link_completed.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1740 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/all_link_record_response.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      735 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/cancel_all_linking.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.815653 pyinsteon-1.5.3/pyinsteon/handlers/from_device/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      293 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      551 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/all_link_cleanup_command.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      901 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/assign_to_all_link_group.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1948 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/broadcast_command.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      911 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/delete_from_all_link_group.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1702 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/ext_get_response.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      580 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/manual_change.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      542 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      660 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/off_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      560 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/off_fast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      689 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/off_fast_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      577 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/on_fast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      676 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/on_fast_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      569 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/on_level.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      657 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/on_level_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2174 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/receive_aldb_record.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      850 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/thermostat_cool_set_point.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      846 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/thermostat_heat_set_point.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      831 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/thermostat_humidity.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      928 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/thermostat_mode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      846 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/thermostat_temperature.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1692 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/from_device/x10_received.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      909 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/get_first_all_link_record.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1032 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/get_im_configuration.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      854 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/get_im_info.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      845 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/get_next_all_link_record.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1531 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/inbound_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1882 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/manage_all_link_record.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2858 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/outbound_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1188 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/read_eeprom.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1787 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/read_eeprom_response.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      948 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/send_all_link.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      427 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/send_all_link_off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/send_all_link_on.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1560 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/set_im_configuration.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      961 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/start_all_linking.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/pyinsteon/handlers/to_device/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      491 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1588 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/all_link_cleanup_command.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3741 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/direct_command.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1150 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/engine_version_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      826 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/enter_linking_mode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      705 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/enter_unlinking_mode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1711 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/extended_get.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1930 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/extended_set.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      934 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/factory_reset.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1011 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/get_operating_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      749 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/group_off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      744 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/group_on.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      562 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/id_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      761 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/night_mode_off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      754 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/night_mode_on.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      733 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      634 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/off_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      746 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/off_fast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      802 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/on_fast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      881 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/on_level.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      704 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/on_level_all_link_cleanup.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/peek.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      532 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/ping.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      694 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/poke.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1046 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/product_data_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1382 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/read_aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1249 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/set_leds.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      771 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/set_msb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1638 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/set_operating_flags.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1966 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/status_request.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1392 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/temperature_down.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1384 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/temperature_up.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1701 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/thermostat_cool_set_point.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1710 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/thermostat_heat_set_point.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1609 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/thermostat_mode.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1311 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/trigger_scene_off.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1412 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/trigger_scene_on.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1338 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/write_aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2069 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/to_device/x10_send.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2172 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/handlers/write_eeprom.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      457 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/listener_exception_handler.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/pyinsteon/managers/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      187 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9814 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/aldb_im_read_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5038 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/aldb_im_write_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11273 2023-12-11 23:18:04.000000 pyinsteon-1.5.3/pyinsteon/managers/aldb_read_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3426 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/aldb_write_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10515 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/device_id_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10560 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/managers/device_link_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14859 2023-12-11 23:18:04.000000 pyinsteon-1.5.3/pyinsteon/managers/device_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2465 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/ext_get_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1367 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/ext_prop_read_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1967 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/ext_prop_write_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7401 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/managers/get_set_ext_property_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6907 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/managers/get_set_op_flag_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3447 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/heartbeat_manager.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/pyinsteon/managers/link_manager/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7992 2023-12-11 23:18:04.000000 pyinsteon-1.5.3/pyinsteon/managers/link_manager/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1503 2023-12-11 23:18:04.000000 pyinsteon-1.5.3/pyinsteon/managers/link_manager/default_links.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2704 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/low_batter_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7170 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/managers/on_level_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5027 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/peek_poke_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12017 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/saved_devices_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11025 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/scene_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7302 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/thermostat_status_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1086 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2008 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/wet_dry_manager.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4954 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/managers/x10_manager.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/pyinsteon/protocol/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3137 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    32025 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/protocol/command_to_msg.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6120 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/http_reader_writer.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8549 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/http_transport.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      111 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/hub_connection_exception.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/pyinsteon/protocol/messages/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1896 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/messages/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4046 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/messages/inbound.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1367 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/messages/message_definition.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14193 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/messages/message_definitions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    11565 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/messages/outbound.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/pyinsteon/protocol/mock/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/mock/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1925 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/mock/mock_reader.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8033 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/mock/mock_transport.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15192 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/msg_to_topic.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      838 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/msg_to_url.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9176 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/protocol.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2074 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/serial_transport.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      811 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/protocol/topic_converters.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       83 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/run_tool.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1217 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/subscriber_base.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/pyinsteon/tools/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18580 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/tools/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24420 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/tools/advanced.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10429 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/tools/aldb.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    10133 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/tools/commands.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17469 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/tools/config.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1873 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/tools/log_filter.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7748 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/tools/scenes.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    49447 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/tools/tools_base.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3246 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/tools/utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6012 2023-11-30 13:36:46.000000 pyinsteon-1.5.3/pyinsteon/topics.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    12422 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/utils.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4753 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/pyinsteon/x10_address.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/pyinsteon.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2652 2023-12-11 23:19:17.000000 pyinsteon-1.5.3/pyinsteon.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8831 2023-12-11 23:19:17.000000 pyinsteon-1.5.3/pyinsteon.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-12-11 23:19:17.000000 pyinsteon-1.5.3/pyinsteon.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       56 2023-12-11 23:19:17.000000 pyinsteon-1.5.3/pyinsteon.egg-info/entry_points.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-12-11 23:19:17.000000 pyinsteon-1.5.3/pyinsteon.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       68 2023-12-11 23:19:17.000000 pyinsteon-1.5.3/pyinsteon.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-12-11 23:19:17.000000 pyinsteon-1.5.3/pyinsteon.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6578 2023-12-11 23:18:04.000000 pyinsteon-1.5.3/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-12-11 23:19:17.825653 pyinsteon-1.5.3/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1473 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/tests/test_address.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      184 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/tests/test_nothing.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2364 2023-08-29 13:18:44.000000 pyinsteon-1.5.3/tests/test_x10_address.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.395855 pyinsteon-1.6.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1548 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/DESCRIPTION.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1067 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/LICENSE.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       53 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2654 2024-05-10 12:54:50.391855 pyinsteon-1.6.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2146 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/README.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.359855 pyinsteon-1.6.0/pyinsteon/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3731 2023-11-16 20:51:16.000000 pyinsteon-1.6.0/pyinsteon/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      126 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/__main__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2917 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/address.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.363855 pyinsteon-1.6.0/pyinsteon/aldb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      183 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/aldb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5205 2023-11-16 20:51:16.000000 pyinsteon-1.6.0/pyinsteon/aldb/aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19535 2023-11-16 20:51:16.000000 pyinsteon-1.6.0/pyinsteon/aldb/aldb_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1841 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/aldb/aldb_battery.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9046 2023-12-30 16:00:07.000000 pyinsteon-1.6.0/pyinsteon/aldb/aldb_record.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4042 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/aldb/mock_modem_aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3920 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/aldb/modem_aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4255 2023-12-30 16:00:07.000000 pyinsteon-1.6.0/pyinsteon/aldb/no_aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    22629 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/commands.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.363855 pyinsteon-1.6.0/pyinsteon/config/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5540 2023-09-11 05:34:24.000000 pyinsteon-1.6.0/pyinsteon/config/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1130 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/config/derived_property.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3686 2023-11-09 20:53:26.000000 pyinsteon-1.6.0/pyinsteon/config/device_flag.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      603 2023-03-20 12:21:27.000000 pyinsteon-1.6.0/pyinsteon/config/extended_property.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1813 2023-11-09 20:54:54.000000 pyinsteon-1.6.0/pyinsteon/config/load_button.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      418 2023-03-20 12:21:27.000000 pyinsteon-1.6.0/pyinsteon/config/modem_config.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2150 2023-11-09 20:54:57.000000 pyinsteon-1.6.0/pyinsteon/config/momentary_delay.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1794 2023-08-14 21:20:51.000000 pyinsteon-1.6.0/pyinsteon/config/op_flag_property.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3502 2023-08-31 04:34:07.000000 pyinsteon-1.6.0/pyinsteon/config/op_flag_property_byte.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      624 2023-03-20 12:21:27.000000 pyinsteon-1.6.0/pyinsteon/config/operating_flag.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5374 2023-11-16 20:51:16.000000 pyinsteon-1.6.0/pyinsteon/config/radio_button.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1692 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/config/ramp_rate.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3635 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/config/relay_mode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3493 2023-11-16 20:51:16.000000 pyinsteon-1.6.0/pyinsteon/config/toggle_button.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10950 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/constants.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.367854 pyinsteon-1.6.0/pyinsteon/data_types/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       32 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/data_types/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5126 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/data_types/all_link_record_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4242 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/data_types/im_config_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3663 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/data_types/io_sensor_config_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8465 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/data_types/message_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5551 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/data_types/user_data.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      226 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/default_link.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.371855 pyinsteon-1.6.0/pyinsteon/device_types/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/device_types/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1287 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/access_control.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6666 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/device_types/battery_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    19858 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/climate_control.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11142 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/device_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1132 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/device_commands.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    51005 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/dimmable_lighting_control.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1801 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/energy_management.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5015 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/general_controller.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      486 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/device_types/hub.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25149 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/i3_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    41968 2023-08-31 04:34:07.000000 pyinsteon-1.6.0/pyinsteon/device_types/ipdb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      517 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/device_types/mock_modem.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8007 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/device_types/modem_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4998 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/on_off_controller_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4400 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/on_off_responder_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4866 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/open_close_controller_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3717 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/open_close_responder_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      646 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/device_types/plm.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26958 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/security_health_safety.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12624 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/sensors_actuators.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24398 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/switched_lighting_control.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      137 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/device_types/unknown_device.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4166 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/variable_controller_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4095 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/device_types/variable_responder_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2294 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/device_types/window_coverings.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7184 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/device_types/x10.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4838 2023-12-30 16:00:07.000000 pyinsteon-1.6.0/pyinsteon/device_types/x10_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3364 2023-05-16 19:30:12.000000 pyinsteon-1.6.0/pyinsteon/events.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.371855 pyinsteon-1.6.0/pyinsteon/groups/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1450 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/groups/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1032 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/groups/fan.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2487 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/groups/group_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1540 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/groups/on_level.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1549 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/groups/on_off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1374 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/groups/open_close.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4591 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/groups/thermostat.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1046 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/groups/wet_dry.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.375855 pyinsteon-1.6.0/pyinsteon/handlers/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4317 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/all_link_cleanup_failure_report.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      756 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/all_link_cleanup_status_report.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      998 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/all_link_completed.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1740 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/all_link_record_response.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      735 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/cancel_all_linking.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.379855 pyinsteon-1.6.0/pyinsteon/handlers/from_device/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      293 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      551 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/all_link_cleanup_command.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      901 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/assign_to_all_link_group.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2343 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/broadcast_command.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      911 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/delete_from_all_link_group.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1702 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/ext_get_response.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      580 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/manual_change.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      542 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      660 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/off_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      948 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/off_at_ramp_rate.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      560 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/off_fast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      689 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/off_fast_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      944 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/on_at_ramp_rate.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      577 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/on_fast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      676 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/on_fast_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      569 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/on_level.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      657 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/on_level_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2174 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/receive_aldb_record.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      850 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/thermostat_cool_set_point.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      846 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/thermostat_heat_set_point.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      831 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/thermostat_humidity.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      928 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/thermostat_mode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      846 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/thermostat_temperature.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1692 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/from_device/x10_received.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      909 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/get_first_all_link_record.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1032 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/get_im_configuration.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      854 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/get_im_info.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      845 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/get_next_all_link_record.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1531 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/handlers/inbound_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1882 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/manage_all_link_record.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2858 2024-04-25 17:21:40.000000 pyinsteon-1.6.0/pyinsteon/handlers/outbound_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1188 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/read_eeprom.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1787 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/handlers/read_eeprom_response.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      948 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/send_all_link.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      427 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/handlers/send_all_link_off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/handlers/send_all_link_on.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1560 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/set_im_configuration.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      961 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/start_all_linking.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.383854 pyinsteon-1.6.0/pyinsteon/handlers/to_device/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      491 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1588 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/all_link_cleanup_command.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3741 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/direct_command.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1150 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/engine_version_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      826 2023-03-07 05:38:59.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/enter_linking_mode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      705 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/enter_unlinking_mode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1711 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/extended_get.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1930 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/extended_set.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      934 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/factory_reset.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1011 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/get_operating_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      749 2023-08-31 04:34:07.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/group_off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      744 2023-08-31 04:34:07.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/group_on.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      562 2023-01-23 13:39:25.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/id_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      761 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/night_mode_off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      754 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/night_mode_on.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      733 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      634 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/off_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      746 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/off_fast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      802 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/on_fast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      881 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/on_level.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      704 2023-05-17 15:22:44.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/on_level_all_link_cleanup.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      688 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/peek.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      532 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/ping.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      694 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/poke.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1046 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/product_data_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1382 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/read_aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1249 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/set_leds.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      771 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/set_msb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1638 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/set_operating_flags.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2080 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/status_request.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1392 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/temperature_down.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1384 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/temperature_up.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1701 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/thermostat_cool_set_point.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1710 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/thermostat_heat_set_point.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1609 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/thermostat_mode.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1311 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/trigger_scene_off.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1412 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/trigger_scene_on.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1338 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/write_aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2069 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/to_device/x10_send.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2172 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/handlers/write_eeprom.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      457 2024-04-26 15:51:22.000000 pyinsteon-1.6.0/pyinsteon/listener_exception_handler.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.387855 pyinsteon-1.6.0/pyinsteon/managers/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      187 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/managers/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9814 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/managers/aldb_im_read_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5038 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/managers/aldb_im_write_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11273 2023-12-30 16:00:07.000000 pyinsteon-1.6.0/pyinsteon/managers/aldb_read_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3426 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/managers/aldb_write_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10515 2023-08-31 03:11:28.000000 pyinsteon-1.6.0/pyinsteon/managers/device_id_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10560 2023-11-16 20:51:16.000000 pyinsteon-1.6.0/pyinsteon/managers/device_link_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14859 2023-12-30 16:00:07.000000 pyinsteon-1.6.0/pyinsteon/managers/device_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2465 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/managers/ext_get_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1367 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/managers/ext_prop_read_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1967 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/managers/ext_prop_write_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7401 2023-08-31 04:34:07.000000 pyinsteon-1.6.0/pyinsteon/managers/get_set_ext_property_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6907 2023-08-31 04:34:07.000000 pyinsteon-1.6.0/pyinsteon/managers/get_set_op_flag_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3447 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/managers/heartbeat_manager.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.387855 pyinsteon-1.6.0/pyinsteon/managers/link_manager/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8898 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/managers/link_manager/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1503 2024-05-02 14:05:49.000000 pyinsteon-1.6.0/pyinsteon/managers/link_manager/default_links.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2704 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/managers/low_batter_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7170 2023-08-31 04:34:07.000000 pyinsteon-1.6.0/pyinsteon/managers/on_level_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5027 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/managers/peek_poke_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12017 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/managers/saved_devices_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11025 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/managers/scene_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3781 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/managers/status_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7315 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/managers/thermostat_status_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1086 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/managers/utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2008 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/managers/wet_dry_manager.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4954 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/managers/x10_manager.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.391855 pyinsteon-1.6.0/pyinsteon/protocol/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3137 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/protocol/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    32025 2023-08-31 04:34:07.000000 pyinsteon-1.6.0/pyinsteon/protocol/command_to_msg.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6120 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/protocol/http_reader_writer.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8549 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/protocol/http_transport.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      111 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/protocol/hub_connection_exception.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.391855 pyinsteon-1.6.0/pyinsteon/protocol/messages/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1896 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/protocol/messages/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4046 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/protocol/messages/inbound.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1367 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/protocol/messages/message_definition.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    14193 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/protocol/messages/message_definitions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    11565 2023-08-14 21:21:43.000000 pyinsteon-1.6.0/pyinsteon/protocol/messages/outbound.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.391855 pyinsteon-1.6.0/pyinsteon/protocol/mock/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/protocol/mock/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1925 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/protocol/mock/mock_reader.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8033 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/protocol/mock/mock_transport.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15192 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/protocol/msg_to_topic.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      838 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/protocol/msg_to_url.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9565 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/protocol/protocol.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2074 2023-02-02 01:25:31.000000 pyinsteon-1.6.0/pyinsteon/protocol/serial_transport.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      811 2023-05-31 15:51:29.000000 pyinsteon-1.6.0/pyinsteon/protocol/topic_converters.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       83 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/run_tool.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1217 2023-08-14 21:20:41.000000 pyinsteon-1.6.0/pyinsteon/subscriber_base.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.391855 pyinsteon-1.6.0/pyinsteon/tools/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    18580 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/tools/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24420 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/tools/advanced.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10429 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/tools/aldb.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10133 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/tools/commands.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17469 2023-08-31 04:34:07.000000 pyinsteon-1.6.0/pyinsteon/tools/config.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1873 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/tools/log_filter.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7748 2023-07-25 18:02:20.000000 pyinsteon-1.6.0/pyinsteon/tools/scenes.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    49447 2023-11-16 20:51:16.000000 pyinsteon-1.6.0/pyinsteon/tools/tools_base.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3246 2023-11-10 19:24:40.000000 pyinsteon-1.6.0/pyinsteon/tools/utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6119 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/topics.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    12660 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyinsteon/utils.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4753 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/pyinsteon/x10_address.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.391855 pyinsteon-1.6.0/pyinsteon.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2654 2024-05-10 12:54:50.000000 pyinsteon-1.6.0/pyinsteon.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8969 2024-05-10 12:54:50.000000 pyinsteon-1.6.0/pyinsteon.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-10 12:54:50.000000 pyinsteon-1.6.0/pyinsteon.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       56 2024-05-10 12:54:50.000000 pyinsteon-1.6.0/pyinsteon.egg-info/entry_points.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-10 12:54:50.000000 pyinsteon-1.6.0/pyinsteon.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       68 2024-05-10 12:54:50.000000 pyinsteon-1.6.0/pyinsteon.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2024-05-10 12:54:50.000000 pyinsteon-1.6.0/pyinsteon.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6677 2024-05-10 12:14:39.000000 pyinsteon-1.6.0/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-05-10 12:54:50.395855 pyinsteon-1.6.0/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-10 12:54:50.391855 pyinsteon-1.6.0/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1473 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/tests/test_address.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      184 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/tests/test_nothing.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2364 2022-08-05 17:55:10.000000 pyinsteon-1.6.0/tests/test_x10_address.py
```

### Comparing `pyinsteon-1.5.3/DESCRIPTION.rst` & `pyinsteon-1.6.0/DESCRIPTION.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 platform for the `Home Assistant <https://home-assistant.io/>`__
 automation platform but it is structured to be general-purpose and
 should be usable for other applications as well.
 
 Requirements
 ------------
 
--  Python 3.8, 3.9, 3.10 or 3.11
+-  Python 3.9, 3.10 or 3.11, 3.12
 -  Posix or Windows based system
 -  Some form of Insteon PLM or Hub
 -  At least one Insteon device
 
 Installation
 ------------
```

### Comparing `pyinsteon-1.5.3/LICENSE.rst` & `pyinsteon-1.6.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/PKG-INFO` & `pyinsteon-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pyinsteon
-Version: 1.5.3
+Version: 1.6.0
 Summary: Open-source Insteon home automation module running on Python 3.
 Author-email: The pyinsteon authors <pyinsteon@harrisnj.net>
 License: MIT License
 Project-URL: Source Code, https://github.com/pyinsteon/pyinsteon
 Project-URL: Bug Reports, https://github.com/pyinsteon/pyinsteon/issues
 Keywords: home,automation,insteon,python,python3
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.8.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: pyserial
 Requires-Dist: pyserial-asyncio>=0.5
 Requires-Dist: aiohttp
 Requires-Dist: pypubsub
 Requires-Dist: aiofiles
@@ -42,15 +42,15 @@
 platform for the `Home Assistant <https://home-assistant.io/>`__
 automation platform but it is structured to be general-purpose and
 should be usable for other applications as well.
 
 Requirements
 ------------
 
--  Python 3.8, 3.9, 3.10 or 3.11
+-  Python 3.9, 3.10 or 3.11, 3.12
 -  Posix or Windows based system
 -  Some form of Insteon PLM or Hub
 -  At least one Insteon device
 
 Installation
 ------------
```

### Comparing `pyinsteon-1.5.3/README.rst` & `pyinsteon-1.6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 platform for the `Home Assistant <https://home-assistant.io/>`__
 automation platform but it is structured to be general-purpose and
 should be usable for other applications as well.
 
 Requirements
 ------------
 
--  Python 3.8 3.9, 3.10 or 3.11
+-  Python 3.9, 3.10, 3.11 or 3.12
 -  Posix or Windows based system
 -  Some form of Insteon PLM or Hub
 -  At least one Insteon device
 
 Installation
 ------------
```

### Comparing `pyinsteon-1.5.3/pyinsteon/__init__.py` & `pyinsteon-1.6.0/pyinsteon/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/address.py` & `pyinsteon-1.6.0/pyinsteon/address.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/aldb/aldb.py` & `pyinsteon-1.6.0/pyinsteon/aldb/aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/aldb/aldb_base.py` & `pyinsteon-1.6.0/pyinsteon/aldb/aldb_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/aldb/aldb_battery.py` & `pyinsteon-1.6.0/pyinsteon/aldb/aldb_battery.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/aldb/aldb_record.py` & `pyinsteon-1.6.0/pyinsteon/aldb/aldb_record.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/aldb/mock_modem_aldb.py` & `pyinsteon-1.6.0/pyinsteon/aldb/mock_modem_aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/aldb/modem_aldb.py` & `pyinsteon-1.6.0/pyinsteon/aldb/modem_aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/aldb/no_aldb.py` & `pyinsteon-1.6.0/pyinsteon/aldb/no_aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/commands.py` & `pyinsteon-1.6.0/pyinsteon/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Collection of topics mapped to commands (cmd1, cmd2)."""
+
 from collections import namedtuple
 import logging
 from typing import Tuple
 
 from .topics import (
     ALL_LINK_CLEANUP_STATUS_REPORT,
     ASSIGN_TO_ALL_LINK_GROUP,
@@ -44,17 +45,19 @@
     LEAK_DETECTOR_ANNOUNCE,
     MANUALLY_TURNED_OFF,
     MANUALLY_TURNED_ON,
     NIGHT_MODE_OFF,
     NIGHT_MODE_ON,
     OFF,
     OFF_AT_RAMP_RATE,
+    OFF_AT_RAMP_RATE_INBOUND,
     OFF_FAST,
     ON,
     ON_AT_RAMP_RATE,
+    ON_AT_RAMP_RATE_INBOUND,
     ON_FAST,
     PEEK,
     PEEK_INTERNAL,
     PING,
     POKE,
     POKE_INTERNAL,
     POOL_CONTROL,
@@ -195,15 +198,15 @@
         """Get a list of topics from a cmd1 value."""
         return self._commands_topic_map.get(cmd1)
 
     def use_group(self, topic):
         """Return if a topic requires a group number."""
         return self._use_group.get(topic)
 
-    def get_topics(self, cmd1, cmd2, flags, userdata=None, send=False) -> str:
+    def get_topics(self, cmd1, cmd2, flags, userdata=None, send=False):
         """Generate a topic from a cmd1, cmd2 and extended flag."""
         found = False
         for topic in self._commands_topic_map.get(cmd1, {}):
             command = self._topics[topic]
             if _check_match(command, cmd1, cmd2, userdata):
                 found = True
                 yield topic
@@ -677,14 +680,32 @@
     cmd2=0x00,
     ud_allowed=True,
     ud_required=False,
     userdata=None,
     use_group=False,
 )
 commands.add(
+    topic=ON_AT_RAMP_RATE_INBOUND,
+    cmd1=0x34,
+    cmd2=None,
+    ud_allowed=False,
+    ud_required=False,
+    userdata=None,
+    use_group=True,
+)
+commands.add(
+    topic=OFF_AT_RAMP_RATE_INBOUND,
+    cmd1=0x35,
+    cmd2=None,
+    ud_allowed=False,
+    ud_required=False,
+    userdata=None,
+    use_group=True,
+)
+commands.add(
     topic=NIGHT_MODE_ON,
     cmd1=0x3B,
     cmd2=None,
     ud_allowed=False,
     ud_required=False,
     userdata=None,
     use_group=False,
```

### Comparing `pyinsteon-1.5.3/pyinsteon/config/__init__.py` & `pyinsteon-1.6.0/pyinsteon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/derived_property.py` & `pyinsteon-1.6.0/pyinsteon/config/derived_property.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/device_flag.py` & `pyinsteon-1.6.0/pyinsteon/config/device_flag.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/extended_property.py` & `pyinsteon-1.6.0/pyinsteon/config/extended_property.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/load_button.py` & `pyinsteon-1.6.0/pyinsteon/config/load_button.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/momentary_delay.py` & `pyinsteon-1.6.0/pyinsteon/config/momentary_delay.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/op_flag_property.py` & `pyinsteon-1.6.0/pyinsteon/config/op_flag_property.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/op_flag_property_byte.py` & `pyinsteon-1.6.0/pyinsteon/config/op_flag_property_byte.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/operating_flag.py` & `pyinsteon-1.6.0/pyinsteon/config/operating_flag.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/radio_button.py` & `pyinsteon-1.6.0/pyinsteon/config/radio_button.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/ramp_rate.py` & `pyinsteon-1.6.0/pyinsteon/config/ramp_rate.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/relay_mode.py` & `pyinsteon-1.6.0/pyinsteon/config/relay_mode.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/config/toggle_button.py` & `pyinsteon-1.6.0/pyinsteon/config/toggle_button.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/constants.py` & `pyinsteon-1.6.0/pyinsteon/constants.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/data_types/all_link_record_flags.py` & `pyinsteon-1.6.0/pyinsteon/data_types/all_link_record_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/data_types/im_config_flags.py` & `pyinsteon-1.6.0/pyinsteon/data_types/im_config_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/data_types/io_sensor_config_flags.py` & `pyinsteon-1.6.0/pyinsteon/data_types/io_sensor_config_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/data_types/message_flags.py` & `pyinsteon-1.6.0/pyinsteon/data_types/message_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/data_types/user_data.py` & `pyinsteon-1.6.0/pyinsteon/data_types/user_data.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/access_control.py` & `pyinsteon-1.6.0/pyinsteon/device_types/access_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Access control device types."""
 
-
 from ..events import OFF_EVENT, OFF_FAST_EVENT, ON_EVENT, ON_FAST_EVENT
 from ..groups import ON_OFF_SWITCH
 from .on_off_responder_base import OnOffResponderBase
 
 
 class AccessControl_Morningstar(OnOffResponderBase):
     """Access Control MorningStar device."""
@@ -21,15 +20,15 @@
         state_name=ON_OFF_SWITCH,
         on_event_name=ON_EVENT,
         off_event_name=OFF_EVENT,
         on_fast_event_name=ON_FAST_EVENT,
         off_fast_event_name=OFF_FAST_EVENT,
     ):
         """Init the OnOffResponderBase class."""
-        buttons = {1: ON_OFF_SWITCH} if buttons is None else buttons
+        buttons = {1: (ON_OFF_SWITCH, 0)} if buttons is None else buttons
         super().__init__(
             address,
             cat,
             subcat,
             firmware,
             description,
             model,
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/battery_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/battery_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/climate_control.py` & `pyinsteon-1.6.0/pyinsteon/device_types/climate_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Thermostat device types."""
+
 from datetime import datetime
 import logging
 
 from ..aldb.aldb import ALDB
 from ..aldb.aldb_battery import ALDBBattery
 from ..config import (
     BACKLIGHT,
@@ -88,19 +89,14 @@
             subcat=subcat,
             firmware=firmware,
             description=description,
             model=model,
         )
         self._aldb = ALDB(self._address, mem_addr=0x1FFF)
 
-    # pylint: disable=arguments-differ
-    async def async_status(self, group=None):
-        """Get the status of the device."""
-        return await self._managers[STATUS_COMMAND].async_status()
-
     async def async_set_cool_set_point(self, temperature):
         """Set the cool set point."""
         temperature = max(1, min(temperature, 127))
         return await self._handlers["cool_set_point_command"].async_send(temperature)
 
     async def async_set_heat_set_point(self, temperature):
         """Set the cool set point."""
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/device_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/device_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 
 from ..address import Address
 from ..aldb.aldb import ALDB
 from ..config.extended_property import ExtendedProperty
 from ..config.operating_flag import OperatingFlag
 from ..constants import DeviceCategory, EngineVersion, PropertyType, ResponseStatus
 from ..default_link import DefaultLink
+from ..device_types.device_commands import STATUS_COMMAND
 from ..handlers.to_device.engine_version_request import EngineVersionRequest
 from ..handlers.to_device.ping import PingCommand
 from ..handlers.to_device.product_data_request import ProductDataRequestCommand
 from ..managers.get_set_ext_property_manager import GetSetExtendedPropertyManager
 from ..managers.get_set_op_flag_manager import GetSetOperatingFlagsManager
 from ..managers.link_manager.default_links import async_add_default_links
+from ..managers.status_manager import StatusManager
 from ..topics import ENGINE_VERSION
 from ..utils import multiple_status, publish_topic
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Device(ABC):
@@ -172,14 +174,15 @@
         self._engine_version = version
         publish_topic(
             f"{self._address.id}.{ENGINE_VERSION}", version=self._engine_version
         )
 
     async def async_status(self, group=None):
         """Get the status of the device."""
+        return ResponseStatus.SUCCESS
 
     async def async_read_config(self, read_aldb: bool = True):
         """Get all configuration settings.
 
         This includes:
         - Engine Version
         - Operating flags
@@ -239,14 +242,15 @@
     def _register_groups(self):
         """Add the groups to the device."""
 
     def _register_handlers_and_managers(self):
         """Add all handlers to the device and register listeners."""
         self._handlers["product_data_cmd"] = ProductDataRequestCommand(self._address)
         self._handlers["engine_version_cmd"] = EngineVersionRequest(self._address)
+        self._managers[STATUS_COMMAND] = StatusManager(self._address)
 
     def _subscribe_to_handelers_and_managers(self):
         """Subscribe groups and events to handlers and managers."""
         self._handlers["product_data_cmd"] = ProductDataRequestCommand(self._address)
         self._handlers["engine_version_cmd"].subscribe(self._engine_version_received)
 
     def _register_default_links(self):
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/device_commands.py` & `pyinsteon-1.6.0/pyinsteon/device_types/device_commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,31 +9,29 @@
 OPEN_INBOUND = "open_inbound"
 CLOSE_INBOUND = "close_inbound"
 
 ON_HEARTBEAT_INBOUND = "on_heartbeat_inbound"
 OFF_HEARTBEAT_INBOUND = "off_heartbeat_inbound"
 
 STATUS_COMMAND = "status_command"
-STATUS_COMMAND_HUB = "status_command_hub"
-STATUS_COMMAND_FAN = "status_command_fan"
-STATUS_COMMAND_LOAD = "status_command_load"
 
 ON_COMMAND = "on_command"
 OFF_COMMAND = "off_command"
 ON_FAST_COMMAND = "on_fast_command"
 OFF_FAST_COMMAND = "off_fast_command"
 
 GET_OPERATING_FLAGS_COMMAND = "get_operating_flags"
 SET_OPERATING_FLAGS_COMMAND = "set_operating_flags"
 EXTENDED_GET_COMMAND = "extended_get"
 EXTENDED_SET_COMMAND = "extended_set"
 EXTENDED_GET_RESPONSE = "extended_get_response"
 
 SET_LEDS_COMMAND = "set_leds"
-GET_LEDS_COMMAND = "get_leds"
 TRIGGER_SCENE_ON_COMMAND = "trigger_scene_on"
 TRIGGER_SCENE_OFF_COMMAND = "trigger_scene_off"
 
 GET_IM_CONFIG_COMMAND = "get_im_config"
 SET_IM_CONFIG_COMMAND = "set_im_config"
 
 MANUAL_CHANGE = "manual_change"
+ON_AT_RAMP_RATE = "on_at_ramp_rate"
+OFF_AT_RAMP_RATE = "off_at_ramp_rate"
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/dimmable_lighting_control.py` & `pyinsteon-1.6.0/pyinsteon/device_types/dimmable_lighting_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Dimmable Lighting Control Devices (CATEGORY 0x01)."""
+
 import asyncio
 from collections.abc import Iterable
 from functools import partial
 from typing import Dict, Union
 
 from ..config import (
     CLEANUP_REPORT_ON,
@@ -64,61 +65,56 @@
     ON_OFF_SWITCH_G,
     ON_OFF_SWITCH_H,
 )
 from ..groups.on_level import OnLevel
 from ..groups.on_off import OnOff
 from ..handlers.from_device.manual_change import ManualChangeInbound
 from ..handlers.to_device.group_off import GroupOffCommand
-from ..handlers.to_device.group_on import GroupOnCommand
 from ..handlers.to_device.set_leds import SetLedsCommandHandler
-from ..handlers.to_device.status_request import StatusRequestCommand
 from ..handlers.to_device.trigger_scene_off import TriggerSceneOffCommandHandler
 from ..handlers.to_device.trigger_scene_on import TriggerSceneOnCommandHandler
 from ..utils import bit_is_set, multiple_status, set_bit, set_fan_speed
 from .device_commands import (
-    GET_LEDS_COMMAND,
     MANUAL_CHANGE,
     OFF_COMMAND,
     OFF_FAST_COMMAND,
     ON_COMMAND,
     ON_FAST_COMMAND,
     SET_LEDS_COMMAND,
     STATUS_COMMAND,
-    STATUS_COMMAND_FAN,
 )
 from .i3_base import I3VariableResponderBase
 from .variable_controller_base import ON_LEVEL_MANAGER
 from .variable_responder_base import VariableResponderBase
 
 
 class DimmableLightingControl(VariableResponderBase):
     """Dimmable Lighting Control Device."""
 
     def _register_handlers_and_managers(self):
         """Register command handlers and managers."""
         super()._register_handlers_and_managers()
-        self._handlers[STATUS_COMMAND] = StatusRequestCommand(
-            self._address, status_type=2
-        )
         for group, group_prop in self._groups.items():
             if isinstance(group_prop, OnLevel):
                 self._handlers[group][MANUAL_CHANGE] = ManualChangeInbound(
                     self._address, group
                 )
 
     def _subscribe_to_handelers_and_managers(self):
         """Subscribe methods to handlers and managers."""
         super()._subscribe_to_handelers_and_managers()
+        self._managers[STATUS_COMMAND].remove_status_type(0)
+        self._managers[STATUS_COMMAND].add_status_type(2, self._handle_status)
         for group, group_prop in self._groups.items():
             if isinstance(group_prop, OnLevel):
                 self._handlers[group][MANUAL_CHANGE].subscribe(
                     self._async_on_manual_change
                 )
 
-    async def _async_on_manual_change(self):
+    async def _async_on_manual_change(self, group=None):
         """Respond to a manual change of the device."""
         await self.async_status()
 
 
 class DimmableLightingControl_LampLinc(DimmableLightingControl):
     """LampLinc based dimmable lights."""
 
@@ -215,15 +211,15 @@
 
 
 class DimmableLightingControl_OutletLinc(DimmableLightingControl):
     """OutletLinc based dimmable lights."""
 
     def __init__(self, address, cat, subcat, firmware=0, description="", model=""):
         """Init the DimmableLightingControl_OutletLinc class."""
-        buttons = {1: DIMMABLE_OUTLET}
+        buttons = {1: (DIMMABLE_OUTLET, 0)}
         super().__init__(
             address,
             cat,
             subcat,
             firmware=firmware,
             description=description,
             model=model,
@@ -269,15 +265,15 @@
 
     Device Class 0x01 subcat 0x2e
 
     """
 
     def __init__(self, address, cat, subcat, firmware=0, description="", model=""):
         """Init the DimmableLightingControl_FanLinc class."""
-        buttons = {1: DIMMABLE_LIGHT, 2: DIMMABLE_FAN}
+        buttons = {1: (DIMMABLE_LIGHT, 0), 2: (DIMMABLE_FAN, 3)}
         super().__init__(
             address,
             cat,
             subcat,
             firmware=firmware,
             description=description,
             model=model,
@@ -342,50 +338,17 @@
             UNCLEAR: Device received the message but did not confirm the action
 
         """
         group = 2
         command = OFF_FAST_COMMAND if fast else OFF_COMMAND
         return await self._handlers[group][command].async_send()
 
-    async def async_status(self):
-        """Request the status fo the light and the fan."""
-        light_status = await super().async_status()
-        fan_status = await self.async_fan_status()
-        if light_status == fan_status == ResponseStatus.SUCCESS:
-            return ResponseStatus.SUCCESS
-        if ResponseStatus.DIRECT_NAK_PRE_NAK in (light_status, fan_status):
-            return ResponseStatus.DIRECT_NAK_PRE_NAK
-        return ResponseStatus.FAILURE
-
-    async def async_light_status(self):
-        """Request the status of the light."""
-        return await super().async_status()
-
-    def fan_status(self):
-        """Request the status of the fan."""
-        self._handlers[STATUS_COMMAND_FAN].send()
-
-    async def async_fan_status(self):
-        """Request the status of the fan.
-
-        Returns a ResponseStatus value
-            FAILURE: Device did not acknowledge the message
-            SUCCESS: Device acknowledged the message
-            UNCLEAR: Device received the message but did not confirm the action
-
-        """
-        return await self._handlers[STATUS_COMMAND_FAN].async_send()
-
-    def _register_handlers_and_managers(self):
-        super()._register_handlers_and_managers()
-        self._handlers[STATUS_COMMAND_FAN] = StatusRequestCommand(self._address, 3)
-
     def _subscribe_to_handelers_and_managers(self):
         super()._subscribe_to_handelers_and_managers()
-        self._handlers[STATUS_COMMAND_FAN].subscribe(self._handle_fan_status)
+        self._managers[STATUS_COMMAND].add_status_type(3, self._handle_fan_status)
 
     def _register_op_flags_and_props(self):
         super()._register_op_flags_and_props()
 
         self._add_operating_flag(PROGRAM_LOCK_ON, 0, 0, 0, 1)
         self._add_operating_flag(LED_BLINK_ON_TX_ON, 0, 1, 2, 3)
         self._add_operating_flag(RESUME_DIM_ON, 0, 2, 4, 5)
@@ -475,25 +438,14 @@
         return await cmd.async_send(on_level, fast)
 
     async def async_trigger_scene_off(self, group: int, fast: bool = False):
         """Trigger an All-Link group off."""
         cmd = TriggerSceneOffCommandHandler(self._address, group)
         return await cmd.async_send(fast)
 
-    async def async_status(self):
-        """Check the status of the device."""
-        retries = 5
-        status = ResponseStatus.UNSENT
-        while retries and status != ResponseStatus.SUCCESS:
-            status0 = await super().async_status()
-            status1 = await self._handlers[GET_LEDS_COMMAND].async_send()
-            status = multiple_status(status0, status1)
-            retries -= 1
-        return status
-
     def set_radio_buttons(self, buttons: Iterable):
         """Set a group of buttons to act as radio buttons.
 
         This takes in a iterable set of buttons (eg. (3,4,5,6)) to act as radio buttons where
         no two buttons are on at the same time.
         """
         if len(buttons) < 2:
@@ -632,33 +584,37 @@
         else:
             toggle_mask.new_value = set_bit(toggle_mask_test, button - 1, True)
             on_off_mask.new_value = set_bit(on_off_mask_test, button - 1, False)
 
     def _register_handlers_and_managers(self):
         super()._register_handlers_and_managers()
         self._handlers[SET_LEDS_COMMAND] = SetLedsCommandHandler(address=self.address)
-        self._handlers[GET_LEDS_COMMAND] = StatusRequestCommand(
-            self._address, status_type=1
-        )
 
     def _register_groups(self):
         for button in self._buttons:
-            name = self._buttons[button]
+            name = self._buttons[button][0]
+            status_type = self._buttons[button][1]
             if button == 1:
                 self._groups[button] = OnLevel(
-                    name=name, address=self._address, group=button
+                    name=name,
+                    address=self._address,
+                    group=button,
+                    status_type=status_type,
                 )
             else:
                 self._groups[button] = OnOff(
-                    name=name, address=self._address, group=button
+                    name=name,
+                    address=self._address,
+                    group=button,
+                    status_type=status_type,
                 )
 
     def _subscribe_to_handelers_and_managers(self):
         super()._subscribe_to_handelers_and_managers()
-        self._handlers[GET_LEDS_COMMAND].subscribe(self._led_status)
+        self._managers[STATUS_COMMAND].add_status_type(1, self._led_status)
         for group in self._buttons:
             if group != 1:
                 led_method = partial(self._async_led_follow_check, group=group)
                 self._managers[group][ON_LEVEL_MANAGER].subscribe(led_method)
 
     def _async_led_follow_check(self, group, on_level):
         """Check the other LEDs to confirm if they follow the effected LED."""
@@ -786,19 +742,19 @@
 
 class DimmableLightingControl_KeypadLinc_6(DimmableLightingControl_KeypadLinc):
     """KeypadLinc 6 button dimmer."""
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the DimmableLightingControl_KeypadLinc_6 class."""
         buttons = {
-            1: DIMMABLE_LIGHT_MAIN,
-            3: ON_OFF_SWITCH_A,
-            4: ON_OFF_SWITCH_B,
-            5: ON_OFF_SWITCH_C,
-            6: ON_OFF_SWITCH_D,
+            1: (DIMMABLE_LIGHT_MAIN, 0),
+            3: (ON_OFF_SWITCH_A, 1),
+            4: (ON_OFF_SWITCH_B, 1),
+            5: (ON_OFF_SWITCH_C, 1),
+            6: (ON_OFF_SWITCH_D, 1),
         }
         super().__init__(
             address=address,
             cat=cat,
             subcat=subcat,
             firmware=firmware,
             description=description,
@@ -809,22 +765,22 @@
 
 class DimmableLightingControl_KeypadLinc_8(DimmableLightingControl_KeypadLinc):
     """KeypadLinc 8 button dimmer."""
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the DimmableLightingControl_KeypadLinc_6 class."""
         buttons = {
-            1: DIMMABLE_LIGHT_MAIN,
-            2: ON_OFF_SWITCH_B,
-            3: ON_OFF_SWITCH_C,
-            4: ON_OFF_SWITCH_D,
-            5: ON_OFF_SWITCH_E,
-            6: ON_OFF_SWITCH_F,
-            7: ON_OFF_SWITCH_G,
-            8: ON_OFF_SWITCH_H,
+            1: (DIMMABLE_LIGHT_MAIN, 0),
+            2: (ON_OFF_SWITCH_B, 1),
+            3: (ON_OFF_SWITCH_C, 1),
+            4: (ON_OFF_SWITCH_D, 1),
+            5: (ON_OFF_SWITCH_E, 1),
+            6: (ON_OFF_SWITCH_F, 1),
+            7: (ON_OFF_SWITCH_G, 1),
+            8: (ON_OFF_SWITCH_H, 1),
         }
         super().__init__(
             address=address,
             cat=cat,
             subcat=subcat,
             firmware=firmware,
             description=description,
@@ -832,31 +788,26 @@
             buttons=buttons,
         )
 
 
 class DimmableLightingControl_Dial(I3VariableResponderBase):
     """Dimmable i3 Dial."""
 
-    def _register_handlers_and_managers(self):
-        """Register command handlers and managers."""
-        super()._register_handlers_and_managers()
-        self._handlers[STATUS_COMMAND] = StatusRequestCommand(
-            self._address, status_type=2
-        )
-
     def _subscribe_to_handelers_and_managers(self):
         """Subscribe methods to handlers and managers."""
         super()._subscribe_to_handelers_and_managers()
+        self._managers[STATUS_COMMAND].remove_status_type(0)
+        self._managers[STATUS_COMMAND].add_status_type(2, self._handle_status)
         for group, group_prop in self._groups.items():
             if isinstance(group_prop, OnLevel):
                 self._handlers[group][MANUAL_CHANGE].subscribe(
                     self._async_on_manual_change
                 )
 
-    async def _async_on_manual_change(self):
+    async def _async_on_manual_change(self, group=None):
         """Respond to a manual change of the device."""
         await self.async_status()
 
     def _register_config(self):
         """Register configuration items."""
         super()._register_config()
         self._config[RAMP_RATE_IN_SEC] = RampRateProperty(
@@ -876,18 +827,18 @@
         4: f"{NIGHT_MODE_ON}_kpl",
         5: f"{NO_CACHE}_kpl",
     }
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the DimmableLightingControl_I3_KeypadLink_4 class."""
         buttons = {
-            1: ON_OFF_SWITCH_A,
-            2: ON_OFF_SWITCH_B,
-            3: ON_OFF_SWITCH_C,
-            4: ON_OFF_SWITCH_D,
+            1: (ON_OFF_SWITCH_A, 1),
+            2: (ON_OFF_SWITCH_B, 1),
+            3: (ON_OFF_SWITCH_C, 1),
+            4: (ON_OFF_SWITCH_D, 1),
         }
         super().__init__(
             address=address,
             cat=cat,
             subcat=subcat,
             firmware=firmware,
             description=description,
@@ -903,15 +854,15 @@
         load_button = 1 if load_button in [0, None] else load_button
         return load_button
 
     async def async_on(self, on_level: int = 0xFF, group: int = 0, fast: bool = False):
         """Turn on the button LED."""
         group = self.load_button if not group else group
         led_kwargs = {}
-        event = OFF_FAST_EVENT if fast else OFF_EVENT
+        event = ON_FAST_EVENT if fast else ON_EVENT
         result_load = ResponseStatus.SUCCESS
         result_led = ResponseStatus.SUCCESS
         if group != self.load_button:
             load_new_state = self._get_led_follow_state(
                 button1=group, button2=self.load_button, new_state=on_level
             )
             if load_new_state != bool(self._groups[self.load_button].value):
@@ -974,30 +925,14 @@
         return await cmd.async_send(on_level, fast)
 
     async def async_trigger_scene_off(self, group: int, fast: bool = False):
         """Trigger an All-Link group off."""
         cmd = TriggerSceneOffCommandHandler(self._address, group)
         return await cmd.async_send(fast)
 
-    async def async_status(self):
-        """Check the status of the device."""
-        retries = 5
-        status = ResponseStatus.UNSENT
-        while retries and status != ResponseStatus.SUCCESS:
-            status0 = await super().async_status()
-            status1 = await self._handlers[GET_LEDS_COMMAND].async_send()
-            status = multiple_status(status0, status1)
-            retries -= 1
-        return status
-
-    async def async_group_on(self, group: int) -> ResponseStatus:
-        """Trigger a group on."""
-        cmd = GroupOnCommand(address=self._address)
-        return await cmd.async_send(group=group)
-
     async def async_group_off(self, group: int) -> ResponseStatus:
         """Trigger a group off."""
         cmd = GroupOffCommand(address=self._address)
         return await cmd.async_send(group=group)
 
     def set_radio_buttons(self, buttons: Iterable):
         """Set a group of buttons to act as radio buttons.
@@ -1201,25 +1136,22 @@
             self._properties[LOAD_BUTTON_NUMBER],
             list(self._groups),
         )
 
     def _register_handlers_and_managers(self):
         super()._register_handlers_and_managers()
         self._handlers[SET_LEDS_COMMAND] = SetLedsCommandHandler(address=self.address)
-        self._handlers[GET_LEDS_COMMAND] = StatusRequestCommand(
-            self._address, status_type=1
-        )
         self._add_ext_prop_write_manager(
             {3: self._operating_flags[TRIGGER_GROUP_MASK]}, 0x0C, 0x00, 0x00
         )
 
     def _subscribe_to_handelers_and_managers(self):
         # Not running super due to the LOAD_BUTTON_NUMBER config property
         super()._subscribe_to_handelers_and_managers()
-        self._handlers[GET_LEDS_COMMAND].subscribe(self._async_handle_led_status)
+        self._managers[STATUS_COMMAND].add_status_type(1, self._async_handle_led_status)
         for group in self._buttons:
             led_method = partial(self._async_led_follow_check, group=group)
             self._managers[group][ON_LEVEL_MANAGER].subscribe(
                 led_method,
             )
         self._properties[LOAD_BUTTON_NUMBER].subscribe(
             self._handle_load_button_property__changed
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/energy_management.py` & `pyinsteon-1.6.0/pyinsteon/device_types/energy_management.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Energy Management Control devices (CATEGORY 0x09)."""
 
 from ..config import LOAD_SENSE_ON, PROGRAM_LOCK_ON
 from ..events import OFF_EVENT, OFF_FAST_EVENT, ON_EVENT, ON_FAST_EVENT
 from ..groups import LOAD_SENSOR, ON_OFF_SWITCH
-from ..handlers.to_device.status_request import StatusRequestCommand
-from ..utils import multiple_status
-from .device_commands import STATUS_COMMAND_LOAD
+from .device_commands import STATUS_COMMAND
 from .on_off_responder_base import OnOffResponderBase
 
 
 class EnergyManagement_LoadController(OnOffResponderBase):
     """Load Controller device."""
 
     def __init__(
@@ -24,49 +22,36 @@
         state_name=ON_OFF_SWITCH,
         on_event_name=ON_EVENT,
         off_event_name=OFF_EVENT,
         on_fast_event_name=ON_FAST_EVENT,
         off_fast_event_name=OFF_FAST_EVENT,
     ):
         """Init the EnergyManagement_LoadController class."""
-        buttons = {1: ON_OFF_SWITCH, 2: LOAD_SENSOR} if buttons is None else buttons
+        buttons = (
+            {1: (ON_OFF_SWITCH, 0), 2: (LOAD_SENSOR, 1)} if buttons is None else buttons
+        )
         super().__init__(
             address,
             cat,
             subcat,
             firmware,
             description,
             model,
             buttons,
             on_event_name,
             off_event_name,
             on_fast_event_name,
             off_fast_event_name,
         )
 
-    async def async_status(self, group=None):
-        """Request the status of the device."""
-        result1 = result2 = None
-        if group in [0, 1, None]:
-            result1 = await super().async_status()
-        if group in [2, None]:
-            result2 = await self._handlers[2][STATUS_COMMAND_LOAD].async_send()
-        return multiple_status(result1, result2)
-
     def _register_op_flags_and_props(self):
         super()._register_op_flags_and_props()
         self._add_operating_flag(PROGRAM_LOCK_ON, 0, 0, 0, 1)
         self._add_operating_flag(LOAD_SENSE_ON, 0, 5, 6, 7)
 
-    def _register_handlers_and_managers(self):
-        super()._register_handlers_and_managers()
-        self._handlers[2][STATUS_COMMAND_LOAD] = StatusRequestCommand(
-            self._address, status_type=1
-        )
-
     def _subscribe_to_handelers_and_managers(self):
         super()._subscribe_to_handelers_and_managers()
-        self._handlers[2][STATUS_COMMAND_LOAD].subscribe(self._sensor_status)
+        self._managers[STATUS_COMMAND].add_status_type(1, self._sensor_status)
 
     def _sensor_status(self, db_version, status):
         """Set the sensor status value."""
         self._groups[2].set_value(status)
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/general_controller.py` & `pyinsteon-1.6.0/pyinsteon/device_types/general_controller.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """General controller devices (cat: 0x00)."""
+
 from ..aldb.no_aldb import NoALDB
 from ..config import (
     GROUPED_ON,
     KEY_BEEP_ON,
     LED_ON,
     PROGRAM_LOCK_ON,
     SEND_ON_ONLY,
     STAY_AWAKE_ON,
 )
-from ..constants import ResponseStatus
 from ..groups import (
     ON_OFF_SWITCH_A,
     ON_OFF_SWITCH_B,
     ON_OFF_SWITCH_C,
     ON_OFF_SWITCH_D,
     ON_OFF_SWITCH_E,
     ON_OFF_SWITCH_F,
@@ -36,38 +36,38 @@
 
 class GeneralController_ControlLinc(VariableControllerBase):
     """ControLinc 2430 device."""
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the GeneralController_ControlLinc class."""
         buttons = {
-            1: ON_OFF_SWITCH_A,
-            2: ON_OFF_SWITCH_B,
-            3: ON_OFF_SWITCH_C,
-            4: ON_OFF_SWITCH_D,
-            5: ON_OFF_SWITCH_E,
-            6: ON_OFF_SWITCH_F,
+            1: (ON_OFF_SWITCH_A, None),
+            2: (ON_OFF_SWITCH_B, None),
+            3: (ON_OFF_SWITCH_C, None),
+            4: (ON_OFF_SWITCH_D, None),
+            5: (ON_OFF_SWITCH_E, None),
+            6: (ON_OFF_SWITCH_F, None),
         }
         super().__init__(
             address, cat, subcat, firmware, description, model, buttons=buttons
         )
 
 
 class GeneralController_RemoteLinc(BatteryDeviceBase, VariableControllerBase):
     """RemoteLinc 2440 device."""
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the GeneralController_RemoteLinc class."""
         buttons = {
-            1: ON_OFF_SWITCH_A,
-            2: ON_OFF_SWITCH_B,
-            3: ON_OFF_SWITCH_C,
-            4: ON_OFF_SWITCH_D,
-            5: ON_OFF_SWITCH_E,
-            6: ON_OFF_SWITCH_F,
+            1: (ON_OFF_SWITCH_A, None),
+            2: (ON_OFF_SWITCH_B, None),
+            3: (ON_OFF_SWITCH_C, None),
+            4: (ON_OFF_SWITCH_D, None),
+            5: (ON_OFF_SWITCH_E, None),
+            6: (ON_OFF_SWITCH_F, None),
         }
         super().__init__(
             address, cat, subcat, firmware, description, model, buttons=buttons
         )
 
     def _register_op_flags_and_props(self):
         super()._register_op_flags_and_props()
@@ -89,18 +89,14 @@
     ):
         """Init the GeneralController_MiniRemoteBase class."""
         super().__init__(
             address, cat, subcat, firmware, description, model, buttons=buttons
         )
         self._database_delta = 0
 
-    async def async_status(self, group=0):
-        """Return success always."""
-        return ResponseStatus.SUCCESS
-
     def _register_op_flags_and_props(self):
         super()._register_op_flags_and_props()
         self._add_operating_flag(PROGRAM_LOCK_ON, 0, 0, 0, 1)
         self._add_operating_flag(LED_ON, 0, 1, 2, 3)
         self._add_operating_flag(KEY_BEEP_ON, 0, 2, 4, 5)
         self._add_operating_flag(STAY_AWAKE_ON, 0, 3, 6, 7)
         self._add_operating_flag(SEND_ON_ONLY, 0, 4, 8, 9)
@@ -108,47 +104,47 @@
 
 
 class GeneralController_MiniRemote_Switch(GeneralController_MiniRemoteBase):
     """RemoteLinc 2440 device with a single button."""
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the GeneralController_MiniRemote_Switch class."""
-        buttons = {1: ON_OFF_SWITCH_A, 2: ON_OFF_SWITCH_B}
+        buttons = {1: (ON_OFF_SWITCH_A, None), 2: (ON_OFF_SWITCH_B, None)}
         super().__init__(
             address, cat, subcat, firmware, description, model, buttons=buttons
         )
 
 
 class GeneralController_MiniRemote_4(GeneralController_MiniRemoteBase):
     """RemoteLinc 2440 device."""
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the GeneralController_MiniRemote_4 class."""
         buttons = {
-            1: ON_OFF_SWITCH_A,
-            2: ON_OFF_SWITCH_B,
-            3: ON_OFF_SWITCH_C,
-            4: ON_OFF_SWITCH_D,
+            1: (ON_OFF_SWITCH_A, None),
+            2: (ON_OFF_SWITCH_B, None),
+            3: (ON_OFF_SWITCH_C, None),
+            4: (ON_OFF_SWITCH_D, None),
         }
         super().__init__(
             address, cat, subcat, firmware, description, model, buttons=buttons
         )
 
 
 class GeneralController_MiniRemote_8(GeneralController_MiniRemoteBase):
     """RemoteLinc 2440 device."""
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the GeneralController_MiniRemote_8 class."""
         buttons = {
-            1: ON_OFF_SWITCH_B,
-            2: ON_OFF_SWITCH_A,
-            3: ON_OFF_SWITCH_D,
-            4: ON_OFF_SWITCH_C,
-            5: ON_OFF_SWITCH_F,
-            6: ON_OFF_SWITCH_E,
-            7: ON_OFF_SWITCH_H,
-            8: ON_OFF_SWITCH_G,
+            1: (ON_OFF_SWITCH_B, None),
+            2: (ON_OFF_SWITCH_A, None),
+            3: (ON_OFF_SWITCH_D, None),
+            4: (ON_OFF_SWITCH_C, None),
+            5: (ON_OFF_SWITCH_F, None),
+            6: (ON_OFF_SWITCH_E, None),
+            7: (ON_OFF_SWITCH_H, None),
+            8: (ON_OFF_SWITCH_G, None),
         }
         super().__init__(
             address, cat, subcat, firmware, description, model, buttons=buttons
         )
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/i3_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/i3_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """I3 device base classes."""
+
 import asyncio
 from collections import namedtuple
 from typing import Dict, List, Tuple, Union
 
 from ..config import (
     ACK_A_SCENE,
     BLUE_LED_OFF,
@@ -45,21 +46,23 @@
 )
 from ..config.extended_property import ExtendedProperty
 from ..config.op_flag_property_byte import OpFlagPropertyByte
 from ..config.operating_flag import OperatingFlag
 from ..constants import PropertyType, ResponseStatus
 from ..groups.on_level import OnLevel
 from ..handlers.from_device.manual_change import ManualChangeInbound
+from ..handlers.from_device.off_at_ramp_rate import OffAtRampRateInbound
+from ..handlers.from_device.on_at_ramp_rate import OnAtRampRateInbound
 from ..handlers.to_device.factory_reset import FactoryResetCommand
 from ..handlers.to_device.night_mode_off import NightModeOffCommand
 from ..handlers.to_device.night_mode_on import NightModeOnCommand
 from ..managers.ext_prop_read_manager import ExtendedPropertyReadManager
 from ..managers.ext_prop_write_manager import ExtendedPropertyWriteManager
 from ..utils import multiple_status
-from .device_commands import MANUAL_CHANGE
+from .device_commands import MANUAL_CHANGE, OFF_AT_RAMP_RATE, ON_AT_RAMP_RATE
 from .on_off_responder_base import OnOffResponderBase
 from .variable_responder_base import VariableResponderBase
 
 OP_FLAG_1F_00 = f"{OPERATING_FLAGS}_1f_00"
 OP_FLAG_1F_05 = f"{OPERATING_FLAGS}_1f_05"
 OP_FLAG_DATA_4 = f"{OPERATING_FLAGS}_data_4"
 
@@ -579,23 +582,46 @@
     def _register_op_flags_and_props(self) -> None:
         self._register_default_op_flags_and_props(dimmable=True, additional_flags=[])
 
     def _register_handlers_and_managers(self) -> None:
         super()._register_handlers_and_managers()
         for group, group_prop in self._groups.items():
             if isinstance(group_prop, OnLevel):
+                self._handlers[group][ON_AT_RAMP_RATE] = OnAtRampRateInbound(
+                    self._address, group
+                )
+                self._handlers[group][OFF_AT_RAMP_RATE] = OffAtRampRateInbound(
+                    self._address, group
+                )
                 self._handlers[group][MANUAL_CHANGE] = ManualChangeInbound(
                     self._address, group
                 )
 
     def _subscribe_to_handelers_and_managers(self) -> None:
         super()._subscribe_to_handelers_and_managers()
         for group, group_prop in self._groups.items():
             if isinstance(group_prop, OnLevel):
                 self._handlers[group][MANUAL_CHANGE].subscribe(self.async_status)
+                # pylint: disable=cell-var-from-loop
+                self._handlers[group][OFF_AT_RAMP_RATE].subscribe(
+                    lambda on_level, ramp_rate: self._handle_on_off_at_ramp_rate(
+                        group, on_level, ramp_rate
+                    ),
+                    force_strong_ref=True,
+                )
+                self._handlers[group][ON_AT_RAMP_RATE].subscribe(
+                    lambda on_level, ramp_rate: self._handle_on_off_at_ramp_rate(
+                        group, on_level, ramp_rate
+                    ),
+                    force_strong_ref=True,
+                )
+
+    def _handle_on_off_at_ramp_rate(self, group: int, on_level: int, ramp_rate: int):
+        """Handle the on and off at ramp rate inbound broadcast messages."""
+        self._groups[group].set_value(on_level)
 
 
 # pylint: disable=super-with-arguments
 class I3OnOffResponderBase(I3Base, OnOffResponderBase):
     """I3 on/off responder base class."""
 
     def _register_op_flags_and_props(self) -> None:
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/ipdb.py` & `pyinsteon-1.6.0/pyinsteon/device_types/ipdb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/mock_modem.py` & `pyinsteon-1.6.0/pyinsteon/device_types/mock_modem.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/modem_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/modem_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/on_off_controller_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/on_off_controller_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Dimmable Lighting Control Devices (CATEGORY 0x01)."""
+
 from ..default_link import DefaultLink
 from ..events import OFF_EVENT, ON_EVENT, Event
 from ..groups import ON_OFF_SWITCH
 from ..groups.on_off import OnOff
-from ..handlers.to_device.status_request import StatusRequestCommand
 from ..managers.on_level_manager import OnLevelManager
+from ..managers.status_manager import StatusManager
 from .device_base import Device
 from .device_commands import STATUS_COMMAND
 
 ON_LEVEL_MANAGER = "on_level_manager"
 
 
 class OnOffControllerBase(Device):
@@ -26,30 +27,22 @@
         on_event_name=ON_EVENT,
         off_event_name=OFF_EVENT,
         on_fast_event_name=None,
         off_fast_event_name=None,
     ):
         """Init the OnOffControllerBase class."""
 
-        self._buttons = {1: ON_OFF_SWITCH} if buttons is None else buttons
+        self._buttons = {1: (ON_OFF_SWITCH, 0)} if buttons is None else buttons
         self._on_event_name = on_event_name
         self._off_event_name = off_event_name
         self._on_fast_event_name = on_fast_event_name
         self._off_fast_event_name = off_fast_event_name
 
         super().__init__(address, cat, subcat, firmware, description, model)
 
-    def status(self, group=None):
-        """Request the status of the device."""
-        self._handlers[STATUS_COMMAND].send()
-
-    async def async_status(self, group=None):
-        """Request the status of the device."""
-        return await self._handlers[STATUS_COMMAND].async_send()
-
     def _register_default_links(self):
         """Register default links for the device."""
         super()._register_default_links()
         for group in self._buttons:
             link = DefaultLink(
                 is_controller=True,
                 group=group,
@@ -61,34 +54,36 @@
                 modem_data3=0,
             )
             self._default_links.append(link)
 
     def _register_handlers_and_managers(self):
         super()._register_handlers_and_managers()
 
-        self._handlers[STATUS_COMMAND] = StatusRequestCommand(self._address, 0)
+        self._managers[STATUS_COMMAND] = StatusManager(self._address)
         for group in self._buttons:
             if self._managers.get(group) is None:
                 self._managers[group] = {}
             self._managers[group][ON_LEVEL_MANAGER] = OnLevelManager(
                 self._address, group
             )
 
     def _register_groups(self):
         super()._register_groups()
         for group in self._buttons:
-            if self._buttons[group] is not None:
-                name = self._buttons[group]
-                self._groups[group] = OnOff(name, self._address, group)
+            name = self._buttons[group][0]
+            status_type = self._buttons[group][1]
+            self._groups[group] = OnOff(
+                name=name, address=self._address, group=group, status_type=status_type
+            )
 
     def _register_events(self):
         super()._register_events()
         for group in self._buttons:
             self._events[group] = {}
-            button = self._buttons[group]
+            button = self._buttons[group][0]
             if self._on_event_name:
                 self._events[group][self._on_event_name] = Event(
                     self._on_event_name, self._address, group, button
                 )
 
             if self._off_event_name:
                 self._events[group][self._off_event_name] = Event(
@@ -103,15 +98,15 @@
             if self._off_fast_event_name:
                 self._events[group][self._off_fast_event_name] = Event(
                     self._off_fast_event_name, self._address, group, button
                 )
 
     def _subscribe_to_handelers_and_managers(self):
         super()._subscribe_to_handelers_and_managers()
-        self._handlers[STATUS_COMMAND].subscribe(self._handle_status)
+        self._managers[STATUS_COMMAND].add_status_type(0, self._handle_status)
         for group in self._buttons:
             if self._groups.get(group) is not None:
                 self._managers[group][ON_LEVEL_MANAGER].subscribe(
                     self._groups[group].set_value
                 )
             if self._on_event_name:
                 event = self._events[group][self._on_event_name]
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/on_off_responder_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/on_off_responder_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 """Switched Lighting Control devices (CATEGORY 0x02)."""
+
 from ..events import OFF_EVENT, ON_EVENT
 from ..groups import ON_OFF_SWITCH
 from ..handlers.to_device.off import OffCommand
 from ..handlers.to_device.off_fast import OffFastCommand
 from ..handlers.to_device.on_fast import OnFastCommand
 from ..handlers.to_device.on_level import OnLevelCommand
-from .device_commands import OFF_COMMAND, OFF_FAST_COMMAND, ON_COMMAND, ON_FAST_COMMAND
+from .device_commands import (
+    OFF_COMMAND,
+    OFF_FAST_COMMAND,
+    ON_COMMAND,
+    ON_FAST_COMMAND,
+    STATUS_COMMAND,
+)
 from .on_off_controller_base import OnOffControllerBase
 
 
 class OnOffResponderBase(OnOffControllerBase):
     """Switched Lighting Control device."""
 
     def __init__(
@@ -23,15 +30,15 @@
         buttons=None,
         on_event_name=ON_EVENT,
         off_event_name=OFF_EVENT,
         on_fast_event_name=None,
         off_fast_event_name=None,
     ):
         """Init the OnOffResponderBase class."""
-        buttons = {1: ON_OFF_SWITCH} if buttons is None else buttons
+        buttons = {1: (ON_OFF_SWITCH, 0)} if buttons is None else buttons
         super().__init__(
             address,
             cat,
             subcat,
             firmware,
             description,
             model,
@@ -58,28 +65,30 @@
         self._handlers[group][OFF_COMMAND].send()
 
     async def async_off(self, group: int = 0):
         """Turn off the device."""
         group = 1 if not group else group
         return await self._handlers[group][OFF_COMMAND].async_send()
 
+    async def async_status(self, group=None):
+        """Get the device status."""
+        status_type = self._groups[group].status_type if group is not None else None
+        return await self._managers[STATUS_COMMAND].async_status(status_type)
+
     def _register_handlers_and_managers(self):
         super()._register_handlers_and_managers()
         for group in self._buttons:
-            if self._buttons[group] is not None:
-                if self._handlers.get(group) is None:
-                    self._handlers[group] = {}
-                self._handlers[group][ON_COMMAND] = OnLevelCommand(self._address, group)
-                self._handlers[group][OFF_COMMAND] = OffCommand(self._address, group)
-                self._handlers[group][ON_FAST_COMMAND] = OnFastCommand(
-                    self._address, group
-                )
-                self._handlers[group][OFF_FAST_COMMAND] = OffFastCommand(
-                    self._address, group
-                )
+            if self._handlers.get(group) is None:
+                self._handlers[group] = {}
+            self._handlers[group][ON_COMMAND] = OnLevelCommand(self._address, group)
+            self._handlers[group][OFF_COMMAND] = OffCommand(self._address, group)
+            self._handlers[group][ON_FAST_COMMAND] = OnFastCommand(self._address, group)
+            self._handlers[group][OFF_FAST_COMMAND] = OffFastCommand(
+                self._address, group
+            )
 
     def _subscribe_to_handelers_and_managers(self):
         super()._subscribe_to_handelers_and_managers()
         for group in self._buttons:
             if self._groups.get(group):
                 self._handlers[group][ON_COMMAND].subscribe(
                     self._groups[group].set_value
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/open_close_controller_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/open_close_controller_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Dimmable Lighting Control Devices (CATEGORY 0x01)."""
+
 from ..default_link import DefaultLink
 from ..events import CLOSE_EVENT, OPEN_EVENT, Event
 from ..groups import OPEN_CLOSE_SENSOR
 from ..groups.open_close import NormallyClosed, NormallyOpen
-from ..handlers.to_device.status_request import StatusRequestCommand
 from ..managers.on_level_manager import OnLevelManager
+from ..managers.status_manager import StatusManager
 from .device_base import Device
 from .device_commands import STATUS_COMMAND
 
 
 class OpenCloseControllerBase(Device):
     """Base device for Open/Close controllers."""
 
@@ -28,22 +29,14 @@
         """Init the OpenCloseControllerBase class."""
         self._state_name = state_name
         self._open_event_name = open_event_name
         self._close_event_name = close_event_name
         self._normally_open = normally_open
         super().__init__(address, cat, subcat, firmware, description, model)
 
-    def status(self, group=None):
-        """Request the status of the device."""
-        self._handlers[STATUS_COMMAND].send()
-
-    async def async_status(self, group=None):
-        """Request the status of the device."""
-        return await self._handlers[STATUS_COMMAND].async_send()
-
     def _register_default_links(self):
         super()._register_default_links()
         link = DefaultLink(
             is_controller=True,
             group=1,
             dev_data1=255,
             dev_data2=28,
@@ -52,15 +45,15 @@
             modem_data2=0,
             modem_data3=0,
         )
         self._default_links.append(link)
 
     def _register_handlers_and_managers(self):
         super()._register_handlers_and_managers()
-        self._handlers[STATUS_COMMAND] = StatusRequestCommand(self._address, 0)
+        self._managers[STATUS_COMMAND] = StatusManager(self._address)
         self._managers[1] = OnLevelManager(self._address, 1)
 
     def _register_groups(self):
         """Register a Normally Open state."""
         if self._normally_open:
             self._groups[1] = NormallyOpen(self._state_name, self._address, 1)
         else:
@@ -73,15 +66,15 @@
         )
         self._events[1][self._close_event_name] = Event(
             self._close_event_name, self._address, 1
         )
 
     def _subscribe_to_handelers_and_managers(self):
         super()._subscribe_to_handelers_and_managers()
-        self._handlers[STATUS_COMMAND].subscribe(self._handle_status)
+        self._managers[STATUS_COMMAND].add_status_type(0, self._handle_status)
         self._managers[1].subscribe(self._groups[1].set_value)
         if self._normally_open:
             # Open is OFF and Close is ON
             self._managers[1].subscribe_off(
                 self._events[1][self._open_event_name].trigger
             )
             self._managers[1].subscribe_on(
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/open_close_responder_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/open_close_responder_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 """Dimmable Lighting Control Devices (CATEGORY 0x01)."""
+
 from ..handlers.to_device.off import OffCommand
 from ..handlers.to_device.off_fast import OffFastCommand
 from ..handlers.to_device.on_fast import OnFastCommand
 from ..handlers.to_device.on_level import OnLevelCommand
-from ..handlers.to_device.status_request import StatusRequestCommand
-from .device_commands import (
-    OFF_COMMAND,
-    OFF_FAST_COMMAND,
-    ON_COMMAND,
-    ON_FAST_COMMAND,
-    STATUS_COMMAND,
-)
+from .device_commands import OFF_COMMAND, OFF_FAST_COMMAND, ON_COMMAND, ON_FAST_COMMAND
 from .open_close_controller_base import OpenCloseControllerBase
 
 
 class OpenCloseResponderBase(OpenCloseControllerBase):
     """Variable Responder Base Device."""
 
     def open(self, open_level=0xFF, group=0, fast=False):
@@ -73,22 +67,16 @@
             UNCLEAR: Device received the message but did not confirm the action
 
         """
         group = 1 if not group else group
         command = OFF_FAST_COMMAND if fast else OFF_COMMAND
         return await self._handlers[group][command].async_send()
 
-    # pylint: disable=arguments-differ
-    async def async_status(self):
-        """Get the status of the device state."""
-        return await self._handlers[STATUS_COMMAND].async_send()
-
     def _register_handlers_and_managers(self):
         super()._register_handlers_and_managers()
-        self._handlers[STATUS_COMMAND] = StatusRequestCommand(self._address)
         group = 1
         if self._handlers.get(group) is None:
             self._handlers[group] = {}
         self._handlers[group][ON_COMMAND] = OnLevelCommand(self._address, group)
         self._handlers[group][OFF_COMMAND] = OffCommand(self._address, group)
         self._handlers[group][ON_FAST_COMMAND] = OnFastCommand(self._address, group)
         self._handlers[group][OFF_FAST_COMMAND] = OffFastCommand(self._address, group)
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/plm.py` & `pyinsteon-1.6.0/pyinsteon/device_types/plm.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/security_health_safety.py` & `pyinsteon-1.6.0/pyinsteon/device_types/security_health_safety.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Security, Heath and Safety device types."""
+
 from ..config import (
     AMBIENT_LIGHT_INTENSITY,
     BATTERY_LEVEL,
     BATTERY_LOW_LEVEL,
     CLEANUP_REPORT_ON,
     DATABASE_DELTA,
     HARDWARE_LED_OFF,
@@ -90,15 +91,15 @@
 
     DOOR_GROUP = 1
     LOW_BATTERY_GROUP = 3
     HEARTBEAT_GROUP = 4
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the SecurityHealthSafety_DoorSensor class."""
-        buttons = {1: DOOR_SENSOR}
+        buttons = {1: (DOOR_SENSOR, None)}
         super().__init__(
             address=address,
             cat=cat,
             subcat=subcat,
             firmware=firmware,
             description=description,
             model=model,
@@ -221,15 +222,15 @@
 
     MOTION_GROUP = 1
     LIGHT_GROUP = 2
     LOW_BATTERY_GROUP = 3
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the SecurityHealthSafety_DoorSensor class."""
-        buttons = {1: MOTION_SENSOR}
+        buttons = {1: (MOTION_SENSOR, None)}
         self._light_manager = OnLevelManager(address, self.LIGHT_GROUP)
         self._low_battery_manager = LowBatteryManager(address, self.LOW_BATTERY_GROUP)
         super().__init__(
             address=address,
             cat=cat,
             subcat=subcat,
             firmware=firmware,
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/sensors_actuators.py` & `pyinsteon-1.6.0/pyinsteon/device_types/sensors_actuators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Sensor/Actuator devices."""
+
 import asyncio
 
 from ..config import (
     DELAY,
     LED_BLINK_ON_TX_ON,
     MOMENTARY_DELAY,
     MOMENTARY_FOLLOW_SENSE,
@@ -15,27 +16,25 @@
     SENSE_SENDS_OFF,
     X10_HOUSE,
     X10_OFF,
     X10_UNIT,
 )
 from ..config.momentary_delay import MomentaryDelayProperty
 from ..config.relay_mode import RelayModeProperty
-from ..constants import PropertyType, RelayMode, ResponseStatus
+from ..constants import PropertyType, RelayMode
 from ..default_link import DefaultLink
 from ..events import CLOSE_EVENT, OFF_EVENT, ON_EVENT, OPEN_EVENT, Event
 from ..groups import OPEN_CLOSE_SENSOR, RELAY
 from ..groups.on_off import OnOff
 from ..groups.open_close import NormallyClosed
 from ..handlers.to_device.off import OffCommand
 from ..handlers.to_device.on_level import OnLevelCommand
-from ..handlers.to_device.status_request import STATUS_REQUEST, StatusRequestCommand
 from ..managers.on_level_manager import OnLevelManager
-from ..utils import multiple_status
 from .device_base import Device
-from .device_commands import OFF_COMMAND, ON_COMMAND
+from .device_commands import OFF_COMMAND, ON_COMMAND, STATUS_COMMAND
 from .on_off_responder_base import OnOffResponderBase
 
 ON_LEVEL_MANAGER = "on_level_manager"
 RELAY_GROUP = 1
 SENSOR_GROUP = 2
 
 
@@ -135,62 +134,18 @@
         """Turn off the relay."""
         self._handlers[RELAY_GROUP][OFF_COMMAND].send()
 
     async def async_off(self, group: int = 0):
         """Turn off the relay."""
         return await self._handlers[RELAY_GROUP][OFF_COMMAND].async_send()
 
-    def status(self, group=None):
-        """Get the status of the relay and/or the sensor."""
-        if group in [1, None]:
-            self.relay_status()
-        if group == [2, None]:
-            self.sensor_status()
-
     async def async_status(self, group=None):
-        """Get the status of the relay and/or the sensor."""
-        response_1 = None
-        response_2 = None
-        if group in [1, None]:
-            response_1 = await self.async_relay_status()
-        if group in [2, None]:
-            response_2 = await self.async_sensor_status()
-        return multiple_status(response_1, response_2)
-
-    def relay_status(self):
-        """Get the status of the relay switch."""
-        self._handlers[RELAY_GROUP][STATUS_REQUEST].send()
-
-    async def async_relay_status(self):
-        """Get the status of the relay switch."""
-        async with self._status_lock:
-            response = None
-            retries = 3
-            while response != ResponseStatus.SUCCESS and retries:
-                response = await self._handlers[RELAY_GROUP][
-                    STATUS_REQUEST
-                ].async_send()
-                retries -= 1
-            return response
-
-    def sensor_status(self):
-        """Get the status of the sensor."""
-        self._handlers[SENSOR_GROUP][STATUS_REQUEST].send()
-
-    async def async_sensor_status(self):
-        """Get the status of the sensor."""
-        async with self._status_lock:
-            response = None
-            retries = 3
-            while response != ResponseStatus.SUCCESS and retries:
-                response = await self._handlers[SENSOR_GROUP][
-                    STATUS_REQUEST
-                ].async_send()
-                retries -= 1
-            return response
+        """Get the device status."""
+        status_type = self._groups[group].status_type if group is not None else None
+        return await self._managers[STATUS_COMMAND].async_status(status_type)
 
     def _register_op_flags_and_props(self):
         self._add_operating_flag(PROGRAM_LOCK_ON, 0, 0, 0, 1)
         self._add_operating_flag(LED_BLINK_ON_TX_ON, 0, 1, 2, 3)
         self._add_operating_flag(
             RELAY_ON_SENSE_ON, 0, 2, 4, 5, prop_type=PropertyType.ADVANCED
         )  # Sensor triggers relay
@@ -243,33 +198,29 @@
         self._handlers[RELAY_GROUP] = {}
         self._handlers[RELAY_GROUP][ON_COMMAND] = OnLevelCommand(
             self._address, RELAY_GROUP
         )
         self._handlers[RELAY_GROUP][OFF_COMMAND] = OffCommand(
             self._address, RELAY_GROUP
         )
-        self._handlers[RELAY_GROUP][STATUS_REQUEST] = StatusRequestCommand(
-            self._address
-        )
 
         self._handlers[SENSOR_GROUP] = {}
-        self._handlers[SENSOR_GROUP][STATUS_REQUEST] = StatusRequestCommand(
-            self.address, 1
-        )
 
     def _register_groups(self):
         """Register the device groups.
 
         There really is only one group in the device, group 1. Both the relay and the sensor
         both send updates on group 1 for broadcast messages. We create two groups because
         we can keep the status of the relay and the sensor separate.
         """
-        self._groups[RELAY_GROUP] = OnOff(RELAY, self._address, RELAY_GROUP)
+        self._groups[RELAY_GROUP] = OnOff(
+            RELAY, self._address, RELAY_GROUP, status_type=0
+        )
         self._groups[SENSOR_GROUP] = NormallyClosed(
-            OPEN_CLOSE_SENSOR, self._address, SENSOR_GROUP
+            OPEN_CLOSE_SENSOR, self._address, SENSOR_GROUP, status_type=1
         )
 
     def _register_events(self):
         self._events[ON_EVENT] = Event(ON_EVENT, self._address, 0)
         self._events[OFF_EVENT] = Event(OFF_EVENT, self._address, 0)
         self._events[RELAY_GROUP] = {}
         self._events[RELAY_GROUP][ON_EVENT] = Event(
@@ -295,26 +246,23 @@
         current status of the device is for both the relay and the sensor.
         """
         super()._subscribe_to_handelers_and_managers()
         switch_on_event = self._events[RELAY_GROUP][ON_EVENT]
         switch_off_event = self._events[RELAY_GROUP][OFF_EVENT]
         on_cmd = self._handlers[RELAY_GROUP][ON_COMMAND]
         off_cmd = self._handlers[RELAY_GROUP][OFF_COMMAND]
-        switch_status_cmd = self._handlers[RELAY_GROUP][STATUS_REQUEST]
 
         on_cmd.subscribe(self._async_switch_changed)
         off_cmd.subscribe(self._async_switch_changed)
         on_cmd.subscribe(switch_on_event.trigger)
         off_cmd.subscribe(switch_off_event.trigger)
-        switch_status_cmd.subscribe(self._handle_switch_status)
 
         self._managers[ON_LEVEL_MANAGER].subscribe(self._async_on_off_received)
-        self._handlers[SENSOR_GROUP][STATUS_REQUEST].subscribe(
-            self._handle_sensor_status
-        )
+        self._managers[STATUS_COMMAND].add_status_type(0, self._handle_switch_status)
+        self._managers[STATUS_COMMAND].add_status_type(1, self._handle_sensor_status)
 
     def _register_default_links(self):
         link = DefaultLink(
             is_controller=True,
             group=RELAY_GROUP,
             dev_data1=0,
             dev_data2=0,
@@ -361,22 +309,22 @@
         else:
             self._events[OFF_EVENT].trigger(on_level=0)
         orig_sensor = self._groups[SENSOR_GROUP].value
         orig_relay = self._groups[RELAY_GROUP].value
 
         # Need to get status since we don't know if the on/off message was for the relay
         # or the sensor. Get the sensor first since that is the most likely change.
-        await self.async_sensor_status()
+        await self.async_status(group=1)
         if self._groups[SENSOR_GROUP].value != orig_sensor:
             if self._groups[SENSOR_GROUP].value:
                 self._events[SENSOR_GROUP][OPEN_EVENT].trigger(on_level=255)
             else:
                 self._events[SENSOR_GROUP][CLOSE_EVENT].trigger(on_level=0)
 
-        await self.async_relay_status()
+        await self.async_status(group=0)
         if self._groups[RELAY_GROUP].value != orig_relay:
             if self._groups[RELAY_GROUP].value:
                 self._events[RELAY_GROUP][ON_EVENT].trigger(on_level=255)
                 if self._operating_flags[MOMENTARY_MODE_ON].value:
                     await self._delay_wait()
             else:
                 self._events[RELAY_GROUP][OFF_EVENT].trigger(on_level=0)
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/switched_lighting_control.py` & `pyinsteon-1.6.0/pyinsteon/device_types/switched_lighting_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Switched Lighting Control devices (CATEGORY 0x02)."""
+
 import asyncio
 from functools import partial
 from typing import Dict, Iterable
 
 from ..config import (
     BLUE_LED_OFF,
     DO_NOT_ROTATE_TO_OFF,
@@ -53,17 +54,16 @@
     ON_OFF_SWITCH_F,
     ON_OFF_SWITCH_G,
     ON_OFF_SWITCH_H,
     ON_OFF_SWITCH_MAIN,
 )
 from ..groups.on_off import OnOff
 from ..handlers.to_device.set_leds import SetLedsCommandHandler
-from ..handlers.to_device.status_request import StatusRequestCommand
-from ..utils import bit_is_set, multiple_status, set_bit
-from .device_commands import GET_LEDS_COMMAND, SET_LEDS_COMMAND, STATUS_COMMAND
+from ..utils import bit_is_set, set_bit
+from .device_commands import SET_LEDS_COMMAND, STATUS_COMMAND
 from .i3_base import I3Base, OpsFlagDef
 from .on_off_controller_base import ON_LEVEL_MANAGER
 from .on_off_responder_base import OnOffResponderBase
 
 
 class SwitchedLightingControl(OnOffResponderBase):
     """Switched Lighting Control device."""
@@ -80,15 +80,15 @@
         state_name=ON_OFF_SWITCH,
         on_event_name=ON_EVENT,
         off_event_name=OFF_EVENT,
         on_fast_event_name=ON_FAST_EVENT,
         off_fast_event_name=OFF_FAST_EVENT,
     ):
         """Init the OnOffResponderBase class."""
-        buttons = {1: ON_OFF_SWITCH} if buttons is None else buttons
+        buttons = {1: (ON_OFF_SWITCH, 0)} if buttons is None else buttons
         super().__init__(
             address,
             cat,
             subcat,
             firmware,
             description,
             model,
@@ -255,25 +255,14 @@
                 result = await self._handlers[SET_LEDS_COMMAND].async_send(**kwargs)
         if result == ResponseStatus.SUCCESS:
             self._update_leds(group=group, value=0, event=OFF_EVENT)
         elif result == ResponseStatus.DIRECT_NAK_PRE_NAK:
             await self.async_status()
         return result
 
-    async def async_status(self, group=None):
-        """Check the status of the device."""
-        retries = 5
-        status = ResponseStatus.UNSENT
-        while retries and status != ResponseStatus.SUCCESS:
-            status0 = await super().async_status()
-            status1 = await self._handlers[GET_LEDS_COMMAND].async_send()
-            status = multiple_status(status0, status1)
-            retries -= 1
-        return status
-
     def set_radio_buttons(self, buttons: Iterable):
         """Set a group of buttons to act as radio buttons.
 
         This takes in a iterable set of buttons (eg. (3,4,5,6)) to act as radio buttons where
         no two buttons are on at the same time.
         """
         if len(buttons) < 2:
@@ -409,31 +398,30 @@
             on_off_mask.new_value = set_bit(on_off_mask_test, button - 1, True)
         else:
             toggle_mask.new_value = set_bit(toggle_mask_test, button - 1, True)
             on_off_mask.new_value = set_bit(on_off_mask_test, button - 1, False)
 
     def _register_handlers_and_managers(self):
         super()._register_handlers_and_managers()
-        self._handlers[STATUS_COMMAND] = StatusRequestCommand(
-            self._address, status_type=2
-        )
         self._handlers[SET_LEDS_COMMAND] = SetLedsCommandHandler(address=self.address)
-        self._handlers[GET_LEDS_COMMAND] = StatusRequestCommand(
-            self._address, status_type=1
-        )
 
     def _register_groups(self):
         super()._register_groups()
         for button in self._buttons:
-            name = self._buttons[button]
-            self._groups[button] = OnOff(name=name, address=self._address, group=button)
+            name = self._buttons[button][0]
+            status_type = self._buttons[button][1]
+            self._groups[button] = OnOff(
+                name=name, address=self._address, group=button, status_type=status_type
+            )
 
     def _subscribe_to_handelers_and_managers(self):
         super()._subscribe_to_handelers_and_managers()
-        self._handlers[GET_LEDS_COMMAND].subscribe(self._led_status)
+        self._managers[STATUS_COMMAND].remove_status_type(0)
+        self._managers[STATUS_COMMAND].add_status_type(2, self._handle_status)
+        self._managers[STATUS_COMMAND].add_status_type(1, self._led_status)
         for group in self._buttons:
             if self._groups.get(group) is not None:
                 led_method = partial(self._led_follow_check, group=group)
                 self._managers[group][ON_LEVEL_MANAGER].subscribe(led_method)
 
     def _led_follow_check(self, group, on_level):
         """Check the other LEDs to confirm if they follow the effected LED."""
@@ -548,19 +536,19 @@
 
 class SwitchedLightingControl_KeypadLinc_6(SwitchedLightingControl_KeypadLinc):
     """KeypadLinc 6 button switch."""
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the SwitchedLightingControl_KeypadLinc_6 class."""
         buttons = {
-            1: ON_OFF_SWITCH_MAIN,
-            3: ON_OFF_SWITCH_A,
-            4: ON_OFF_SWITCH_B,
-            5: ON_OFF_SWITCH_C,
-            6: ON_OFF_SWITCH_D,
+            1: (ON_OFF_SWITCH_MAIN, 0),
+            3: (ON_OFF_SWITCH_A, 1),
+            4: (ON_OFF_SWITCH_B, 1),
+            5: (ON_OFF_SWITCH_C, 1),
+            6: (ON_OFF_SWITCH_D, 1),
         }
         super().__init__(
             address=address,
             cat=cat,
             subcat=subcat,
             firmware=firmware,
             description=description,
@@ -571,22 +559,22 @@
 
 class SwitchedLightingControl_KeypadLinc_8(SwitchedLightingControl_KeypadLinc):
     """KeypadLinc 8 button switch."""
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the SwitchedLightingControl_KeypadLinc_8 class."""
         buttons = {
-            1: ON_OFF_SWITCH_MAIN,
-            2: ON_OFF_SWITCH_B,
-            3: ON_OFF_SWITCH_C,
-            4: ON_OFF_SWITCH_D,
-            5: ON_OFF_SWITCH_E,
-            6: ON_OFF_SWITCH_F,
-            7: ON_OFF_SWITCH_G,
-            8: ON_OFF_SWITCH_H,
+            1: (ON_OFF_SWITCH_MAIN, 0),
+            2: (ON_OFF_SWITCH_B, 1),
+            3: (ON_OFF_SWITCH_C, 1),
+            4: (ON_OFF_SWITCH_D, 1),
+            5: (ON_OFF_SWITCH_E, 1),
+            6: (ON_OFF_SWITCH_F, 1),
+            7: (ON_OFF_SWITCH_G, 1),
+            8: (ON_OFF_SWITCH_H, 1),
         }
         super().__init__(
             address=address,
             cat=cat,
             subcat=subcat,
             firmware=firmware,
             description=description,
@@ -602,61 +590,22 @@
     """
 
     TOP_GROUP = 1
     BOTTOM_GROUP = 2
 
     def __init__(self, address, cat, subcat, firmware=0x00, description="", model=""):
         """Init the SwitchedLightingControl_KeypadLinc class."""
-        buttons = {1: ON_OFF_OUTLET_TOP, 2: ON_OFF_OUTLET_BOTTOM}
+        buttons = {1: (ON_OFF_OUTLET_TOP, 1), 2: (ON_OFF_OUTLET_BOTTOM, 1)}
         super().__init__(
             address, cat, subcat, firmware, description, model, buttons=buttons
         )
 
-    def status(self, group=None):
-        """Request the status of the device."""
-        if group is None:
-            self._handlers[STATUS_COMMAND].send()
-        if group in [1, 2]:
-            self._handlers[group][STATUS_COMMAND].send()
-
-    async def async_status(self, group=None):
-        """Request the status of the device."""
-        if group is None:
-            return await self._handlers[STATUS_COMMAND].async_send()
-        if group in [1, 2]:
-            return await self._handlers[group][STATUS_COMMAND].async_send()
-
-    def _register_handlers_and_managers(self):
-        super()._register_handlers_and_managers()
-        self._handlers[STATUS_COMMAND] = StatusRequestCommand(self._address, 1)
-
-        if self._handlers.get(self.TOP_GROUP) is None:
-            self._handlers[self.TOP_GROUP] = {}
-        self._handlers[self.TOP_GROUP][STATUS_COMMAND] = StatusRequestCommand(
-            self._address, 0
-        )
-
-        if self._handlers.get(self.BOTTOM_GROUP) is None:
-            self._handlers[self.BOTTOM_GROUP] = {}
-        self._handlers[self.BOTTOM_GROUP][STATUS_COMMAND] = self._handlers[
-            STATUS_COMMAND
-        ]
-
     def _subscribe_to_handelers_and_managers(self):
         super()._subscribe_to_handelers_and_managers()
-
-        self._handlers[self.TOP_GROUP][STATUS_COMMAND].subscribe(
-            self._handle_top_status
-        )
-
-        self._handlers[STATUS_COMMAND].subscribe(self._handle_status)
-
-    def _handle_top_status(self, db_version, status):
-        """Set the status of the top outlet."""
-        self._groups[self.TOP_GROUP].value = status
+        self._managers[STATUS_COMMAND].add_status_type(1, self._handle_status)
 
     def _handle_status(self, db_version, status):
         """Set the status of the top and bottom outlets."""
         self._groups[self.TOP_GROUP].value = 1 if (status & 0x01) else 0
         self._groups[self.BOTTOM_GROUP].value = 1 if (status & 0x02) else 0
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/variable_controller_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/variable_controller_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Dimmable Lighting Control Devices (CATEGORY 0x01)."""
 
 from ..default_link import DefaultLink
 from ..events import OFF_EVENT, OFF_FAST_EVENT, ON_EVENT, ON_FAST_EVENT, Event
 from ..groups import DIMMABLE_LIGHT
 from ..groups.on_level import OnLevel
-from ..handlers.to_device.status_request import StatusRequestCommand
 from ..managers.on_level_manager import OnLevelManager
+from ..managers.status_manager import StatusManager
 from .device_base import Device
 from .device_commands import STATUS_COMMAND
 
 ON_LEVEL_MANAGER = "on_level_manager"
 
 
 class VariableControllerBase(Device):
@@ -22,29 +22,17 @@
         subcat,
         firmware=0x00,
         description="",
         model="",
         buttons=None,
     ):
         """Init the VariableControllerBase class."""
-        self._buttons = {1: DIMMABLE_LIGHT} if buttons is None else buttons
+        self._buttons = {1: (DIMMABLE_LIGHT, 0)} if buttons is None else buttons
         super().__init__(address, cat, subcat, firmware, description, model)
 
-    # pylint: disable=arguments-differ
-    async def async_status(self):
-        """Request the status of the device.
-
-        Returns a ResponseStatus value
-            FAILURE: Device did not acknowledge the message
-            SUCCESS: Device acknowledged the message
-            UNCLEAR: Device received the message but did not confirm the action
-
-        """
-        return await self._handlers[STATUS_COMMAND].async_send()
-
     def _register_default_links(self):
         """Register default links.
 
         Default links:
             is_controller group dev_data1 dev_data2 dev_data3 modem_data1 modem_data2 modem_data3
 
         """
@@ -60,27 +48,30 @@
                 modem_data2=0,
                 modem_data3=0,
             )
             self._default_links.append(link)
 
     def _register_handlers_and_managers(self):
         super()._register_handlers_and_managers()
-        self._handlers[STATUS_COMMAND] = StatusRequestCommand(self._address)
+        self._managers[STATUS_COMMAND] = StatusManager(self._address)
         for group in self._buttons:
             if self._managers.get(group) is None:
                 self._managers[group] = {}
             self._managers[group][ON_LEVEL_MANAGER] = OnLevelManager(
                 self._address, group
             )
 
     def _register_groups(self):
         super()._register_groups()
         for group in self._buttons:
-            name = self._buttons[group]
-            self._groups[group] = OnLevel(name=name, address=self._address, group=group)
+            name = self._buttons[group][0]
+            status_type = self._buttons[group][1]
+            self._groups[group] = OnLevel(
+                name=name, address=self._address, group=group, status_type=status_type
+            )
 
     def _register_events(self):
         super()._register_events()
         for group in self._buttons:
             if self._events.get(group) is None:
                 self._events[group] = {}
             button = self._buttons[group]
@@ -95,15 +86,17 @@
             )
             self._events[group][OFF_FAST_EVENT] = Event(
                 OFF_FAST_EVENT, self._address, group, button
             )
 
     def _subscribe_to_handelers_and_managers(self):
         super()._subscribe_to_handelers_and_managers()
-        self._handlers[STATUS_COMMAND].subscribe(self._handle_status)
+        self._managers[STATUS_COMMAND].add_status_type(
+            status_type=0, callback_function=self._handle_status
+        )
         for group in self._buttons:
             state = self._groups[group]
             self._managers[group][ON_LEVEL_MANAGER].subscribe(state.set_value)
 
             event = self._events[group][ON_EVENT]
             self._managers[group][ON_LEVEL_MANAGER].subscribe_on(event.trigger)
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/variable_responder_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/variable_responder_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Dimmable Lighting Control Devices (CATEGORY 0x01)."""
+
 from ..handlers.to_device.off import OffCommand
 from ..handlers.to_device.off_fast import OffFastCommand
 from ..handlers.to_device.on_fast import OnFastCommand
 from ..handlers.to_device.on_level import OnLevelCommand
-from ..handlers.to_device.status_request import StatusRequestCommand
 from .device_commands import (
     OFF_COMMAND,
     OFF_FAST_COMMAND,
     ON_COMMAND,
     ON_FAST_COMMAND,
     STATUS_COMMAND,
 )
@@ -73,21 +73,21 @@
             UNCLEAR: Device received the message but did not confirm the action
 
         """
         group = 1 if not group else group
         command = OFF_FAST_COMMAND if fast else OFF_COMMAND
         return await self._handlers[group][command].async_send()
 
-    async def async_status(self):
-        """Get the status of the device state."""
-        return await self._handlers[STATUS_COMMAND].async_send()
+    async def async_status(self, group=None):
+        """Get the device status."""
+        status_type = self._groups[group].status_type if group is not None else None
+        return await self._managers[STATUS_COMMAND].async_status(status_type)
 
     def _register_handlers_and_managers(self):
         super()._register_handlers_and_managers()
-        self._handlers[STATUS_COMMAND] = StatusRequestCommand(self._address)
         for group in self._buttons:
             if self._handlers.get(group) is None:
                 self._handlers[group] = {}
             self._handlers[group][ON_COMMAND] = OnLevelCommand(self._address, group)
             self._handlers[group][OFF_COMMAND] = OffCommand(self._address, group)
             self._handlers[group][ON_FAST_COMMAND] = OnFastCommand(self._address, group)
             self._handlers[group][OFF_FAST_COMMAND] = OffFastCommand(
```

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/window_coverings.py` & `pyinsteon-1.6.0/pyinsteon/device_types/window_coverings.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/x10.py` & `pyinsteon-1.6.0/pyinsteon/device_types/x10.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/device_types/x10_base.py` & `pyinsteon-1.6.0/pyinsteon/device_types/x10_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/events.py` & `pyinsteon-1.6.0/pyinsteon/events.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/groups/__init__.py` & `pyinsteon-1.6.0/pyinsteon/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/groups/fan.py` & `pyinsteon-1.6.0/pyinsteon/groups/fan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 """Fan On Level state."""
+
 from ..address import Address
 from ..constants import FanSpeed, FanSpeedRange
 from .group_base import GroupBase
 
 
 class FanOnLevel(GroupBase):
     """On / Off state."""
 
     def __init__(
-        self, name: str, address: Address, group: int = 0, default: FanSpeed = None
+        self,
+        name: str,
+        address: Address,
+        group: int = 0,
+        default: FanSpeed = None,
+        status_type: int = 0,
     ):
         """Init the FanOnLevel class."""
-        super().__init__(name, address, group, default, value_type=FanSpeed)
+        super().__init__(
+            name, address, group, default, value_type=FanSpeed, status_type=status_type
+        )
         self._is_dimmable = True
 
     # pylint: disable=arguments-differ
     def set_value(self, on_level):
         """Set the value of the state from the handlers."""
         if on_level in FanSpeedRange.OFF:
             fan_speed = FanSpeed.OFF
```

### Comparing `pyinsteon-1.5.3/pyinsteon/groups/group_base.py` & `pyinsteon-1.6.0/pyinsteon/groups/group_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,32 @@
 
 class GroupBase(SubscriberBase):
     """Device group base class."""
 
     __meta__ = ABC
 
     def __init__(
-        self, name: str, address: Address, group=0, default=None, value_type: type = int
+        self,
+        name: str,
+        address: Address,
+        group=0,
+        default=None,
+        value_type: type = int,
+        status_type: int = 0,
     ):
         """Init the StateBase class."""
         self._address = address
         topic = f"state_{self._address.id}_{name}_{group}"
         super().__init__(subscriber_topic=topic)
         self._name = name
         self._group = group
         self._value = int(default) if default is not None else None
         self._type = value_type
         self._is_dimmable: bool = False
+        self._status_type = status_type
 
     @property
     def is_dimmable(self) -> bool:
         """Return if the state is dimmable.
 
         If true, the state can support values 0 - 255.
         If false, the state only supports values 0 and 255.
@@ -68,11 +75,16 @@
         self._call_subscribers(
             name=self._name,
             address=self._address.id,
             value=self._value,
             group=self._group,
         )
 
+    @property
+    def status_type(self):
+        """Return the status type to get the group state."""
+        return self._status_type
+
     @abstractmethod
     def set_value(self, **kwargs):
         """Set the value of the state from a Handler."""
         raise NotImplementedError
```

### Comparing `pyinsteon-1.5.3/pyinsteon/groups/on_level.py` & `pyinsteon-1.6.0/pyinsteon/groups/on_level.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 """On Leve state."""
+
 import logging
 
 from ..address import Address
 from .group_base import GroupBase
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class OnLevel(GroupBase):
     """Variable On Level state."""
 
     def __init__(
-        self, name: str, address: Address, group: int = 0, default: int = None
+        self,
+        name: str,
+        address: Address,
+        group: int = 0,
+        default: int = None,
+        status_type: int = 0,
     ):
         """Init the OnLevel class."""
-        super().__init__(name, address, group, default, value_type=int)
+        super().__init__(
+            name, address, group, default, value_type=int, status_type=status_type
+        )
         self._is_dimmable: bool = True
 
     @property
     def value(self):
         """Return the value of the state."""
         return self._value
```

### Comparing `pyinsteon-1.5.3/pyinsteon/groups/on_off.py` & `pyinsteon-1.6.0/pyinsteon/groups/on_off.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 """On / Off state."""
+
 from ..address import Address
 from .group_base import GroupBase
 
 
 class OnOff(GroupBase):
     """On / Off state."""
 
     def __init__(
-        self, name: str, address: Address, group: int = 0, default: int = None
+        self,
+        name: str,
+        address: Address,
+        group: int = 0,
+        default: int = None,
+        status_type: int = 0,
     ):
         """Init the OnLevel class."""
-        super().__init__(name, address, group, default, value_type=int)
+        super().__init__(
+            name, address, group, default, value_type=int, status_type=status_type
+        )
 
     # pylint: disable=arguments-differ
     def set_value(self, on_level):
         """Set the value of the state from the handlers."""
         self.value = 0xFF if on_level else 0
```

### Comparing `pyinsteon-1.5.3/pyinsteon/groups/open_close.py` & `pyinsteon-1.6.0/pyinsteon/groups/open_close.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 """Open / Close sensor groups."""
+
 from ..address import Address
 from .group_base import GroupBase
 
 
 class NormallyOpen(GroupBase):
     """Normally open sensor state."""
 
     def __init__(
-        self, name: str, address: Address, group: int = 0, default: int = None
+        self,
+        name: str,
+        address: Address,
+        group: int = 0,
+        default: int = None,
+        status_type: int = 0,
     ):
         """Init the OnLevel class."""
-        super().__init__(name, address, group, default, value_type=int)
+        super().__init__(
+            name, address, group, default, value_type=int, status_type=status_type
+        )
 
     # pylint: disable=arguments-differ
     def set_value(self, on_level):
         """Set the value of the state from the handlers."""
         # Off is a Open state and On is an Closed state
         self.value = 0xFF if on_level else 0
 
 
 class NormallyClosed(GroupBase):
     """Normally closed sensor state."""
 
     def __init__(
-        self, name: str, address: Address, group: int = 0, default: int = None
+        self,
+        name: str,
+        address: Address,
+        group: int = 0,
+        default: int = None,
+        status_type: int = 0,
     ):
-        """Init the OnLevel class."""
-        super().__init__(name, address, group, default, value_type=int)
+        """Init the NormallyClosed class."""
+        super().__init__(
+            name, address, group, default, value_type=int, status_type=status_type
+        )
 
     # pylint: disable=arguments-differ
     def set_value(self, on_level):
         """Set the value of the state from the handlers."""
         # Off is a Closed state and On is an Open state
         self.value = 0 if on_level else 0xFF
```

### Comparing `pyinsteon-1.5.3/pyinsteon/groups/thermostat.py` & `pyinsteon-1.6.0/pyinsteon/groups/thermostat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Temperature state."""
+
 from ..address import Address
 from ..constants import ThermostatMode
 from .group_base import GroupBase
 
 
 class Temperature(GroupBase):
     """Temperature state."""
 
     def __init__(
         self,
         name: str,
         address: Address,
         group: int = 0,
         default: float = None,
+        status_type: int = 0,
     ):
         """Init the Temperature class."""
-        super().__init__(name, address, group, default, value_type=float)
+        super().__init__(
+            name, address, group, default, value_type=float, status_type=status_type
+        )
         self._is_dimmable = True
 
     # pylint: disable=arguments-differ
     def set_value(self, temperature):
         """Set the temperature value."""
         self.value = temperature
```

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/__init__.py` & `pyinsteon-1.6.0/pyinsteon/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/all_link_cleanup_failure_report.py` & `pyinsteon-1.6.0/pyinsteon/handlers/all_link_cleanup_failure_report.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/all_link_cleanup_status_report.py` & `pyinsteon-1.6.0/pyinsteon/handlers/all_link_cleanup_status_report.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/all_link_completed.py` & `pyinsteon-1.6.0/pyinsteon/handlers/all_link_completed.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/all_link_record_response.py` & `pyinsteon-1.6.0/pyinsteon/handlers/all_link_record_response.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/cancel_all_linking.py` & `pyinsteon-1.6.0/pyinsteon/handlers/cancel_all_linking.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/all_link_cleanup_command.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/all_link_cleanup_command.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/assign_to_all_link_group.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/assign_to_all_link_group.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/delete_from_all_link_group.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/delete_from_all_link_group.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/ext_get_response.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/ext_get_response.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/manual_change.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/manual_change.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/off.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/off.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/off_all_link_cleanup.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/off_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/off_fast.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/off_fast.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/off_fast_all_link_cleanup.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/off_fast_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/on_fast.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/on_fast.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/on_fast_all_link_cleanup.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/on_fast_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/on_level.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/on_level.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/on_level_all_link_cleanup.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/on_level_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/receive_aldb_record.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/receive_aldb_record.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/thermostat_cool_set_point.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/thermostat_cool_set_point.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/thermostat_heat_set_point.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/thermostat_heat_set_point.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/thermostat_humidity.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/thermostat_humidity.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/thermostat_mode.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/thermostat_mode.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/thermostat_temperature.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/thermostat_temperature.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/from_device/x10_received.py` & `pyinsteon-1.6.0/pyinsteon/handlers/from_device/x10_received.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/get_first_all_link_record.py` & `pyinsteon-1.6.0/pyinsteon/handlers/get_first_all_link_record.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/get_im_configuration.py` & `pyinsteon-1.6.0/pyinsteon/handlers/get_im_configuration.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/get_im_info.py` & `pyinsteon-1.6.0/pyinsteon/handlers/get_im_info.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/get_next_all_link_record.py` & `pyinsteon-1.6.0/pyinsteon/handlers/get_next_all_link_record.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/inbound_base.py` & `pyinsteon-1.6.0/pyinsteon/handlers/inbound_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/manage_all_link_record.py` & `pyinsteon-1.6.0/pyinsteon/handlers/manage_all_link_record.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/outbound_base.py` & `pyinsteon-1.6.0/pyinsteon/handlers/outbound_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/read_eeprom.py` & `pyinsteon-1.6.0/pyinsteon/handlers/read_eeprom.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/read_eeprom_response.py` & `pyinsteon-1.6.0/pyinsteon/handlers/read_eeprom_response.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/send_all_link.py` & `pyinsteon-1.6.0/pyinsteon/handlers/send_all_link.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/set_im_configuration.py` & `pyinsteon-1.6.0/pyinsteon/handlers/set_im_configuration.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/start_all_linking.py` & `pyinsteon-1.6.0/pyinsteon/handlers/start_all_linking.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/all_link_cleanup_command.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/all_link_cleanup_command.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/direct_command.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/direct_command.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/engine_version_request.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/engine_version_request.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/enter_linking_mode.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/enter_linking_mode.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/enter_unlinking_mode.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/enter_unlinking_mode.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/extended_get.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/extended_get.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/extended_set.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/extended_set.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/factory_reset.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/factory_reset.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/get_operating_flags.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/get_operating_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/group_off.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/group_off.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/group_on.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/group_on.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/id_request.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/id_request.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/night_mode_off.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/night_mode_off.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/night_mode_on.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/night_mode_on.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/off.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/off.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/off_all_link_cleanup.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/off_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/off_fast.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/off_fast.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/on_fast.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/on_fast.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/on_level.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/on_level.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/on_level_all_link_cleanup.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/on_level_all_link_cleanup.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/peek.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/peek.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/ping.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/ping.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/poke.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/poke.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/product_data_request.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/product_data_request.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/read_aldb.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/read_aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/set_leds.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/set_leds.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/set_msb.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/set_msb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/set_operating_flags.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/set_operating_flags.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/status_request.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/status_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """Manage outbound ON command to a device."""
+
 import asyncio
 
 from .. import ack_handler, status_handler
 from ... import pub
 from ...constants import MessageFlagType, ResponseStatus
 from ...topics import STATUS_REQUEST
 from .direct_command import DirectCommandHandlerBase
 
 
 class StatusRequestCommand(DirectCommandHandlerBase):
     """Manage an outbound Status command to a device."""
 
     def __init__(self, address, status_type: int = 0):
         """Init the OnLevelCommand class."""
-        super().__init__(topic=STATUS_REQUEST, address=address, group=None)
         self._status_type = status_type
+        super().__init__(topic=STATUS_REQUEST, address=address, group=None)
         self._subscriber_topic = f"handler.{self._address.id}.{self._status_type}.{STATUS_REQUEST}.{str(MessageFlagType.DIRECT).lower()}"
 
+    @property
+    def status_type(self):
+        """Return the status type."""
+        return self._status_type
+
     # pylint: disable=arguments-differ, useless-super-delegation
     async def async_send(self):
         """Send the ON command async."""
         return await super().async_send(status_type=self._status_type)
 
     @ack_handler
     async def async_handle_ack(self, cmd1, cmd2, user_data):
```

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/temperature_down.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/temperature_down.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/temperature_up.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/temperature_up.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/thermostat_cool_set_point.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/thermostat_cool_set_point.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/thermostat_heat_set_point.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/thermostat_heat_set_point.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/thermostat_mode.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/thermostat_mode.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/trigger_scene_off.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/trigger_scene_off.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/trigger_scene_on.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/trigger_scene_on.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/write_aldb.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/write_aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/to_device/x10_send.py` & `pyinsteon-1.6.0/pyinsteon/handlers/to_device/x10_send.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/handlers/write_eeprom.py` & `pyinsteon-1.6.0/pyinsteon/handlers/write_eeprom.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/aldb_im_read_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/aldb_im_read_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/aldb_im_write_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/aldb_im_write_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/aldb_read_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/aldb_read_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/aldb_write_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/aldb_write_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/device_id_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/device_id_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/device_link_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/device_link_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/device_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/device_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/ext_get_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/ext_get_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/ext_prop_read_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/ext_prop_read_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/ext_prop_write_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/ext_prop_write_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/get_set_ext_property_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/get_set_ext_property_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/get_set_op_flag_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/get_set_op_flag_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/heartbeat_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/heartbeat_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/link_manager/__init__.py` & `pyinsteon-1.6.0/pyinsteon/managers/link_manager/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,58 +65,84 @@
     return EngineVersion.UNKNOWN
 
 
 async def async_enter_linking_mode(
     link_mode: AllLinkMode, group: int, address: Address = None
 ):
     """Put the Insteon Modem into linking mode."""
-
     if address is not None:
+        # pylint: disable=import-outside-toplevel
+        from ... import devices
+
         address = Address(address)
-        engine_version = await _get_engine_version(address)
+        device = devices[address]
+        if device:
+            engine_version = device.engine_version
+        else:
+            engine_version = await _get_engine_version(address)
 
     link_cmd = StartAllLinkingCommandHandler()
     response_modem = await link_cmd.async_send(link_mode=link_mode, group=group)
     _LOGGER.debug("Enter linking mode modem response: %s", str(response_modem))
 
-    response_device = None
+    response_device = ResponseStatus.UNSENT
     if address is not None:
-        extended = engine_version == EngineVersion.I2CS
+        extended = engine_version in [EngineVersion.I2CS, EngineVersion.UNKNOWN]
         device_link_cmd = EnterLinkingModeCommand(address)
-        response_device = await device_link_cmd.async_send(
-            group=group, extended=extended
-        )
-        if response_device != ResponseStatus.SUCCESS:
+        retries = 3
+        while retries and response_device != ResponseStatus.SUCCESS:
+            response_device = await device_link_cmd.async_send(
+                group=group, extended=extended
+            )
+            retries -= 1
+        retries = 3
+        while retries and response_device != ResponseStatus.SUCCESS:
             response_device = await device_link_cmd.async_send(
                 group=group, extended=not extended
             )
+            retries -= 1
         _LOGGER.debug("Enter linking mode device response: %s", str(response_device))
     return response_modem, response_device
 
 
 async def async_enter_unlinking_mode(group: int, address: Address = None):
     """Put the Insteon Modem into unlinking mode."""
+
     if address is not None:
+        # pylint: disable=import-outside-toplevel
+        from ... import devices
+
         address = Address(address)
-        engine_version = await _get_engine_version(address)
+        device = devices[address]
+        if device:
+            engine_version = device.engine_version
+        else:
+            engine_version = await _get_engine_version(address)
     modem_link_cmd = StartAllLinkingCommandHandler()
     link_mode = AllLinkMode.DELETE
     response_modem = await modem_link_cmd.async_send(link_mode=link_mode, group=group)
 
     _LOGGER.debug("Enter linking mode modem response: %s", str(response_modem))
 
-    response_device = None
+    response_device = ResponseStatus.UNSENT
     if address is not None:
-        extended = engine_version == EngineVersion.I2CS
+        extended = engine_version in [EngineVersion.I2CS, EngineVersion.UNKNOWN]
         device_link_cmd = EnterUnlinkingModeCommand(address)
-        await device_link_cmd.async_send(group=group, extended=extended)
-        if response_device != ResponseStatus.SUCCESS:
+        retries = 3
+        while retries and response_device != ResponseStatus.SUCCESS:
+            response_device = await device_link_cmd.async_send(
+                group=group, extended=extended
+            )
+            retries -= 1
+        retries = 3
+        while retries and response_device != ResponseStatus.SUCCESS:
             response_device = await device_link_cmd.async_send(
                 group=group, extended=not extended
             )
+            retries -= 1
         _LOGGER.debug("Enter linking mode device response: %s", str(response_device))
 
     return response_modem, response_device
 
 
 async def async_link_devices(
     controller: Device, responder: Device, group: int = 0, data1=255, data2=28, data3=1
```

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/link_manager/default_links.py` & `pyinsteon-1.6.0/pyinsteon/managers/link_manager/default_links.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/low_batter_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/low_batter_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/on_level_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/on_level_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/peek_poke_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/peek_poke_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/saved_devices_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/saved_devices_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/scene_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/scene_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/thermostat_status_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/thermostat_status_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Thermostat status manager."""
+
 import asyncio
 from collections import namedtuple
 import logging
 
 from ..address import Address
 from ..constants import ResponseStatus, ThermostatMode
 from ..handlers.from_device.ext_get_response import ExtendedGetResponseHandler
@@ -66,15 +67,15 @@
         )
         self._set_point_received_topic = (
             f"{self._address.id}.thermostat_status_manager.set_point_received"
         )
         self._status_listeners = []
         self._set_point_listeners = []
 
-    async def async_status(self):
+    async def async_status(self, group=None):
         """Read the device status."""
         status1 = await self._status()
         status2 = await self._set_point()
         return multiple_status(status1, status2)
 
     def subscribe_status(self, listener, force_strong_ref=False):
         """Subscribe to status updates."""
```

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/utils.py` & `pyinsteon-1.6.0/pyinsteon/managers/utils.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/wet_dry_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/wet_dry_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/managers/x10_manager.py` & `pyinsteon-1.6.0/pyinsteon/managers/x10_manager.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/__init__.py` & `pyinsteon-1.6.0/pyinsteon/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/command_to_msg.py` & `pyinsteon-1.6.0/pyinsteon/protocol/command_to_msg.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/http_reader_writer.py` & `pyinsteon-1.6.0/pyinsteon/protocol/http_reader_writer.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/http_transport.py` & `pyinsteon-1.6.0/pyinsteon/protocol/http_transport.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/messages/__init__.py` & `pyinsteon-1.6.0/pyinsteon/protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/messages/inbound.py` & `pyinsteon-1.6.0/pyinsteon/protocol/messages/inbound.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/messages/message_definition.py` & `pyinsteon-1.6.0/pyinsteon/protocol/messages/message_definition.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/messages/message_definitions.py` & `pyinsteon-1.6.0/pyinsteon/protocol/messages/message_definitions.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/messages/outbound.py` & `pyinsteon-1.6.0/pyinsteon/protocol/messages/outbound.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/mock/mock_reader.py` & `pyinsteon-1.6.0/pyinsteon/protocol/mock/mock_reader.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/mock/mock_transport.py` & `pyinsteon-1.6.0/pyinsteon/protocol/mock/mock_transport.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/msg_to_topic.py` & `pyinsteon-1.6.0/pyinsteon/protocol/msg_to_topic.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/msg_to_url.py` & `pyinsteon-1.6.0/pyinsteon/protocol/msg_to_url.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/protocol.py` & `pyinsteon-1.6.0/pyinsteon/protocol/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 import asyncio
 from enum import Enum
 import logging
 from queue import SimpleQueue
 from typing import Union
 
+from ..address import Address
 from ..constants import AckNak
 from ..utils import log_error, publish_topic
 from .command_to_msg import register_command_handlers
 from .messages.inbound import create
 from .messages.outbound import outbound_write_manager, register_outbound_handlers
 from .msg_to_topic import convert_to_topic
 
 _LOGGER = logging.getLogger(__name__)
+_LOGGER_PYINSTEON = logging.getLogger("pyinsteon")
 _LOGGER_MSG = logging.getLogger("pyinsteon.messages")
 MAX_RECONNECT_WAIT_TIME = 300
 
 
 def _get_addresses_in_msg(msg):
     """Return a list of addresses included in a message."""
     addresses = []
@@ -33,17 +35,19 @@
     return addresses
 
 
 # pylint: disable=broad-except
 async def _publish_message(msg):
     """Convert an inbound message to a topic and publish to listeners."""
     _LOGGER_MSG.debug("RX: %s", repr(msg))
-    if _LOGGER_MSG.level == 0 or _LOGGER_MSG.level > logging.DEBUG:
+    if (_LOGGER_MSG.level == 0 or _LOGGER_MSG.level > logging.DEBUG) and (
+        _LOGGER_PYINSTEON.level == 0 or _LOGGER_PYINSTEON.level > logging.DEBUG
+    ):
         for addr in _get_addresses_in_msg(msg):
-            logger = logging.getLogger(f"pyinsteon.{addr.id}")
+            logger = logging.getLogger(f"pyinsteon.{Address(addr).id}")
             logger.debug("RX: %s", repr(msg))
     topic = None
     kwargs = {}
     try:
         for topic, kwargs in convert_to_topic(msg):
             publish_topic(topic, **kwargs)
     except ValueError:
@@ -221,17 +225,22 @@
             _LOGGER.debug("Modem writer started.")
             try:
                 while self._transport and not self._transport.is_closing():
                     _, msg = await self._message_queue.get()
                     if msg is None:
                         return
                     _LOGGER_MSG.debug("TX: %s", repr(msg))
-                    if _LOGGER_MSG.level == 0 or _LOGGER_MSG.level > logging.DEBUG:
+                    if (
+                        _LOGGER_MSG.level == 0 or _LOGGER_MSG.level > logging.DEBUG
+                    ) and (
+                        _LOGGER_PYINSTEON.level == 0
+                        or _LOGGER_PYINSTEON.level > logging.DEBUG
+                    ):
                         for addr in _get_addresses_in_msg(msg):
-                            logger = logging.getLogger(f"pyinsteon.{addr.id}")
+                            logger = logging.getLogger(f"pyinsteon.{Address(addr).id}")
                             logger.debug("TX: %s", repr(msg))
                     while not self._last_message.empty():
                         self._last_message.get()
                     self._last_message.put(msg)
                     await self._transport.async_write(msg)
                     await asyncio.sleep(self._transport.write_wait)
             except RuntimeError as error:
```

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/serial_transport.py` & `pyinsteon-1.6.0/pyinsteon/protocol/serial_transport.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/protocol/topic_converters.py` & `pyinsteon-1.6.0/pyinsteon/protocol/topic_converters.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/subscriber_base.py` & `pyinsteon-1.6.0/pyinsteon/subscriber_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/tools/__init__.py` & `pyinsteon-1.6.0/pyinsteon/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/tools/advanced.py` & `pyinsteon-1.6.0/pyinsteon/tools/advanced.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/tools/aldb.py` & `pyinsteon-1.6.0/pyinsteon/tools/aldb.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/tools/commands.py` & `pyinsteon-1.6.0/pyinsteon/tools/commands.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/tools/config.py` & `pyinsteon-1.6.0/pyinsteon/tools/config.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/tools/log_filter.py` & `pyinsteon-1.6.0/pyinsteon/tools/log_filter.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/tools/scenes.py` & `pyinsteon-1.6.0/pyinsteon/tools/scenes.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/tools/tools_base.py` & `pyinsteon-1.6.0/pyinsteon/tools/tools_base.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/tools/utils.py` & `pyinsteon-1.6.0/pyinsteon/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon/topics.py` & `pyinsteon-1.6.0/pyinsteon/topics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants used to ensure topic consistantancy."""
+
 DEVICE_LIST_CHANGED = "device_list_changed"
 
 STANDARD_RECEIVED = "standard_message_received"
 EXTENDED_RECEIVED = "extended_message_received"
 X10_RECEIVED = "x10_received"
 ALL_LINKING_COMPLETED = "all_linking_completed"
 BUTTON_EVENT_REPORT = "button_event_report"
@@ -70,17 +71,19 @@
 SET_STATUS = "set_status"
 SET_ADDRESS_MSB = "set_address_msb"
 POKE = "poke"
 PEEK = "peek"
 PEEK_INTERNAL = "peek_internal"
 POKE_INTERNAL = "poke_internal"
 ON_AT_RAMP_RATE = "on_at_ramp_rate"
+ON_AT_RAMP_RATE_INBOUND = "on_at_ramp_rate_inbound"
 EXTENDED_GET_SET = "extended_get_set"
 EXTENDED_GET_RESPONSE = "extended_get_response"
 OFF_AT_RAMP_RATE = "off_at_ramp_rate"
+OFF_AT_RAMP_RATE_INBOUND = "off_at_ramp_rate_inbound"
 EXTENDED_READ_WRITE_ALDB = "extended_read_write_aldb"
 EXTENDED_TRIGGER_ALL_LINK = "extended_trigger_all_link"
 ALDB_RECORD_RECEIVED = "aldb_record_received"
 BEEP = "beep"
 GROUP_ON = "group_on"
 GROUP_OFF = "group_off"
 FACTORY_RESET = "factory_reset"
```

### Comparing `pyinsteon-1.5.3/pyinsteon/utils.py` & `pyinsteon-1.6.0/pyinsteon/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility methods."""
+
 import asyncio
 from collections.abc import Iterable
 from enum import Enum, IntEnum
 from functools import partial, wraps
 from inspect import isawaitable, iscoroutinefunction
 import logging
 import traceback
@@ -308,14 +309,19 @@
 
 def publish_topic(topic, logger=None, **kwargs):
     """Publish a topic and log errors."""
     # Send log message as caller not utils.
     if logger is None:
         logger = logging.getLogger(__name__)
     try:
+        pub_topic = pub.getDefaultTopicMgr().getTopic(topic, okIfNone=True)
+        if pub_topic:
+            for listener in pub_topic.listeners:
+                if listener.isDead():
+                    pub_topic.unsubscribe(listener)
         pub.sendMessage(topic, **kwargs)
     except pub.ExcHandlerError as exc:
         logger.error("pubsub ExcHandlerError")
         logger.error("Error processing topic: %s", topic)
         logger.error("Error in topic listner: %s", exc.badExcListenerID)
     except pub.SenderMissingReqdMsgDataError as exc:
         logger.error("SenderMissingReqdMsgDataError")
```

### Comparing `pyinsteon-1.5.3/pyinsteon/x10_address.py` & `pyinsteon-1.6.0/pyinsteon/x10_address.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/pyinsteon.egg-info/PKG-INFO` & `pyinsteon-1.6.0/pyinsteon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pyinsteon
-Version: 1.5.3
+Version: 1.6.0
 Summary: Open-source Insteon home automation module running on Python 3.
 Author-email: The pyinsteon authors <pyinsteon@harrisnj.net>
 License: MIT License
 Project-URL: Source Code, https://github.com/pyinsteon/pyinsteon
 Project-URL: Bug Reports, https://github.com/pyinsteon/pyinsteon/issues
 Keywords: home,automation,insteon,python,python3
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Home Automation
-Requires-Python: >=3.8.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: pyserial
 Requires-Dist: pyserial-asyncio>=0.5
 Requires-Dist: aiohttp
 Requires-Dist: pypubsub
 Requires-Dist: aiofiles
@@ -42,15 +42,15 @@
 platform for the `Home Assistant <https://home-assistant.io/>`__
 automation platform but it is structured to be general-purpose and
 should be usable for other applications as well.
 
 Requirements
 ------------
 
--  Python 3.8, 3.9, 3.10 or 3.11
+-  Python 3.9, 3.10 or 3.11, 3.12
 -  Posix or Windows based system
 -  Some form of Insteon PLM or Hub
 -  At least one Insteon device
 
 Installation
 ------------
```

### Comparing `pyinsteon-1.5.3/pyinsteon.egg-info/SOURCES.txt` & `pyinsteon-1.6.0/pyinsteon.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -113,16 +113,18 @@
 pyinsteon/handlers/from_device/assign_to_all_link_group.py
 pyinsteon/handlers/from_device/broadcast_command.py
 pyinsteon/handlers/from_device/delete_from_all_link_group.py
 pyinsteon/handlers/from_device/ext_get_response.py
 pyinsteon/handlers/from_device/manual_change.py
 pyinsteon/handlers/from_device/off.py
 pyinsteon/handlers/from_device/off_all_link_cleanup.py
+pyinsteon/handlers/from_device/off_at_ramp_rate.py
 pyinsteon/handlers/from_device/off_fast.py
 pyinsteon/handlers/from_device/off_fast_all_link_cleanup.py
+pyinsteon/handlers/from_device/on_at_ramp_rate.py
 pyinsteon/handlers/from_device/on_fast.py
 pyinsteon/handlers/from_device/on_fast_all_link_cleanup.py
 pyinsteon/handlers/from_device/on_level.py
 pyinsteon/handlers/from_device/on_level_all_link_cleanup.py
 pyinsteon/handlers/from_device/receive_aldb_record.py
 pyinsteon/handlers/from_device/thermostat_cool_set_point.py
 pyinsteon/handlers/from_device/thermostat_heat_set_point.py
@@ -184,14 +186,15 @@
 pyinsteon/managers/get_set_op_flag_manager.py
 pyinsteon/managers/heartbeat_manager.py
 pyinsteon/managers/low_batter_manager.py
 pyinsteon/managers/on_level_manager.py
 pyinsteon/managers/peek_poke_manager.py
 pyinsteon/managers/saved_devices_manager.py
 pyinsteon/managers/scene_manager.py
+pyinsteon/managers/status_manager.py
 pyinsteon/managers/thermostat_status_manager.py
 pyinsteon/managers/utils.py
 pyinsteon/managers/wet_dry_manager.py
 pyinsteon/managers/x10_manager.py
 pyinsteon/managers/link_manager/__init__.py
 pyinsteon/managers/link_manager/default_links.py
 pyinsteon/protocol/__init__.py
```

### Comparing `pyinsteon-1.5.3/pyproject.toml` & `pyinsteon-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "pyinsteon"
-version     = "1.5.3"
+version     = "1.6.0"
 license     = {text = "MIT License"}
 description = "Open-source Insteon home automation module running on Python 3."
 readme      = "DESCRIPTION.rst"
 authors     = [
     {name = "The pyinsteon authors", email = "pyinsteon@harrisnj.net"}
 ]
 keywords    = ["home", "automation", "insteon", "python", "python3"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Home Automation",
 ]
-requires-python = ">=3.8.0"
+requires-python = ">=3.9.0"
 dependencies    = [
         "pyserial",
         "pyserial-asyncio>=0.5",
         "aiohttp",
         "pypubsub",
         "aiofiles",
         "voluptuous",
@@ -181,14 +181,17 @@
     "too-many-locals",
     "too-many-public-methods",
     "too-many-return-statements",
     "too-many-statements",
     "line-too-long",
     "deprecated-typing-alias",
     "consider-alternative-union-syntax",
+    "duplicate-code",  # to be added back after cleanup
+    "cyclic-import",
+    "use-yield-from"
 ]
 enable = [
     #"useless-suppression",  # temporarily every now and then to clean them up
     "use-symbolic-message-instead",
 ]
 
 [tool.pylint.REPORTS]
```

### Comparing `pyinsteon-1.5.3/tests/test_address.py` & `pyinsteon-1.6.0/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `pyinsteon-1.5.3/tests/test_x10_address.py` & `pyinsteon-1.6.0/tests/test_x10_address.py`

 * *Files identical despite different names*

