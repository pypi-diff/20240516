# Comparing `tmp/psa_car_controller-3.5.0.tar.gz` & `tmp/psa_car_controller-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psa_car_controller-3.5.0.tar", max compression
+gzip compressed data, was "psa_car_controller-3.5.1.tar", max compression
```

## Comparing `psa_car_controller-3.5.0.tar` & `psa_car_controller-3.5.1.tar`

### file list

```diff
@@ -1,216 +1,216 @@
--rw-r--r--   0        0        0    35149 2024-03-23 16:52:00.978045 psa_car_controller-3.5.0/LICENSE
--rw-r--r--   0        0        0      264 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/__init__.py
--rwxr-xr-x   0        0        0      753 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/__main__.py
--rw-r--r--   0        0        0        0 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/common/__init__.py
--rw-r--r--   0        0        0     1802 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/common/mylogger.py
--rw-r--r--   0        0        0     1612 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/common/utils.py
--rw-r--r--   0        0        0      458 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/AccountInformation.py
--rw-r--r--   0        0        0    12141 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/RemoteClient.py
--rw-r--r--   0        0        0      678 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/RemoteCredentials.py
--rw-r--r--   0        0        0        0 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/__init__.py
--rw-r--r--   0        0        0    13601 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/__init__.py
--rw-r--r--   0        0        0      319 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/api/__init__.py
--rw-r--r--   0        0        0   102100 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/api/trips_api.py
--rw-r--r--   0        0        0     4895 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/api/user_api.py
--rw-r--r--   0        0        0    81355 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/api/vehicles_api.py
--rw-r--r--   0        0        0    26152 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/api_client.py
--rw-r--r--   0        0        0     9746 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/configuration.py
--rw-r--r--   0        0        0    13204 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/__init__.py
--rw-r--r--   0        0        0    14820 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/adas.py
--rw-r--r--   0        0        0     5627 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/adas_park_assist.py
--rw-r--r--   0        0        0     9420 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alert.py
--rw-r--r--   0        0        0     3512 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alert_end_position.py
--rw-r--r--   0        0        0     5935 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alert_links.py
--rw-r--r--   0        0        0     7817 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alert_msg_enum.py
--rw-r--r--   0        0        0     4139 2024-03-23 16:52:00.986045 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alerts.py
--rw-r--r--   0        0        0     4153 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alerts_embedded.py
--rw-r--r--   0        0        0     4722 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/battery.py
--rw-r--r--   0        0        0     4546 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/bounded_program.py
--rw-r--r--   0        0        0     3699 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/charging_status_enum.py
--rw-r--r--   0        0        0     5092 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/circle_zone.py
--rw-r--r--   0        0        0     5020 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/circle_zone_coordinates.py
--rw-r--r--   0        0        0     7252 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collection_result.py
--rw-r--r--   0        0        0     9937 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collision.py
--rw-r--r--   0        0        0     5347 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collision_links.py
--rw-r--r--   0        0        0     8727 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collision_obj.py
--rw-r--r--   0        0        0     4434 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collision_obj_front.py
--rw-r--r--   0        0        0     4183 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collisions.py
--rw-r--r--   0        0        0     4277 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collisions_embedded.py
--rw-r--r--   0        0        0     4349 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/created_at_field.py
--rw-r--r--   0        0        0     6734 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/data_monitor_trigger.py
--rw-r--r--   0        0        0    11217 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/data_trigger.py
--rw-r--r--   0        0        0     5064 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/default_alert_push.py
--rw-r--r--   0        0        0     4984 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/default_alert_push_attributes.py
--rw-r--r--   0        0        0     6197 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/doors_state.py
--rw-r--r--   0        0        0     5478 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/doors_state_opening.py
--rw-r--r--   0        0        0     5417 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/e_coaching.py
--rw-r--r--   0        0        0     5347 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/e_coaching_links.py
--rw-r--r--   0        0        0     5871 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/e_coaching_scores.py
--rw-r--r--   0        0        0     9824 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/energy.py
--rw-r--r--   0        0        0     4982 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/energy_battery.py
--rw-r--r--   0        0        0     5286 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/energy_battery_health.py
--rw-r--r--   0        0        0     9612 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/energy_charging.py
--rw-r--r--   0        0        0     5435 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/engine.py
--rw-r--r--   0        0        0     4055 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/engine_oil.py
--rw-r--r--   0        0        0     5643 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/environment.py
--rw-r--r--   0        0        0     4128 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/environment_luminosity.py
--rw-r--r--   0        0        0     7583 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/event.py
--rw-r--r--   0        0        0     4079 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/event_links.py
--rw-r--r--   0        0        0     4802 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/extension.py
--rw-r--r--   0        0        0     3500 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/extension_type.py
--rw-r--r--   0        0        0     5295 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/geometry.py
--rw-r--r--   0        0        0     4329 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/ignition.py
--rw-r--r--   0        0        0     3488 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/index_range.py
--rw-r--r--   0        0        0     5945 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/kinetic.py
--rw-r--r--   0        0        0     5463 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/lighting.py
--rw-r--r--   0        0        0     9859 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/link.py
--rw-r--r--   0        0        0     4209 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/maintenance.py
--rw-r--r--   0        0        0     5419 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/maintenance_links.py
--rw-r--r--   0        0        0     6315 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/maintenance_obj.py
--rw-r--r--   0        0        0     6172 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor.py
--rw-r--r--   0        0        0     3484 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_id.py
--rw-r--r--   0        0        0     4695 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_links.py
--rw-r--r--   0        0        0    10499 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_parameter.py
--rw-r--r--   0        0        0     8856 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_parameter_trigger_param.py
--rw-r--r--   0        0        0     4820 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_ref.py
--rw-r--r--   0        0        0     5444 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_ref_links.py
--rw-r--r--   0        0        0     3609 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_status.py
--rw-r--r--   0        0        0     4448 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_status_setter.py
--rw-r--r--   0        0        0     7349 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_subscribe.py
--rw-r--r--   0        0        0     5397 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_batch_notify.py
--rw-r--r--   0        0        0     7551 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_retry_policy.py
--rw-r--r--   0        0        0     6109 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_trigger.py
--rw-r--r--   0        0        0     6320 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_webhook.py
--rw-r--r--   0        0        0     6610 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_webhook_attributes.py
--rw-r--r--   0        0        0     4161 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitors.py
--rw-r--r--   0        0        0     4242 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitors_embedded.py
--rw-r--r--   0        0        0     4309 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/overall_autonomy.py
--rw-r--r--   0        0        0     4979 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/point.py
--rw-r--r--   0        0        0     5073 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/polygon_zone.py
--rw-r--r--   0        0        0     5682 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/position.py
--rw-r--r--   0        0        0     6994 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/position_properties.py
--rw-r--r--   0        0        0     4417 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/preconditioning.py
--rw-r--r--   0        0        0     7491 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/preconditioning_air_conditioning.py
--rw-r--r--   0        0        0     3536 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/preconditioning_program.py
--rw-r--r--   0        0        0     4339 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/privacy.py
--rw-r--r--   0        0        0     6995 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/program.py
--rw-r--r--   0        0        0     5226 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/program_occurence.py
--rw-r--r--   0        0        0     5810 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/safety.py
--rw-r--r--   0        0        0     5057 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/service_type.py
--rw-r--r--   0        0        0    13183 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/status.py
--rw-r--r--   0        0        0     4207 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/status_embedded.py
--rw-r--r--   0        0        0     3524 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/status_extension_type.py
--rw-r--r--   0        0        0     4723 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/status_links.py
--rw-r--r--   0        0        0     6339 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/tab_links.py
--rw-r--r--   0        0        0     4172 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry.py
--rw-r--r--   0        0        0     4310 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_embedded.py
--rw-r--r--   0        0        0     3500 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_enum.py
--rw-r--r--   0        0        0     6374 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_extension.py
--rw-r--r--   0        0        0     3536 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_extension_type.py
--rw-r--r--   0        0        0     7575 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message.py
--rw-r--r--   0        0        0     4314 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_embedded.py
--rw-r--r--   0        0        0    10914 2024-03-23 16:52:00.990044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle.py
--rw-r--r--   0        0        0     4328 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_braking_system.py
--rw-r--r--   0        0        0     4434 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission.py
--rw-r--r--   0        0        0     5268 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox.py
--rw-r--r--   0        0        0     4790 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_gear.py
--rw-r--r--   0        0        0     5900 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_mode.py
--rw-r--r--   0        0        0     4784 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_monitor_trigger.py
--rw-r--r--   0        0        0     3484 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_range.py
--rw-r--r--   0        0        0     4199 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_stamped.py
--rw-r--r--   0        0        0     5591 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_trigger.py
--rw-r--r--   0        0        0     6021 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_zone_monitor_trigger.py
--rw-r--r--   0        0        0     5052 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_zone_trigger.py
--rw-r--r--   0        0        0    14784 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/trip.py
--rw-r--r--   0        0        0     5020 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/trip_avg_consumption.py
--rw-r--r--   0        0        0     5975 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/trip_links.py
--rw-r--r--   0        0        0     6658 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/trips.py
--rw-r--r--   0        0        0     4122 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/trips_embedded.py
--rw-r--r--   0        0        0     4333 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/updated_field.py
--rw-r--r--   0        0        0     3460 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/url.py
--rw-r--r--   0        0        0     7611 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/user.py
--rw-r--r--   0        0        0     4183 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/user_embedded.py
--rw-r--r--   0        0        0     4719 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/user_links.py
--rw-r--r--   0        0        0     3472 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vect2_d.py
--rw-r--r--   0        0        0     9581 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicle.py
--rw-r--r--   0        0        0     5494 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicle_engine.py
--rw-r--r--   0        0        0     8094 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicle_links.py
--rw-r--r--   0        0        0     5122 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicle_odometer.py
--rw-r--r--   0        0        0     4161 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicles.py
--rw-r--r--   0        0        0     4215 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicles_embedded.py
--rw-r--r--   0        0        0     4172 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/way_points.py
--rw-r--r--   0        0        0     5596 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/way_points_embedded.py
--rw-r--r--   0        0        0     5211 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/x_error.py
--rw-r--r--   0        0        0     5949 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/zone_monitor_trigger.py
--rw-r--r--   0        0        0     5507 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/zone_trigger.py
--rw-r--r--   0        0        0     5119 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/zone_trigger_place.py
--rw-r--r--   0        0        0     5137 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/zone_trigger_place_center.py
--rw-r--r--   0        0        0    14251 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/rest.py
--rw-r--r--   0        0        0     2795 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/constants.py
--rw-r--r--   0        0        0     1564 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/mqtt_request.py
--rw-r--r--   0        0        0     5512 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/oauth.py
--rw-r--r--   0        0        0        0 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/otp/__init__.py
--rw-r--r--   0        0        0     7320 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/otp/load.py
--rw-r--r--   0        0        0     2962 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/otp/oaep.py
--rw-r--r--   0        0        0    11755 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/otp/otp.py
--rw-r--r--   0        0        0      876 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/otp/tokenizer.py
--rw-r--r--   0        0        0        0 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/setup/__init__.py
--rw-r--r--   0        0        0     2488 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/setup/apk_parser.py
--rwxr-xr-x   0        0        0     5597 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/setup/app_decoder.py
--rw-r--r--   0        0        0     1993 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psa/setup/github.py
--rw-r--r--   0        0        0        0 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/application/__init__.py
--rw-r--r--   0        0        0     2711 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/application/abrp.py
--rw-r--r--   0        0        0     2927 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/application/battery_charge_curve.py
--rw-r--r--   0        0        0     5479 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/application/car_controller.py
--rw-r--r--   0        0        0     7232 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/application/charge_control.py
--rw-r--r--   0        0        0     4736 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/application/charging.py
--rw-r--r--   0        0        0     5115 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/application/ecomix.py
--rw-r--r--   0        0        0    11030 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/application/psa_client.py
--rw-r--r--   0        0        0     2747 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/application/trip_parser.py
--rw-r--r--   0        0        0        0 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/model/__init__.py
--rw-r--r--   0        0        0      186 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/model/battery_curve.py
--rw-r--r--   0        0        0      227 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/model/battery_soh.py
--rw-r--r--   0        0        0     4641 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/model/car.py
--rw-r--r--   0        0        0     1178 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/model/car_model.py
--rw-r--r--   0        0        0     2806 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/model/car_status.py
--rw-r--r--   0        0        0      854 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/model/charge.py
--rw-r--r--   0        0        0     3746 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/model/trip.py
--rw-r--r--   0        0        0     1349 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/repository/car_model.py
--rw-r--r--   0        0        0     7044 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/repository/config_repository.py
--rw-r--r--   0        0        0    14919 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/repository/db.py
--rw-r--r--   0        0        0     7128 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/repository/trips.py
--rw-r--r--   0        0        0    12599 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/resources/car_models.yml
--rw-r--r--   0        0        0     1507 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/psacc/utils/utils.py
--rw-r--r--   0        0        0       18 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/web/__init__.py
--rw-r--r--   0        0        0     3423 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/web/app.py
--rw-r--r--   0        0        0      313 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/web/assets/99_custom_overides.css
--rw-r--r--   0        0        0     8424 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/web/assets/clientside.js
--rw-r--r--   0        0        0     3588 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/web/assets/images/battery-charge-line.svg
--rw-r--r--   0        0        0      295 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/web/assets/images/battery-charge.svg
--rw-r--r--   0        0        0     1859 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/web/assets/images/battery-soh.svg
--rw-r--r--   0        0        0     3577 2024-03-23 16:52:00.994044 psa_car_controller-3.5.0/psa_car_controller/web/assets/images/consumption.svg
--rw-r--r--   0        0        0     7480 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/assets/images/electricity bill.svg
--rw-r--r--   0        0        0     2040 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/assets/images/mileage.svg
--rw-r--r--   0        0        0     3094 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/assets/images/pollution.svg
--rw-r--r--   0        0        0     1070 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/assets/images/settings.svg
--rw-r--r--   0        0        0      582 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/assets/images/sync.svg
--rw-r--r--   0        0        0    26505 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/assets/sprites/osm-liberty.json
--rw-r--r--   0        0        0   103877 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/assets/sprites/osm-liberty.png
--rw-r--r--   0        0        0    26581 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/assets/sprites/osm-liberty@2x.json
--rw-r--r--   0        0        0   202875 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/assets/sprites/osm-liberty@2x.png
--rw-r--r--   0        0        0      908 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/assets/style.json
--rw-r--r--   0        0        0     1279 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/dash_custom.py
--rw-r--r--   0        0        0    10277 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/figures.py
--rw-r--r--   0        0        0     1633 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/tools/Button.py
--rw-r--r--   0        0        0     1030 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/tools/Switch.py
--rw-r--r--   0        0        0     4784 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/tools/figurefilter.py
--rw-r--r--   0        0        0     3273 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/tools/utils.py
--rw-r--r--   0        0        0        0 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/view/__init__.py
--rw-r--r--   0        0        0     7020 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/view/api.py
--rw-r--r--   0        0        0     2635 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/view/config_oauth.py
--rw-r--r--   0        0        0     7033 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/view/config_views.py
--rw-r--r--   0        0        0     4026 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/view/control.py
--rw-r--r--   0        0        0    17850 2024-03-23 16:52:00.998044 psa_car_controller-3.5.0/psa_car_controller/web/view/views.py
--rw-r--r--   0        0        0     1852 2024-03-23 16:52:25.877897 psa_car_controller-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 psa_car_controller-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-16 17:35:49.388740 psa_car_controller-3.5.1/LICENSE
+-rw-r--r--   0        0        0      264 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/__init__.py
+-rwxr-xr-x   0        0        0      753 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/common/__init__.py
+-rw-r--r--   0        0        0     1802 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/common/mylogger.py
+-rw-r--r--   0        0        0     1612 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/common/utils.py
+-rw-r--r--   0        0        0      458 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/AccountInformation.py
+-rw-r--r--   0        0        0    12379 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/RemoteClient.py
+-rw-r--r--   0        0        0      678 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/RemoteCredentials.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/__init__.py
+-rw-r--r--   0        0        0    13601 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/__init__.py
+-rw-r--r--   0        0        0      319 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/api/__init__.py
+-rw-r--r--   0        0        0   102100 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/api/trips_api.py
+-rw-r--r--   0        0        0     4895 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/api/user_api.py
+-rw-r--r--   0        0        0    81355 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/api/vehicles_api.py
+-rw-r--r--   0        0        0    26152 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/api_client.py
+-rw-r--r--   0        0        0     9746 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/configuration.py
+-rw-r--r--   0        0        0    13204 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/__init__.py
+-rw-r--r--   0        0        0    14820 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/adas.py
+-rw-r--r--   0        0        0     5627 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/adas_park_assist.py
+-rw-r--r--   0        0        0     9420 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alert.py
+-rw-r--r--   0        0        0     3512 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alert_end_position.py
+-rw-r--r--   0        0        0     5935 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alert_links.py
+-rw-r--r--   0        0        0     7817 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alert_msg_enum.py
+-rw-r--r--   0        0        0     4139 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alerts.py
+-rw-r--r--   0        0        0     4153 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alerts_embedded.py
+-rw-r--r--   0        0        0     4722 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/battery.py
+-rw-r--r--   0        0        0     4546 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/bounded_program.py
+-rw-r--r--   0        0        0     3699 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/charging_status_enum.py
+-rw-r--r--   0        0        0     5092 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/circle_zone.py
+-rw-r--r--   0        0        0     5020 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/circle_zone_coordinates.py
+-rw-r--r--   0        0        0     7252 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collection_result.py
+-rw-r--r--   0        0        0     9937 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collision.py
+-rw-r--r--   0        0        0     5347 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collision_links.py
+-rw-r--r--   0        0        0     8727 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collision_obj.py
+-rw-r--r--   0        0        0     4434 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collision_obj_front.py
+-rw-r--r--   0        0        0     4183 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collisions.py
+-rw-r--r--   0        0        0     4277 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collisions_embedded.py
+-rw-r--r--   0        0        0     4349 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/created_at_field.py
+-rw-r--r--   0        0        0     6734 2024-05-16 17:35:49.396740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/data_monitor_trigger.py
+-rw-r--r--   0        0        0    11217 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/data_trigger.py
+-rw-r--r--   0        0        0     5064 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/default_alert_push.py
+-rw-r--r--   0        0        0     4984 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/default_alert_push_attributes.py
+-rw-r--r--   0        0        0     6197 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/doors_state.py
+-rw-r--r--   0        0        0     5478 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/doors_state_opening.py
+-rw-r--r--   0        0        0     5417 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/e_coaching.py
+-rw-r--r--   0        0        0     5347 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/e_coaching_links.py
+-rw-r--r--   0        0        0     5871 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/e_coaching_scores.py
+-rw-r--r--   0        0        0     9824 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/energy.py
+-rw-r--r--   0        0        0     4982 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/energy_battery.py
+-rw-r--r--   0        0        0     5286 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/energy_battery_health.py
+-rw-r--r--   0        0        0     9612 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/energy_charging.py
+-rw-r--r--   0        0        0     5435 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/engine.py
+-rw-r--r--   0        0        0     4055 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/engine_oil.py
+-rw-r--r--   0        0        0     5643 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/environment.py
+-rw-r--r--   0        0        0     4128 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/environment_luminosity.py
+-rw-r--r--   0        0        0     7583 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/event.py
+-rw-r--r--   0        0        0     4079 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/event_links.py
+-rw-r--r--   0        0        0     4802 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/extension.py
+-rw-r--r--   0        0        0     3500 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/extension_type.py
+-rw-r--r--   0        0        0     5295 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/geometry.py
+-rw-r--r--   0        0        0     4329 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/ignition.py
+-rw-r--r--   0        0        0     3488 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/index_range.py
+-rw-r--r--   0        0        0     5945 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/kinetic.py
+-rw-r--r--   0        0        0     5463 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/lighting.py
+-rw-r--r--   0        0        0     9859 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/link.py
+-rw-r--r--   0        0        0     4209 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/maintenance.py
+-rw-r--r--   0        0        0     5419 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/maintenance_links.py
+-rw-r--r--   0        0        0     6315 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/maintenance_obj.py
+-rw-r--r--   0        0        0     6172 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor.py
+-rw-r--r--   0        0        0     3484 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_id.py
+-rw-r--r--   0        0        0     4695 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_links.py
+-rw-r--r--   0        0        0    10499 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_parameter.py
+-rw-r--r--   0        0        0     8856 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_parameter_trigger_param.py
+-rw-r--r--   0        0        0     4820 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_ref.py
+-rw-r--r--   0        0        0     5444 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_ref_links.py
+-rw-r--r--   0        0        0     3609 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_status.py
+-rw-r--r--   0        0        0     4448 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_status_setter.py
+-rw-r--r--   0        0        0     7349 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_subscribe.py
+-rw-r--r--   0        0        0     5397 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_batch_notify.py
+-rw-r--r--   0        0        0     7551 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_retry_policy.py
+-rw-r--r--   0        0        0     6109 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_trigger.py
+-rw-r--r--   0        0        0     6320 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_webhook.py
+-rw-r--r--   0        0        0     6610 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_webhook_attributes.py
+-rw-r--r--   0        0        0     4161 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitors.py
+-rw-r--r--   0        0        0     4242 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitors_embedded.py
+-rw-r--r--   0        0        0     4309 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/overall_autonomy.py
+-rw-r--r--   0        0        0     4979 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/point.py
+-rw-r--r--   0        0        0     5073 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/polygon_zone.py
+-rw-r--r--   0        0        0     5682 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/position.py
+-rw-r--r--   0        0        0     6994 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/position_properties.py
+-rw-r--r--   0        0        0     4417 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/preconditioning.py
+-rw-r--r--   0        0        0     7491 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/preconditioning_air_conditioning.py
+-rw-r--r--   0        0        0     3536 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/preconditioning_program.py
+-rw-r--r--   0        0        0     4339 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/privacy.py
+-rw-r--r--   0        0        0     6995 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/program.py
+-rw-r--r--   0        0        0     5226 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/program_occurence.py
+-rw-r--r--   0        0        0     5810 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/safety.py
+-rw-r--r--   0        0        0     5057 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/service_type.py
+-rw-r--r--   0        0        0    13183 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/status.py
+-rw-r--r--   0        0        0     4207 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/status_embedded.py
+-rw-r--r--   0        0        0     3524 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/status_extension_type.py
+-rw-r--r--   0        0        0     4723 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/status_links.py
+-rw-r--r--   0        0        0     6339 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/tab_links.py
+-rw-r--r--   0        0        0     4172 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry.py
+-rw-r--r--   0        0        0     4310 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_embedded.py
+-rw-r--r--   0        0        0     3500 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_enum.py
+-rw-r--r--   0        0        0     6374 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_extension.py
+-rw-r--r--   0        0        0     3536 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_extension_type.py
+-rw-r--r--   0        0        0     7575 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message.py
+-rw-r--r--   0        0        0     4314 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_embedded.py
+-rw-r--r--   0        0        0    10914 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle.py
+-rw-r--r--   0        0        0     4328 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_braking_system.py
+-rw-r--r--   0        0        0     4434 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission.py
+-rw-r--r--   0        0        0     5268 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox.py
+-rw-r--r--   0        0        0     4790 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_gear.py
+-rw-r--r--   0        0        0     5900 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_mode.py
+-rw-r--r--   0        0        0     4784 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_monitor_trigger.py
+-rw-r--r--   0        0        0     3484 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_range.py
+-rw-r--r--   0        0        0     4199 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_stamped.py
+-rw-r--r--   0        0        0     5591 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_trigger.py
+-rw-r--r--   0        0        0     6021 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_zone_monitor_trigger.py
+-rw-r--r--   0        0        0     5052 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_zone_trigger.py
+-rw-r--r--   0        0        0    14784 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/trip.py
+-rw-r--r--   0        0        0     5020 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/trip_avg_consumption.py
+-rw-r--r--   0        0        0     5975 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/trip_links.py
+-rw-r--r--   0        0        0     6658 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/trips.py
+-rw-r--r--   0        0        0     4122 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/trips_embedded.py
+-rw-r--r--   0        0        0     4333 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/updated_field.py
+-rw-r--r--   0        0        0     3460 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/url.py
+-rw-r--r--   0        0        0     7611 2024-05-16 17:35:49.400740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/user.py
+-rw-r--r--   0        0        0     4183 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/user_embedded.py
+-rw-r--r--   0        0        0     4719 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/user_links.py
+-rw-r--r--   0        0        0     3472 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vect2_d.py
+-rw-r--r--   0        0        0     9581 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicle.py
+-rw-r--r--   0        0        0     5494 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicle_engine.py
+-rw-r--r--   0        0        0     8094 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicle_links.py
+-rw-r--r--   0        0        0     5122 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicle_odometer.py
+-rw-r--r--   0        0        0     4161 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicles.py
+-rw-r--r--   0        0        0     4215 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicles_embedded.py
+-rw-r--r--   0        0        0     4172 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/way_points.py
+-rw-r--r--   0        0        0     5596 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/way_points_embedded.py
+-rw-r--r--   0        0        0     5211 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/x_error.py
+-rw-r--r--   0        0        0     5949 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/zone_monitor_trigger.py
+-rw-r--r--   0        0        0     5507 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/zone_trigger.py
+-rw-r--r--   0        0        0     5119 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/zone_trigger_place.py
+-rw-r--r--   0        0        0     5137 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/zone_trigger_place_center.py
+-rw-r--r--   0        0        0    14251 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/rest.py
+-rw-r--r--   0        0        0     2795 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/constants.py
+-rw-r--r--   0        0        0     1564 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/mqtt_request.py
+-rw-r--r--   0        0        0     5512 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/oauth.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/otp/__init__.py
+-rw-r--r--   0        0        0     7320 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/otp/load.py
+-rw-r--r--   0        0        0     2962 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/otp/oaep.py
+-rw-r--r--   0        0        0    11755 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/otp/otp.py
+-rw-r--r--   0        0        0      876 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/otp/tokenizer.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/setup/__init__.py
+-rw-r--r--   0        0        0     2488 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/setup/apk_parser.py
+-rwxr-xr-x   0        0        0     5597 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/setup/app_decoder.py
+-rw-r--r--   0        0        0     1993 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psa/setup/github.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/application/__init__.py
+-rw-r--r--   0        0        0     2711 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/application/abrp.py
+-rw-r--r--   0        0        0     2927 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/application/battery_charge_curve.py
+-rw-r--r--   0        0        0     5479 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/application/car_controller.py
+-rw-r--r--   0        0        0     7232 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/application/charge_control.py
+-rw-r--r--   0        0        0     4736 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/application/charging.py
+-rw-r--r--   0        0        0     5115 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/application/ecomix.py
+-rw-r--r--   0        0        0    11030 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/application/psa_client.py
+-rw-r--r--   0        0        0     2747 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/application/trip_parser.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/model/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/model/battery_curve.py
+-rw-r--r--   0        0        0      227 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/model/battery_soh.py
+-rw-r--r--   0        0        0     4641 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/model/car.py
+-rw-r--r--   0        0        0     1178 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/model/car_model.py
+-rw-r--r--   0        0        0     2806 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/model/car_status.py
+-rw-r--r--   0        0        0      854 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/model/charge.py
+-rw-r--r--   0        0        0     3746 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/model/trip.py
+-rw-r--r--   0        0        0     1349 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/repository/car_model.py
+-rw-r--r--   0        0        0     7044 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/repository/config_repository.py
+-rw-r--r--   0        0        0    14919 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/repository/db.py
+-rw-r--r--   0        0        0     7128 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/repository/trips.py
+-rw-r--r--   0        0        0    13215 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/resources/car_models.yml
+-rw-r--r--   0        0        0     1507 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/psacc/utils/utils.py
+-rw-r--r--   0        0        0       18 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/__init__.py
+-rw-r--r--   0        0        0     3423 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/app.py
+-rw-r--r--   0        0        0      313 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/99_custom_overides.css
+-rw-r--r--   0        0        0     8424 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/clientside.js
+-rw-r--r--   0        0        0     3588 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/images/battery-charge-line.svg
+-rw-r--r--   0        0        0      295 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/images/battery-charge.svg
+-rw-r--r--   0        0        0     1859 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/images/battery-soh.svg
+-rw-r--r--   0        0        0     3577 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/images/consumption.svg
+-rw-r--r--   0        0        0     7480 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/images/electricity bill.svg
+-rw-r--r--   0        0        0     2040 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/images/mileage.svg
+-rw-r--r--   0        0        0     3094 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/images/pollution.svg
+-rw-r--r--   0        0        0     1070 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/images/settings.svg
+-rw-r--r--   0        0        0      582 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/images/sync.svg
+-rw-r--r--   0        0        0    26505 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/sprites/osm-liberty.json
+-rw-r--r--   0        0        0   103877 2024-05-16 17:35:49.404740 psa_car_controller-3.5.1/psa_car_controller/web/assets/sprites/osm-liberty.png
+-rw-r--r--   0        0        0    26581 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/assets/sprites/osm-liberty@2x.json
+-rw-r--r--   0        0        0   202875 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/assets/sprites/osm-liberty@2x.png
+-rw-r--r--   0        0        0      908 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/assets/style.json
+-rw-r--r--   0        0        0     1279 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/dash_custom.py
+-rw-r--r--   0        0        0    10277 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/figures.py
+-rw-r--r--   0        0        0     1633 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/tools/Button.py
+-rw-r--r--   0        0        0     1030 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/tools/Switch.py
+-rw-r--r--   0        0        0     4784 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/tools/figurefilter.py
+-rw-r--r--   0        0        0     3273 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/tools/utils.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/view/__init__.py
+-rw-r--r--   0        0        0     7020 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/view/api.py
+-rw-r--r--   0        0        0     2635 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/view/config_oauth.py
+-rw-r--r--   0        0        0     7033 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/view/config_views.py
+-rw-r--r--   0        0        0     4026 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/view/control.py
+-rw-r--r--   0        0        0    17850 2024-05-16 17:35:49.408740 psa_car_controller-3.5.1/psa_car_controller/web/view/views.py
+-rw-r--r--   0        0        0     1852 2024-05-16 17:36:04.168626 psa_car_controller-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 psa_car_controller-3.5.1/PKG-INFO
```

### Comparing `psa_car_controller-3.5.0/LICENSE` & `psa_car_controller-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/__main__.py` & `psa_car_controller-3.5.1/psa_car_controller/__main__.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/common/mylogger.py` & `psa_car_controller-3.5.1/psa_car_controller/common/mylogger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/common/utils.py` & `psa_car_controller-3.5.1/psa_car_controller/common/utils.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/RemoteClient.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/RemoteClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             "x-introspect-realm": self.account_info.realm,
             "accept": "application/hal+json",
             "User-Agent": "okhttp/4.8.0",
         }
         self.last_request = None
         self.mqtt_client = None
         self.otp = None
