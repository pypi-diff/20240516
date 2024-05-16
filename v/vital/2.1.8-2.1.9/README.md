# Comparing `tmp/vital-2.1.8.tar.gz` & `tmp/vital-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-2.1.8.tar", max compression
+gzip compressed data, was "vital-2.1.9.tar", max compression
```

## Comparing `vital-2.1.8.tar` & `vital-2.1.9.tar`

### file list

```diff
@@ -1,284 +1,284 @@
--rw-r--r--   0        0        0     3329 2024-05-10 08:37:28.807833 vital-2.1.8/README.md
--rw-r--r--   0        0        0      396 2024-05-10 08:37:28.807833 vital-2.1.8/pyproject.toml
--rw-r--r--   0        0        0    14803 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/__init__.py
--rw-r--r--   0        0        0     5248 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/client.py
--rw-r--r--   0        0        0      519 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/api_error.py
--rw-r--r--   0        0        0     1080 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      308 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/environment.py
--rw-r--r--   0        0        0      236 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/errors/bad_request_error.py
--rw-r--r--   0        0        0      313 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/py.typed
--rw-r--r--   0        0        0      532 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/activity/__init__.py
--rw-r--r--   0        0        0     8604 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/activity/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/body/__init__.py
--rw-r--r--   0        0        0     8520 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/body/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/devices/__init__.py
--rw-r--r--   0        0        0     3641 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/devices/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/insurance/__init__.py
--rw-r--r--   0        0        0     7153 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/insurance/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/introspect/__init__.py
--rw-r--r--   0        0        0     7869 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/introspect/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/lab_tests/__init__.py
--rw-r--r--   0        0        0    75759 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/lab_tests/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/link/__init__.py
--rw-r--r--   0        0        0    44285 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/link/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/meal/__init__.py
--rw-r--r--   0        0        0     4703 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/meal/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/profile/__init__.py
--rw-r--r--   0        0        0     6502 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/profile/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/providers/__init__.py
--rw-r--r--   0        0        0     2668 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/providers/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/sleep/__init__.py
--rw-r--r--   0        0        0    15040 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/sleep/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/team/__init__.py
--rw-r--r--   0        0        0    18402 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/team/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/testkit/__init__.py
--rw-r--r--   0        0        0     8435 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/testkit/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/user/__init__.py
--rw-r--r--   0        0        0    40454 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/user/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/vitals/__init__.py
--rw-r--r--   0        0        0   209296 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/vitals/client.py
--rw-r--r--   0        0        0       65 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/workouts/__init__.py
--rw-r--r--   0        0        0    11221 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/resources/workouts/client.py
--rw-r--r--   0        0        0    21631 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/__init__.py
--rw-r--r--   0        0        0     1103 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/activity_v_2_in_db.py
--rw-r--r--   0        0        0      967 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/address.py
--rw-r--r--   0        0        0      971 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_availability_slots.py
--rw-r--r--   0        0        0     1074 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_event_status.py
--rw-r--r--   0        0        0      748 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_provider.py
--rw-r--r--   0        0        0      661 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_service_type.py
--rw-r--r--   0        0        0     1044 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_status.py
--rw-r--r--   0        0        0      149 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/appointment_type.py
--rw-r--r--   0        0        0      957 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/area_info.py
--rw-r--r--   0        0        0      510 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/attempt_status.py
--rw-r--r--   0        0        0      649 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/auth_type.py
--rw-r--r--   0        0        0      537 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/availability.py
--rw-r--r--   0        0        0     1468 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/biomarker_result.py
--rw-r--r--   0        0        0     1168 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/body_v_2_in_db.py
--rw-r--r--   0        0        0      970 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_activity_response.py
--rw-r--r--   0        0        0      950 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_body_response.py
--rw-r--r--   0        0        0     3581 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_activity.py
--rw-r--r--   0        0        0     1010 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_api_key.py
--rw-r--r--   0        0        0     1815 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_appointment.py
--rw-r--r--   0        0        0      934 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_appointment_cancellation_reason.py
--rw-r--r--   0        0        0     1051 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_appointment_event.py
--rw-r--r--   0        0        0     1193 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_at_home_phlebotomy_order.py
--rw-r--r--   0        0        0     1030 2024-05-10 08:37:28.807833 vital-2.1.8/src/vital/types/client_facing_at_home_phlebotomy_order_details.py
--rw-r--r--   0        0        0     1634 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_blood_oxygen_timeseries.py
--rw-r--r--   0        0        0     1632 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_blood_pressure_timeseries.py
--rw-r--r--   0        0        0     1637 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_body.py
--rw-r--r--   0        0        0     1631 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_body_fat_timeseries.py
--rw-r--r--   0        0        0     1630 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_body_weight_timeseries.py
--rw-r--r--   0        0        0     1859 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_caffeine_timeseries.py
--rw-r--r--   0        0        0     1983 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_calories_active_timeseries.py
--rw-r--r--   0        0        0     1722 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_calories_basal_timeseries.py
--rw-r--r--   0        0        0     1623 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_cholesterol_timeseries.py
--rw-r--r--   0        0        0     1071 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_diagnosis_information.py
--rw-r--r--   0        0        0     1929 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_distance_timeseries.py
--rw-r--r--   0        0        0     1540 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py
--rw-r--r--   0        0        0     1707 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_floors_climbed_timeseries.py
--rw-r--r--   0        0        0     1048 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_food.py
--rw-r--r--   0        0        0     1619 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_glucose_timeseries.py
--rw-r--r--   0        0        0     1236 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_heart_rate.py
--rw-r--r--   0        0        0     1606 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_heart_rate_timeseries.py
--rw-r--r--   0        0        0     1624 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_hrv_timeseries.py
--rw-r--r--   0        0        0     1968 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_hypnogram_timeseries.py
--rw-r--r--   0        0        0     1612 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_ige_timeseries.py
--rw-r--r--   0        0        0     1612 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_igg_timeseries.py
--rw-r--r--   0        0        0     1183 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_lab.py
--rw-r--r--   0        0        0     1780 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_lab_test.py
--rw-r--r--   0        0        0      945 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_loinc.py
--rw-r--r--   0        0        0     1147 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_marker.py
--rw-r--r--   0        0        0     1262 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_marker_complete.py
--rw-r--r--   0        0        0     1003 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_meal_response.py
--rw-r--r--   0        0        0     1861 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_mindfulness_minutes_timeseries.py
--rw-r--r--   0        0        0     3286 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_order.py
--rw-r--r--   0        0        0     1311 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_order_details.py
--rw-r--r--   0        0        0      967 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_order_event.py
--rw-r--r--   0        0        0     1060 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_patient_details_compatible.py
--rw-r--r--   0        0        0     1239 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_payor_search_response.py
--rw-r--r--   0        0        0      916 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_physician.py
--rw-r--r--   0        0        0     1210 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_profile.py
--rw-r--r--   0        0        0     1164 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_provider.py
--rw-r--r--   0        0        0     1418 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_provider_detailed.py
--rw-r--r--   0        0        0     1302 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_provider_with_status.py
--rw-r--r--   0        0        0     6046 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_resource.py
--rw-r--r--   0        0        0     1639 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_respiratory_rate_timeseries.py
--rw-r--r--   0        0        0     1088 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_result.py
--rw-r--r--   0        0        0     1862 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_shipment.py
--rw-r--r--   0        0        0     4877 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_sleep.py
--rw-r--r--   0        0        0     1497 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_sleep_stream.py
--rw-r--r--   0        0        0     1898 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_source.py
--rw-r--r--   0        0        0     1003 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_sport.py
--rw-r--r--   0        0        0     1918 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_steps_timeseries.py
--rw-r--r--   0        0        0     1447 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_stream.py
--rw-r--r--   0        0        0     1573 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_stress_level_timeseries.py
--rw-r--r--   0        0        0     1936 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_team.py
--rw-r--r--   0        0        0      992 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_test_kit_order_details.py
--rw-r--r--   0        0        0     1273 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_testkit_order.py
--rw-r--r--   0        0        0     2915 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_user.py
--rw-r--r--   0        0        0     1367 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_user_key.py
--rw-r--r--   0        0        0     1844 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_vo_2_max_timeseries.py
--rw-r--r--   0        0        0     1002 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_walk_in_order_details.py
--rw-r--r--   0        0        0     1129 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_walk_in_test_order.py
--rw-r--r--   0        0        0     1638 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_water_timeseries.py
--rw-r--r--   0        0        0     4328 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_facing_workout.py
--rw-r--r--   0        0        0      955 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_sleep_response.py
--rw-r--r--   0        0        0      951 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_user_id_conflict.py
--rw-r--r--   0        0        0      966 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/client_workout_response.py
--rw-r--r--   0        0        0     1271 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/connected_source_client_facing.py
--rw-r--r--   0        0        0     1184 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/connection_status.py
--rw-r--r--   0        0        0      734 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/connection_status_state.py
--rw-r--r--   0        0        0     1126 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/consent.py
--rw-r--r--   0        0        0     1519 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/consent_type.py
--rw-r--r--   0        0        0      930 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/day_slots.py
--rw-r--r--   0        0        0     1240 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/delegated_flow_type.py
--rw-r--r--   0        0        0      897 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/demo_connection_status.py
--rw-r--r--   0        0        0      892 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/demo_providers.py
--rw-r--r--   0        0        0     1053 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/device_v_2_in_db.py
--rw-r--r--   0        0        0      153 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/email_providers.py
--rw-r--r--   0        0        0      936 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/energy.py
--rw-r--r--   0        0        0     1172 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/event_destination_preferences.py
--rw-r--r--   0        0        0      762 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/event_destination_preferences_enabled_item.py
--rw-r--r--   0        0        0      754 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/event_destination_preferences_preferred.py
--rw-r--r--   0        0        0     1169 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/fallback_birth_date.py
--rw-r--r--   0        0        0     1376 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/fallback_time_zone.py
--rw-r--r--   0        0        0     1623 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/fats.py
--rw-r--r--   0        0        0      762 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/gender.py
--rw-r--r--   0        0        0     1110 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/get_markers_response.py
--rw-r--r--   0        0        0     1048 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/get_orders_response.py
--rw-r--r--   0        0        0     1087 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_blood_oxygen.py
--rw-r--r--   0        0        0     1254 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_blood_oxygen_response.py
--rw-r--r--   0        0        0     1095 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_blood_pressure.py
--rw-r--r--   0        0        0     1262 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_blood_pressure_response.py
--rw-r--r--   0        0        0     1071 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_body_fat.py
--rw-r--r--   0        0        0     1238 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_body_fat_response.py
--rw-r--r--   0        0        0     1083 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_body_weight.py
--rw-r--r--   0        0        0     1250 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_body_weight_response.py
--rw-r--r--   0        0        0     1074 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_caffeine.py
--rw-r--r--   0        0        0     1241 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_caffeine_response.py
--rw-r--r--   0        0        0     1099 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_calories_active.py
--rw-r--r--   0        0        0     1266 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_calories_active_response.py
--rw-r--r--   0        0        0     1095 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_calories_basal.py
--rw-r--r--   0        0        0     1262 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_calories_basal_response.py
--rw-r--r--   0        0        0     1086 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_cholesterol.py
--rw-r--r--   0        0        0     1253 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_cholesterol_response.py
--rw-r--r--   0        0        0     1074 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_distance.py
--rw-r--r--   0        0        0     1241 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_distance_response.py
--rw-r--r--   0        0        0     1139 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_electrocardiogram_voltage.py
--rw-r--r--   0        0        0     1306 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_electrocardiogram_voltage_response.py
--rw-r--r--   0        0        0     1095 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_floors_climbed.py
--rw-r--r--   0        0        0     1262 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_floors_climbed_response.py
--rw-r--r--   0        0        0     1070 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_glucose.py
--rw-r--r--   0        0        0     1237 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_glucose_response.py
--rw-r--r--   0        0        0     1079 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_heart_rate.py
--rw-r--r--   0        0        0     1246 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_heart_rate_response.py
--rw-r--r--   0        0        0     1054 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_hrv.py
--rw-r--r--   0        0        0     1221 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_hrv_response.py
--rw-r--r--   0        0        0     1078 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_hypnogram.py
--rw-r--r--   0        0        0     1245 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_hypnogram_response.py
--rw-r--r--   0        0        0     1054 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_ige.py
--rw-r--r--   0        0        0     1221 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_ige_response.py
--rw-r--r--   0        0        0     1054 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_igg.py
--rw-r--r--   0        0        0     1221 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_igg_response.py
--rw-r--r--   0        0        0     1115 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_mindfulness_minutes.py
--rw-r--r--   0        0        0     1282 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_mindfulness_minutes_response.py
--rw-r--r--   0        0        0     1103 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_respiratory_rate.py
--rw-r--r--   0        0        0     1270 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_respiratory_rate_response.py
--rw-r--r--   0        0        0     1062 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_steps.py
--rw-r--r--   0        0        0     1229 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_steps_response.py
--rw-r--r--   0        0        0     1087 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_stress_level.py
--rw-r--r--   0        0        0     1254 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_stress_level_response.py
--rw-r--r--   0        0        0     1068 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_vo_2_max.py
--rw-r--r--   0        0        0     1235 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_vo_2_max_response.py
--rw-r--r--   0        0        0     1062 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_water.py
--rw-r--r--   0        0        0     1229 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/grouped_water_response.py
--rw-r--r--   0        0        0     3022 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/health_insurance_create_request.py
--rw-r--r--   0        0        0      811 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/health_insurance_create_request_back_image.py
--rw-r--r--   0        0        0      816 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/health_insurance_create_request_front_image.py
--rw-r--r--   0        0        0      876 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/health_insurance_create_request_patient_signature_image.py
--rw-r--r--   0        0        0      732 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/historical_pull_status.py
--rw-r--r--   0        0        0      966 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/http_validation_error.py
--rw-r--r--   0        0        0      864 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/jpeg.py
--rw-r--r--   0        0        0     1289 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_results_metadata.py
--rw-r--r--   0        0        0     1034 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_results_raw.py
--rw-r--r--   0        0        0      223 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_results_raw_results.py
--rw-r--r--   0        0        0      827 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_test_collection_method.py
--rw-r--r--   0        0        0      898 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_test_sample_type.py
--rw-r--r--   0        0        0      729 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lab_test_status.py
--rw-r--r--   0        0        0      949 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/last_attempt.py
--rw-r--r--   0        0        0      936 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/libre_config.py
--rw-r--r--   0        0        0      960 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/link_token_exchange_response.py
--rw-r--r--   0        0        0      879 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/lng_lat.py
--rw-r--r--   0        0        0     1553 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/macros.py
--rw-r--r--   0        0        0     1792 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/manual_providers.py
--rw-r--r--   0        0        0      501 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/marker_type.py
--rw-r--r--   0        0        0     1444 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/meal_in_db_base_client_facing_source.py
--rw-r--r--   0        0        0     1233 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/metrics_result.py
--rw-r--r--   0        0        0     1272 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/micros.py
--rw-r--r--   0        0        0     2126 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/o_auth_providers.py
--rw-r--r--   0        0        0     9798 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/order_status.py
--rw-r--r--   0        0        0     1265 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/order_top_level_status.py
--rw-r--r--   0        0        0     1001 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/paginated_users_response.py
--rw-r--r--   0        0        0     1779 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/password_providers.py
--rw-r--r--   0        0        0     1063 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/patient_address_compatible.py
--rw-r--r--   0        0        0     1000 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/patient_details.py
--rw-r--r--   0        0        0     1004 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/person_details.py
--rw-r--r--   0        0        0      993 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/phlebotomy_area_info.py
--rw-r--r--   0        0        0     1065 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/phlebotomy_provider_info.py
--rw-r--r--   0        0        0     1281 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/physician_create_request.py
--rw-r--r--   0        0        0     1008 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/physician_create_request_base.py
--rw-r--r--   0        0        0      806 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/physician_create_request_signature_image.py
--rw-r--r--   0        0        0      863 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/png.py
--rw-r--r--   0        0        0      973 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/post_order_response.py
--rw-r--r--   0        0        0     1113 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/profile_in_db.py
--rw-r--r--   0        0        0     1284 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/provider_link_response.py
--rw-r--r--   0        0        0      750 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/provider_link_response_state.py
--rw-r--r--   0        0        0      978 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/provider_mfa_request.py
--rw-r--r--   0        0        0      476 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/provider_mfa_request_method.py
--rw-r--r--   0        0        0     5340 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/providers.py
--rw-r--r--   0        0        0      943 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_activity.py
--rw-r--r--   0        0        0      923 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_body.py
--rw-r--r--   0        0        0      935 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_devices.py
--rw-r--r--   0        0        0      917 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_profile.py
--rw-r--r--   0        0        0      928 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_sleep.py
--rw-r--r--   0        0        0      939 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/raw_workout.py
--rw-r--r--   0        0        0     1360 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/region.py
--rw-r--r--   0        0        0     1055 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/resource_availability.py
--rw-r--r--   0        0        0      761 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/responsible_relationship.py
--rw-r--r--   0        0        0      662 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/result_type.py
--rw-r--r--   0        0        0     1000 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/scope_requirements_grants.py
--rw-r--r--   0        0        0      925 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/scope_requirements_str.py
--rw-r--r--   0        0        0     1020 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/shipping_address.py
--rw-r--r--   0        0        0     1146 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/single_historical_pull_statistics.py
--rw-r--r--   0        0        0     1125 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/single_provider_historical_pull_response.py
--rw-r--r--   0        0        0     1081 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/single_resource_statistics.py
--rw-r--r--   0        0        0     1052 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/single_user_historical_pull_response.py
--rw-r--r--   0        0        0     1026 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/single_user_resource_response.py
--rw-r--r--   0        0        0     1152 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/sleep_v_2_in_db.py
--rw-r--r--   0        0        0     1246 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/source.py
--rw-r--r--   0        0        0     1209 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/source_auth_type.py
--rw-r--r--   0        0        0     1123 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/source_link.py
--rw-r--r--   0        0        0      892 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/source_type.py
--rw-r--r--   0        0        0     1303 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/team_config.py
--rw-r--r--   0        0        0     1147 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/time_slot.py
--rw-r--r--   0        0        0      903 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/timeseries_metric_point.py
--rw-r--r--   0        0        0     4865 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/timeseries_resource.py
--rw-r--r--   0        0        0     1138 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/us_address.py
--rw-r--r--   0        0        0     1040 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_historical_pulls_response.py
--rw-r--r--   0        0        0     1305 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_refresh_error_response.py
--rw-r--r--   0        0        0     1357 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_refresh_success_response.py
--rw-r--r--   0        0        0     1015 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_resources_response.py
--rw-r--r--   0        0        0      906 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_sign_in_token_response.py
--rw-r--r--   0        0        0      952 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/user_success_response.py
--rw-r--r--   0        0        0      992 2024-05-10 08:37:28.811833 vital-2.1.8/src/vital/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-10 08:37:28.815833 vital-2.1.8/src/vital/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      904 2024-05-10 08:37:28.815833 vital-2.1.8/src/vital/types/vital_token_created_response.py
--rw-r--r--   0        0        0     1217 2024-05-10 08:37:28.815833 vital-2.1.8/src/vital/types/workout_v_2_in_db.py
--rw-r--r--   0        0        0     3831 1970-01-01 00:00:00.000000 vital-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3329 2024-05-16 09:05:08.723565 vital-2.1.9/README.md
+-rw-r--r--   0        0        0      396 2024-05-16 09:05:08.723565 vital-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0    14803 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/__init__.py
+-rw-r--r--   0        0        0     5248 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/client.py
+-rw-r--r--   0        0        0      519 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/core/api_error.py
+-rw-r--r--   0        0        0     1080 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      308 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/environment.py
+-rw-r--r--   0        0        0      236 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/errors/bad_request_error.py
+-rw-r--r--   0        0        0      313 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/py.typed
+-rw-r--r--   0        0        0      532 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/activity/__init__.py
+-rw-r--r--   0        0        0     8604 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/activity/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/body/__init__.py
+-rw-r--r--   0        0        0     8520 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/body/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/devices/__init__.py
+-rw-r--r--   0        0        0     3641 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/devices/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/insurance/__init__.py
+-rw-r--r--   0        0        0     7153 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/insurance/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/introspect/__init__.py
+-rw-r--r--   0        0        0     7869 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/introspect/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/lab_tests/__init__.py
+-rw-r--r--   0        0        0    75759 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/lab_tests/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/link/__init__.py
+-rw-r--r--   0        0        0    44285 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/link/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/meal/__init__.py
+-rw-r--r--   0        0        0     4703 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/meal/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/profile/__init__.py
+-rw-r--r--   0        0        0     6502 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/profile/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/providers/__init__.py
+-rw-r--r--   0        0        0     2668 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/providers/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/sleep/__init__.py
+-rw-r--r--   0        0        0    15040 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/sleep/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/team/__init__.py
+-rw-r--r--   0        0        0    18402 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/team/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/testkit/__init__.py
+-rw-r--r--   0        0        0     8435 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/testkit/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/user/__init__.py
+-rw-r--r--   0        0        0    40498 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/user/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/vitals/__init__.py
+-rw-r--r--   0        0        0   209296 2024-05-16 09:05:08.723565 vital-2.1.9/src/vital/resources/vitals/client.py
+-rw-r--r--   0        0        0       65 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/resources/workouts/__init__.py
+-rw-r--r--   0        0        0    11221 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/resources/workouts/client.py
+-rw-r--r--   0        0        0    21631 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/activity_v_2_in_db.py
+-rw-r--r--   0        0        0      967 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/address.py
+-rw-r--r--   0        0        0      971 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/appointment_availability_slots.py
+-rw-r--r--   0        0        0     1074 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/appointment_event_status.py
+-rw-r--r--   0        0        0      748 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/appointment_provider.py
+-rw-r--r--   0        0        0      661 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/appointment_service_type.py
+-rw-r--r--   0        0        0     1044 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/appointment_status.py
+-rw-r--r--   0        0        0      149 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/appointment_type.py
+-rw-r--r--   0        0        0      957 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/area_info.py
+-rw-r--r--   0        0        0      510 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/attempt_status.py
+-rw-r--r--   0        0        0      649 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/auth_type.py
+-rw-r--r--   0        0        0      537 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/availability.py
+-rw-r--r--   0        0        0     1468 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/biomarker_result.py
+-rw-r--r--   0        0        0     1168 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/body_v_2_in_db.py
+-rw-r--r--   0        0        0      970 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_activity_response.py
+-rw-r--r--   0        0        0      950 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_body_response.py
+-rw-r--r--   0        0        0     3581 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_activity.py
+-rw-r--r--   0        0        0     1010 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_api_key.py
+-rw-r--r--   0        0        0     1815 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_appointment.py
+-rw-r--r--   0        0        0      934 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_appointment_cancellation_reason.py
+-rw-r--r--   0        0        0     1051 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_appointment_event.py
+-rw-r--r--   0        0        0     1193 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_at_home_phlebotomy_order.py
+-rw-r--r--   0        0        0     1030 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_at_home_phlebotomy_order_details.py
+-rw-r--r--   0        0        0     1634 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_blood_oxygen_timeseries.py
+-rw-r--r--   0        0        0     1632 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_blood_pressure_timeseries.py
+-rw-r--r--   0        0        0     1637 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_body.py
+-rw-r--r--   0        0        0     1631 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_body_fat_timeseries.py
+-rw-r--r--   0        0        0     1630 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_body_weight_timeseries.py
+-rw-r--r--   0        0        0     1859 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_caffeine_timeseries.py
+-rw-r--r--   0        0        0     1983 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_calories_active_timeseries.py
+-rw-r--r--   0        0        0     1722 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_calories_basal_timeseries.py
+-rw-r--r--   0        0        0     1623 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_cholesterol_timeseries.py
+-rw-r--r--   0        0        0     1071 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_diagnosis_information.py
+-rw-r--r--   0        0        0     1929 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_distance_timeseries.py
+-rw-r--r--   0        0        0     1540 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py
+-rw-r--r--   0        0        0     1707 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_floors_climbed_timeseries.py
+-rw-r--r--   0        0        0     1048 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_food.py
+-rw-r--r--   0        0        0     1619 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_glucose_timeseries.py
+-rw-r--r--   0        0        0     1236 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_heart_rate.py
+-rw-r--r--   0        0        0     1606 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_heart_rate_timeseries.py
+-rw-r--r--   0        0        0     1624 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_hrv_timeseries.py
+-rw-r--r--   0        0        0     1968 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_hypnogram_timeseries.py
+-rw-r--r--   0        0        0     1612 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_ige_timeseries.py
+-rw-r--r--   0        0        0     1612 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_igg_timeseries.py
+-rw-r--r--   0        0        0     1183 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_lab.py
+-rw-r--r--   0        0        0     1780 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_lab_test.py
+-rw-r--r--   0        0        0      945 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_loinc.py
+-rw-r--r--   0        0        0     1147 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_marker.py
+-rw-r--r--   0        0        0     1262 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_marker_complete.py
+-rw-r--r--   0        0        0     1003 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_meal_response.py
+-rw-r--r--   0        0        0     1861 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_mindfulness_minutes_timeseries.py
+-rw-r--r--   0        0        0     3286 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_order.py
+-rw-r--r--   0        0        0     1311 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_order_details.py
+-rw-r--r--   0        0        0      967 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_order_event.py
+-rw-r--r--   0        0        0     1060 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_patient_details_compatible.py
+-rw-r--r--   0        0        0     1239 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_payor_search_response.py
+-rw-r--r--   0        0        0      916 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_physician.py
+-rw-r--r--   0        0        0     1210 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_profile.py
+-rw-r--r--   0        0        0     1164 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_provider.py
+-rw-r--r--   0        0        0     1418 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_provider_detailed.py
+-rw-r--r--   0        0        0     1302 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_provider_with_status.py
+-rw-r--r--   0        0        0     6046 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_resource.py
+-rw-r--r--   0        0        0     1639 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_respiratory_rate_timeseries.py
+-rw-r--r--   0        0        0     1088 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_result.py
+-rw-r--r--   0        0        0     1862 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_shipment.py
+-rw-r--r--   0        0        0     4877 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_sleep.py
+-rw-r--r--   0        0        0     1497 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_sleep_stream.py
+-rw-r--r--   0        0        0     1898 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_source.py
+-rw-r--r--   0        0        0     1003 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_sport.py
+-rw-r--r--   0        0        0     1918 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_steps_timeseries.py
+-rw-r--r--   0        0        0     1447 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_stream.py
+-rw-r--r--   0        0        0     1573 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_stress_level_timeseries.py
+-rw-r--r--   0        0        0     1936 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_team.py
+-rw-r--r--   0        0        0      992 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_test_kit_order_details.py
+-rw-r--r--   0        0        0     1273 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_testkit_order.py
+-rw-r--r--   0        0        0     2926 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_user.py
+-rw-r--r--   0        0        0     1367 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_user_key.py
+-rw-r--r--   0        0        0     1844 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_vo_2_max_timeseries.py
+-rw-r--r--   0        0        0     1002 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_walk_in_order_details.py
+-rw-r--r--   0        0        0     1129 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_walk_in_test_order.py
+-rw-r--r--   0        0        0     1638 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_water_timeseries.py
+-rw-r--r--   0        0        0     4328 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_facing_workout.py
+-rw-r--r--   0        0        0      955 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_sleep_response.py
+-rw-r--r--   0        0        0      951 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_user_id_conflict.py
+-rw-r--r--   0        0        0      966 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/client_workout_response.py
+-rw-r--r--   0        0        0     1271 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/connected_source_client_facing.py
+-rw-r--r--   0        0        0     1184 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/connection_status.py
+-rw-r--r--   0        0        0      734 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/connection_status_state.py
+-rw-r--r--   0        0        0     1126 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/consent.py
+-rw-r--r--   0        0        0     1519 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/consent_type.py
+-rw-r--r--   0        0        0      930 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/day_slots.py
+-rw-r--r--   0        0        0     1240 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/delegated_flow_type.py
+-rw-r--r--   0        0        0      897 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/demo_connection_status.py
+-rw-r--r--   0        0        0      892 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/demo_providers.py
+-rw-r--r--   0        0        0     1053 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/device_v_2_in_db.py
+-rw-r--r--   0        0        0      153 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/email_providers.py
+-rw-r--r--   0        0        0      936 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/energy.py
+-rw-r--r--   0        0        0     1172 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/event_destination_preferences.py
+-rw-r--r--   0        0        0      762 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/event_destination_preferences_enabled_item.py
+-rw-r--r--   0        0        0      754 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/event_destination_preferences_preferred.py
+-rw-r--r--   0        0        0     1169 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/fallback_birth_date.py
+-rw-r--r--   0        0        0     1376 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/fallback_time_zone.py
+-rw-r--r--   0        0        0     1623 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/fats.py
+-rw-r--r--   0        0        0      762 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/gender.py
+-rw-r--r--   0        0        0     1110 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/get_markers_response.py
+-rw-r--r--   0        0        0     1048 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/get_orders_response.py
+-rw-r--r--   0        0        0     1087 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_blood_oxygen.py
+-rw-r--r--   0        0        0     1254 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_blood_oxygen_response.py
+-rw-r--r--   0        0        0     1095 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_blood_pressure.py
+-rw-r--r--   0        0        0     1262 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_blood_pressure_response.py
+-rw-r--r--   0        0        0     1071 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_body_fat.py
+-rw-r--r--   0        0        0     1238 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_body_fat_response.py
+-rw-r--r--   0        0        0     1083 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_body_weight.py
+-rw-r--r--   0        0        0     1250 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_body_weight_response.py
+-rw-r--r--   0        0        0     1074 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_caffeine.py
+-rw-r--r--   0        0        0     1241 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_caffeine_response.py
+-rw-r--r--   0        0        0     1099 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_calories_active.py
+-rw-r--r--   0        0        0     1266 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_calories_active_response.py
+-rw-r--r--   0        0        0     1095 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_calories_basal.py
+-rw-r--r--   0        0        0     1262 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_calories_basal_response.py
+-rw-r--r--   0        0        0     1086 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_cholesterol.py
+-rw-r--r--   0        0        0     1253 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_cholesterol_response.py
+-rw-r--r--   0        0        0     1074 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_distance.py
+-rw-r--r--   0        0        0     1241 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_distance_response.py
+-rw-r--r--   0        0        0     1139 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_electrocardiogram_voltage.py
+-rw-r--r--   0        0        0     1306 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_electrocardiogram_voltage_response.py
+-rw-r--r--   0        0        0     1095 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_floors_climbed.py
+-rw-r--r--   0        0        0     1262 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_floors_climbed_response.py
+-rw-r--r--   0        0        0     1070 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_glucose.py
+-rw-r--r--   0        0        0     1237 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_glucose_response.py
+-rw-r--r--   0        0        0     1079 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_heart_rate.py
+-rw-r--r--   0        0        0     1246 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_heart_rate_response.py
+-rw-r--r--   0        0        0     1054 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_hrv.py
+-rw-r--r--   0        0        0     1221 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_hrv_response.py
+-rw-r--r--   0        0        0     1078 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_hypnogram.py
+-rw-r--r--   0        0        0     1245 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_hypnogram_response.py
+-rw-r--r--   0        0        0     1054 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_ige.py
+-rw-r--r--   0        0        0     1221 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_ige_response.py
+-rw-r--r--   0        0        0     1054 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_igg.py
+-rw-r--r--   0        0        0     1221 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_igg_response.py
+-rw-r--r--   0        0        0     1115 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_mindfulness_minutes.py
+-rw-r--r--   0        0        0     1282 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_mindfulness_minutes_response.py
+-rw-r--r--   0        0        0     1103 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_respiratory_rate.py
+-rw-r--r--   0        0        0     1270 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_respiratory_rate_response.py
+-rw-r--r--   0        0        0     1062 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_steps.py
+-rw-r--r--   0        0        0     1229 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_steps_response.py
+-rw-r--r--   0        0        0     1087 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_stress_level.py
+-rw-r--r--   0        0        0     1254 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_stress_level_response.py
+-rw-r--r--   0        0        0     1068 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_vo_2_max.py
+-rw-r--r--   0        0        0     1235 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_vo_2_max_response.py
+-rw-r--r--   0        0        0     1062 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_water.py
+-rw-r--r--   0        0        0     1229 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/grouped_water_response.py
+-rw-r--r--   0        0        0     3022 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/health_insurance_create_request.py
+-rw-r--r--   0        0        0      811 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/health_insurance_create_request_back_image.py
+-rw-r--r--   0        0        0      816 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/health_insurance_create_request_front_image.py
+-rw-r--r--   0        0        0      876 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/health_insurance_create_request_patient_signature_image.py
+-rw-r--r--   0        0        0      732 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/historical_pull_status.py
+-rw-r--r--   0        0        0      966 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/http_validation_error.py
+-rw-r--r--   0        0        0      864 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/jpeg.py
+-rw-r--r--   0        0        0     1289 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/lab_results_metadata.py
+-rw-r--r--   0        0        0     1034 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/lab_results_raw.py
+-rw-r--r--   0        0        0      223 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/lab_results_raw_results.py
+-rw-r--r--   0        0        0      827 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/lab_test_collection_method.py
+-rw-r--r--   0        0        0      898 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/lab_test_sample_type.py
+-rw-r--r--   0        0        0      729 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/lab_test_status.py
+-rw-r--r--   0        0        0      949 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/last_attempt.py
+-rw-r--r--   0        0        0      936 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/libre_config.py
+-rw-r--r--   0        0        0      960 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/link_token_exchange_response.py
+-rw-r--r--   0        0        0      879 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/lng_lat.py
+-rw-r--r--   0        0        0     1553 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/macros.py
+-rw-r--r--   0        0        0     1792 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/manual_providers.py
+-rw-r--r--   0        0        0      501 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/marker_type.py
+-rw-r--r--   0        0        0     1444 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/meal_in_db_base_client_facing_source.py
+-rw-r--r--   0        0        0     1233 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/metrics_result.py
+-rw-r--r--   0        0        0     1272 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/micros.py
+-rw-r--r--   0        0        0     2126 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/o_auth_providers.py
+-rw-r--r--   0        0        0     9798 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/order_status.py
+-rw-r--r--   0        0        0     1265 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/order_top_level_status.py
+-rw-r--r--   0        0        0     1001 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/paginated_users_response.py
+-rw-r--r--   0        0        0     1971 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/password_providers.py
+-rw-r--r--   0        0        0     1063 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/patient_address_compatible.py
+-rw-r--r--   0        0        0     1000 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/patient_details.py
+-rw-r--r--   0        0        0     1004 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/person_details.py
+-rw-r--r--   0        0        0      993 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/phlebotomy_area_info.py
+-rw-r--r--   0        0        0     1065 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/phlebotomy_provider_info.py
+-rw-r--r--   0        0        0     1281 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/physician_create_request.py
+-rw-r--r--   0        0        0     1008 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/physician_create_request_base.py
+-rw-r--r--   0        0        0      806 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/physician_create_request_signature_image.py
+-rw-r--r--   0        0        0      863 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/png.py
+-rw-r--r--   0        0        0      973 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/post_order_response.py
+-rw-r--r--   0        0        0     1113 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/profile_in_db.py
+-rw-r--r--   0        0        0     1306 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/provider_link_response.py
+-rw-r--r--   0        0        0      750 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/provider_link_response_state.py
+-rw-r--r--   0        0        0      978 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/provider_mfa_request.py
+-rw-r--r--   0        0        0      476 2024-05-16 09:05:08.727565 vital-2.1.9/src/vital/types/provider_mfa_request_method.py
+-rw-r--r--   0        0        0     5340 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/providers.py
+-rw-r--r--   0        0        0      943 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/raw_activity.py
+-rw-r--r--   0        0        0      923 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/raw_body.py
+-rw-r--r--   0        0        0      935 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/raw_devices.py
+-rw-r--r--   0        0        0      917 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/raw_profile.py
+-rw-r--r--   0        0        0      928 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/raw_sleep.py
+-rw-r--r--   0        0        0      939 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/raw_workout.py
+-rw-r--r--   0        0        0     1360 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/region.py
+-rw-r--r--   0        0        0     1055 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/resource_availability.py
+-rw-r--r--   0        0        0      761 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/responsible_relationship.py
+-rw-r--r--   0        0        0      662 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/result_type.py
+-rw-r--r--   0        0        0     1000 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/scope_requirements_grants.py
+-rw-r--r--   0        0        0      925 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/scope_requirements_str.py
+-rw-r--r--   0        0        0     1020 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/shipping_address.py
+-rw-r--r--   0        0        0     1146 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/single_historical_pull_statistics.py
+-rw-r--r--   0        0        0     1125 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/single_provider_historical_pull_response.py
+-rw-r--r--   0        0        0     1081 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/single_resource_statistics.py
+-rw-r--r--   0        0        0     1052 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/single_user_historical_pull_response.py
+-rw-r--r--   0        0        0     1026 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/single_user_resource_response.py
+-rw-r--r--   0        0        0     1152 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/sleep_v_2_in_db.py
+-rw-r--r--   0        0        0     1246 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/source.py
+-rw-r--r--   0        0        0     1209 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/source_auth_type.py
+-rw-r--r--   0        0        0     1123 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/source_link.py
+-rw-r--r--   0        0        0      892 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/source_type.py
+-rw-r--r--   0        0        0     1303 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/team_config.py
+-rw-r--r--   0        0        0     1147 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/time_slot.py
+-rw-r--r--   0        0        0      903 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/timeseries_metric_point.py
+-rw-r--r--   0        0        0     4865 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/timeseries_resource.py
+-rw-r--r--   0        0        0     1138 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/us_address.py
+-rw-r--r--   0        0        0     1040 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/user_historical_pulls_response.py
+-rw-r--r--   0        0        0     1305 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/user_refresh_error_response.py
+-rw-r--r--   0        0        0     1357 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/user_refresh_success_response.py
+-rw-r--r--   0        0        0     1015 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/user_resources_response.py
+-rw-r--r--   0        0        0      906 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/user_sign_in_token_response.py
+-rw-r--r--   0        0        0      952 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/user_success_response.py
+-rw-r--r--   0        0        0      992 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      904 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/vital_token_created_response.py
+-rw-r--r--   0        0        0     1217 2024-05-16 09:05:08.731565 vital-2.1.9/src/vital/types/workout_v_2_in_db.py
+-rw-r--r--   0        0        0     3831 1970-01-01 00:00:00.000000 vital-2.1.9/PKG-INFO
```

### Comparing `vital-2.1.8/README.md` & `vital-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/__init__.py` & `vital-2.1.9/src/vital/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/client.py` & `vital-2.1.9/src/vital/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/core/__init__.py` & `vital-2.1.9/src/vital/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/core/client_wrapper.py` & `vital-2.1.9/src/vital/core/client_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "vital",
-            "X-Fern-SDK-Version": "2.1.8",
+            "X-Fern-SDK-Version": "2.1.9",
         }
         headers["x-vital-api-key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `vital-2.1.8/src/vital/core/datetime_utils.py` & `vital-2.1.9/src/vital/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/core/jsonable_encoder.py` & `vital-2.1.9/src/vital/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/__init__.py` & `vital-2.1.9/src/vital/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/activity/client.py` & `vital-2.1.9/src/vital/resources/activity/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/body/client.py` & `vital-2.1.9/src/vital/resources/body/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/devices/client.py` & `vital-2.1.9/src/vital/resources/devices/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/insurance/client.py` & `vital-2.1.9/src/vital/resources/insurance/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/introspect/client.py` & `vital-2.1.9/src/vital/resources/introspect/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/lab_tests/client.py` & `vital-2.1.9/src/vital/resources/lab_tests/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/link/client.py` & `vital-2.1.9/src/vital/resources/link/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/meal/client.py` & `vital-2.1.9/src/vital/resources/meal/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/profile/client.py` & `vital-2.1.9/src/vital/resources/profile/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/providers/client.py` & `vital-2.1.9/src/vital/resources/providers/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/sleep/client.py` & `vital-2.1.9/src/vital/resources/sleep/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/team/client.py` & `vital-2.1.9/src/vital/resources/team/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/testkit/client.py` & `vital-2.1.9/src/vital/resources/testkit/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/user/client.py` & `vital-2.1.9/src/vital/resources/user/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                                                             Fallback time zone of the user, in the form of a valid IANA tzdatabase identifier (e.g., `Europe/London` or `America/Los_Angeles`).
                                                             Used when pulling data from sources that are completely time zone agnostic (e.g., all time is relative to UTC clock, without any time zone attributions on data points).
 
             - fallback_birth_date: typing.Optional[str]. Fallback date of birth of the user, in YYYY-mm-dd format. Used for calculating max heartrate for providers that don not provide users' age.
 
             - ingestion_start: typing.Optional[str]. Starting bound for user data ingestion. Data older than this date will not be ingested.
 
-            - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data newer than this date will not be ingested and the connection deregistered.
+            - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data from this date or later will not be ingested and the connection will be deregistered.
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.user.create(
@@ -298,15 +298,15 @@
                                                             Fallback time zone of the user, in the form of a valid IANA tzdatabase identifier (e.g., `Europe/London` or `America/Los_Angeles`).
                                                             Used when pulling data from sources that are completely time zone agnostic (e.g., all time is relative to UTC clock, without any time zone attributions on data points).
 
             - fallback_birth_date: typing.Optional[str]. Fallback date of birth of the user, in YYYY-mm-dd format. Used for calculating max heartrate for providers that don not provide users' age.
 
             - ingestion_start: typing.Optional[str]. Starting bound for user data ingestion. Data older than this date will not be ingested.
 
-            - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data newer than this date will not be ingested and the connection deregistered.
+            - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data from this date or later will not be ingested and the connection will be deregistered.
         ---
         from vital.client import Vital
 
         client = Vital(
             api_key="YOUR_API_KEY",
         )
         client.user.patch(
@@ -534,15 +534,15 @@
                                                             Fallback time zone of the user, in the form of a valid IANA tzdatabase identifier (e.g., `Europe/London` or `America/Los_Angeles`).
                                                             Used when pulling data from sources that are completely time zone agnostic (e.g., all time is relative to UTC clock, without any time zone attributions on data points).
 
             - fallback_birth_date: typing.Optional[str]. Fallback date of birth of the user, in YYYY-mm-dd format. Used for calculating max heartrate for providers that don not provide users' age.
 
             - ingestion_start: typing.Optional[str]. Starting bound for user data ingestion. Data older than this date will not be ingested.
 
-            - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data newer than this date will not be ingested and the connection deregistered.
+            - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data from this date or later will not be ingested and the connection will be deregistered.
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.user.create(
@@ -746,15 +746,15 @@
                                                             Fallback time zone of the user, in the form of a valid IANA tzdatabase identifier (e.g., `Europe/London` or `America/Los_Angeles`).
                                                             Used when pulling data from sources that are completely time zone agnostic (e.g., all time is relative to UTC clock, without any time zone attributions on data points).
 
             - fallback_birth_date: typing.Optional[str]. Fallback date of birth of the user, in YYYY-mm-dd format. Used for calculating max heartrate for providers that don not provide users' age.
 
             - ingestion_start: typing.Optional[str]. Starting bound for user data ingestion. Data older than this date will not be ingested.
 
-            - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data newer than this date will not be ingested and the connection deregistered.
+            - ingestion_end: typing.Optional[str]. Ending bound for user data ingestion. Data from this date or later will not be ingested and the connection will be deregistered.
         ---
         from vital.client import AsyncVital
 
         client = AsyncVital(
             api_key="YOUR_API_KEY",
         )
         await client.user.patch(
```

### Comparing `vital-2.1.8/src/vital/resources/vitals/client.py` & `vital-2.1.9/src/vital/resources/vitals/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/resources/workouts/client.py` & `vital-2.1.9/src/vital/resources/workouts/client.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/__init__.py` & `vital-2.1.9/src/vital/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/activity_v_2_in_db.py` & `vital-2.1.9/src/vital/types/activity_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/address.py` & `vital-2.1.9/src/vital/types/address.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/appointment_availability_slots.py` & `vital-2.1.9/src/vital/types/appointment_availability_slots.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/appointment_event_status.py` & `vital-2.1.9/src/vital/types/appointment_event_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/appointment_provider.py` & `vital-2.1.9/src/vital/types/appointment_provider.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/appointment_service_type.py` & `vital-2.1.9/src/vital/types/appointment_service_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/appointment_status.py` & `vital-2.1.9/src/vital/types/appointment_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/area_info.py` & `vital-2.1.9/src/vital/types/area_info.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/auth_type.py` & `vital-2.1.9/src/vital/types/auth_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/availability.py` & `vital-2.1.9/src/vital/types/availability.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/biomarker_result.py` & `vital-2.1.9/src/vital/types/biomarker_result.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/body_v_2_in_db.py` & `vital-2.1.9/src/vital/types/body_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_activity_response.py` & `vital-2.1.9/src/vital/types/client_activity_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_body_response.py` & `vital-2.1.9/src/vital/types/client_body_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_activity.py` & `vital-2.1.9/src/vital/types/client_facing_activity.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_api_key.py` & `vital-2.1.9/src/vital/types/client_facing_api_key.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_appointment.py` & `vital-2.1.9/src/vital/types/client_facing_appointment.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_appointment_cancellation_reason.py` & `vital-2.1.9/src/vital/types/client_facing_appointment_cancellation_reason.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_appointment_event.py` & `vital-2.1.9/src/vital/types/client_facing_appointment_event.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_at_home_phlebotomy_order.py` & `vital-2.1.9/src/vital/types/client_facing_at_home_phlebotomy_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_at_home_phlebotomy_order_details.py` & `vital-2.1.9/src/vital/types/client_facing_at_home_phlebotomy_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_blood_oxygen_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_blood_oxygen_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_blood_pressure_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_blood_pressure_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_body.py` & `vital-2.1.9/src/vital/types/client_facing_body.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_body_fat_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_body_fat_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_body_weight_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_body_weight_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_caffeine_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_caffeine_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_calories_active_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_calories_active_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_calories_basal_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_calories_basal_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_cholesterol_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_cholesterol_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_diagnosis_information.py` & `vital-2.1.9/src/vital/types/client_facing_diagnosis_information.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_distance_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_distance_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_electrocardiogram_voltage_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_floors_climbed_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_floors_climbed_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_food.py` & `vital-2.1.9/src/vital/types/client_facing_food.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_glucose_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_glucose_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_heart_rate.py` & `vital-2.1.9/src/vital/types/client_facing_heart_rate.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_heart_rate_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_heart_rate_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_hrv_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_hrv_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_hypnogram_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_hypnogram_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_ige_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_ige_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_igg_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_igg_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_lab.py` & `vital-2.1.9/src/vital/types/client_facing_lab.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_lab_test.py` & `vital-2.1.9/src/vital/types/client_facing_lab_test.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_loinc.py` & `vital-2.1.9/src/vital/types/client_facing_loinc.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_marker.py` & `vital-2.1.9/src/vital/types/client_facing_marker.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_marker_complete.py` & `vital-2.1.9/src/vital/types/client_facing_marker_complete.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_meal_response.py` & `vital-2.1.9/src/vital/types/client_facing_meal_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_mindfulness_minutes_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_mindfulness_minutes_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_order.py` & `vital-2.1.9/src/vital/types/client_facing_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_order_details.py` & `vital-2.1.9/src/vital/types/client_facing_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_order_event.py` & `vital-2.1.9/src/vital/types/client_facing_order_event.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_patient_details_compatible.py` & `vital-2.1.9/src/vital/types/client_facing_patient_details_compatible.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_payor_search_response.py` & `vital-2.1.9/src/vital/types/client_facing_payor_search_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_physician.py` & `vital-2.1.9/src/vital/types/client_facing_physician.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_profile.py` & `vital-2.1.9/src/vital/types/client_facing_profile.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_provider.py` & `vital-2.1.9/src/vital/types/client_facing_provider.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_provider_detailed.py` & `vital-2.1.9/src/vital/types/client_facing_provider_detailed.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_provider_with_status.py` & `vital-2.1.9/src/vital/types/client_facing_provider_with_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_resource.py` & `vital-2.1.9/src/vital/types/client_facing_resource.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_respiratory_rate_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_respiratory_rate_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_result.py` & `vital-2.1.9/src/vital/types/client_facing_result.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_shipment.py` & `vital-2.1.9/src/vital/types/client_facing_shipment.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_sleep.py` & `vital-2.1.9/src/vital/types/client_facing_sleep.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_sleep_stream.py` & `vital-2.1.9/src/vital/types/client_facing_sleep_stream.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_source.py` & `vital-2.1.9/src/vital/types/client_facing_source.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_sport.py` & `vital-2.1.9/src/vital/types/client_facing_sport.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_steps_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_steps_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_stream.py` & `vital-2.1.9/src/vital/types/client_facing_stream.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_stress_level_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_stress_level_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_team.py` & `vital-2.1.9/src/vital/types/client_facing_team.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_test_kit_order_details.py` & `vital-2.1.9/src/vital/types/client_facing_test_kit_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_testkit_order.py` & `vital-2.1.9/src/vital/types/client_facing_testkit_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_user.py` & `vital-2.1.9/src/vital/types/client_facing_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     fallback_birth_date: typing.Optional[FallbackBirthDate] = pydantic.Field(
         description="Fallback date of birth of the user, in YYYY-mm-dd format. Used for calculating max heartrate for providers that don not provide users' age."
     )
     ingestion_start: typing.Optional[str] = pydantic.Field(
         description="Starting bound for user data ingestion. Data older than this date will not be ingested."
     )
     ingestion_end: typing.Optional[str] = pydantic.Field(
-        description="Ending bound for user data ingestion. Data newer than this date will not be ingested and the connection deregistered."
+        description="Ending bound for user data ingestion. Data from this date or later will not be ingested and the connection will be deregistered."
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vital-2.1.8/src/vital/types/client_facing_user_key.py` & `vital-2.1.9/src/vital/types/client_facing_user_key.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_vo_2_max_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_vo_2_max_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_walk_in_order_details.py` & `vital-2.1.9/src/vital/types/client_facing_walk_in_order_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_walk_in_test_order.py` & `vital-2.1.9/src/vital/types/client_facing_walk_in_test_order.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_water_timeseries.py` & `vital-2.1.9/src/vital/types/client_facing_water_timeseries.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_facing_workout.py` & `vital-2.1.9/src/vital/types/client_facing_workout.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_sleep_response.py` & `vital-2.1.9/src/vital/types/client_sleep_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_user_id_conflict.py` & `vital-2.1.9/src/vital/types/client_user_id_conflict.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/client_workout_response.py` & `vital-2.1.9/src/vital/types/client_workout_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/connected_source_client_facing.py` & `vital-2.1.9/src/vital/types/connected_source_client_facing.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/connection_status.py` & `vital-2.1.9/src/vital/types/connection_status.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class ConnectionStatus(pydantic.BaseModel):
     state: ConnectionStatusState
+    redirect_url: typing.Optional[str]
     error_type: typing.Optional[str]
     error: typing.Optional[str]
     provider_mfa: typing.Optional[ProviderMfaRequest]
     success: bool
-    redirect_url: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.8/src/vital/types/connection_status_state.py` & `vital-2.1.9/src/vital/types/connection_status_state.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/consent.py` & `vital-2.1.9/src/vital/types/consent.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/consent_type.py` & `vital-2.1.9/src/vital/types/consent_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/day_slots.py` & `vital-2.1.9/src/vital/types/day_slots.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/delegated_flow_type.py` & `vital-2.1.9/src/vital/types/delegated_flow_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/demo_connection_status.py` & `vital-2.1.9/src/vital/types/demo_connection_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/demo_providers.py` & `vital-2.1.9/src/vital/types/demo_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/device_v_2_in_db.py` & `vital-2.1.9/src/vital/types/device_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/energy.py` & `vital-2.1.9/src/vital/types/energy.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/event_destination_preferences.py` & `vital-2.1.9/src/vital/types/event_destination_preferences.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/event_destination_preferences_enabled_item.py` & `vital-2.1.9/src/vital/types/event_destination_preferences_enabled_item.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/event_destination_preferences_preferred.py` & `vital-2.1.9/src/vital/types/event_destination_preferences_preferred.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/fallback_birth_date.py` & `vital-2.1.9/src/vital/types/fallback_birth_date.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/fallback_time_zone.py` & `vital-2.1.9/src/vital/types/fallback_time_zone.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/fats.py` & `vital-2.1.9/src/vital/types/fats.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/gender.py` & `vital-2.1.9/src/vital/types/gender.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/get_markers_response.py` & `vital-2.1.9/src/vital/types/get_markers_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/get_orders_response.py` & `vital-2.1.9/src/vital/types/get_orders_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_blood_oxygen.py` & `vital-2.1.9/src/vital/types/grouped_blood_oxygen.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_blood_oxygen_response.py` & `vital-2.1.9/src/vital/types/grouped_blood_oxygen_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_blood_pressure.py` & `vital-2.1.9/src/vital/types/grouped_blood_pressure.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_blood_pressure_response.py` & `vital-2.1.9/src/vital/types/grouped_blood_pressure_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_body_fat.py` & `vital-2.1.9/src/vital/types/grouped_body_fat.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_body_fat_response.py` & `vital-2.1.9/src/vital/types/grouped_body_fat_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_body_weight.py` & `vital-2.1.9/src/vital/types/grouped_body_weight.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_body_weight_response.py` & `vital-2.1.9/src/vital/types/grouped_body_weight_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_caffeine.py` & `vital-2.1.9/src/vital/types/grouped_caffeine.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_caffeine_response.py` & `vital-2.1.9/src/vital/types/grouped_caffeine_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_calories_active.py` & `vital-2.1.9/src/vital/types/grouped_calories_active.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_calories_active_response.py` & `vital-2.1.9/src/vital/types/grouped_calories_active_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_calories_basal.py` & `vital-2.1.9/src/vital/types/grouped_calories_basal.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_calories_basal_response.py` & `vital-2.1.9/src/vital/types/grouped_calories_basal_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_cholesterol.py` & `vital-2.1.9/src/vital/types/grouped_cholesterol.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_cholesterol_response.py` & `vital-2.1.9/src/vital/types/grouped_cholesterol_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_distance.py` & `vital-2.1.9/src/vital/types/grouped_distance.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_distance_response.py` & `vital-2.1.9/src/vital/types/grouped_distance_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_electrocardiogram_voltage.py` & `vital-2.1.9/src/vital/types/grouped_electrocardiogram_voltage.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_electrocardiogram_voltage_response.py` & `vital-2.1.9/src/vital/types/grouped_electrocardiogram_voltage_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_floors_climbed.py` & `vital-2.1.9/src/vital/types/grouped_floors_climbed.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_floors_climbed_response.py` & `vital-2.1.9/src/vital/types/grouped_floors_climbed_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_glucose.py` & `vital-2.1.9/src/vital/types/grouped_glucose.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_glucose_response.py` & `vital-2.1.9/src/vital/types/grouped_glucose_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_heart_rate.py` & `vital-2.1.9/src/vital/types/grouped_heart_rate.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_heart_rate_response.py` & `vital-2.1.9/src/vital/types/grouped_heart_rate_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_hrv.py` & `vital-2.1.9/src/vital/types/grouped_hrv.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_hrv_response.py` & `vital-2.1.9/src/vital/types/grouped_hrv_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_hypnogram.py` & `vital-2.1.9/src/vital/types/grouped_hypnogram.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_hypnogram_response.py` & `vital-2.1.9/src/vital/types/grouped_hypnogram_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_ige.py` & `vital-2.1.9/src/vital/types/grouped_ige.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_ige_response.py` & `vital-2.1.9/src/vital/types/grouped_ige_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_igg.py` & `vital-2.1.9/src/vital/types/grouped_igg.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_igg_response.py` & `vital-2.1.9/src/vital/types/grouped_igg_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_mindfulness_minutes.py` & `vital-2.1.9/src/vital/types/grouped_mindfulness_minutes.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_mindfulness_minutes_response.py` & `vital-2.1.9/src/vital/types/grouped_mindfulness_minutes_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_respiratory_rate.py` & `vital-2.1.9/src/vital/types/grouped_respiratory_rate.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_respiratory_rate_response.py` & `vital-2.1.9/src/vital/types/grouped_respiratory_rate_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_steps.py` & `vital-2.1.9/src/vital/types/grouped_steps.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_steps_response.py` & `vital-2.1.9/src/vital/types/grouped_steps_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_stress_level.py` & `vital-2.1.9/src/vital/types/grouped_stress_level.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_stress_level_response.py` & `vital-2.1.9/src/vital/types/grouped_stress_level_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_vo_2_max.py` & `vital-2.1.9/src/vital/types/grouped_vo_2_max.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_vo_2_max_response.py` & `vital-2.1.9/src/vital/types/grouped_vo_2_max_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_water.py` & `vital-2.1.9/src/vital/types/grouped_water.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/grouped_water_response.py` & `vital-2.1.9/src/vital/types/grouped_water_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/health_insurance_create_request.py` & `vital-2.1.9/src/vital/types/health_insurance_create_request.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/health_insurance_create_request_back_image.py` & `vital-2.1.9/src/vital/types/health_insurance_create_request_back_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/health_insurance_create_request_front_image.py` & `vital-2.1.9/src/vital/types/health_insurance_create_request_front_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/health_insurance_create_request_patient_signature_image.py` & `vital-2.1.9/src/vital/types/health_insurance_create_request_patient_signature_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/historical_pull_status.py` & `vital-2.1.9/src/vital/types/historical_pull_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/http_validation_error.py` & `vital-2.1.9/src/vital/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/jpeg.py` & `vital-2.1.9/src/vital/types/jpeg.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/lab_results_metadata.py` & `vital-2.1.9/src/vital/types/lab_results_metadata.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/lab_results_raw.py` & `vital-2.1.9/src/vital/types/lab_results_raw.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/lab_test_collection_method.py` & `vital-2.1.9/src/vital/types/lab_test_collection_method.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/lab_test_sample_type.py` & `vital-2.1.9/src/vital/types/lab_test_sample_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/lab_test_status.py` & `vital-2.1.9/src/vital/types/lab_test_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/last_attempt.py` & `vital-2.1.9/src/vital/types/last_attempt.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/libre_config.py` & `vital-2.1.9/src/vital/types/libre_config.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/link_token_exchange_response.py` & `vital-2.1.9/src/vital/types/link_token_exchange_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/lng_lat.py` & `vital-2.1.9/src/vital/types/lng_lat.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/macros.py` & `vital-2.1.9/src/vital/types/macros.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/manual_providers.py` & `vital-2.1.9/src/vital/types/manual_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/meal_in_db_base_client_facing_source.py` & `vital-2.1.9/src/vital/types/meal_in_db_base_client_facing_source.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/metrics_result.py` & `vital-2.1.9/src/vital/types/metrics_result.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/micros.py` & `vital-2.1.9/src/vital/types/micros.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/o_auth_providers.py` & `vital-2.1.9/src/vital/types/o_auth_providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/order_status.py` & `vital-2.1.9/src/vital/types/order_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/order_top_level_status.py` & `vital-2.1.9/src/vital/types/order_top_level_status.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/paginated_users_response.py` & `vital-2.1.9/src/vital/types/paginated_users_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/password_providers.py` & `vital-2.1.9/src/vital/types/password_providers.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,27 +17,29 @@
     ZWIFT = "zwift"
     EIGHT_SLEEP = "eight_sleep"
     BEURER_API = "beurer_api"
     DEXCOM = "dexcom"
     HAMMERHEAD = "hammerhead"
     MY_FITNESS_PAL = "my_fitness_pal"
     KARDIA = "kardia"
+    ABBOTT_LIBREVIEW = "abbott_libreview"
 
     def visit(
         self,
         whoop: typing.Callable[[], T_Result],
         renpho: typing.Callable[[], T_Result],
         peloton: typing.Callable[[], T_Result],
         zwift: typing.Callable[[], T_Result],
         eight_sleep: typing.Callable[[], T_Result],
         beurer_api: typing.Callable[[], T_Result],
         dexcom: typing.Callable[[], T_Result],
         hammerhead: typing.Callable[[], T_Result],
         my_fitness_pal: typing.Callable[[], T_Result],
         kardia: typing.Callable[[], T_Result],
+        abbott_libreview: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is PasswordProviders.WHOOP:
             return whoop()
         if self is PasswordProviders.RENPHO:
             return renpho()
         if self is PasswordProviders.PELOTON:
             return peloton()
@@ -51,7 +53,9 @@
             return dexcom()
         if self is PasswordProviders.HAMMERHEAD:
             return hammerhead()
         if self is PasswordProviders.MY_FITNESS_PAL:
             return my_fitness_pal()
         if self is PasswordProviders.KARDIA:
             return kardia()
+        if self is PasswordProviders.ABBOTT_LIBREVIEW:
+            return abbott_libreview()
```

### Comparing `vital-2.1.8/src/vital/types/patient_address_compatible.py` & `vital-2.1.9/src/vital/types/patient_address_compatible.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/patient_details.py` & `vital-2.1.9/src/vital/types/patient_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/person_details.py` & `vital-2.1.9/src/vital/types/person_details.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/phlebotomy_area_info.py` & `vital-2.1.9/src/vital/types/phlebotomy_area_info.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/phlebotomy_provider_info.py` & `vital-2.1.9/src/vital/types/phlebotomy_provider_info.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/physician_create_request.py` & `vital-2.1.9/src/vital/types/physician_create_request.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/physician_create_request_base.py` & `vital-2.1.9/src/vital/types/physician_create_request_base.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/physician_create_request_signature_image.py` & `vital-2.1.9/src/vital/types/physician_create_request_signature_image.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/png.py` & `vital-2.1.9/src/vital/types/png.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/post_order_response.py` & `vital-2.1.9/src/vital/types/post_order_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/profile_in_db.py` & `vital-2.1.9/src/vital/types/profile_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/provider_link_response.py` & `vital-2.1.9/src/vital/types/provider_link_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,20 +12,21 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class ProviderLinkResponse(pydantic.BaseModel):
     state: ProviderLinkResponseState
+    redirect_url: typing.Optional[str]
     error_type: typing.Optional[str]
     error: typing.Optional[str]
     provider_mfa: typing.Optional[ProviderMfaRequest]
     provider: PasswordProviders
     connected: bool
-    provider_id: typing.Optional[str]
+    provider_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vital-2.1.8/src/vital/types/provider_link_response_state.py` & `vital-2.1.9/src/vital/types/provider_link_response_state.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/provider_mfa_request.py` & `vital-2.1.9/src/vital/types/provider_mfa_request.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/providers.py` & `vital-2.1.9/src/vital/types/providers.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/raw_activity.py` & `vital-2.1.9/src/vital/types/raw_activity.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/raw_body.py` & `vital-2.1.9/src/vital/types/raw_body.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/raw_devices.py` & `vital-2.1.9/src/vital/types/raw_devices.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/raw_profile.py` & `vital-2.1.9/src/vital/types/raw_profile.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/raw_sleep.py` & `vital-2.1.9/src/vital/types/raw_sleep.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/raw_workout.py` & `vital-2.1.9/src/vital/types/raw_workout.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/region.py` & `vital-2.1.9/src/vital/types/region.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/resource_availability.py` & `vital-2.1.9/src/vital/types/resource_availability.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/responsible_relationship.py` & `vital-2.1.9/src/vital/types/responsible_relationship.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/result_type.py` & `vital-2.1.9/src/vital/types/result_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/scope_requirements_grants.py` & `vital-2.1.9/src/vital/types/scope_requirements_grants.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/scope_requirements_str.py` & `vital-2.1.9/src/vital/types/scope_requirements_str.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/shipping_address.py` & `vital-2.1.9/src/vital/types/shipping_address.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/single_historical_pull_statistics.py` & `vital-2.1.9/src/vital/types/single_historical_pull_statistics.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/single_provider_historical_pull_response.py` & `vital-2.1.9/src/vital/types/single_provider_historical_pull_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/single_resource_statistics.py` & `vital-2.1.9/src/vital/types/single_resource_statistics.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/single_user_historical_pull_response.py` & `vital-2.1.9/src/vital/types/single_user_historical_pull_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/single_user_resource_response.py` & `vital-2.1.9/src/vital/types/single_user_resource_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/sleep_v_2_in_db.py` & `vital-2.1.9/src/vital/types/sleep_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/source.py` & `vital-2.1.9/src/vital/types/source.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/source_auth_type.py` & `vital-2.1.9/src/vital/types/source_auth_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/source_link.py` & `vital-2.1.9/src/vital/types/source_link.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/source_type.py` & `vital-2.1.9/src/vital/types/source_type.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/team_config.py` & `vital-2.1.9/src/vital/types/team_config.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/time_slot.py` & `vital-2.1.9/src/vital/types/time_slot.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/timeseries_metric_point.py` & `vital-2.1.9/src/vital/types/timeseries_metric_point.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/timeseries_resource.py` & `vital-2.1.9/src/vital/types/timeseries_resource.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/us_address.py` & `vital-2.1.9/src/vital/types/us_address.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/user_historical_pulls_response.py` & `vital-2.1.9/src/vital/types/user_historical_pulls_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/user_refresh_error_response.py` & `vital-2.1.9/src/vital/types/user_refresh_error_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/user_refresh_success_response.py` & `vital-2.1.9/src/vital/types/user_refresh_success_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/user_resources_response.py` & `vital-2.1.9/src/vital/types/user_resources_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/user_sign_in_token_response.py` & `vital-2.1.9/src/vital/types/user_sign_in_token_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/user_success_response.py` & `vital-2.1.9/src/vital/types/user_success_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/validation_error.py` & `vital-2.1.9/src/vital/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/vital_token_created_response.py` & `vital-2.1.9/src/vital/types/vital_token_created_response.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/src/vital/types/workout_v_2_in_db.py` & `vital-2.1.9/src/vital/types/workout_v_2_in_db.py`

 * *Files identical despite different names*

### Comparing `vital-2.1.8/PKG-INFO` & `vital-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital
-Version: 2.1.8
+Version: 2.1.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

