# Comparing `tmp/vital-2.1.7.tar.gz` & `tmp/vital-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-2.1.7.tar", max compression
+gzip compressed data, was "vital-2.1.8.tar", max compression
```

## Comparing `vital-2.1.7.tar` & `vital-2.1.8.tar`

### file list

```diff
@@ -1,282 +1,284 @@
--rw-r--r--   0        0        0     3329 2024-05-03 11:59:10.065057 vital-2.1.7/README.md
--rw-r--r--   0        0        0      396 2024-05-03 11:59:10.069057 vital-2.1.7/pyproject.toml
--rw-r--r--   0        0        0    14691 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/__init__.py
--rw-r--r--   0        0        0     5248 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/client.py
--rw-r--r--   0        0        0      519 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/core/api_error.py
--rw-r--r--   0        0        0     1080 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      308 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/environment.py
--rw-r--r--   0        0        0      236 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/errors/bad_request_error.py
--rw-r--r--   0        0        0      313 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/py.typed
--rw-r--r--   0        0        0      532 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/activity/__init__.py
--rw-r--r--   0        0        0     8604 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/activity/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/body/__init__.py
--rw-r--r--   0        0        0     8520 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/body/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/devices/__init__.py
--rw-r--r--   0        0        0     3641 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/devices/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/insurance/__init__.py
--rw-r--r--   0        0        0     6695 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/insurance/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/introspect/__init__.py
--rw-r--r--   0        0        0     8197 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/introspect/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/lab_tests/__init__.py
--rw-r--r--   0        0        0    67299 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/lab_tests/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/link/__init__.py
--rw-r--r--   0        0        0    44285 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/link/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/meal/__init__.py
--rw-r--r--   0        0        0     4703 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/meal/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/profile/__init__.py
--rw-r--r--   0        0        0     5698 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/profile/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/providers/__init__.py
--rw-r--r--   0        0        0     2668 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/providers/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/sleep/__init__.py
--rw-r--r--   0        0        0    15040 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/sleep/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/team/__init__.py
--rw-r--r--   0        0        0    18010 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/team/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/testkit/__init__.py
--rw-r--r--   0        0        0     8435 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/testkit/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/user/__init__.py
--rw-r--r--   0        0        0    36394 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/user/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/vitals/__init__.py
--rw-r--r--   0        0        0   209296 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/vitals/client.py
--rw-r--r--   0        0        0       65 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/workouts/__init__.py
--rw-r--r--   0        0        0    11221 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/resources/workouts/client.py
--rw-r--r--   0        0        0    21454 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/__init__.py
--rw-r--r--   0        0        0     1103 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/activity_v_2_in_db.py
--rw-r--r--   0        0        0      967 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/address.py
--rw-r--r--   0        0        0      971 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/appointment_availability_slots.py
--rw-r--r--   0        0        0     1074 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/appointment_event_status.py
--rw-r--r--   0        0        0      748 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/appointment_provider.py
--rw-r--r--   0        0        0      661 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/appointment_service_type.py
--rw-r--r--   0        0        0     1044 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/appointment_status.py
--rw-r--r--   0        0        0      149 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/appointment_type.py
--rw-r--r--   0        0        0      957 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/area_info.py
--rw-r--r--   0        0        0      510 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/attempt_status.py
--rw-r--r--   0        0        0      649 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/auth_type.py
--rw-r--r--   0        0        0      537 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/availability.py
--rw-r--r--   0        0        0     1468 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/biomarker_result.py
--rw-r--r--   0        0        0     1168 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/body_v_2_in_db.py
--rw-r--r--   0        0        0      970 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_activity_response.py
--rw-r--r--   0        0        0      950 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_body_response.py
--rw-r--r--   0        0        0     3581 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_activity.py
--rw-r--r--   0        0        0     1010 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_api_key.py
--rw-r--r--   0        0        0     1815 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_appointment.py
--rw-r--r--   0        0        0      934 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_appointment_cancellation_reason.py
--rw-r--r--   0        0        0     1051 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_appointment_event.py
--rw-r--r--   0        0        0     1193 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_at_home_phlebotomy_order.py
--rw-r--r--   0        0        0     1030 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_at_home_phlebotomy_order_details.py
--rw-r--r--   0        0        0     1634 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_blood_oxygen_timeseries.py
--rw-r--r--   0        0        0     1632 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_blood_pressure_timeseries.py
--rw-r--r--   0        0        0     1637 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_body.py
--rw-r--r--   0        0        0     1631 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_body_fat_timeseries.py
--rw-r--r--   0        0        0     1630 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_body_weight_timeseries.py
--rw-r--r--   0        0        0     1859 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_caffeine_timeseries.py
--rw-r--r--   0        0        0     1919 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_calories_active_timeseries.py
--rw-r--r--   0        0        0     1658 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_calories_basal_timeseries.py
--rw-r--r--   0        0        0     1623 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_cholesterol_timeseries.py
--rw-r--r--   0        0        0     1071 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_diagnosis_information.py
--rw-r--r--   0        0        0     1874 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_distance_timeseries.py
--rw-r--r--   0        0        0     1540 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py
--rw-r--r--   0        0        0     1656 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_floors_climbed_timeseries.py
--rw-r--r--   0        0        0     1048 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_food.py
--rw-r--r--   0        0        0     1619 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_glucose_timeseries.py
--rw-r--r--   0        0        0     1236 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_heart_rate.py
--rw-r--r--   0        0        0     1606 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_heart_rate_timeseries.py
--rw-r--r--   0        0        0     1624 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_hrv_timeseries.py
--rw-r--r--   0        0        0     1968 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_hypnogram_timeseries.py
--rw-r--r--   0        0        0     1612 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_ige_timeseries.py
--rw-r--r--   0        0        0     1612 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_igg_timeseries.py
--rw-r--r--   0        0        0     1183 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_lab.py
--rw-r--r--   0        0        0     1780 2024-05-03 11:59:10.069057 vital-2.1.7/src/vital/types/client_facing_lab_test.py
--rw-r--r--   0        0        0      945 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_loinc.py
--rw-r--r--   0        0        0     1147 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_marker.py
--rw-r--r--   0        0        0     1262 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_marker_complete.py
--rw-r--r--   0        0        0     1003 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_meal_response.py
--rw-r--r--   0        0        0     1861 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_mindfulness_minutes_timeseries.py
--rw-r--r--   0        0        0     3286 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_order.py
--rw-r--r--   0        0        0     1311 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_order_details.py
--rw-r--r--   0        0        0      967 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_order_event.py
--rw-r--r--   0        0        0     1060 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_patient_details_compatible.py
--rw-r--r--   0        0        0     1239 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_payor_search_response.py
--rw-r--r--   0        0        0      916 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_physician.py
--rw-r--r--   0        0        0     1210 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_profile.py
--rw-r--r--   0        0        0     1164 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_provider.py
--rw-r--r--   0        0        0     1418 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_provider_detailed.py
--rw-r--r--   0        0        0     1302 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_provider_with_status.py
--rw-r--r--   0        0        0     6046 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_resource.py
--rw-r--r--   0        0        0     1639 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_respiratory_rate_timeseries.py
--rw-r--r--   0        0        0     1088 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_result.py
--rw-r--r--   0        0        0     1862 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_shipment.py
--rw-r--r--   0        0        0     4877 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_sleep.py
--rw-r--r--   0        0        0     1497 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_sleep_stream.py
--rw-r--r--   0        0        0     1898 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_source.py
--rw-r--r--   0        0        0     1003 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_sport.py
--rw-r--r--   0        0        0     1867 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_steps_timeseries.py
--rw-r--r--   0        0        0     1447 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_stream.py
--rw-r--r--   0        0        0     1573 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_stress_level_timeseries.py
--rw-r--r--   0        0        0     1936 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_team.py
--rw-r--r--   0        0        0      992 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_test_kit_order_details.py
--rw-r--r--   0        0        0     1273 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_testkit_order.py
--rw-r--r--   0        0        0     2915 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_user.py
--rw-r--r--   0        0        0     1367 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_user_key.py
--rw-r--r--   0        0        0     1844 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_vo_2_max_timeseries.py
--rw-r--r--   0        0        0     1002 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_walk_in_order_details.py
--rw-r--r--   0        0        0     1129 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_walk_in_test_order.py
--rw-r--r--   0        0        0     1638 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_water_timeseries.py
--rw-r--r--   0        0        0     4268 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_facing_workout.py
--rw-r--r--   0        0        0      955 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_sleep_response.py
--rw-r--r--   0        0        0      951 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_user_id_conflict.py
--rw-r--r--   0        0        0      966 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/client_workout_response.py
--rw-r--r--   0        0        0     1271 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/connected_source_client_facing.py
--rw-r--r--   0        0        0     1077 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/connection_status.py
--rw-r--r--   0        0        0      487 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/connection_status_state.py
--rw-r--r--   0        0        0     1126 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/consent.py
--rw-r--r--   0        0        0     1519 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/consent_type.py
--rw-r--r--   0        0        0      930 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/day_slots.py
--rw-r--r--   0        0        0     1240 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/delegated_flow_type.py
--rw-r--r--   0        0        0      897 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/demo_connection_status.py
--rw-r--r--   0        0        0      892 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/demo_providers.py
--rw-r--r--   0        0        0     1053 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/device_v_2_in_db.py
--rw-r--r--   0        0        0      153 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/email_providers.py
--rw-r--r--   0        0        0      936 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/energy.py
--rw-r--r--   0        0        0     1172 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/event_destination_preferences.py
--rw-r--r--   0        0        0      762 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/event_destination_preferences_enabled_item.py
--rw-r--r--   0        0        0      754 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/event_destination_preferences_preferred.py
--rw-r--r--   0        0        0     1169 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/fallback_birth_date.py
--rw-r--r--   0        0        0     1376 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/fallback_time_zone.py
--rw-r--r--   0        0        0     1623 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/fats.py
--rw-r--r--   0        0        0      762 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/gender.py
--rw-r--r--   0        0        0     1110 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/get_markers_response.py
--rw-r--r--   0        0        0     1048 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/get_orders_response.py
--rw-r--r--   0        0        0     1087 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_blood_oxygen.py
--rw-r--r--   0        0        0     1254 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_blood_oxygen_response.py
--rw-r--r--   0        0        0     1095 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_blood_pressure.py
--rw-r--r--   0        0        0     1262 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_blood_pressure_response.py
--rw-r--r--   0        0        0     1071 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_body_fat.py
--rw-r--r--   0        0        0     1238 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_body_fat_response.py
--rw-r--r--   0        0        0     1083 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_body_weight.py
--rw-r--r--   0        0        0     1250 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_body_weight_response.py
--rw-r--r--   0        0        0     1074 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_caffeine.py
--rw-r--r--   0        0        0     1241 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_caffeine_response.py
--rw-r--r--   0        0        0     1099 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_calories_active.py
--rw-r--r--   0        0        0     1266 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_calories_active_response.py
--rw-r--r--   0        0        0     1095 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_calories_basal.py
--rw-r--r--   0        0        0     1262 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_calories_basal_response.py
--rw-r--r--   0        0        0     1086 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_cholesterol.py
--rw-r--r--   0        0        0     1253 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_cholesterol_response.py
--rw-r--r--   0        0        0     1074 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_distance.py
--rw-r--r--   0        0        0     1241 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_distance_response.py
--rw-r--r--   0        0        0     1139 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_electrocardiogram_voltage.py
--rw-r--r--   0        0        0     1306 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_electrocardiogram_voltage_response.py
--rw-r--r--   0        0        0     1095 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_floors_climbed.py
--rw-r--r--   0        0        0     1262 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_floors_climbed_response.py
--rw-r--r--   0        0        0     1070 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_glucose.py
--rw-r--r--   0        0        0     1237 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_glucose_response.py
--rw-r--r--   0        0        0     1079 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_heart_rate.py
--rw-r--r--   0        0        0     1246 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_heart_rate_response.py
--rw-r--r--   0        0        0     1054 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_hrv.py
--rw-r--r--   0        0        0     1221 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_hrv_response.py
--rw-r--r--   0        0        0     1078 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_hypnogram.py
--rw-r--r--   0        0        0     1245 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_hypnogram_response.py
--rw-r--r--   0        0        0     1054 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_ige.py
--rw-r--r--   0        0        0     1221 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_ige_response.py
--rw-r--r--   0        0        0     1054 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_igg.py
--rw-r--r--   0        0        0     1221 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_igg_response.py
--rw-r--r--   0        0        0     1115 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_mindfulness_minutes.py
--rw-r--r--   0        0        0     1282 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_mindfulness_minutes_response.py
--rw-r--r--   0        0        0     1103 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_respiratory_rate.py
--rw-r--r--   0        0        0     1270 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_respiratory_rate_response.py
--rw-r--r--   0        0        0     1062 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_steps.py
--rw-r--r--   0        0        0     1229 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_steps_response.py
--rw-r--r--   0        0        0     1087 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_stress_level.py
--rw-r--r--   0        0        0     1254 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_stress_level_response.py
--rw-r--r--   0        0        0     1068 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_vo_2_max.py
--rw-r--r--   0        0        0     1235 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_vo_2_max_response.py
--rw-r--r--   0        0        0     1062 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_water.py
--rw-r--r--   0        0        0     1229 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/grouped_water_response.py
--rw-r--r--   0        0        0     3022 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/health_insurance_create_request.py
--rw-r--r--   0        0        0      811 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/health_insurance_create_request_back_image.py
--rw-r--r--   0        0        0      816 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/health_insurance_create_request_front_image.py
--rw-r--r--   0        0        0      876 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/health_insurance_create_request_patient_signature_image.py
--rw-r--r--   0        0        0      732 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/historical_pull_status.py
--rw-r--r--   0        0        0      966 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/http_validation_error.py
--rw-r--r--   0        0        0      864 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/jpeg.py
--rw-r--r--   0        0        0     1289 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/lab_results_metadata.py
--rw-r--r--   0        0        0     1034 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/lab_results_raw.py
--rw-r--r--   0        0        0      223 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/lab_results_raw_results.py
--rw-r--r--   0        0        0      827 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/lab_test_collection_method.py
--rw-r--r--   0        0        0      898 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/lab_test_sample_type.py
--rw-r--r--   0        0        0      729 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/lab_test_status.py
--rw-r--r--   0        0        0      949 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/last_attempt.py
--rw-r--r--   0        0        0      936 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/libre_config.py
--rw-r--r--   0        0        0      960 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/link_token_exchange_response.py
--rw-r--r--   0        0        0      879 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/lng_lat.py
--rw-r--r--   0        0        0     1553 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/macros.py
--rw-r--r--   0        0        0     1792 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/manual_providers.py
--rw-r--r--   0        0        0      501 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/marker_type.py
--rw-r--r--   0        0        0     1444 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/meal_in_db_base_client_facing_source.py
--rw-r--r--   0        0        0     1233 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/metrics_result.py
--rw-r--r--   0        0        0     1272 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/micros.py
--rw-r--r--   0        0        0     2126 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/o_auth_providers.py
--rw-r--r--   0        0        0     9798 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/order_status.py
--rw-r--r--   0        0        0     1265 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/order_top_level_status.py
--rw-r--r--   0        0        0     1001 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/paginated_users_response.py
--rw-r--r--   0        0        0     1779 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/password_providers.py
--rw-r--r--   0        0        0     1063 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/patient_address_compatible.py
--rw-r--r--   0        0        0     1000 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/patient_details.py
--rw-r--r--   0        0        0     1004 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/person_details.py
--rw-r--r--   0        0        0      993 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/phlebotomy_area_info.py
--rw-r--r--   0        0        0     1065 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/phlebotomy_provider_info.py
--rw-r--r--   0        0        0     1281 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/physician_create_request.py
--rw-r--r--   0        0        0     1008 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/physician_create_request_base.py
--rw-r--r--   0        0        0      806 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/physician_create_request_signature_image.py
--rw-r--r--   0        0        0      863 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/png.py
--rw-r--r--   0        0        0      973 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/post_order_response.py
--rw-r--r--   0        0        0     1106 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/profile_in_db.py
--rw-r--r--   0        0        0     1177 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/provider_link_response.py
--rw-r--r--   0        0        0      499 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/provider_link_response_state.py
--rw-r--r--   0        0        0     5156 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/providers.py
--rw-r--r--   0        0        0      943 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/raw_activity.py
--rw-r--r--   0        0        0      923 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/raw_body.py
--rw-r--r--   0        0        0      935 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/raw_devices.py
--rw-r--r--   0        0        0      917 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/raw_profile.py
--rw-r--r--   0        0        0      928 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/raw_sleep.py
--rw-r--r--   0        0        0      939 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/raw_workout.py
--rw-r--r--   0        0        0     1360 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/region.py
--rw-r--r--   0        0        0     1055 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/resource_availability.py
--rw-r--r--   0        0        0      761 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/responsible_relationship.py
--rw-r--r--   0        0        0      662 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/result_type.py
--rw-r--r--   0        0        0     1000 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/scope_requirements_grants.py
--rw-r--r--   0        0        0      925 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/scope_requirements_str.py
--rw-r--r--   0        0        0     1020 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/shipping_address.py
--rw-r--r--   0        0        0     1146 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/single_historical_pull_statistics.py
--rw-r--r--   0        0        0     1125 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/single_provider_historical_pull_response.py
--rw-r--r--   0        0        0     1081 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/single_resource_statistics.py
--rw-r--r--   0        0        0     1052 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/single_user_historical_pull_response.py
--rw-r--r--   0        0        0     1026 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/single_user_resource_response.py
--rw-r--r--   0        0        0     1152 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/sleep_v_2_in_db.py
--rw-r--r--   0        0        0     1246 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/source.py
--rw-r--r--   0        0        0     1209 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/source_auth_type.py
--rw-r--r--   0        0        0     1123 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/source_link.py
--rw-r--r--   0        0        0      892 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/source_type.py
--rw-r--r--   0        0        0     1303 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/team_config.py
--rw-r--r--   0        0        0     1147 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/time_slot.py
--rw-r--r--   0        0        0      903 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/timeseries_metric_point.py
--rw-r--r--   0        0        0     4865 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/timeseries_resource.py
--rw-r--r--   0        0        0     1138 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/us_address.py
--rw-r--r--   0        0        0     1040 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/user_historical_pulls_response.py
--rw-r--r--   0        0        0     1304 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/user_refresh_error_response.py
--rw-r--r--   0        0        0     1356 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/user_refresh_success_response.py
--rw-r--r--   0        0        0     1015 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/user_resources_response.py
--rw-r--r--   0        0        0      906 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/user_sign_in_token_response.py
--rw-r--r--   0        0        0      952 2024-05-03 11:59:10.073057 vital-2.1.7/src/vital/types/user_success_response.py
--rw-r--r--   0        0        0      992 2024-05-03 11:59:10.077057 vital-2.1.7/src/vital/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-03 11:59:10.077057 vital-2.1.7/src/vital/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      904 2024-05-03 11:59:10.077057 vital-2.1.7/src/vital/types/vital_token_created_response.py
--rw-r--r--   0        0        0     1217 2024-05-03 11:59:10.077057 vital-2.1.7/src/vital/types/workout_v_2_in_db.py
--rw-r--r--   0        0        0     3831 1970-01-01 00:00:00.000000 vital-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3329 2024-05-10 08:37:28.807833 vital-2.1.8/README.md
+-rw-r--r--   0        0        0      396 2024-05-10 08:37:28.807833 vital-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0    14803 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/__init__.py
+-rw-r--r--   0        0        0     5248 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/client.py
+-rw-r--r--   0        0        0      519 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/api_error.py
+-rw-r--r--   0        0        0     1080 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      308 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/environment.py
+-rw-r--r--   0        0        0      236 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/errors/bad_request_error.py
+-rw-r--r--   0        0        0      313 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/py.typed
+-rw-r--r--   0        0        0      532 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/activity/__init__.py
+-rw-r--r--   0        0        0     8604 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/activity/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/body/__init__.py
+-rw-r--r--   0        0        0     8520 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/body/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/devices/__init__.py
+-rw-r--r--   0        0        0     3641 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/devices/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/insurance/__init__.py
+-rw-r--r--   0        0        0     7153 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/insurance/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/introspect/__init__.py
+-rw-r--r--   0        0        0     7869 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/introspect/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/lab_tests/__init__.py
+-rw-r--r--   0        0        0    75759 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/lab_tests/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/link/__init__.py
+-rw-r--r--   0        0        0    44285 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/link/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/meal/__init__.py
+-rw-r--r--   0        0        0     4703 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/meal/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/profile/__init__.py
+-rw-r--r--   0        0        0     6502 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/profile/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/providers/__init__.py
+-rw-r--r--   0        0        0     2668 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/providers/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/sleep/__init__.py
+-rw-r--r--   0        0        0    15040 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/sleep/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/team/__init__.py
+-rw-r--r--   0        0        0    18402 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/team/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/testkit/__init__.py
+-rw-r--r--   0        0        0     8435 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/testkit/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/user/__init__.py
+-rw-r--r--   0        0        0    40454 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/user/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/vitals/__init__.py
+-rw-r--r--   0        0        0   209296 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/vitals/client.py
+-rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/workouts/__init__.py
+-rw-r--r--   0        0        0    11221 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/workouts/client.py
+-rw-r--r--   0        0        0    21631 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/activity_v_2_in_db.py
+-rw-r--r--   0        0        0      967 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/address.py
+-rw-r--r--   0        0        0      971 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_availability_slots.py
+-rw-r--r--   0        0        0     1074 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_event_status.py
+-rw-r--r--   0        0        0      748 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_provider.py
+-rw-r--r--   0        0        0      661 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_service_type.py
+-rw-r--r--   0        0        0     1044 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_status.py
+-rw-r--r--   0        0        0      149 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_type.py
+-rw-r--r--   0        0        0      957 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/area_info.py
+-rw-r--r--   0        0        0      510 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/attempt_status.py
+-rw-r--r--   0        0        0      649 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/auth_type.py
+-rw-r--r--   0        0        0      537 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/availability.py
+-rw-r--r--   0        0        0     1468 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/biomarker_result.py
+-rw-r--r--   0        0        0     1168 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/body_v_2_in_db.py
+-rw-r--r--   0        0        0      970 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_activity_response.py
+-rw-r--r--   0        0        0      950 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_body_response.py
+-rw-r--r--   0        0        0     3581 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_activity.py
+-rw-r--r--   0        0        0     1010 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_api_key.py
+-rw-r--r--   0        0        0     1815 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_appointment.py
+-rw-r--r--   0        0        0      934 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_appointment_cancellation_reason.py
+-rw-r--r--   0        0        0     1051 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_appointment_event.py
+-rw-r--r--   0        0        0     1193 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_at_home_phlebotomy_order.py
+-rw-r--r--   0        0        0     1030 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_at_home_phlebotomy_order_details.py
+-rw-r--r--   0        0        0     1634 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_blood_oxygen_timeseries.py
+-rw-r--r--   0        0        0     1632 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_blood_pressure_timeseries.py
+-rw-r--r--   0        0        0     1637 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_body.py
+-rw-r--r--   0        0        0     1631 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_body_fat_timeseries.py
+-rw-r--r--   0        0        0     1630 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_body_weight_timeseries.py
+-rw-r--r--   0        0        0     1859 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_caffeine_timeseries.py
+-rw-r--r--   0        0        0     1983 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_calories_active_timeseries.py
+-rw-r--r--   0        0        0     1722 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_calories_basal_timeseries.py
+-rw-r--r--   0        0        0     1623 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_cholesterol_timeseries.py
+-rw-r--r--   0        0        0     1071 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_diagnosis_information.py
+-rw-r--r--   0        0        0     1929 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_distance_timeseries.py
+-rw-r--r--   0        0        0     1540 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py
+-rw-r--r--   0        0        0     1707 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_floors_climbed_timeseries.py
+-rw-r--r--   0        0        0     1048 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_food.py
+-rw-r--r--   0        0        0     1619 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_glucose_timeseries.py
+-rw-r--r--   0        0        0     1236 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_heart_rate.py
+-rw-r--r--   0        0        0     1606 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_heart_rate_timeseries.py
+-rw-r--r--   0        0        0     1624 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_hrv_timeseries.py
+-rw-r--r--   0        0        0     1968 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_hypnogram_timeseries.py
+-rw-r--r--   0        0        0     1612 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_ige_timeseries.py
+-rw-r--r--   0        0        0     1612 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_igg_timeseries.py
+-rw-r--r--   0        0        0     1183 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_lab.py
+-rw-r--r--   0        0        0     1780 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_lab_test.py
+-rw-r--r--   0        0        0      945 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_loinc.py
+-rw-r--r--   0        0        0     1147 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_marker.py
+-rw-r--r--   0        0        0     1262 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_marker_complete.py
+-rw-r--r--   0        0        0     1003 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_meal_response.py
+-rw-r--r--   0        0        0     1861 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_mindfulness_minutes_timeseries.py
+-rw-r--r--   0        0        0     3286 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_order.py
+-rw-r--r--   0        0        0     1311 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_order_details.py
+-rw-r--r--   0        0        0      967 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_order_event.py
+-rw-r--r--   0        0        0     1060 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_patient_details_compatible.py
+-rw-r--r--   0        0        0     1239 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_payor_search_response.py
+-rw-r--r--   0        0        0      916 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_physician.py
+-rw-r--r--   0        0        0     1210 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_profile.py
+-rw-r--r--   0        0        0     1164 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_provider.py
+-rw-r--r--   0        0        0     1418 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_provider_detailed.py
+-rw-r--r--   0        0        0     1302 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_provider_with_status.py
+-rw-r--r--   0        0        0     6046 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_resource.py
+-rw-r--r--   0        0        0     1639 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_respiratory_rate_timeseries.py
+-rw-r--r--   0        0        0     1088 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_result.py
+-rw-r--r--   0        0        0     1862 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_shipment.py
+-rw-r--r--   0        0        0     4877 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_sleep.py
+-rw-r--r--   0        0        0     1497 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_sleep_stream.py
+-rw-r--r--   0        0        0     1898 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_source.py
+-rw-r--r--   0        0        0     1003 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_sport.py
+-rw-r--r--   0        0        0     1918 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_steps_timeseries.py
+-rw-r--r--   0        0        0     1447 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_stream.py
+-rw-r--r--   0        0        0     1573 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_stress_level_timeseries.py
+-rw-r--r--   0        0        0     1936 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_team.py
+-rw-r--r--   0        0        0      992 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_test_kit_order_details.py
+-rw-r--r--   0        0        0     1273 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_testkit_order.py
+-rw-r--r--   0        0        0     2915 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_user.py
+-rw-r--r--   0        0        0     1367 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_user_key.py
+-rw-r--r--   0        0        0     1844 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_vo_2_max_timeseries.py
+-rw-r--r--   0        0        0     1002 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_walk_in_order_details.py
+-rw-r--r--   0        0        0     1129 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_walk_in_test_order.py
+-rw-r--r--   0        0        0     1638 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_water_timeseries.py
+-rw-r--r--   0        0        0     4328 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_workout.py
+-rw-r--r--   0        0        0      955 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_sleep_response.py
+-rw-r--r--   0        0        0      951 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_user_id_conflict.py
+-rw-r--r--   0        0        0      966 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_workout_response.py
+-rw-r--r--   0        0        0     1271 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/connected_source_client_facing.py
+-rw-r--r--   0        0        0     1184 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/connection_status.py
+-rw-r--r--   0        0        0      734 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/connection_status_state.py
+-rw-r--r--   0        0        0     1126 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/consent.py
+-rw-r--r--   0        0        0     1519 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/consent_type.py
+-rw-r--r--   0        0        0      930 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/day_slots.py
+-rw-r--r--   0        0        0     1240 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/delegated_flow_type.py
+-rw-r--r--   0        0        0      897 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/demo_connection_status.py
+-rw-r--r--   0        0        0      892 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/demo_providers.py
+-rw-r--r--   0        0        0     1053 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/device_v_2_in_db.py
+-rw-r--r--   0        0        0      153 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/email_providers.py
+-rw-r--r--   0        0        0      936 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/energy.py
+-rw-r--r--   0        0        0     1172 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/event_destination_preferences.py
+-rw-r--r--   0        0        0      762 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/event_destination_preferences_enabled_item.py
+-rw-r--r--   0        0        0      754 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/event_destination_preferences_preferred.py
+-rw-r--r--   0        0        0     1169 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/fallback_birth_date.py
+-rw-r--r--   0        0        0     1376 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/fallback_time_zone.py
+-rw-r--r--   0        0        0     1623 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/fats.py
+-rw-r--r--   0        0        0      762 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/gender.py
+-rw-r--r--   0        0        0     1110 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/get_markers_response.py
+-rw-r--r--   0        0        0     1048 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/get_orders_response.py
+-rw-r--r--   0        0        0     1087 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_blood_oxygen.py
+-rw-r--r--   0        0        0     1254 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_blood_oxygen_response.py
+-rw-r--r--   0        0        0     1095 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_blood_pressure.py
+-rw-r--r--   0        0        0     1262 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_blood_pressure_response.py
+-rw-r--r--   0        0        0     1071 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_body_fat.py
+-rw-r--r--   0        0        0     1238 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_body_fat_response.py
+-rw-r--r--   0        0        0     1083 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_body_weight.py
+-rw-r--r--   0        0        0     1250 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_body_weight_response.py
+-rw-r--r--   0        0        0     1074 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_caffeine.py
+-rw-r--r--   0        0        0     1241 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_caffeine_response.py
+-rw-r--r--   0        0        0     1099 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_calories_active.py
+-rw-r--r--   0        0        0     1266 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_calories_active_response.py
+-rw-r--r--   0        0        0     1095 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_calories_basal.py
+-rw-r--r--   0        0        0     1262 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_calories_basal_response.py
+-rw-r--r--   0        0        0     1086 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_cholesterol.py
+-rw-r--r--   0        0        0     1253 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_cholesterol_response.py
+-rw-r--r--   0        0        0     1074 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_distance.py
+-rw-r--r--   0        0        0     1241 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_distance_response.py
+-rw-r--r--   0        0        0     1139 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_electrocardiogram_voltage.py
+-rw-r--r--   0        0        0     1306 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_electrocardiogram_voltage_response.py
+-rw-r--r--   0        0        0     1095 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_floors_climbed.py
+-rw-r--r--   0        0        0     1262 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_floors_climbed_response.py
+-rw-r--r--   0        0        0     1070 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_glucose.py
+-rw-r--r--   0        0        0     1237 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_glucose_response.py
+-rw-r--r--   0        0        0     1079 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_heart_rate.py
+-rw-r--r--   0        0        0     1246 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_heart_rate_response.py
+-rw-r--r--   0        0        0     1054 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_hrv.py
+-rw-r--r--   0        0        0     1221 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_hrv_response.py
+-rw-r--r--   0        0        0     1078 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_hypnogram.py
+-rw-r--r--   0        0        0     1245 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_hypnogram_response.py
+-rw-r--r--   0        0        0     1054 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_ige.py
+-rw-r--r--   0        0        0     1221 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_ige_response.py
+-rw-r--r--   0        0        0     1054 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_igg.py
+-rw-r--r--   0        0        0     1221 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_igg_response.py
+-rw-r--r--   0        0        0     1115 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_mindfulness_minutes.py
+-rw-r--r--   0        0        0     1282 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_mindfulness_minutes_response.py
+-rw-r--r--   0        0        0     1103 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_respiratory_rate.py
+-rw-r--r--   0        0        0     1270 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_respiratory_rate_response.py
+-rw-r--r--   0        0        0     1062 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_steps.py
+-rw-r--r--   0        0        0     1229 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_steps_response.py
+-rw-r--r--   0        0        0     1087 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_stress_level.py
+-rw-r--r--   0        0        0     1254 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_stress_level_response.py
+-rw-r--r--   0        0        0     1068 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_vo_2_max.py
+-rw-r--r--   0        0        0     1235 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_vo_2_max_response.py
+-rw-r--r--   0        0        0     1062 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_water.py
+-rw-r--r--   0        0        0     1229 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_water_response.py
+-rw-r--r--   0        0        0     3022 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/health_insurance_create_request.py
+-rw-r--r--   0        0        0      811 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/health_insurance_create_request_back_image.py
+-rw-r--r--   0        0        0      816 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/health_insurance_create_request_front_image.py
+-rw-r--r--   0        0        0      876 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/health_insurance_create_request_patient_signature_image.py
+-rw-r--r--   0        0        0      732 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/historical_pull_status.py
+-rw-r--r--   0        0        0      966 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/http_validation_error.py
+-rw-r--r--   0        0        0      864 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/jpeg.py
+-rw-r--r--   0        0        0     1289 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_results_metadata.py
+-rw-r--r--   0        0        0     1034 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_results_raw.py
+-rw-r--r--   0        0        0      223 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_results_raw_results.py
+-rw-r--r--   0        0        0      827 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_test_collection_method.py
+-rw-r--r--   0        0        0      898 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_test_sample_type.py
+-rw-r--r--   0        0        0      729 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_test_status.py
+-rw-r--r--   0        0        0      949 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/last_attempt.py
+-rw-r--r--   0        0        0      936 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/libre_config.py
+-rw-r--r--   0        0        0      960 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/link_token_exchange_response.py
+-rw-r--r--   0        0        0      879 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lng_lat.py
+-rw-r--r--   0        0        0     1553 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/macros.py
+-rw-r--r--   0        0        0     1792 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/manual_providers.py
+-rw-r--r--   0        0        0      501 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/marker_type.py
+-rw-r--r--   0        0        0     1444 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/meal_in_db_base_client_facing_source.py
+-rw-r--r--   0        0        0     1233 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/metrics_result.py
+-rw-r--r--   0        0        0     1272 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/micros.py
+-rw-r--r--   0        0        0     2126 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/o_auth_providers.py
+-rw-r--r--   0        0        0     9798 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/order_status.py
+-rw-r--r--   0        0        0     1265 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/order_top_level_status.py
+-rw-r--r--   0        0        0     1001 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/paginated_users_response.py
+-rw-r--r--   0        0        0     1779 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/password_providers.py
+-rw-r--r--   0        0        0     1063 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/patient_address_compatible.py
+-rw-r--r--   0        0        0     1000 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/patient_details.py
+-rw-r--r--   0        0        0     1004 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/person_details.py
+-rw-r--r--   0        0        0      993 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/phlebotomy_area_info.py
+-rw-r--r--   0        0        0     1065 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/phlebotomy_provider_info.py
+-rw-r--r--   0        0        0     1281 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/physician_create_request.py
+-rw-r--r--   0        0        0     1008 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/physician_create_request_base.py
+-rw-r--r--   0        0        0      806 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/physician_create_request_signature_image.py
+-rw-r--r--   0        0        0      863 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/png.py
+-rw-r--r--   0        0        0      973 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/post_order_response.py
+-rw-r--r--   0        0        0     1113 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/profile_in_db.py
+-rw-r--r--   0        0        0     1284 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/provider_link_response.py
+-rw-r--r--   0        0        0      750 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/provider_link_response_state.py
+-rw-r--r--   0        0        0      978 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/provider_mfa_request.py
+-rw-r--r--   0        0        0      476 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/provider_mfa_request_method.py
+-rw-r--r--   0        0        0     5340 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/providers.py
+-rw-r--r--   0        0        0      943 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_activity.py
+-rw-r--r--   0        0        0      923 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_body.py
+-rw-r--r--   0        0        0      935 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_devices.py
+-rw-r--r--   0        0        0      917 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_profile.py
+-rw-r--r--   0        0        0      928 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_sleep.py
+-rw-r--r--   0        0        0      939 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_workout.py
+-rw-r--r--   0        0        0     1360 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/region.py
+-rw-r--r--   0        0        0     1055 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/resource_availability.py
+-rw-r--r--   0        0        0      761 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/responsible_relationship.py
+-rw-r--r--   0        0        0      662 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/result_type.py
+-rw-r--r--   0        0        0     1000 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/scope_requirements_grants.py
+-rw-r--r--   0        0        0      925 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/scope_requirements_str.py
+-rw-r--r--   0        0        0     1020 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/shipping_address.py
+-rw-r--r--   0        0        0     1146 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/single_historical_pull_statistics.py
+-rw-r--r--   0        0        0     1125 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/single_provider_historical_pull_response.py
+-rw-r--r--   0        0        0     1081 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/single_resource_statistics.py
+-rw-r--r--   0        0        0     1052 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/single_user_historical_pull_response.py
+-rw-r--r--   0        0        0     1026 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/single_user_resource_response.py
+-rw-r--r--   0        0        0     1152 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/sleep_v_2_in_db.py
+-rw-r--r--   0        0        0     1246 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/source.py
+-rw-r--r--   0        0        0     1209 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/source_auth_type.py
+-rw-r--r--   0        0        0     1123 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/source_link.py
+-rw-r--r--   0        0        0      892 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/source_type.py
+-rw-r--r--   0        0        0     1303 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/team_config.py
+-rw-r--r--   0        0        0     1147 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/time_slot.py
+-rw-r--r--   0        0        0      903 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/timeseries_metric_point.py
+-rw-r--r--   0        0        0     4865 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/timeseries_resource.py
+-rw-r--r--   0        0        0     1138 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/us_address.py
+-rw-r--r--   0        0        0     1040 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_historical_pulls_response.py
+-rw-r--r--   0        0        0     1305 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_refresh_error_response.py
+-rw-r--r--   0        0        0     1357 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_refresh_success_response.py
+-rw-r--r--   0        0        0     1015 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_resources_response.py
+-rw-r--r--   0        0        0      906 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_sign_in_token_response.py
+-rw-r--r--   0        0        0      952 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_success_response.py
+-rw-r--r--   0        0        0      992 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-10 08:37:28.815833 vital-2.1.8/src/vital/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      904 2024-05-10 08:37:28.815833 vital-2.1.8/src/vital/types/vital_token_created_response.py
+-rw-r--r--   0        0        0     1217 2024-05-10 08:37:28.815833 vital-2.1.8/src/vital/types/workout_v_2_in_db.py
+-rw-r--r--   0        0        0     3831 1970-01-01 00:00:00.000000 vital-2.1.8/PKG-INFO
```

### Comparing `vital-2.1.7/README.md` & `vital-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/__init__.py` & `vital-2.1.8/src/vital/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,16 @@
     PhysicianCreateRequestSignatureImage_ImageJpeg,
     PhysicianCreateRequestSignatureImage_ImagePng,
     Png,
     PostOrderResponse,
     ProfileInDb,
     ProviderLinkResponse,
     ProviderLinkResponseState,