+        self._lock = threading.Lock()
 
     def __on_mqtt_connect(self, client, userdata, result_code, _):  # pylint: disable=unused-argument
         logger.info("Connected with result code %s", result_code)
         topics = [MQTT_RESP_TOPIC + self.account_info.get_mqtt_customer_id() + "/#"]
         for car in self.vehicles_list:
             topics.append(MQTT_EVENT_TOPIC + car.vin)
         for topic in topics:
@@ -142,47 +143,48 @@
         if store:
             self.last_request = mqtt_request
 
     def mqtt_request(self, vin, req_parameters, topic):
         return MQTTRequest(topic, vin, req_parameters, self.account_info.get_mqtt_customer_id())
 
     def _refresh_remote_token(self, force=False):
-        bad_remote_token = self.remoteCredentials.refresh_token is None
-        if not force and not bad_remote_token and self.remoteCredentials.last_update:
-            last_update: datetime = self.remoteCredentials.last_update
-            if (datetime.now() - last_update).total_seconds() < MQTT_TOKEN_TTL:
-                return True
-        try:
-            self.manager.refresh_token_now()
-            if bad_remote_token:
-                logger.error("remote_refresh_token isn't defined")
-            else:
-                res = self.manager.post(REMOTE_URL + self.account_info.client_id,
-                                        json={"grant_type": "refresh_token",
-                                              "refresh_token": self.remoteCredentials.refresh_token},
-                                        headers=self.headers)
-                data = res.json()
-                logger.debug("refresh_remote_token: %s", data)
-                if "access_token" in data:
-                    self.remoteCredentials.access_token = data["access_token"]
-                    self.remoteCredentials.refresh_token = data["refresh_token"]
-                    bad_remote_token = False
+        with self._lock:
+            bad_remote_token = self.remoteCredentials.refresh_token is None
+            if not force and not bad_remote_token and self.remoteCredentials.last_update:
+                last_update: datetime = self.remoteCredentials.last_update
+                if (datetime.now() - last_update).total_seconds() < MQTT_TOKEN_TTL:
+                    return True
+            try:
+                self.manager.refresh_token_now()
+                if bad_remote_token:
+                    logger.warning("remote_refresh_token isn't defined")
                 else:
-                    logger.error("can't refresh_remote_token: %s\n Create a new one", data)
-                    bad_remote_token = True
-            if bad_remote_token:
-                otp_code = self.get_otp_code()
-                self._get_remote_access_token(otp_code)
-            self.remote_token_last_update = datetime.now()
-            self.mqtt_client.username_pw_set("IMA_OAUTH_ACCESS_TOKEN", self.remoteCredentials.access_token)
-            return True
-        except (RequestException, RateLimitException, KeyError) as e:
-            logger.exception("Can't refresh remote token %s", e)
-            time.sleep(60)
-            return False
+                    res = self.manager.post(REMOTE_URL + self.account_info.client_id,
+                                            json={"grant_type": "refresh_token",
+                                                  "refresh_token": self.remoteCredentials.refresh_token},
+                                            headers=self.headers)
+                    data = res.json()
+                    logger.debug("refresh_remote_token: %s", data)
+                    if "access_token" in data:
+                        self.remoteCredentials.access_token = data["access_token"]
+                        bad_remote_token = False
+                        if "refresh_token" in data:
+                            self.remoteCredentials.refresh_token = data["refresh_token"]
+                    else:
+                        logger.error("can't refresh_remote_token: %s\n Create a new one", data)
+                        bad_remote_token = True
+                if bad_remote_token:
+                    otp_code = self.get_otp_code()
+                    self._get_remote_access_token(otp_code)
+                self.remote_token_last_update = datetime.now()
+                self.mqtt_client.username_pw_set("IMA_OAUTH_ACCESS_TOKEN", self.remoteCredentials.access_token)
+                return True
+            except (RequestException, RateLimitException, KeyError):
+                logger.exception("Can't refresh remote token, please redo otp procedure")
+                return False
 
     def get_sms_otp_code(self):
         res = self.manager.post(
             "https://api.groupe-psa.com/applications/cvs/v4/mobile/smsCode?client_id=" + self.account_info.client_id,
             headers=self.headers)
         return res