+    ProviderMfaRequest,
+    ProviderMfaRequestMethod,
     Providers,
     RawActivity,
     RawBody,
     RawDevices,
     RawProfile,
     RawSleep,
     RawWorkout,
@@ -468,14 +470,16 @@
     "PhysicianCreateRequestSignatureImage_ImageJpeg",
     "PhysicianCreateRequestSignatureImage_ImagePng",
     "Png",
     "PostOrderResponse",
     "ProfileInDb",
     "ProviderLinkResponse",
     "ProviderLinkResponseState",
+    "ProviderMfaRequest",
+    "ProviderMfaRequestMethod",
     "Providers",
     "RawActivity",
     "RawBody",
     "RawDevices",
     "RawProfile",
     "RawSleep",
     "RawWorkout",
```

### Comparing `vital-2.1.7/src/vital/client.py` & `vital-2.1.8/src/vital/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/core/__init__.py` & `vital-2.1.8/src/vital/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/core/client_wrapper.py` & `vital-2.1.8/src/vital/core/client_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "vital",
-            "X-Fern-SDK-Version": "2.1.7",
+            "X-Fern-SDK-Version": "2.1.8",
         }
         headers["x-vital-api-key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `vital-2.1.7/src/vital/core/datetime_utils.py` & `vital-2.1.8/src/vital/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/core/jsonable_encoder.py` & `vital-2.1.8/src/vital/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/resources/__init__.py` & `vital-2.1.8/src/vital/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/resources/activity/client.py` & `vital-2.1.8/src/vital/resources/activity/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.activity.get(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/activity/{user_id}"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -91,16 +91,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.activity.get_raw(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/activity/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -143,16 +143,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.activity.get(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/activity/{user_id}"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -190,16 +190,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.activity.get_raw(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/activity/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
```

### Comparing `vital-2.1.7/src/vital/resources/body/client.py` & `vital-2.1.8/src/vital/resources/body/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.body.get(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/body/{user_id}"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -91,16 +91,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.body.get_raw(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/body/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -143,16 +143,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.body.get(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/body/{user_id}"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -190,16 +190,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.body.get_raw(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/body/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
```

### Comparing `vital-2.1.7/src/vital/resources/devices/client.py` & `vital-2.1.8/src/vital/resources/devices/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.devices.get_raw(
-            user_id="user-id",
+            user_id="user_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/devices/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider}),
             headers=self._client_wrapper.get_headers(),
@@ -72,15 +72,15 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.devices.get_raw(
-            user_id="user-id",
+            user_id="user_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/devices/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider}),
             headers=self._client_wrapper.get_headers(),
```

### Comparing `vital-2.1.7/src/vital/resources/insurance/client.py` & `vital-2.1.8/src/vital/resources/insurance/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,23 @@
         self, *, insurance_name: str, insurance_state: typing.Optional[str] = OMIT
     ) -> typing.List[ClientFacingPayorSearchResponse]:
         """
         Parameters:
             - insurance_name: str.
 
             - insurance_state: typing.Optional[str].
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.insurance.search_payor_info(
+            insurance_name="insurance_name",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"insurance_name": insurance_name}
         if insurance_state is not OMIT:
             _request["insurance_state"] = insurance_state
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/insurance/search/payor"),
@@ -62,15 +71,15 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.insurance.search_diagnosis(
-            diagnosis_query="diagnosis-query",
+            diagnosis_query="diagnosis_query",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/insurance/search/diagnosis"),
             params=remove_none_from_dict({"diagnosis_query": diagnosis_query}),
             headers=self._client_wrapper.get_headers(),
@@ -95,14 +104,23 @@
         self, *, insurance_name: str, insurance_state: typing.Optional[str] = OMIT
     ) -> typing.List[ClientFacingPayorSearchResponse]:
         """
         Parameters:
             - insurance_name: str.
 
             - insurance_state: typing.Optional[str].
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.insurance.search_payor_info(
+            insurance_name="insurance_name",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"insurance_name": insurance_name}
         if insurance_state is not OMIT:
             _request["insurance_state"] = insurance_state
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/insurance/search/payor"),
@@ -127,15 +145,15 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.insurance.search_diagnosis(
-            diagnosis_query="diagnosis-query",
+            diagnosis_query="diagnosis_query",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/insurance/search/diagnosis"),
             params=remove_none_from_dict({"diagnosis_query": diagnosis_query}),
             headers=self._client_wrapper.get_headers(),
```

### Comparing `vital-2.1.7/src/vital/resources/introspect/client.py` & `vital-2.1.8/src/vital/resources/introspect/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,23 +37,20 @@
 
             - provider: typing.Optional[Providers].
 
             - user_limit: typing.Optional[int].
 
             - cursor: typing.Optional[str].
         ---
-        from vital import Providers
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
-        client.introspect.get_user_resources(
-            provider=Providers.OURA,
-        )
+        client.introspect.get_user_resources()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/introspect/resources"),
             params=remove_none_from_dict(
                 {"user_id": user_id, "provider": provider, "user_limit": user_limit, "cursor": cursor}
             ),
@@ -84,23 +81,20 @@
 
             - provider: typing.Optional[Providers].
 
             - user_limit: typing.Optional[int].
 
             - cursor: typing.Optional[str].
         ---
-        from vital import Providers
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
-        client.introspect.get_user_historical_pulls(
-            provider=Providers.OURA,
-        )
+        client.introspect.get_user_historical_pulls()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/introspect/historical_pull"),
             params=remove_none_from_dict(
                 {"user_id": user_id, "provider": provider, "user_limit": user_limit, "cursor": cursor}
             ),
@@ -136,23 +130,20 @@
 
             - provider: typing.Optional[Providers].
 
             - user_limit: typing.Optional[int].
 
             - cursor: typing.Optional[str].
         ---
-        from vital import Providers
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
-        await client.introspect.get_user_resources(
-            provider=Providers.OURA,
-        )
+        await client.introspect.get_user_resources()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/introspect/resources"),
             params=remove_none_from_dict(
                 {"user_id": user_id, "provider": provider, "user_limit": user_limit, "cursor": cursor}
             ),
@@ -183,23 +174,20 @@
 
             - provider: typing.Optional[Providers].
 
             - user_limit: typing.Optional[int].
 
             - cursor: typing.Optional[str].
         ---
-        from vital import Providers
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
-        await client.introspect.get_user_historical_pulls(
-            provider=Providers.OURA,
-        )
+        await client.introspect.get_user_historical_pulls()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/introspect/historical_pull"),
             params=remove_none_from_dict(
                 {"user_id": user_id, "provider": provider, "user_limit": user_limit, "cursor": cursor}
             ),
```

### Comparing `vital-2.1.7/src/vital/resources/lab_tests/client.py` & `vital-2.1.8/src/vital/resources/lab_tests/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,14 +97,29 @@
             - method: LabTestCollectionMethod.
 
             - sample_type: LabTestSampleType.
 
             - description: str.
 
             - fasting: typing.Optional[bool].
+        ---
+        from vital import LabTestCollectionMethod, LabTestSampleType
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.create(
+            marker_ids=[1],
+            lab_id=1,
+            name="name",
+            method=LabTestCollectionMethod.TESTKIT,
+            sample_type=LabTestSampleType.DRIED_BLOOD_SPOT,
+            description="description",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {
             "marker_ids": marker_ids,
             "lab_id": lab_id,
             "name": name,
             "method": method.value,
             "sample_type": sample_type.value,
@@ -186,15 +201,15 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.lab_tests.get_markers_for_lab_test(
-            lab_test_id="lab-test-id",
+            lab_test_id="lab_test_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v3/lab_tests/{lab_test_id}/markers"),
             params=remove_none_from_dict({"page": page, "size": size}),
             headers=self._client_wrapper.get_headers(),
@@ -214,14 +229,24 @@
         """
         GET a specific marker for the given lab and provider_id
 
         Parameters:
             - provider_id: str.
 
             - lab_id: int.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.get_markers_by_lab_and_provider_id(
+            provider_id="provider_id",
+            lab_id=1,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v3/lab_tests/{lab_id}/markers/{provider_id}"
             ),
             headers=self._client_wrapper.get_headers(),
@@ -265,14 +290,23 @@
 
     def get_by_id(self, lab_test_id: str) -> ClientFacingLabTest:
         """
         GET all the lab tests the team has access to.
 
         Parameters:
             - lab_test_id: str.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.get_by_id(
+            lab_test_id="lab_test_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v3/lab_tests/{lab_test_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -289,14 +323,29 @@
     def get_phlebotomy_appointment_availability(self, *, request: UsAddress) -> AppointmentAvailabilitySlots:
         """
         Return the available time slots to book an appointment with a phlebotomist
         for the given address and order.
 
         Parameters:
             - request: UsAddress.
+        ---
+        from vital import UsAddress
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.get_phlebotomy_appointment_availability(
+            request=UsAddress(
+                first_line="first_line",
+                city="city",
+                state="state",
+                zip_code="zip_code",
+            ),
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", "v3/order/phlebotomy/appointment/availability"
             ),
             json=jsonable_encoder(request),
@@ -317,14 +366,24 @@
         """
         Book an at-home phlebotomy appointment.
 
         Parameters:
             - order_id: str. Your Order ID.
 
             - booking_key: str.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.book_phlebotomy_appointment(
+            order_id="order_id",
+            booking_key="booking_key",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/phlebotomy/appointment/book"
             ),
             json=jsonable_encoder({"booking_key": booking_key}),
@@ -349,14 +408,31 @@
 
         Parameters:
             - order_id: str. Your Order ID.
 
             - address: UsAddress. At-home phlebotomy appointment address.
 
             - provider: AppointmentProvider.
+        ---
+        from vital import AppointmentProvider, UsAddress
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.request_phlebotomy_appointment(
+            order_id="order_id",
+            address=UsAddress(
+                first_line="first_line",
+                city="city",
+                state="state",
+                zip_code="zip_code",
+            ),
+            provider=AppointmentProvider.GETLABS,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/phlebotomy/appointment/request"
             ),
             json=jsonable_encoder({"address": address, "provider": provider}),
@@ -377,14 +453,24 @@
         """
         Reschedule a previously booked at-home phlebotomy appointment.
 
         Parameters:
             - order_id: str. Your Order ID.
 
             - booking_key: str.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.reschedule_phlebotomy_appointment(
+            order_id="order_id",
+            booking_key="booking_key",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/phlebotomy/appointment/reschedule"
             ),
             json=jsonable_encoder({"booking_key": booking_key}),
@@ -409,14 +495,24 @@
 
         Parameters:
             - order_id: str. Your Order ID.
 
             - cancellation_reason_id: str.
 
             - notes: typing.Optional[str].
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.cancel_phlebotomy_appointment(
+            order_id="order_id",
+            cancellation_reason_id="cancellation_reason_id",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"cancellation_reason_id": cancellation_reason_id}
         if notes is not OMIT:
             _request["notes"] = notes
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
@@ -466,14 +562,23 @@
 
     def get_phlebotomy_appointment(self, order_id: str) -> ClientFacingAppointment:
         """
         Get the appointment associated with an order.
 
         Parameters:
             - order_id: str. Your Order ID.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.get_phlebotomy_appointment(
+            order_id="order_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/phlebotomy/appointment"
             ),
             headers=self._client_wrapper.get_headers(),
@@ -495,14 +600,23 @@
 
         Information returned:
 
         - Whether a given zip code is served by our Phlebotomy network.
 
         Parameters:
             - zip_code: str. Zip code of the area to check
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.get_area_info(
+            zip_code="zip_code",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/order/area/info"),
             params=remove_none_from_dict({"zip_code": zip_code}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -531,27 +645,40 @@
             timeout=60,
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _chunk in _response.iter_bytes():
                     yield _chunk
                 return
             _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    pydantic.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_result_metadata(self, order_id: str) -> LabResultsMetadata:
         """
         Return metadata related to order results, such as lab metadata,
         provider and sample dates.
 
         Parameters:
             - order_id: str.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.get_result_metadata(
+            order_id="order_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/result/metadata"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -567,14 +694,23 @@
 
     def get_result_raw(self, order_id: str) -> LabResultsRaw:
         """
         Return both metadata and raw json test data
 
         Parameters:
             - order_id: str.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.get_result_raw(
+            order_id="order_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/result"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -602,14 +738,18 @@
             timeout=60,
         ) as _response:
             if 200 <= _response.status_code < 300:
                 for _chunk in _response.iter_bytes():
                     yield _chunk
                 return
             _response.read()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    pydantic.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_order(self, order_id: str) -> ClientFacingOrder:
@@ -734,14 +874,23 @@
 
         Parameters:
             - order_id: str.
 
             - final_status: typing.Optional[OrderStatus].
 
             - delay: typing.Optional[int].
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.lab_tests.simulate_order_process(
+            order_id="order_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/test"),
             params=remove_none_from_dict({"final_status": final_status, "delay": delay}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -872,14 +1021,29 @@
             - method: LabTestCollectionMethod.
 
             - sample_type: LabTestSampleType.
 
             - description: str.
 
             - fasting: typing.Optional[bool].
+        ---
+        from vital import LabTestCollectionMethod, LabTestSampleType
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.create(
+            marker_ids=[1],
+            lab_id=1,
+            name="name",
+            method=LabTestCollectionMethod.TESTKIT,
+            sample_type=LabTestSampleType.DRIED_BLOOD_SPOT,
+            description="description",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {
             "marker_ids": marker_ids,
             "lab_id": lab_id,
             "name": name,
             "method": method.value,
             "sample_type": sample_type.value,
@@ -961,15 +1125,15 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.lab_tests.get_markers_for_lab_test(
-            lab_test_id="lab-test-id",
+            lab_test_id="lab_test_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v3/lab_tests/{lab_test_id}/markers"),
             params=remove_none_from_dict({"page": page, "size": size}),
             headers=self._client_wrapper.get_headers(),
@@ -989,14 +1153,24 @@
         """
         GET a specific marker for the given lab and provider_id
 
         Parameters:
             - provider_id: str.
 
             - lab_id: int.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.get_markers_by_lab_and_provider_id(
+            provider_id="provider_id",
+            lab_id=1,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v3/lab_tests/{lab_id}/markers/{provider_id}"
             ),
             headers=self._client_wrapper.get_headers(),
@@ -1040,14 +1214,23 @@
 
     async def get_by_id(self, lab_test_id: str) -> ClientFacingLabTest:
         """
         GET all the lab tests the team has access to.
 
         Parameters:
             - lab_test_id: str.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.get_by_id(
+            lab_test_id="lab_test_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v3/lab_tests/{lab_test_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -1064,14 +1247,29 @@
     async def get_phlebotomy_appointment_availability(self, *, request: UsAddress) -> AppointmentAvailabilitySlots:
         """
         Return the available time slots to book an appointment with a phlebotomist
         for the given address and order.
 
         Parameters:
             - request: UsAddress.
+        ---
+        from vital import UsAddress
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.get_phlebotomy_appointment_availability(
+            request=UsAddress(
+                first_line="first_line",
+                city="city",
+                state="state",
+                zip_code="zip_code",
+            ),
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", "v3/order/phlebotomy/appointment/availability"
             ),
             json=jsonable_encoder(request),
@@ -1092,14 +1290,24 @@
         """
         Book an at-home phlebotomy appointment.
 
         Parameters:
             - order_id: str. Your Order ID.
 
             - booking_key: str.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.book_phlebotomy_appointment(
+            order_id="order_id",
+            booking_key="booking_key",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/phlebotomy/appointment/book"
             ),
             json=jsonable_encoder({"booking_key": booking_key}),
@@ -1124,14 +1332,31 @@
 
         Parameters:
             - order_id: str. Your Order ID.
 
             - address: UsAddress. At-home phlebotomy appointment address.
 
             - provider: AppointmentProvider.
+        ---
+        from vital import AppointmentProvider, UsAddress
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.request_phlebotomy_appointment(
+            order_id="order_id",
+            address=UsAddress(
+                first_line="first_line",
+                city="city",
+                state="state",
+                zip_code="zip_code",
+            ),
+            provider=AppointmentProvider.GETLABS,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/phlebotomy/appointment/request"
             ),
             json=jsonable_encoder({"address": address, "provider": provider}),
@@ -1152,14 +1377,24 @@
         """
         Reschedule a previously booked at-home phlebotomy appointment.
 
         Parameters:
             - order_id: str. Your Order ID.
 
             - booking_key: str.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.reschedule_phlebotomy_appointment(
+            order_id="order_id",
+            booking_key="booking_key",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/phlebotomy/appointment/reschedule"
             ),
             json=jsonable_encoder({"booking_key": booking_key}),
@@ -1184,14 +1419,24 @@
 
         Parameters:
             - order_id: str. Your Order ID.
 
             - cancellation_reason_id: str.
 
             - notes: typing.Optional[str].
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.cancel_phlebotomy_appointment(
+            order_id="order_id",
+            cancellation_reason_id="cancellation_reason_id",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"cancellation_reason_id": cancellation_reason_id}
         if notes is not OMIT:
             _request["notes"] = notes
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(
@@ -1243,14 +1488,23 @@
 
     async def get_phlebotomy_appointment(self, order_id: str) -> ClientFacingAppointment:
         """
         Get the appointment associated with an order.
 
         Parameters:
             - order_id: str. Your Order ID.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.get_phlebotomy_appointment(
+            order_id="order_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/phlebotomy/appointment"
             ),
             headers=self._client_wrapper.get_headers(),
@@ -1272,14 +1526,23 @@
 
         Information returned:
 
         - Whether a given zip code is served by our Phlebotomy network.
 
         Parameters:
             - zip_code: str. Zip code of the area to check
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.get_area_info(
+            zip_code="zip_code",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v3/order/area/info"),
             params=remove_none_from_dict({"zip_code": zip_code}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -1308,27 +1571,40 @@
             timeout=60,
         ) as _response:
             if 200 <= _response.status_code < 300:
                 async for _chunk in _response.aiter_bytes():
                     yield _chunk
                 return
             await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    pydantic.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_result_metadata(self, order_id: str) -> LabResultsMetadata:
         """
         Return metadata related to order results, such as lab metadata,
         provider and sample dates.
 
         Parameters:
             - order_id: str.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.get_result_metadata(
+            order_id="order_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/result/metadata"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -1344,14 +1620,23 @@
 
     async def get_result_raw(self, order_id: str) -> LabResultsRaw:
         """
         Return both metadata and raw json test data
 
         Parameters:
             - order_id: str.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.get_result_raw(
+            order_id="order_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/result"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -1379,14 +1664,18 @@
             timeout=60,
         ) as _response:
             if 200 <= _response.status_code < 300:
                 async for _chunk in _response.aiter_bytes():
                     yield _chunk
                 return
             await _response.aread()
+            if _response.status_code == 422:
+                raise UnprocessableEntityError(
+                    pydantic.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
+                )
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_order(self, order_id: str) -> ClientFacingOrder:
@@ -1511,14 +1800,23 @@
 
         Parameters:
             - order_id: str.
 
             - final_status: typing.Optional[OrderStatus].
 
             - delay: typing.Optional[int].
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.lab_tests.simulate_order_process(
+            order_id="order_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v3/order/{order_id}/test"),
             params=remove_none_from_dict({"final_status": final_status, "delay": delay}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
```

### Comparing `vital-2.1.7/src/vital/resources/link/client.py` & `vital-2.1.8/src/vital/resources/link/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/resources/meal/client.py` & `vital-2.1.8/src/vital/resources/meal/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.meal.get(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/meal/{user_id}"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -95,16 +95,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.meal.get(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/meal/{user_id}"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
```

### Comparing `vital-2.1.7/src/vital/resources/profile/client.py` & `vital-2.1.8/src/vital/resources/profile/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,23 @@
         """
         Get Daily profile for user_id
 
         Parameters:
             - user_id: str.
 
             - provider: typing.Optional[str]. Provider oura/strava etc
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.profile.get(
+            user_id="user_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/profile/{user_id}"),
             params=remove_none_from_dict({"provider": provider}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -52,14 +61,23 @@
         """
         Get Daily profile for user_id
 
         Parameters:
             - user_id: str.
 
             - provider: typing.Optional[str]. Provider oura/strava etc
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.profile.get_raw(
+            user_id="user_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/profile/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -83,14 +101,23 @@
         """
         Get Daily profile for user_id
 
         Parameters:
             - user_id: str.
 
             - provider: typing.Optional[str]. Provider oura/strava etc
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.profile.get(
+            user_id="user_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/profile/{user_id}"),
             params=remove_none_from_dict({"provider": provider}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -109,14 +136,23 @@
         """
         Get Daily profile for user_id
 
         Parameters:
             - user_id: str.
 
             - provider: typing.Optional[str]. Provider oura/strava etc
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.profile.get_raw(
+            user_id="user_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/profile/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
```

### Comparing `vital-2.1.7/src/vital/resources/providers/client.py` & `vital-2.1.8/src/vital/resources/providers/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/resources/sleep/client.py` & `vital-2.1.8/src/vital/resources/sleep/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.sleep.get(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/sleep/{user_id}"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -92,16 +92,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.sleep.get_stream(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/sleep/{user_id}/stream"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -139,16 +139,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.sleep.get_raw(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/sleep/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -173,15 +173,15 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.sleep.get_stream_by_sleep_id(
-            sleep_id="sleep-id",
+            sleep_id="sleep_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/sleep/{sleep_id}/stream"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -223,16 +223,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.sleep.get(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/sleep/{user_id}"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -270,16 +270,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.sleep.get_stream(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/sleep/{user_id}/stream"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -317,16 +317,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.sleep.get_raw(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/sleep/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -351,15 +351,15 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.sleep.get_stream_by_sleep_id(
-            sleep_id="sleep-id",
+            sleep_id="sleep_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/sleep/{sleep_id}/stream"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
```

### Comparing `vital-2.1.7/src/vital/resources/team/client.py` & `vital-2.1.8/src/vital/resources/team/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,23 @@
 
     def get(self, team_id: str) -> ClientFacingTeam:
         """
         Get team.
 
         Parameters:
             - team_id: str.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.team.get(
+            team_id="team_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/team/{team_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -174,15 +183,15 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.team.update_source_priorities(
-            team_id="team-id",
+            team_id="team_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/team/source/priorities"),
             params=remove_none_from_dict({"team_id": team_id}),
             headers=self._client_wrapper.get_headers(),
@@ -205,15 +214,15 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.team.get_physicians(
-            team_id="team-id",
+            team_id="team_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/team/{team_id}/physicians"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -267,14 +276,23 @@
 
     async def get(self, team_id: str) -> ClientFacingTeam:
         """
         Get team.
 
         Parameters:
             - team_id: str.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.team.get(
+            team_id="team_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/team/{team_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -384,15 +402,15 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.team.update_source_priorities(
-            team_id="team-id",
+            team_id="team_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "PATCH",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/team/source/priorities"),
             params=remove_none_from_dict({"team_id": team_id}),
             headers=self._client_wrapper.get_headers(),
@@ -415,15 +433,15 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.team.get_physicians(
-            team_id="team-id",
+            team_id="team_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/team/{team_id}/physicians"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
```

### Comparing `vital-2.1.7/src/vital/resources/testkit/client.py` & `vital-2.1.8/src/vital/resources/testkit/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/resources/user/client.py` & `vital-2.1.8/src/vital/resources/user/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,14 +40,21 @@
         """
         GET All users for team.
 
         Parameters:
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.user.get_all()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/user"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -82,14 +89,23 @@
                                                             Used when pulling data from sources that are completely time zone agnostic (e.g., all time is relative to UTC clock, without any time zone attributions on data points).
 
             - fallback_birth_date: typing.Optional[str]. Fallback date of birth of the user, in YYYY-mm-dd format. Used for calculating max heartrate for providers that don not provide users' age.
 
             - ingestion_start: typing.Optional[str]. Starting bound for user data ingestion. Data older than this date will not be ingested.
 
             - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data newer than this date will not be ingested and the connection deregistered.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.user.create(
+            client_user_id="client_user_id",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"client_user_id": client_user_id}
         if fallback_time_zone is not OMIT:
             _request["fallback_time_zone"] = fallback_time_zone
         if fallback_birth_date is not OMIT:
             _request["fallback_birth_date"] = fallback_birth_date
         if ingestion_start is not OMIT:
@@ -114,14 +130,22 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_team_metrics(self) -> MetricsResult:
         """
         GET metrics for team.
+
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.user.get_team_metrics()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/user/metrics"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -133,14 +157,23 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_user_sign_in_token(self, user_id: str) -> UserSignInTokenResponse:
         """
         Parameters:
             - user_id: str.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.user.get_user_sign_in_token(
+            user_id="user_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/{user_id}/sign_in_token"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -163,15 +196,15 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.user.get_connected_providers(
-            user_id="user-id",
+            user_id="user_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/providers/{user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -188,14 +221,23 @@
 
     def get(self, user_id: str) -> ClientFacingUser:
         """
         GET User details given the user_id.
 
         Parameters:
             - user_id: str.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.user.get(
+            user_id="user_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/{user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -209,14 +251,23 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, user_id: str) -> UserSuccessResponse:
         """
         Parameters:
             - user_id: str.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.user.delete(
+            user_id="user_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/{user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -255,15 +306,15 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.user.patch(
-            user_id="user-id",
+            user_id="user_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if fallback_time_zone is not OMIT:
             _request["fallback_time_zone"] = fallback_time_zone
         if fallback_birth_date is not OMIT:
             _request["fallback_birth_date"] = fallback_birth_date
@@ -290,14 +341,23 @@
 
     def get_by_client_user_id(self, client_user_id: str) -> ClientFacingUser:
         """
         GET user_id from client_user_id.
 
         Parameters:
             - client_user_id: str. A unique ID representing the end user. Typically this will be a user ID number from your application. Personally identifiable information, such as an email address or phone number, should not be used in the client_user_id.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.user.get_by_client_user_id(
+            client_user_id="client_user_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/resolve/{client_user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -313,14 +373,25 @@
 
     def deregister_provider(self, user_id: str, provider: Providers) -> UserSuccessResponse:
         """
         Parameters:
             - user_id: str.
 
             - provider: Providers. Provider slug. e.g., `oura`, `fitbit`, `garmin`.
+        ---
+        from vital import Providers
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.user.deregister_provider(
+            user_id="user_id",
+            provider=Providers.OURA,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/{user_id}/{provider}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -338,14 +409,21 @@
         self, *, user_id: typing.Optional[str] = None, client_user_id: typing.Optional[str] = None
     ) -> UserSuccessResponse:
         """
         Parameters:
             - user_id: typing.Optional[str]. User ID to undo deletion. Mutually exclusive with `client_user_id`.
 
             - client_user_id: typing.Optional[str]. Client User ID to undo deletion. Mutually exclusive with `user_id`.
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.user.undo_delete()
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/user/undo_delete"),
             params=remove_none_from_dict({"user_id": user_id, "client_user_id": client_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -364,14 +442,23 @@
         """
         Trigger a manual refresh for a specific user
 
         Parameters:
             - user_id: str.
 
             - timeout: typing.Optional[float].
+        ---
+        from vital.client import Vital
+
+        client = Vital(
+            api_key="YOUR_API_KEY",
+        )
+        client.user.refresh(
+            user_id="user_id",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/refresh/{user_id}"),
             params=remove_none_from_dict({"timeout": timeout}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -399,14 +486,21 @@
         """
         GET All users for team.
 
         Parameters:
             - offset: typing.Optional[int].
 
             - limit: typing.Optional[int].
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.user.get_all()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/user"),
             params=remove_none_from_dict({"offset": offset, "limit": limit}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -441,14 +535,23 @@
                                                             Used when pulling data from sources that are completely time zone agnostic (e.g., all time is relative to UTC clock, without any time zone attributions on data points).
 
             - fallback_birth_date: typing.Optional[str]. Fallback date of birth of the user, in YYYY-mm-dd format. Used for calculating max heartrate for providers that don not provide users' age.
 
             - ingestion_start: typing.Optional[str]. Starting bound for user data ingestion. Data older than this date will not be ingested.
 
             - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data newer than this date will not be ingested and the connection deregistered.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.user.create(
+            client_user_id="client_user_id",
+        )
         """
         _request: typing.Dict[str, typing.Any] = {"client_user_id": client_user_id}
         if fallback_time_zone is not OMIT:
             _request["fallback_time_zone"] = fallback_time_zone
         if fallback_birth_date is not OMIT:
             _request["fallback_birth_date"] = fallback_birth_date
         if ingestion_start is not OMIT:
@@ -473,14 +576,22 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_team_metrics(self) -> MetricsResult:
         """
         GET metrics for team.
+
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.user.get_team_metrics()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/user/metrics"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -492,14 +603,23 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_user_sign_in_token(self, user_id: str) -> UserSignInTokenResponse:
         """
         Parameters:
             - user_id: str.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.user.get_user_sign_in_token(
+            user_id="user_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/{user_id}/sign_in_token"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -524,15 +644,15 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.user.get_connected_providers(
-            user_id="user-id",
+            user_id="user_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/providers/{user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -549,14 +669,23 @@
 
     async def get(self, user_id: str) -> ClientFacingUser:
         """
         GET User details given the user_id.
 
         Parameters:
             - user_id: str.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.user.get(
+            user_id="user_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/{user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -570,14 +699,23 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, user_id: str) -> UserSuccessResponse:
         """
         Parameters:
             - user_id: str.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.user.delete(
+            user_id="user_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/{user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -616,15 +754,15 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.user.patch(
-            user_id="user-id",
+            user_id="user_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if fallback_time_zone is not OMIT:
             _request["fallback_time_zone"] = fallback_time_zone
         if fallback_birth_date is not OMIT:
             _request["fallback_birth_date"] = fallback_birth_date
@@ -651,14 +789,23 @@
 
     async def get_by_client_user_id(self, client_user_id: str) -> ClientFacingUser:
         """
         GET user_id from client_user_id.
 
         Parameters:
             - client_user_id: str. A unique ID representing the end user. Typically this will be a user ID number from your application. Personally identifiable information, such as an email address or phone number, should not be used in the client_user_id.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.user.get_by_client_user_id(
+            client_user_id="client_user_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/resolve/{client_user_id}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -674,14 +821,25 @@
 
     async def deregister_provider(self, user_id: str, provider: Providers) -> UserSuccessResponse:
         """
         Parameters:
             - user_id: str.
 
             - provider: Providers. Provider slug. e.g., `oura`, `fitbit`, `garmin`.
+        ---
+        from vital import Providers
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.user.deregister_provider(
+            user_id="user_id",
+            provider=Providers.OURA,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/{user_id}/{provider}"),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
         )
@@ -699,14 +857,21 @@
         self, *, user_id: typing.Optional[str] = None, client_user_id: typing.Optional[str] = None
     ) -> UserSuccessResponse:
         """
         Parameters:
             - user_id: typing.Optional[str]. User ID to undo deletion. Mutually exclusive with `client_user_id`.
 
             - client_user_id: typing.Optional[str]. Client User ID to undo deletion. Mutually exclusive with `user_id`.
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.user.undo_delete()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v2/user/undo_delete"),
             params=remove_none_from_dict({"user_id": user_id, "client_user_id": client_user_id}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
@@ -725,14 +890,23 @@
         """
         Trigger a manual refresh for a specific user
 
         Parameters:
             - user_id: str.
 
             - timeout: typing.Optional[float].
+        ---
+        from vital.client import AsyncVital
+
+        client = AsyncVital(
+            api_key="YOUR_API_KEY",
+        )
+        await client.user.refresh(
+            user_id="user_id",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/user/refresh/{user_id}"),
             params=remove_none_from_dict({"timeout": timeout}),
             headers=self._client_wrapper.get_headers(),
             timeout=60,
```

### Comparing `vital-2.1.7/src/vital/resources/vitals/client.py` & `vital-2.1.8/src/vital/resources/vitals/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,16 +89,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.vo_2_max_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/vo2_max/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -139,16 +139,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.stress_level_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/stress_level/grouped"
             ),
@@ -191,16 +191,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.mindfulness_minutes_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/mindfulness_minutes/grouped"
             ),
@@ -243,16 +243,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.caffeine_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/caffeine/grouped"
             ),
@@ -295,16 +295,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.water_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/water/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -345,16 +345,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.steps_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/steps/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -395,16 +395,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.floors_climbed_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/floors_climbed/grouped"
             ),
@@ -447,16 +447,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.distance_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/distance/grouped"
             ),
@@ -499,16 +499,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.calories_basal_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/calories_basal/grouped"
             ),
@@ -551,16 +551,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.calories_active_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/calories_active/grouped"
             ),
@@ -603,16 +603,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.respiratory_rate_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/respiratory_rate/grouped"
             ),
@@ -655,16 +655,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.ige_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/ige/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -705,16 +705,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.igg_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/igg/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -755,16 +755,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.hypnogram_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/hypnogram/grouped"
             ),
@@ -807,16 +807,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.hrv_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/hrv/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -857,16 +857,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.heartrate_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/heartrate/grouped"
             ),
@@ -909,16 +909,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.glucose_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/glucose/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -959,16 +959,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol/grouped"
             ),
@@ -1011,16 +1011,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.body_weight_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/body_weight/grouped"
             ),
@@ -1063,16 +1063,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.body_fat_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/body_fat/grouped"
             ),
@@ -1115,16 +1115,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.blood_oxygen_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/blood_oxygen/grouped"
             ),
@@ -1167,16 +1167,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.electrocardiogram_voltage_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/electrocardiogram_voltage/grouped"
             ),
@@ -1219,16 +1219,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.blood_pressure_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/blood_pressure/grouped"
             ),
@@ -1268,16 +1268,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.vo_2_max(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/vo2_max"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1313,16 +1313,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.stress_level(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/stress_level"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1358,16 +1358,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.mindfulness_minutes(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/mindfulness_minutes"
             ),
@@ -1405,16 +1405,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.caffeine(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/caffeine"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1450,16 +1450,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.water(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/water"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1495,16 +1495,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.steps(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/steps"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1540,16 +1540,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.floors_climbed(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/floors_climbed"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1585,16 +1585,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.distance(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/distance"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1630,16 +1630,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.calories_basal(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/calories_basal"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1675,16 +1675,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.calories_active(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/calories_active"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1720,16 +1720,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.respiratory_rate(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/respiratory_rate"
             ),
@@ -1767,16 +1767,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.ige(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/ige"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1812,16 +1812,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.igg(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/igg"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1857,16 +1857,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.hypnogram(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/hypnogram"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1902,16 +1902,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.hrv(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/hrv"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1947,16 +1947,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.heartrate(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/heartrate"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -1992,16 +1992,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.glucose(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/glucose"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -2037,16 +2037,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol_triglycerides(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol/triglycerides"
             ),
@@ -2084,16 +2084,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol_total(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol/total"
             ),
@@ -2131,16 +2131,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol_ldl(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol/ldl"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -2176,16 +2176,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol_hdl(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol/hdl"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -2221,16 +2221,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.cholesterol(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -2266,16 +2266,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.body_weight(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/body_weight"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -2311,16 +2311,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.body_fat(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/body_fat"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -2356,16 +2356,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.blood_oxygen(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/blood_oxygen"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -2401,16 +2401,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.electrocardiogram_voltage(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/electrocardiogram_voltage"
             ),
@@ -2448,16 +2448,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.vitals.blood_pressure(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/blood_pressure"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -2501,16 +2501,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.vo_2_max_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/vo2_max/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -2551,16 +2551,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.stress_level_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/stress_level/grouped"
             ),
@@ -2603,16 +2603,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.mindfulness_minutes_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/mindfulness_minutes/grouped"
             ),
@@ -2655,16 +2655,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.caffeine_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/caffeine/grouped"
             ),
@@ -2707,16 +2707,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.water_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/water/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -2757,16 +2757,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.steps_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/steps/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -2807,16 +2807,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.floors_climbed_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/floors_climbed/grouped"
             ),
@@ -2859,16 +2859,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.distance_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/distance/grouped"
             ),
@@ -2911,16 +2911,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.calories_basal_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/calories_basal/grouped"
             ),
@@ -2963,16 +2963,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.calories_active_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/calories_active/grouped"
             ),
@@ -3015,16 +3015,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.respiratory_rate_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/respiratory_rate/grouped"
             ),
@@ -3067,16 +3067,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.ige_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/ige/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -3117,16 +3117,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.igg_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/igg/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -3167,16 +3167,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.hypnogram_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/hypnogram/grouped"
             ),
@@ -3219,16 +3219,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.hrv_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/hrv/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -3269,16 +3269,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.heartrate_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/heartrate/grouped"
             ),
@@ -3321,16 +3321,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.glucose_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/glucose/grouped"),
             params=remove_none_from_dict(
                 {"cursor": cursor, "provider": provider, "start_date": start_date, "end_date": end_date}
@@ -3371,16 +3371,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol/grouped"
             ),
@@ -3423,16 +3423,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.body_weight_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/body_weight/grouped"
             ),
@@ -3475,16 +3475,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.body_fat_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/body_fat/grouped"
             ),
@@ -3527,16 +3527,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.blood_oxygen_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/blood_oxygen/grouped"
             ),
@@ -3579,16 +3579,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.electrocardiogram_voltage_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/electrocardiogram_voltage/grouped"
             ),
@@ -3631,16 +3631,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.blood_pressure_grouped(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/blood_pressure/grouped"
             ),
@@ -3680,16 +3680,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.vo_2_max(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/vo2_max"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -3725,16 +3725,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.stress_level(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/stress_level"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -3770,16 +3770,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.mindfulness_minutes(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/mindfulness_minutes"
             ),
@@ -3817,16 +3817,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.caffeine(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/caffeine"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -3862,16 +3862,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.water(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/water"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -3907,16 +3907,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.steps(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/steps"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -3952,16 +3952,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.floors_climbed(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/floors_climbed"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -3997,16 +3997,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.distance(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/distance"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4042,16 +4042,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.calories_basal(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/calories_basal"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4087,16 +4087,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.calories_active(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/calories_active"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4132,16 +4132,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.respiratory_rate(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/respiratory_rate"
             ),
@@ -4179,16 +4179,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.ige(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/ige"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4224,16 +4224,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.igg(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/igg"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4269,16 +4269,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.hypnogram(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/hypnogram"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4314,16 +4314,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.hrv(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/hrv"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4359,16 +4359,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.heartrate(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/heartrate"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4404,16 +4404,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.glucose(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/glucose"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4449,16 +4449,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol_triglycerides(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol/triglycerides"
             ),
@@ -4496,16 +4496,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol_total(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol/total"
             ),
@@ -4543,16 +4543,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol_ldl(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol/ldl"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4588,16 +4588,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol_hdl(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol/hdl"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4633,16 +4633,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.cholesterol(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/cholesterol"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4678,16 +4678,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.body_weight(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/body_weight"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4723,16 +4723,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.body_fat(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/body_fat"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4768,16 +4768,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.blood_oxygen(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/blood_oxygen"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -4813,16 +4813,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.electrocardiogram_voltage(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/electrocardiogram_voltage"
             ),
@@ -4860,16 +4860,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.vitals.blood_pressure(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/{user_id}/blood_pressure"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
```

### Comparing `vital-2.1.7/src/vital/resources/workouts/client.py` & `vital-2.1.8/src/vital/resources/workouts/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.workouts.get(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/workouts/{user_id}"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -92,16 +92,16 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.workouts.get_raw(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/workouts/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -124,15 +124,15 @@
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.workouts.get_by_workout_id(
-            workout_id="workout-id",
+            workout_id="workout_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/workouts/{workout_id}/stream"
             ),
@@ -176,16 +176,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.workouts.get(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/workouts/{user_id}"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -223,16 +223,16 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.workouts.get_raw(
-            user_id="user-id",
-            start_date="start-date",
+            user_id="user_id",
+            start_date="start_date",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v2/summary/workouts/{user_id}/raw"),
             params=remove_none_from_dict({"provider": provider, "start_date": start_date, "end_date": end_date}),
             headers=self._client_wrapper.get_headers(),
@@ -255,15 +255,15 @@
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.workouts.get_by_workout_id(
-            workout_id="workout-id",
+            workout_id="workout_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"v2/timeseries/workouts/{workout_id}/stream"
             ),
```

### Comparing `vital-2.1.7/src/vital/types/__init__.py` & `vital-2.1.8/src/vital/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,16 @@
     PhysicianCreateRequestSignatureImage_ImagePng,
 )
 from .png import Png
 from .post_order_response import PostOrderResponse
 from .profile_in_db import ProfileInDb
 from .provider_link_response import ProviderLinkResponse
 from .provider_link_response_state import ProviderLinkResponseState
+from .provider_mfa_request import ProviderMfaRequest
+from .provider_mfa_request_method import ProviderMfaRequestMethod
 from .providers import Providers
 from .raw_activity import RawActivity
 from .raw_body import RawBody
 from .raw_devices import RawDevices
 from .raw_profile import RawProfile
 from .raw_sleep import RawSleep
 from .raw_workout import RawWorkout
@@ -455,14 +457,16 @@
     "PhysicianCreateRequestSignatureImage_ImageJpeg",
     "PhysicianCreateRequestSignatureImage_ImagePng",
     "Png",
     "PostOrderResponse",
     "ProfileInDb",
     "ProviderLinkResponse",
     "ProviderLinkResponseState",
+    "ProviderMfaRequest",
+    "ProviderMfaRequestMethod",
     "Providers",
     "RawActivity",
     "RawBody",
     "RawDevices",
     "RawProfile",
     "RawSleep",
     "RawWorkout",
```

### Comparing `vital-2.1.7/src/vital/types/activity_v_2_in_db.py` & `vital-2.1.8/src/vital/types/activity_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/address.py` & `vital-2.1.8/src/vital/types/address.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/appointment_availability_slots.py` & `vital-2.1.8/src/vital/types/appointment_availability_slots.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/appointment_event_status.py` & `vital-2.1.8/src/vital/types/appointment_event_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/appointment_provider.py` & `vital-2.1.8/src/vital/types/appointment_provider.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/appointment_service_type.py` & `vital-2.1.8/src/vital/types/appointment_service_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/appointment_status.py` & `vital-2.1.8/src/vital/types/appointment_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/area_info.py` & `vital-2.1.8/src/vital/types/area_info.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/auth_type.py` & `vital-2.1.8/src/vital/types/auth_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/availability.py` & `vital-2.1.8/src/vital/types/availability.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/biomarker_result.py` & `vital-2.1.8/src/vital/types/biomarker_result.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/body_v_2_in_db.py` & `vital-2.1.8/src/vital/types/body_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_activity_response.py` & `vital-2.1.8/src/vital/types/client_activity_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_body_response.py` & `vital-2.1.8/src/vital/types/client_body_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_activity.py` & `vital-2.1.8/src/vital/types/client_facing_activity.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_api_key.py` & `vital-2.1.8/src/vital/types/client_facing_api_key.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_appointment.py` & `vital-2.1.8/src/vital/types/client_facing_appointment.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_appointment_cancellation_reason.py` & `vital-2.1.8/src/vital/types/client_facing_appointment_cancellation_reason.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_appointment_event.py` & `vital-2.1.8/src/vital/types/client_facing_appointment_event.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_at_home_phlebotomy_order.py` & `vital-2.1.8/src/vital/types/client_facing_at_home_phlebotomy_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_at_home_phlebotomy_order_details.py` & `vital-2.1.8/src/vital/types/client_facing_at_home_phlebotomy_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_blood_oxygen_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_blood_oxygen_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_blood_pressure_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_blood_pressure_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_body.py` & `vital-2.1.8/src/vital/types/client_facing_body.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_body_fat_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_body_fat_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_body_weight_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_body_weight_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_caffeine_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_caffeine_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_calories_active_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_calories_active_timeseries.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     id: typing.Optional[int] = pydantic.Field(description="Deprecated")
     timezone_offset: typing.Optional[int] = pydantic.Field(
         description="Time zone UTC offset in seconds. Positive offset indicates east of UTC; negative offset indicates west of UTC; and null indicates the time zone information is unavailable at source."
     )
     type: typing.Optional[str] = pydantic.Field(
         description="The reading type of the measurement. This is applicable only to Cholesterol, IGG and IGE."
     )
-    unit: typing_extensions.Literal["kcal"]
+    unit: typing_extensions.Literal["kcal"] = pydantic.Field(description="Measured in kilocalories (kcal)")
     timestamp: dt.datetime = pydantic.Field(description="Depracated. The start time (inclusive) of the interval.")
     start: dt.datetime = pydantic.Field(description="The start time (inclusive) of the interval.")
     end: dt.datetime = pydantic.Field(description="The end time (exclusive) of the interval.")
     value: float = pydantic.Field(
         description="Energy consumption caused by the physical activity at the time or interval::kilocalories"
     )
```

### Comparing `vital-2.1.7/src/vital/types/client_facing_calories_basal_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_respiratory_rate_timeseries.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
-
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ClientFacingCaloriesBasalTimeseries(pydantic.BaseModel):
+class ClientFacingRespiratoryRateTimeseries(pydantic.BaseModel):
     id: typing.Optional[int] = pydantic.Field(description="Deprecated")
     timezone_offset: typing.Optional[int] = pydantic.Field(
         description="Time zone UTC offset in seconds. Positive offset indicates east of UTC; negative offset indicates west of UTC; and null indicates the time zone information is unavailable at source."
     )
     type: typing.Optional[str] = pydantic.Field(
         description="The reading type of the measurement. This is applicable only to Cholesterol, IGG and IGE."
     )
-    unit: typing_extensions.Literal["kcal"]
+    unit: str = pydantic.Field(description="Measured in bpm.")
     timestamp: dt.datetime = pydantic.Field(description="The timestamp of the measurement.")
-    value: float = pydantic.Field(description="Basal Metabolic Rate at the time or interval::kilocalories")
+    value: float = pydantic.Field(description="Average respiratory rate::breaths per minute")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/client_facing_cholesterol_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_cholesterol_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_diagnosis_information.py` & `vital-2.1.8/src/vital/types/client_facing_diagnosis_information.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_distance_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_distance_timeseries.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     id: typing.Optional[int] = pydantic.Field(description="Deprecated")
     timezone_offset: typing.Optional[int] = pydantic.Field(
         description="Time zone UTC offset in seconds. Positive offset indicates east of UTC; negative offset indicates west of UTC; and null indicates the time zone information is unavailable at source."
     )
     type: typing.Optional[str] = pydantic.Field(
         description="The reading type of the measurement. This is applicable only to Cholesterol, IGG and IGE."
     )
-    unit: typing_extensions.Literal["m"]
+    unit: typing_extensions.Literal["m"] = pydantic.Field(description="Measured in meters (m)")
     timestamp: dt.datetime = pydantic.Field(description="Depracated. The start time (inclusive) of the interval.")
     start: dt.datetime = pydantic.Field(description="The start time (inclusive) of the interval.")
     end: dt.datetime = pydantic.Field(description="The end time (exclusive) of the interval.")
     value: float = pydantic.Field(description="Distance traveled during activities at the time or interval::steps")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_floors_climbed_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_floors_climbed_timeseries.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     id: typing.Optional[int] = pydantic.Field(description="Deprecated")
     timezone_offset: typing.Optional[int] = pydantic.Field(
         description="Time zone UTC offset in seconds. Positive offset indicates east of UTC; negative offset indicates west of UTC; and null indicates the time zone information is unavailable at source."
     )
     type: typing.Optional[str] = pydantic.Field(
         description="The reading type of the measurement. This is applicable only to Cholesterol, IGG and IGE."
     )
-    unit: typing_extensions.Literal["count"]
+    unit: typing_extensions.Literal["count"] = pydantic.Field(description="Measured in counts")
     timestamp: dt.datetime = pydantic.Field(description="The timestamp of the measurement.")
     value: float = pydantic.Field(description="Number of floors climbed at the time or interval::count")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `vital-2.1.7/src/vital/types/client_facing_food.py` & `vital-2.1.8/src/vital/types/client_facing_food.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_glucose_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_glucose_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_heart_rate.py` & `vital-2.1.8/src/vital/types/client_facing_heart_rate.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_heart_rate_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_heart_rate_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_hrv_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_hrv_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_hypnogram_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_hypnogram_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_ige_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_ige_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_igg_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_igg_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_lab.py` & `vital-2.1.8/src/vital/types/client_facing_lab.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_lab_test.py` & `vital-2.1.8/src/vital/types/client_facing_lab_test.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_loinc.py` & `vital-2.1.8/src/vital/types/client_facing_loinc.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_marker.py` & `vital-2.1.8/src/vital/types/client_facing_marker.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_marker_complete.py` & `vital-2.1.8/src/vital/types/client_facing_marker_complete.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_meal_response.py` & `vital-2.1.8/src/vital/types/client_facing_meal_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_mindfulness_minutes_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_mindfulness_minutes_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_order.py` & `vital-2.1.8/src/vital/types/client_facing_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_order_details.py` & `vital-2.1.8/src/vital/types/client_facing_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_order_event.py` & `vital-2.1.8/src/vital/types/client_facing_order_event.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_patient_details_compatible.py` & `vital-2.1.8/src/vital/types/client_facing_patient_details_compatible.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_payor_search_response.py` & `vital-2.1.8/src/vital/types/client_facing_payor_search_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_physician.py` & `vital-2.1.8/src/vital/types/client_facing_physician.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_profile.py` & `vital-2.1.8/src/vital/types/client_facing_profile.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_provider.py` & `vital-2.1.8/src/vital/types/client_facing_provider.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_provider_detailed.py` & `vital-2.1.8/src/vital/types/client_facing_provider_detailed.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_provider_with_status.py` & `vital-2.1.8/src/vital/types/client_facing_provider_with_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_resource.py` & `vital-2.1.8/src/vital/types/client_facing_resource.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_respiratory_rate_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_stress_level_timeseries.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ClientFacingRespiratoryRateTimeseries(pydantic.BaseModel):
+class ClientFacingStressLevelTimeseries(pydantic.BaseModel):
     id: typing.Optional[int] = pydantic.Field(description="Deprecated")
     timezone_offset: typing.Optional[int] = pydantic.Field(
         description="Time zone UTC offset in seconds. Positive offset indicates east of UTC; negative offset indicates west of UTC; and null indicates the time zone information is unavailable at source."
     )
     type: typing.Optional[str] = pydantic.Field(
         description="The reading type of the measurement. This is applicable only to Cholesterol, IGG and IGE."
     )
-    unit: str = pydantic.Field(description="Measured in bpm.")
+    unit: str = pydantic.Field(description="Measured in percentage (0-100).")
     timestamp: dt.datetime = pydantic.Field(description="The timestamp of the measurement.")
-    value: float = pydantic.Field(description="Average respiratory rate::breaths per minute")
+    value: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/client_facing_result.py` & `vital-2.1.8/src/vital/types/client_facing_result.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_shipment.py` & `vital-2.1.8/src/vital/types/client_facing_shipment.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_sleep.py` & `vital-2.1.8/src/vital/types/client_facing_sleep.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_sleep_stream.py` & `vital-2.1.8/src/vital/types/client_facing_sleep_stream.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_source.py` & `vital-2.1.8/src/vital/types/client_facing_source.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_sport.py` & `vital-2.1.8/src/vital/types/client_facing_sport.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_steps_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_steps_timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     id: typing.Optional[int] = pydantic.Field(description="Deprecated")
     timezone_offset: typing.Optional[int] = pydantic.Field(
         description="Time zone UTC offset in seconds. Positive offset indicates east of UTC; negative offset indicates west of UTC; and null indicates the time zone information is unavailable at source."
     )
     type: typing.Optional[str] = pydantic.Field(
         description="The reading type of the measurement. This is applicable only to Cholesterol, IGG and IGE."
     )
-    unit: typing_extensions.Literal["count"]
+    unit: typing_extensions.Literal["count"] = pydantic.Field(description="Measured in counts")
     timestamp: dt.datetime = pydantic.Field(description="Depracated. The start time (inclusive) of the interval.")
     start: dt.datetime = pydantic.Field(description="The start time (inclusive) of the interval.")
     end: dt.datetime = pydantic.Field(description="The end time (exclusive) of the interval.")
     value: float = pydantic.Field(description="The number of steps sampled at the time or interval::count")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/client_facing_stream.py` & `vital-2.1.8/src/vital/types/client_facing_stream.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_stress_level_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_vo_2_max_timeseries.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ClientFacingStressLevelTimeseries(pydantic.BaseModel):
+class ClientFacingVo2MaxTimeseries(pydantic.BaseModel):
     id: typing.Optional[int] = pydantic.Field(description="Deprecated")
     timezone_offset: typing.Optional[int] = pydantic.Field(
         description="Time zone UTC offset in seconds. Positive offset indicates east of UTC; negative offset indicates west of UTC; and null indicates the time zone information is unavailable at source."
     )
     type: typing.Optional[str] = pydantic.Field(
         description="The reading type of the measurement. This is applicable only to Cholesterol, IGG and IGE."
     )
-    unit: str = pydantic.Field(description="Measured in percentage (0-100).")
-    timestamp: dt.datetime = pydantic.Field(description="The timestamp of the measurement.")
-    value: float
+    unit: str = pydantic.Field(description="Measured in mL/kg/min.")
+    timestamp: dt.datetime = pydantic.Field(description="Depracated. The start time (inclusive) of the interval.")
+    start: dt.datetime = pydantic.Field(description="The start time (inclusive) of the interval.")
+    end: dt.datetime = pydantic.Field(description="The end time (exclusive) of the interval.")
+    value: float = pydantic.Field(description="The recorded value for the interval.")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/client_facing_team.py` & `vital-2.1.8/src/vital/types/client_facing_team.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_test_kit_order_details.py` & `vital-2.1.8/src/vital/types/client_facing_test_kit_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_testkit_order.py` & `vital-2.1.8/src/vital/types/client_facing_testkit_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_user.py` & `vital-2.1.8/src/vital/types/client_facing_user.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_user_key.py` & `vital-2.1.8/src/vital/types/client_facing_user_key.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_vo_2_max_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_calories_basal_timeseries.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+import typing_extensions
+
 from ..core.datetime_utils import serialize_datetime
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ClientFacingVo2MaxTimeseries(pydantic.BaseModel):
+class ClientFacingCaloriesBasalTimeseries(pydantic.BaseModel):
     id: typing.Optional[int] = pydantic.Field(description="Deprecated")
     timezone_offset: typing.Optional[int] = pydantic.Field(
         description="Time zone UTC offset in seconds. Positive offset indicates east of UTC; negative offset indicates west of UTC; and null indicates the time zone information is unavailable at source."
     )
     type: typing.Optional[str] = pydantic.Field(
         description="The reading type of the measurement. This is applicable only to Cholesterol, IGG and IGE."
     )
-    unit: str = pydantic.Field(description="Measured in mL/kg/min.")
-    timestamp: dt.datetime = pydantic.Field(description="Depracated. The start time (inclusive) of the interval.")
-    start: dt.datetime = pydantic.Field(description="The start time (inclusive) of the interval.")
-    end: dt.datetime = pydantic.Field(description="The end time (exclusive) of the interval.")
-    value: float = pydantic.Field(description="The recorded value for the interval.")
+    unit: typing_extensions.Literal["kcal"] = pydantic.Field(description="Measured in kilocalories (kcal)")
+    timestamp: dt.datetime = pydantic.Field(description="The timestamp of the measurement.")
+    value: float = pydantic.Field(description="Basal Metabolic Rate at the time or interval::kilocalories")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/client_facing_walk_in_order_details.py` & `vital-2.1.8/src/vital/types/client_facing_walk_in_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_walk_in_test_order.py` & `vital-2.1.8/src/vital/types/client_facing_walk_in_test_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_water_timeseries.py` & `vital-2.1.8/src/vital/types/client_facing_water_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_facing_workout.py` & `vital-2.1.8/src/vital/types/client_facing_workout.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     max_speed: typing.Optional[float] = pydantic.Field(description="Max speed during workout in m/s::meters/sec")
     average_watts: typing.Optional[float] = pydantic.Field(description="Average watts burned during exercise::watts")
     device_watts: typing.Optional[float] = pydantic.Field(description="Watts burned during exercise::watts")
     max_watts: typing.Optional[float] = pydantic.Field(description="Max watts burned during exercise::watts")
     weighted_average_watts: typing.Optional[float] = pydantic.Field(
         description="Weighted average watts burned during exercise::watts"
     )
-    map: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
-        description="Map of workouts encoded as polyline"
+    map_: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(
+        alias="map", description="Map of workouts encoded as polyline"
     )
     provider_id: str = pydantic.Field(description="Provider ID given for that specific workout")
     source: ClientFacingSource = pydantic.Field(description="Source the data has come from.")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -64,8 +64,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `vital-2.1.7/src/vital/types/client_sleep_response.py` & `vital-2.1.8/src/vital/types/client_sleep_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_user_id_conflict.py` & `vital-2.1.8/src/vital/types/client_user_id_conflict.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/client_workout_response.py` & `vital-2.1.8/src/vital/types/client_workout_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/connected_source_client_facing.py` & `vital-2.1.8/src/vital/types/connected_source_client_facing.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/connection_status.py` & `vital-2.1.8/src/vital/types/link_token_exchange_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .connection_status_state import ConnectionStatusState
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ConnectionStatus(pydantic.BaseModel):
-    success: bool
-    redirect_url: typing.Optional[str]
-    state: ConnectionStatusState
-    error_type: typing.Optional[str]
-    error: typing.Optional[str]
+class LinkTokenExchangeResponse(pydantic.BaseModel):
+    link_token: str = pydantic.Field(description="Link token to use to launch link widget")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/consent.py` & `vital-2.1.8/src/vital/types/consent.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/consent_type.py` & `vital-2.1.8/src/vital/types/consent_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/day_slots.py` & `vital-2.1.8/src/vital/types/day_slots.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/delegated_flow_type.py` & `vital-2.1.8/src/vital/types/delegated_flow_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/demo_connection_status.py` & `vital-2.1.8/src/vital/types/demo_connection_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/demo_providers.py` & `vital-2.1.8/src/vital/types/demo_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/device_v_2_in_db.py` & `vital-2.1.8/src/vital/types/device_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/energy.py` & `vital-2.1.8/src/vital/types/energy.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/event_destination_preferences.py` & `vital-2.1.8/src/vital/types/event_destination_preferences.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/event_destination_preferences_enabled_item.py` & `vital-2.1.8/src/vital/types/event_destination_preferences_enabled_item.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/event_destination_preferences_preferred.py` & `vital-2.1.8/src/vital/types/event_destination_preferences_preferred.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/fallback_birth_date.py` & `vital-2.1.8/src/vital/types/fallback_birth_date.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/fallback_time_zone.py` & `vital-2.1.8/src/vital/types/fallback_time_zone.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/fats.py` & `vital-2.1.8/src/vital/types/fats.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/gender.py` & `vital-2.1.8/src/vital/types/gender.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/get_markers_response.py` & `vital-2.1.8/src/vital/types/get_markers_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/get_orders_response.py` & `vital-2.1.8/src/vital/types/get_orders_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_blood_oxygen.py` & `vital-2.1.8/src/vital/types/grouped_blood_oxygen.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_blood_oxygen_response.py` & `vital-2.1.8/src/vital/types/grouped_blood_oxygen_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_blood_pressure.py` & `vital-2.1.8/src/vital/types/grouped_blood_pressure.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_blood_pressure_response.py` & `vital-2.1.8/src/vital/types/grouped_blood_pressure_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_body_fat.py` & `vital-2.1.8/src/vital/types/grouped_body_fat.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_body_fat_response.py` & `vital-2.1.8/src/vital/types/grouped_body_fat_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_body_weight.py` & `vital-2.1.8/src/vital/types/grouped_body_weight.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_body_weight_response.py` & `vital-2.1.8/src/vital/types/grouped_body_weight_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_caffeine.py` & `vital-2.1.8/src/vital/types/grouped_caffeine.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_caffeine_response.py` & `vital-2.1.8/src/vital/types/grouped_caffeine_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_calories_active.py` & `vital-2.1.8/src/vital/types/grouped_calories_active.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_calories_active_response.py` & `vital-2.1.8/src/vital/types/grouped_calories_active_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_calories_basal.py` & `vital-2.1.8/src/vital/types/grouped_calories_basal.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_calories_basal_response.py` & `vital-2.1.8/src/vital/types/grouped_calories_basal_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_cholesterol.py` & `vital-2.1.8/src/vital/types/grouped_cholesterol.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_cholesterol_response.py` & `vital-2.1.8/src/vital/types/grouped_cholesterol_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_distance.py` & `vital-2.1.8/src/vital/types/grouped_distance.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_distance_response.py` & `vital-2.1.8/src/vital/types/grouped_distance_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_electrocardiogram_voltage.py` & `vital-2.1.8/src/vital/types/grouped_electrocardiogram_voltage.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_electrocardiogram_voltage_response.py` & `vital-2.1.8/src/vital/types/grouped_electrocardiogram_voltage_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_floors_climbed.py` & `vital-2.1.8/src/vital/types/grouped_floors_climbed.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_floors_climbed_response.py` & `vital-2.1.8/src/vital/types/grouped_floors_climbed_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_glucose.py` & `vital-2.1.8/src/vital/types/grouped_glucose.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_glucose_response.py` & `vital-2.1.8/src/vital/types/grouped_glucose_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_heart_rate.py` & `vital-2.1.8/src/vital/types/grouped_heart_rate.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_heart_rate_response.py` & `vital-2.1.8/src/vital/types/grouped_heart_rate_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_hrv.py` & `vital-2.1.8/src/vital/types/grouped_hrv.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_hrv_response.py` & `vital-2.1.8/src/vital/types/grouped_hrv_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_hypnogram.py` & `vital-2.1.8/src/vital/types/grouped_hypnogram.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_hypnogram_response.py` & `vital-2.1.8/src/vital/types/grouped_hypnogram_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_ige.py` & `vital-2.1.8/src/vital/types/grouped_ige.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_ige_response.py` & `vital-2.1.8/src/vital/types/grouped_ige_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_igg.py` & `vital-2.1.8/src/vital/types/grouped_igg.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_igg_response.py` & `vital-2.1.8/src/vital/types/grouped_igg_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_mindfulness_minutes.py` & `vital-2.1.8/src/vital/types/grouped_mindfulness_minutes.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_mindfulness_minutes_response.py` & `vital-2.1.8/src/vital/types/grouped_mindfulness_minutes_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_respiratory_rate.py` & `vital-2.1.8/src/vital/types/grouped_respiratory_rate.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_respiratory_rate_response.py` & `vital-2.1.8/src/vital/types/grouped_respiratory_rate_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_steps.py` & `vital-2.1.8/src/vital/types/grouped_steps.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_steps_response.py` & `vital-2.1.8/src/vital/types/grouped_steps_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_stress_level.py` & `vital-2.1.8/src/vital/types/grouped_stress_level.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_stress_level_response.py` & `vital-2.1.8/src/vital/types/grouped_stress_level_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_vo_2_max.py` & `vital-2.1.8/src/vital/types/grouped_vo_2_max.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_vo_2_max_response.py` & `vital-2.1.8/src/vital/types/grouped_vo_2_max_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_water.py` & `vital-2.1.8/src/vital/types/grouped_water.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/grouped_water_response.py` & `vital-2.1.8/src/vital/types/grouped_water_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/health_insurance_create_request.py` & `vital-2.1.8/src/vital/types/health_insurance_create_request.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/health_insurance_create_request_back_image.py` & `vital-2.1.8/src/vital/types/health_insurance_create_request_back_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/health_insurance_create_request_front_image.py` & `vital-2.1.8/src/vital/types/health_insurance_create_request_front_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/health_insurance_create_request_patient_signature_image.py` & `vital-2.1.8/src/vital/types/health_insurance_create_request_patient_signature_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/historical_pull_status.py` & `vital-2.1.8/src/vital/types/historical_pull_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/http_validation_error.py` & `vital-2.1.8/src/vital/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/jpeg.py` & `vital-2.1.8/src/vital/types/jpeg.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/lab_results_metadata.py` & `vital-2.1.8/src/vital/types/lab_results_metadata.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/lab_results_raw.py` & `vital-2.1.8/src/vital/types/lab_results_raw.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/lab_test_collection_method.py` & `vital-2.1.8/src/vital/types/lab_test_collection_method.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/lab_test_sample_type.py` & `vital-2.1.8/src/vital/types/lab_test_sample_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/lab_test_status.py` & `vital-2.1.8/src/vital/types/lab_test_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/last_attempt.py` & `vital-2.1.8/src/vital/types/last_attempt.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/libre_config.py` & `vital-2.1.8/src/vital/types/libre_config.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/link_token_exchange_response.py` & `vital-2.1.8/src/vital/types/physician_create_request_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class LinkTokenExchangeResponse(pydantic.BaseModel):
-    link_token: str = pydantic.Field(description="Link token to use to launch link widget")
+class PhysicianCreateRequestBase(pydantic.BaseModel):
+    first_name: str
+    last_name: str
+    email: typing.Optional[str]
+    npi: str
+    licensed_states: typing.Optional[typing.List[str]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/lng_lat.py` & `vital-2.1.8/src/vital/types/lng_lat.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/macros.py` & `vital-2.1.8/src/vital/types/macros.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/manual_providers.py` & `vital-2.1.8/src/vital/types/manual_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/meal_in_db_base_client_facing_source.py` & `vital-2.1.8/src/vital/types/meal_in_db_base_client_facing_source.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/metrics_result.py` & `vital-2.1.8/src/vital/types/metrics_result.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/micros.py` & `vital-2.1.8/src/vital/types/micros.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/o_auth_providers.py` & `vital-2.1.8/src/vital/types/o_auth_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/order_status.py` & `vital-2.1.8/src/vital/types/order_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/order_top_level_status.py` & `vital-2.1.8/src/vital/types/order_top_level_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/paginated_users_response.py` & `vital-2.1.8/src/vital/types/paginated_users_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/password_providers.py` & `vital-2.1.8/src/vital/types/password_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/patient_address_compatible.py` & `vital-2.1.8/src/vital/types/patient_address_compatible.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/patient_details.py` & `vital-2.1.8/src/vital/types/patient_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/person_details.py` & `vital-2.1.8/src/vital/types/person_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/phlebotomy_area_info.py` & `vital-2.1.8/src/vital/types/phlebotomy_area_info.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/phlebotomy_provider_info.py` & `vital-2.1.8/src/vital/types/phlebotomy_provider_info.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/physician_create_request.py` & `vital-2.1.8/src/vital/types/physician_create_request.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/physician_create_request_base.py` & `vital-2.1.8/src/vital/types/png.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class PhysicianCreateRequestBase(pydantic.BaseModel):
-    first_name: str
-    last_name: str
-    email: typing.Optional[str]
-    npi: str
-    licensed_states: typing.Optional[typing.List[str]]
+class Png(pydantic.BaseModel):
+    content: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/physician_create_request_signature_image.py` & `vital-2.1.8/src/vital/types/physician_create_request_signature_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/png.py` & `vital-2.1.8/src/vital/types/user_sign_in_token_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class Png(pydantic.BaseModel):
-    content: str
+class UserSignInTokenResponse(pydantic.BaseModel):
+    user_id: str
+    sign_in_token: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/post_order_response.py` & `vital-2.1.8/src/vital/types/post_order_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/profile_in_db.py` & `vital-2.1.8/src/vital/types/workout_v_2_in_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .client_facing_provider import ClientFacingProvider
+from .client_facing_sport import ClientFacingSport
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ProfileInDb(pydantic.BaseModel):
-    data: typing.Optional[str]
+class WorkoutV2InDb(pydantic.BaseModel):
+    timestamp: dt.datetime
+    data: typing.Dict[str, typing.Any]
+    provider_id: str
     user_id: str
     source_id: int
     priority_id: typing.Optional[int]
     id: str
+    sport_id: int
     source: ClientFacingProvider
-    updated_at: typing.Optional[dt.datetime]
+    sport: ClientFacingSport
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/provider_link_response.py` & `vital-2.1.8/src/vital/types/provider_link_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .password_providers import PasswordProviders
 from .provider_link_response_state import ProviderLinkResponseState
+from .provider_mfa_request import ProviderMfaRequest
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class ProviderLinkResponse(pydantic.BaseModel):
-    provider: PasswordProviders
-    connected: bool
-    provider_id: typing.Optional[str]
     state: ProviderLinkResponseState
     error_type: typing.Optional[str]
     error: typing.Optional[str]
+    provider_mfa: typing.Optional[ProviderMfaRequest]
+    provider: PasswordProviders
+    connected: bool
+    provider_id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/providers.py` & `vital-2.1.8/src/vital/types/providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     WHOOP = "whoop"
     STRAVA = "strava"
     RENPHO = "renpho"
     PELOTON = "peloton"
     WAHOO = "wahoo"
     ZWIFT = "zwift"
     FREESTYLE_LIBRE = "freestyle_libre"
+    ABBOTT_LIBREVIEW = "abbott_libreview"
     FREESTYLE_LIBRE_BLE = "freestyle_libre_ble"
     EIGHT_SLEEP = "eight_sleep"
     WITHINGS = "withings"
     APPLE_HEALTH_KIT = "apple_health_kit"
     MANUAL = "manual"
     IHEALTH = "ihealth"
     GOOGLE_FIT = "google_fit"
@@ -53,14 +54,15 @@
         whoop: typing.Callable[[], T_Result],
         strava: typing.Callable[[], T_Result],
         renpho: typing.Callable[[], T_Result],
         peloton: typing.Callable[[], T_Result],
         wahoo: typing.Callable[[], T_Result],
         zwift: typing.Callable[[], T_Result],
         freestyle_libre: typing.Callable[[], T_Result],
+        abbott_libreview: typing.Callable[[], T_Result],
         freestyle_libre_ble: typing.Callable[[], T_Result],
         eight_sleep: typing.Callable[[], T_Result],
         withings: typing.Callable[[], T_Result],
         apple_health_kit: typing.Callable[[], T_Result],
         manual: typing.Callable[[], T_Result],
         ihealth: typing.Callable[[], T_Result],
         google_fit: typing.Callable[[], T_Result],
@@ -97,14 +99,16 @@
             return peloton()
         if self is Providers.WAHOO:
             return wahoo()
         if self is Providers.ZWIFT:
             return zwift()
         if self is Providers.FREESTYLE_LIBRE:
             return freestyle_libre()
+        if self is Providers.ABBOTT_LIBREVIEW:
+            return abbott_libreview()
         if self is Providers.FREESTYLE_LIBRE_BLE:
             return freestyle_libre_ble()
         if self is Providers.EIGHT_SLEEP:
             return eight_sleep()
         if self is Providers.WITHINGS:
             return withings()
         if self is Providers.APPLE_HEALTH_KIT:
```

### Comparing `vital-2.1.7/src/vital/types/raw_activity.py` & `vital-2.1.8/src/vital/types/raw_activity.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/raw_body.py` & `vital-2.1.8/src/vital/types/raw_body.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/raw_devices.py` & `vital-2.1.8/src/vital/types/raw_devices.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/raw_profile.py` & `vital-2.1.8/src/vital/types/raw_profile.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/raw_sleep.py` & `vital-2.1.8/src/vital/types/raw_sleep.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/raw_workout.py` & `vital-2.1.8/src/vital/types/raw_workout.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/region.py` & `vital-2.1.8/src/vital/types/region.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/resource_availability.py` & `vital-2.1.8/src/vital/types/resource_availability.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/responsible_relationship.py` & `vital-2.1.8/src/vital/types/responsible_relationship.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/result_type.py` & `vital-2.1.8/src/vital/types/result_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/scope_requirements_grants.py` & `vital-2.1.8/src/vital/types/scope_requirements_grants.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/scope_requirements_str.py` & `vital-2.1.8/src/vital/types/scope_requirements_str.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/shipping_address.py` & `vital-2.1.8/src/vital/types/shipping_address.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/single_historical_pull_statistics.py` & `vital-2.1.8/src/vital/types/single_historical_pull_statistics.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/single_provider_historical_pull_response.py` & `vital-2.1.8/src/vital/types/single_provider_historical_pull_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/single_resource_statistics.py` & `vital-2.1.8/src/vital/types/single_resource_statistics.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/single_user_historical_pull_response.py` & `vital-2.1.8/src/vital/types/single_user_historical_pull_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/single_user_resource_response.py` & `vital-2.1.8/src/vital/types/single_user_resource_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/sleep_v_2_in_db.py` & `vital-2.1.8/src/vital/types/sleep_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/source.py` & `vital-2.1.8/src/vital/types/source.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/source_auth_type.py` & `vital-2.1.8/src/vital/types/source_auth_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/source_link.py` & `vital-2.1.8/src/vital/types/source_link.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/source_type.py` & `vital-2.1.8/src/vital/types/source_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/team_config.py` & `vital-2.1.8/src/vital/types/team_config.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/time_slot.py` & `vital-2.1.8/src/vital/types/time_slot.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/timeseries_metric_point.py` & `vital-2.1.8/src/vital/types/timeseries_metric_point.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/timeseries_resource.py` & `vital-2.1.8/src/vital/types/timeseries_resource.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/us_address.py` & `vital-2.1.8/src/vital/types/us_address.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/user_historical_pulls_response.py` & `vital-2.1.8/src/vital/types/user_historical_pulls_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/user_refresh_error_response.py` & `vital-2.1.8/src/vital/types/user_refresh_error_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class UserRefreshErrorResponse(pydantic.BaseModel):
-    success: str = pydantic.Field(description="Whether operation was successful or not")
+    success: bool = pydantic.Field(description="Whether operation was successful or not")
     user_id: str = pydantic.Field(
         description="A unique ID representing the end user. Typically this will be a user ID from your application. Personally identifiable information, such as an email address or phone number, should not be used in the client_user_id."
     )
     error: str
     failed_sources: typing.Optional[typing.List[str]]
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `vital-2.1.7/src/vital/types/user_refresh_success_response.py` & `vital-2.1.8/src/vital/types/user_refresh_success_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class UserRefreshSuccessResponse(pydantic.BaseModel):
-    success: str = pydantic.Field(description="Whether operation was successful or not")
+    success: bool = pydantic.Field(description="Whether operation was successful or not")
     user_id: str = pydantic.Field(
         description="A unique ID representing the end user. Typically this will be a user ID from your application. Personally identifiable information, such as an email address or phone number, should not be used in the client_user_id."
     )
     refreshed_sources: typing.List[str]
     in_progress_sources: typing.List[str]
     failed_sources: typing.List[str]
```

### Comparing `vital-2.1.7/src/vital/types/user_resources_response.py` & `vital-2.1.8/src/vital/types/user_resources_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/user_sign_in_token_response.py` & `vital-2.1.8/src/vital/types/vital_token_created_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UserSignInTokenResponse(pydantic.BaseModel):
-    user_id: str
-    sign_in_token: str
+class VitalTokenCreatedResponse(pydantic.BaseModel):
+    code: str
+    exchange_url: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/user_success_response.py` & `vital-2.1.8/src/vital/types/user_success_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/validation_error.py` & `vital-2.1.8/src/vital/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.7/src/vital/types/vital_token_created_response.py` & `vital-2.1.8/src/vital/types/profile_in_db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .client_facing_provider import ClientFacingProvider
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class VitalTokenCreatedResponse(pydantic.BaseModel):
-    code: str
-    exchange_url: str
+class ProfileInDb(pydantic.BaseModel):
+    data: typing.Optional[typing.Any]
+    user_id: str
+    source_id: int
+    priority_id: typing.Optional[int]
+    id: str
+    source: ClientFacingProvider
+    updated_at: typing.Optional[dt.datetime]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/src/vital/types/workout_v_2_in_db.py` & `vital-2.1.8/src/vital/types/connection_status.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .client_facing_provider import ClientFacingProvider
-from .client_facing_sport import ClientFacingSport
+from .connection_status_state import ConnectionStatusState
+from .provider_mfa_request import ProviderMfaRequest
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class WorkoutV2InDb(pydantic.BaseModel):
-    timestamp: dt.datetime
-    data: typing.Dict[str, typing.Any]
-    provider_id: str
-    user_id: str
-    source_id: int
-    priority_id: typing.Optional[int]
-    id: str
-    sport_id: int
-    source: ClientFacingProvider
-    sport: ClientFacingSport
+class ConnectionStatus(pydantic.BaseModel):
+    state: ConnectionStatusState
+    error_type: typing.Optional[str]
+    error: typing.Optional[str]
+    provider_mfa: typing.Optional[ProviderMfaRequest]
+    success: bool
+    redirect_url: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.7/PKG-INFO` & `vital-2.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital
-Version: 2.1.7
+Version: 2.1.8
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