```

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/RemoteCredentials.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/RemoteCredentials.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/__init__.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/__init__.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/api/trips_api.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/api/trips_api.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/api/user_api.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/api/user_api.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/api/vehicles_api.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/api/vehicles_api.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/api_client.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/api_client.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/configuration.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/configuration.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/__init__.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/adas.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/adas.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/adas_park_assist.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/adas_park_assist.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alert.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alert.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alert_end_position.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alert_end_position.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alert_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alert_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alert_msg_enum.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alert_msg_enum.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alerts.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alerts.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/alerts_embedded.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/alerts_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/battery.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/battery.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/bounded_program.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/bounded_program.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/charging_status_enum.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/charging_status_enum.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/circle_zone.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/circle_zone.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/circle_zone_coordinates.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/circle_zone_coordinates.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collection_result.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collection_result.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collision.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collision.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collision_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collision_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collision_obj.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collision_obj.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collision_obj_front.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collision_obj_front.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collisions.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collisions.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/collisions_embedded.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/collisions_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/created_at_field.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/created_at_field.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/data_monitor_trigger.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/data_monitor_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/data_trigger.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/data_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/default_alert_push.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/default_alert_push.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/default_alert_push_attributes.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/default_alert_push_attributes.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/doors_state.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/doors_state.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/doors_state_opening.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/doors_state_opening.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/e_coaching.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/e_coaching.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/e_coaching_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/e_coaching_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/e_coaching_scores.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/e_coaching_scores.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/energy.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/energy.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/energy_battery.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/energy_battery.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/energy_battery_health.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/energy_battery_health.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/energy_charging.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/energy_charging.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/engine.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/engine.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/engine_oil.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/engine_oil.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/environment.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/environment.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/environment_luminosity.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/environment_luminosity.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/event.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/event.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/event_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/event_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/extension.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/extension.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/extension_type.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/extension_type.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/geometry.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/geometry.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/ignition.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/ignition.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/index_range.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/index_range.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/kinetic.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/kinetic.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/lighting.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/lighting.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/link.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/link.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/maintenance.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/maintenance.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/maintenance_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/maintenance_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/maintenance_obj.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/maintenance_obj.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_id.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_id.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_parameter.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_parameter.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_parameter_trigger_param.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_parameter_trigger_param.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_ref.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_ref.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_ref_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_ref_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_status.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_status.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_status_setter.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_status_setter.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_subscribe.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_subscribe.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_batch_notify.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_batch_notify.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_retry_policy.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_subscribe_retry_policy.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_trigger.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_webhook.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_webhook.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitor_webhook_attributes.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitor_webhook_attributes.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitors.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitors.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/monitors_embedded.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/monitors_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/overall_autonomy.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/overall_autonomy.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/point.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/point.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/polygon_zone.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/polygon_zone.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/position.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/position.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/position_properties.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/position_properties.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/preconditioning.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/preconditioning.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/preconditioning_air_conditioning.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/preconditioning_air_conditioning.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/preconditioning_program.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/preconditioning_program.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/privacy.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/privacy.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/program.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/program.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/program_occurence.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/program_occurence.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/safety.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/safety.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/service_type.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/service_type.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/status.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/status.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/status_embedded.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/status_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/status_extension_type.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/status_extension_type.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/status_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/status_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/tab_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/tab_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_embedded.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_enum.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_enum.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_extension.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_extension.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_extension_type.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_extension_type.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_embedded.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_braking_system.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_braking_system.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_gear.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_gear.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_mode.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/telemetry_message_vehicle_transmission_gearbox_mode.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_monitor_trigger.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_monitor_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_range.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_range.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_stamped.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_stamped.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_trigger.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_zone_monitor_trigger.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_zone_monitor_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/time_zone_trigger.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/time_zone_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/trip.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/trip.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/trip_avg_consumption.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/trip_avg_consumption.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/trip_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/trip_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/trips.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/trips.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/trips_embedded.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/trips_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/updated_field.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/updated_field.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/url.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/url.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/user.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/user.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/user_embedded.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/user_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/user_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/user_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vect2_d.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vect2_d.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicle.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicle.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicle_engine.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicle_engine.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicle_links.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicle_links.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicle_odometer.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicle_odometer.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicles.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicles.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/vehicles_embedded.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/vehicles_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/way_points.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/way_points.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/way_points_embedded.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/way_points_embedded.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/x_error.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/x_error.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/zone_monitor_trigger.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/zone_monitor_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/zone_trigger.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/zone_trigger.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/zone_trigger_place.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/zone_trigger_place.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/models/zone_trigger_place_center.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/models/zone_trigger_place_center.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/connected_car_api/rest.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/connected_car_api/rest.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/constants.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/constants.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/mqtt_request.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/mqtt_request.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/oauth.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/oauth.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/otp/load.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/otp/load.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/otp/oaep.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/otp/oaep.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/otp/otp.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/otp/otp.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/otp/tokenizer.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/otp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/setup/apk_parser.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/setup/apk_parser.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/setup/app_decoder.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/setup/app_decoder.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psa/setup/github.py` & `psa_car_controller-3.5.1/psa_car_controller/psa/setup/github.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/application/abrp.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/application/abrp.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/application/battery_charge_curve.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/application/battery_charge_curve.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/application/car_controller.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/application/car_controller.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/application/charge_control.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/application/charge_control.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/application/charging.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/application/charging.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/application/ecomix.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/application/ecomix.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/application/psa_client.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/application/psa_client.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/application/trip_parser.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/application/trip_parser.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/model/car.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/model/car.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/model/car_model.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/model/car_model.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/model/car_status.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/model/car_status.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/model/charge.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/model/charge.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/model/trip.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/model/trip.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/repository/car_model.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/repository/car_model.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/repository/config_repository.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/repository/config_repository.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/repository/db.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/repository/db.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/repository/trips.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/repository/trips.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/resources/car_models.yml` & `psa_car_controller-3.5.1/psa_car_controller/psacc/resources/car_models.yml`

 * *Files 0% similar despite different names*

```diff
@@ -399,30 +399,46 @@
   name: Astra L GSe Hybrid
   battery_power: 12.4
   fuel_capacity: 42
   abrp_name:
   reg: VXKF3DGYTP.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
+- !CarModel
+  name: Astra L Sports Tourer GSe Hybrid
+  battery_power: 12.4
+  fuel_capacity: 42
+  abrp_name:
+  reg: VXKF4DGYTN.*
+  max_elec_consumption: 70
+  max_fuel_consumption: 30
 - !ElecModel
   name: Astra L Electric GS
-  battery_poewr: 51
+  battery_power: 51
   fuel_capacity: 0
   abrp_name: opel:astrae:23:54
   reg: VXKFMZKWZP.*
   max_elec_consumption: 70
 - !CarModel
   name: Astra L Hybrid
   battery_power: 12.4
   fuel_capacity: 42
   abrp_name:
   reg: VXKF3DGXTP.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
 - !CarModel
+  name: Astra L ST Hybrid
+  battery_power: 12.4
+  fuel_capacity: 42
+  abrp_name:
+  reg: VXKF4DGXTP.*
+  max_elec_consumption: 70
+  max_fuel_consumption: 30
+- !CarModel
   name: 308 SW Hybrid
   battery_power: 12.4
   fuel_capacity: 40
   abrp_name:
   reg: VR3F4DGXTN.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
@@ -439,14 +455,22 @@
   battery_power: 0
   fuel_capacity: 56
   abrp_name:
   reg: VR3FPHNSTN.*
   max_elec_consumption: 70
   max_fuel_consumption: 30   
 - !CarModel
+  name: New 308
+  battery_power: 0
+  fuel_capacity: 52
+  abrp_name:
+  reg: VR3FPHNSLN.*
+  max_elec_consumption: 70
+  max_fuel_consumption: 30   
+- !CarModel
   name: C5X
   battery_power: 12.4
   fuel_capacity: 40
   abrp_name:
   reg: VR7NDDGYPN.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
@@ -604,7 +628,13 @@
   name: C5 Aircross Hybrid 2024
   battery_power: 13.2
   fuel_capacity: 43
   abrp_name:
   reg: VR7A4DGL.*
   max_elec_consumption: 70
   max_fuel_consumption: 30
+- !CarModel
+  name: 408 GT 1.3 Petrol
+  battery_power: 0
+  fuel_capacity: 52
+  abrp_name:
+  reg: VR3FPHNSTP.*
```

### Comparing `psa_car_controller-3.5.0/psa_car_controller/psacc/utils/utils.py` & `psa_car_controller-3.5.1/psa_car_controller/psacc/utils/utils.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/app.py` & `psa_car_controller-3.5.1/psa_car_controller/web/app.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/clientside.js` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/clientside.js`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/images/battery-charge-line.svg` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/images/battery-charge-line.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/images/battery-soh.svg` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/images/battery-soh.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/images/consumption.svg` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/images/consumption.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/images/electricity bill.svg` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/images/electricity bill.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/images/mileage.svg` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/images/mileage.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/images/pollution.svg` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/images/pollution.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/images/settings.svg` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/images/settings.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/images/sync.svg` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/images/sync.svg`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/sprites/osm-liberty.json` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/sprites/osm-liberty.json`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/sprites/osm-liberty.png` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/sprites/osm-liberty.png`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/sprites/osm-liberty@2x.json` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/sprites/osm-liberty@2x.json`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/sprites/osm-liberty@2x.png` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/sprites/osm-liberty@2x.png`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/assets/style.json` & `psa_car_controller-3.5.1/psa_car_controller/web/assets/style.json`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/dash_custom.py` & `psa_car_controller-3.5.1/psa_car_controller/web/dash_custom.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/figures.py` & `psa_car_controller-3.5.1/psa_car_controller/web/figures.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/tools/Button.py` & `psa_car_controller-3.5.1/psa_car_controller/web/tools/Button.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/tools/Switch.py` & `psa_car_controller-3.5.1/psa_car_controller/web/tools/Switch.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/tools/figurefilter.py` & `psa_car_controller-3.5.1/psa_car_controller/web/tools/figurefilter.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/tools/utils.py` & `psa_car_controller-3.5.1/psa_car_controller/web/tools/utils.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/view/api.py` & `psa_car_controller-3.5.1/psa_car_controller/web/view/api.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/view/config_oauth.py` & `psa_car_controller-3.5.1/psa_car_controller/web/view/config_oauth.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/view/config_views.py` & `psa_car_controller-3.5.1/psa_car_controller/web/view/config_views.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/view/control.py` & `psa_car_controller-3.5.1/psa_car_controller/web/view/control.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/psa_car_controller/web/view/views.py` & `psa_car_controller-3.5.1/psa_car_controller/web/view/views.py`

 * *Files identical despite different names*

### Comparing `psa_car_controller-3.5.0/pyproject.toml` & `psa_car_controller-3.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psa-car-controller"
-version = "v3.5.0"
+version = "v3.5.1"
 description = "This is a python program to control a psa car with connected_car v4 api."
 authors = ["Florian Bezannier <florian.bezannier@hotmail.fr>"]
 license = "GPL-3.0"
 homepage = "https://github.com/flobz/psa_car_controller"
 repository = "https://github.com/flobz/psa_car_controller"
 include = [
     "LICENSE",
```

### Comparing `psa_car_controller-3.5.0/PKG-INFO` & `psa_car_controller-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psa-car-controller
-Version: 3.5.0
+Version: 3.5.1
 Summary: This is a python program to control a psa car with connected_car v4 api.
 Home-page: https://github.com/flobz/psa_car_controller
 License: GPL-3.0
 Author: Florian Bezannier
 Author-email: florian.bezannier@hotmail.fr
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

