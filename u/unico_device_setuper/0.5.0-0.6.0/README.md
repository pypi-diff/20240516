# Comparing `tmp/unico_device_setuper-0.5.0.tar.gz` & `tmp/unico_device_setuper-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unico_device_setuper-0.5.0.tar", max compression
+gzip compressed data, was "unico_device_setuper-0.6.0.tar", max compression
```

## Comparing `unico_device_setuper-0.5.0.tar` & `unico_device_setuper-0.6.0.tar`

### file list

```diff
@@ -1,469 +1,469 @@
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.833642 unico_device_setuper-0.5.0/README.md
--rw-r--r--   0        0        0     5084 2024-05-15 12:35:15.873227 unico_device_setuper-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-15 12:24:10.031051 unico_device_setuper-0.5.0/unico_device_setuper/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.837642 unico_device_setuper-0.5.0/unico_device_setuper/cli/__init__.py
--rw-r--r--   0        0        0     2196 2024-05-15 07:41:29.465862 unico_device_setuper-0.5.0/unico_device_setuper/cli/main.py
--rw-r--r--   0        0        0     4870 2024-05-15 12:35:15.873227 unico_device_setuper-0.5.0/unico_device_setuper/cli/pkg.py
--rw-r--r--   0        0        0     1632 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/cli/stp.py
--rw-r--r--   0        0        0     1144 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/cli/unav.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.837642 unico_device_setuper-0.5.0/unico_device_setuper/lib/__init__.py
--rw-r--r--   0        0        0     1354 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/aapt.py
--rw-r--r--   0        0        0     1838 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/adb.py
--rw-r--r--   0        0        0     2951 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/auth.py
--rw-r--r--   0        0        0     2013 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/cnsl.py
--rw-r--r--   0        0        0      822 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/datadir.py
--rw-r--r--   0        0        0     2834 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/dl.py
--rw-r--r--   0        0        0    35108 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/__init__.py
--rw-r--r--   0        0        0      152 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/__init__.py
--rw-r--r--   0        0        0       45 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.837642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/__init__.py
--rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/delete_attachment_id.py
--rw-r--r--   0        0        0     2732 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_data_by_id_id.py
--rw-r--r--   0        0        0     2795 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_event_images_id_event.py
--rw-r--r--   0        0        0     2869 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_info_by_foreign_id_mode_id.py
--rw-r--r--   0        0        0     2732 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_info_by_id_id.py
--rw-r--r--   0        0        0     2904 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_producing_place_images_id_producing_place.py
--rw-r--r--   0        0        0     2614 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/post_attachment.py
--rw-r--r--   0        0        0     2933 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/put_attachment_is_visible_in_uni_and_co_id_is_visible.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.837642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/__init__.py
--rw-r--r--   0        0        0     2720 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/delete_auth_id.py
--rw-r--r--   0        0        0     2725 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/delete_auth_user_id.py
--rw-r--r--   0        0        0     2607 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth.py
--rw-r--r--   0        0        0     4107 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth_current_user_info.py
--rw-r--r--   0        0        0     3338 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth_device_login.py
--rw-r--r--   0        0        0     5755 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_login.py
--rw-r--r--   0        0        0     2931 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_register.py
--rw-r--r--   0        0        0     3038 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_reset_password.py
--rw-r--r--   0        0        0     3084 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/put_auth_by_id_id.py
--rw-r--r--   0        0        0     3038 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/put_auth_change_password.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.837642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/back_office/__init__.py
--rw-r--r--   0        0        0     2649 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/back_office/get_back_office_event_definition_email_subscription_all.py
--rw-r--r--   0        0        0     3184 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/back_office/post_back_office_event_definition_email_subscription.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/calendar/__init__.py
--rw-r--r--   0        0        0     3824 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/calendar/get_calendar_calendar_occurrences.py
--rw-r--r--   0        0        0     2956 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/calendar/put_calendar_settings.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/cartography/__init__.py
--rw-r--r--   0        0        0     2628 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/cartography/get_cartography_map_corrections.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/__init__.py
--rw-r--r--   0        0        0     4301 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/get_client.py
--rw-r--r--   0        0        0     2633 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_default_speed_on_segment_km_h.py
--rw-r--r--   0        0        0     2627 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_filling_rate_setting.py
--rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_show_deadheading.py
--rw-r--r--   0        0        0     2563 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/post_client_filling_rate_setting.py
--rw-r--r--   0        0        0     2755 2024-05-15 07:41:29.469862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_color_color.py
--rw-r--r--   0        0        0     3073 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_default_speed_on_segment_km_h.py
--rw-r--r--   0        0        0     2990 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_mapbox.py
--rw-r--r--   0        0        0     3063 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_show_deadheading.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/comment/__init__.py
--rw-r--r--   0        0        0     2728 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/comment/delete_comment_by_id_id.py
--rw-r--r--   0        0        0     2790 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/comment/get_comment_by_event_id_id_event.py
--rw-r--r--   0        0        0     2981 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/comment/post_comment_new.py
--rw-r--r--   0        0        0     3108 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/comment/put_comment_by_id_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/constraint/__init__.py
--rw-r--r--   0        0        0     2657 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/constraint/get_constraint_id.py
--rw-r--r--   0        0        0     2906 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/constraint/put_constraint.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/__init__.py
--rw-r--r--   0        0        0     2730 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/delete_container_by_id_id.py
--rw-r--r--   0        0        0     2612 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container.py
--rw-r--r--   0        0        0     2626 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_all_definitions.py
--rw-r--r--   0        0        0     2628 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_all_serial_numbers.py
--rw-r--r--   0        0        0     2727 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_id_id.py
--rw-r--r--   0        0        0     2901 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_id_producing_place_id_producing_place.py
--rw-r--r--   0        0        0     2847 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_serial_number_serial_number.py
--rw-r--r--   0        0        0     2637 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_containers_with_active_event.py
--rw-r--r--   0        0        0     2735 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_custom_fields_id.py
--rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_filter_options.py
--rw-r--r--   0        0        0     2620 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_filtered.py
--rw-r--r--   0        0        0     2735 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_history_by_id_id.py
--rw-r--r--   0        0        0     3054 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_delete_many.py
--rw-r--r--   0        0        0     2618 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_in_ids.py
--rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_new.py
--rw-r--r--   0        0        0     2964 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_new_many.py
--rw-r--r--   0        0        0     2727 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/put_container_by_id_id.py
--rw-r--r--   0        0        0     3214 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/put_container_update_state_by_id_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container_definition/__init__.py
--rw-r--r--   0        0        0     2622 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container_definition/get_container_definition.py
--rw-r--r--   0        0        0     2560 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container_definition/post_container_definition_new.py
--rw-r--r--   0        0        0     2671 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container_definition/put_container_definition_by_id_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/__init__.py
--rw-r--r--   0        0        0     2727 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/delete_custom_field_id.py
--rw-r--r--   0        0        0     2804 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/delete_custom_field_option_id_option.py
--rw-r--r--   0        0        0     2769 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/get_custom_field_many_target.py
--rw-r--r--   0        0        0     2923 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/post_custom_field.py
--rw-r--r--   0        0        0     3307 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/post_custom_field_option_id_custom_field.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/dashboard/__init__.py
--rw-r--r--   0        0        0     3290 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/dashboard/get_dashboard_stats.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/__init__.py
--rw-r--r--   0        0        0     2608 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot.py
--rw-r--r--   0        0        0     2734 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_as_route_part_by_id_id.py
--rw-r--r--   0        0        0     2760 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_as_route_part_label.py
--rw-r--r--   0        0        0     2723 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_by_id_id.py
--rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_details_id.py
--rw-r--r--   0        0        0     2614 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_labels.py
--rw-r--r--   0        0        0     2543 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/post_depot.py
--rw-r--r--   0        0        0     2723 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/put_depot_by_id_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/__init__.py
--rw-r--r--   0        0        0     2728 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/delete_device_event_id.py
--rw-r--r--   0        0        0     2730 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_attachment_id.py
--rw-r--r--   0        0        0     2620 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_check_in_form.py
--rw-r--r--   0        0        0     2549 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_client.py
--rw-r--r--   0        0        0     2902 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_client_dasri_allow_taken_producing_place_id.py
--rw-r--r--   0        0        0     2854 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_container_by_serial_number_serial_number.py
--rw-r--r--   0        0        0     2629 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_container_definitions.py
--rw-r--r--   0        0        0     2749 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_containers_by_producing_place_id_id.py
--rw-r--r--   0        0        0     2615 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_depots.py
--rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_drivers.py
--rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_event_definitions.py
--rw-r--r--   0        0        0     2635 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_event_definitions_categories.py
--rw-r--r--   0        0        0     3467 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_itinerary_id.py
--rw-r--r--   0        0        0     2623 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_map_corrections.py
--rw-r--r--   0        0        0     3503 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_near_by_producing_place.py
--rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_outlets.py
--rw-r--r--   0        0        0     2623 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_poi_definitions.py
--rw-r--r--   0        0        0     2874 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_pois_id_poi_definition.py
--rw-r--r--   0        0        0     3274 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_round_id_itinerary.py
--rw-r--r--   0        0        0     3060 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_rounds_meta.py
--rw-r--r--   0        0        0     3466 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_search_producing_place.py
--rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.473862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_streams.py
--rw-r--r--   0        0        0     4082 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_update_change_log.py
--rw-r--r--   0        0        0     3470 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_v2_itinerary_id.py
--rw-r--r--   0        0        0     3506 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_v_2_near_by_producing_place.py
--rw-r--r--   0        0        0     2617 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_vehicles.py
--rw-r--r--   0        0        0     2556 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_bsd_sign_many.py
--rw-r--r--   0        0        0     2559 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_dasri_sign_many.py
--rw-r--r--   0        0        0     2997 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_live_data_update.py
--rw-r--r--   0        0        0     2996 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_map_corrections.py
--rw-r--r--   0        0        0     2989 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_submit_check_in.py
--rw-r--r--   0        0        0     2557 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_v2_bsd_create.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/driver/__init__.py
--rw-r--r--   0        0        0     2609 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/driver/get_driver.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/__init__.py
--rw-r--r--   0        0        0     2611 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee.py
--rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_by_id_id.py
--rw-r--r--   0        0        0     2820 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_employee_id_schedule.py
--rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_filter_options.py
--rw-r--r--   0        0        0     2666 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_id_constraint.py
--rw-r--r--   0        0        0     2549 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/post_employee_new.py
--rw-r--r--   0        0        0     3073 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_archive_id.py
--rw-r--r--   0        0        0     2980 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_archive_many.py
--rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_by_id_id.py
--rw-r--r--   0        0        0     2754 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_employee_id_schedule.py
--rw-r--r--   0        0        0     3097 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_id_constraint.py
--rw-r--r--   0        0        0     3073 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_sectors_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/error_report/__init__.py
--rw-r--r--   0        0        0     3062 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/error_report/post_error_report_device_crash_report.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/__init__.py
--rw-r--r--   0        0        0     2548 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_active.py
--rw-r--r--   0        0        0     2551 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_all_active.py
--rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_all_unique_authors.py
--rw-r--r--   0        0        0     2723 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_by_id_id.py
--rw-r--r--   0        0        0     2924 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_count_by_id_round_realisation_id_round_realisation.py
--rw-r--r--   0        0        0     2619 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_count_by_type.py
--rw-r--r--   0        0        0     2615 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_def_all.py
--rw-r--r--   0        0        0     2749 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_def_by_type_type.py
--rw-r--r--   0        0        0     2731 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_detailed_by_id_id.py
--rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_displayable_events.py
--rw-r--r--   0        0        0     2621 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_filter_options.py
--rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_filtered.py
--rw-r--r--   0        0        0     2551 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_to_planify.py
--rw-r--r--   0        0        0     3022 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/post_event_delete_many.py
--rw-r--r--   0        0        0     2612 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/post_event_new.py
--rw-r--r--   0        0        0     2664 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/put_event_update_by_id_id.py
--rw-r--r--   0        0        0     2871 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/put_event_update_state_id_state.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition/__init__.py
--rw-r--r--   0        0        0     2618 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition/get_event_definition.py
--rw-r--r--   0        0        0     2980 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition/post_event_definition_new.py
--rw-r--r--   0        0        0     3107 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition/put_event_definition_by_id_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/__init__.py
--rw-r--r--   0        0        0     2626 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/get_event_definition_category.py
--rw-r--r--   0        0        0     3045 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/post_event_definition_category_new.py
--rw-r--r--   0        0        0     3172 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/put_event_definition_category_by_id_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/export_client/__init__.py
--rw-r--r--   0        0        0     2860 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/export_client/get_export_client_reference_type.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/__init__.py
--rw-r--r--   0        0        0     2635 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_alpes_mesure_filling_rate.py
--rw-r--r--   0        0        0     3127 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_button_collect_request.py
--rw-r--r--   0        0        0     3378 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_create_ifm_itinerary_id_realisation.py
--rw-r--r--   0        0        0     2838 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_elise_work_orders_id_franchise.py
--rw-r--r--   0        0        0     3021 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_live_vehicle_data.py
--rw-r--r--   0        0        0     2717 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_v2_live_vehicle_data.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/icons/__init__.py
--rw-r--r--   0        0        0     2929 2024-05-15 07:41:29.477862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/icons/get_icons.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/intervention/__init__.py
--rw-r--r--   0        0        0     2725 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/intervention/get_intervention_id.py
--rw-r--r--   0        0        0     2945 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/intervention/get_intervention_to_planify.py
--rw-r--r--   0        0        0     3138 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/intervention/put_intervention_id_planned_date.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/logistic/__init__.py
--rw-r--r--   0        0        0     2552 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_as_pois.py
--rw-r--r--   0        0        0     2553 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_by_batch.py
--rw-r--r--   0        0        0     2552 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_export.py
--rw-r--r--   0        0        0     2556 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_total_count.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/mapbox/__init__.py
--rw-r--r--   0        0        0     2609 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/mapbox/get_mapbox.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/message/__init__.py
--rw-r--r--   0        0        0     2548 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/message/post_message_new.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/occurrence/__init__.py
--rw-r--r--   0        0        0     3648 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_export_collect_points.py
--rw-r--r--   0        0        0     3551 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_in_interval.py
--rw-r--r--   0        0        0     3393 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_team_by_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operational/__init__.py
--rw-r--r--   0        0        0     2628 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operational/get_operational_filter_options.py
--rw-r--r--   0        0        0     3053 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operational/post_operational_layers_data_source.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operator/__init__.py
--rw-r--r--   0        0        0     2611 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator.py
--rw-r--r--   0        0        0     2736 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator_by_id_ids.py
--rw-r--r--   0        0        0     2734 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator_history_by_id_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/__init__.py
--rw-r--r--   0        0        0     2609 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet.py
--rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_all_as_route_parts.py
--rw-r--r--   0        0        0     2735 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_as_route_part_by_id_id.py
--rw-r--r--   0        0        0     2761 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_as_route_part_label.py
--rw-r--r--   0        0        0     2724 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_by_id_id.py
--rw-r--r--   0        0        0     2727 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_details_id.py
--rw-r--r--   0        0        0     2615 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_labels.py
--rw-r--r--   0        0        0     2544 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/post_outlet.py
--rw-r--r--   0        0        0     2724 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/put_outlet_by_id_id.py
--rw-r--r--   0        0        0     2999 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/put_outlet_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/place/__init__.py
--rw-r--r--   0        0        0     2723 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_by_id_id.py
--rw-r--r--   0        0        0     3348 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_close_place.py
--rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_operational_places.py
--rw-r--r--   0        0        0     2638 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_with_displayable_producing_places.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/__init__.py
--rw-r--r--   0        0        0     3117 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/delete_producer_unlink_producer_with_producing_place_id_producer_id_producing_place.py
--rw-r--r--   0        0        0     2614 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_all.py
--rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_by_id_id.py
--rw-r--r--   0        0        0     2740 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_by_producing_place_id_id.py
--rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_filter_options.py
--rw-r--r--   0        0        0     2734 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_history_by_id_id.py
--rw-r--r--   0        0        0     2627 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_with_active_event.py
--rw-r--r--   0        0        0     3046 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_delete_many.py
--rw-r--r--   0        0        0     3124 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_id_uni_and_co_user.py
--rw-r--r--   0        0        0     2549 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_new.py
--rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/put_producer_by_id_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/__init__.py
--rw-r--r--   0        0        0     2738 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/delete_producing_place_anomaly_id.py
--rw-r--r--   0        0        0     2732 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_by_id_id.py
--rw-r--r--   0        0        0     2740 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_by_id_producer_id.py
--rw-r--r--   0        0        0     3612 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_collectable_element_rounds_in_interval.py
--rw-r--r--   0        0        0     2849 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_collection_planning_excel_by_id_producing_place_id.py
--rw-r--r--   0        0        0     2740 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_custom_fields_id.py
--rw-r--r--   0        0        0     2630 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_filter_options.py
--rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_filtered.py
--rw-r--r--   0        0        0     2740 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_history_by_id_id.py
--rw-r--r--   0        0        0     2751 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_id_trackdechets_info_company.py
--rw-r--r--   0        0        0     2896 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_producing_place_id_schedule.py
--rw-r--r--   0        0        0     2835 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_producing_place_id_waste_register.py
--rw-r--r--   0        0        0     2632 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_with_active_event.py
--rw-r--r--   0        0        0     3070 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_by_serial_numbers.py
--rw-r--r--   0        0        0     3095 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_delete_many.py
--rw-r--r--   0        0        0     3201 2024-05-15 07:41:29.481862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_distinct_by_containers_ids.py
--rw-r--r--   0        0        0     2644 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_distinct_ids_by_containers_ids.py
--rw-r--r--   0        0        0     2621 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_new.py
--rw-r--r--   0        0        0     3218 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_unique_stream_containers_total_by_ids.py
--rw-r--r--   0        0        0     3244 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_id_update_trackdechets_info.py
--rw-r--r--   0        0        0     2732 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_info_id.py
--rw-r--r--   0        0        0     3061 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_linked_producers.py
--rw-r--r--   0        0        0     2733 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_place_id.py
--rw-r--r--   0        0        0     2830 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_producing_place_id_schedule.py
--rw-r--r--   0        0        0     3122 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_sectors_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/__init__.py
--rw-r--r--   0        0        0     2740 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/delete_producing_place_definition_id.py
--rw-r--r--   0        0        0     2627 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/get_producing_place_definition.py
--rw-r--r--   0        0        0     2737 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/get_producing_place_definition_id.py
--rw-r--r--   0        0        0     2562 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/post_producing_place_definition.py
--rw-r--r--   0        0        0     2671 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/put_producing_place_definition_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/__init__.py
--rw-r--r--   0        0        0     2747 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/delete_realisation_round_outlet_realised_id.py
--rw-r--r--   0        0        0     2734 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_by_id_id.py
--rw-r--r--   0        0        0     3473 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_collect_report_by_id.py
--rw-r--r--   0        0        0     2750 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_container_collect_by_id_id.py
--rw-r--r--   0        0        0     2865 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_external_history_id_realisation.py
--rw-r--r--   0        0        0     2867 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_external_itinerary_id_realisation.py
--rw-r--r--   0        0        0     2632 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_filter_options.py
--rw-r--r--   0        0        0     2737 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_history_id.py
--rw-r--r--   0        0        0     2744 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_outlet_realised_id.py
--rw-r--r--   0        0        0     2747 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_planned_vs_realised_id.py
--rw-r--r--   0        0        0     2748 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_proof_of_passage_by_id_id.py
--rw-r--r--   0        0        0     3086 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_related_external_realisation_vehicle_id_realisation_date.py
--rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_stats.py
--rw-r--r--   0        0        0     3111 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/post_realisation_round_delete_many.py
--rw-r--r--   0        0        0     3077 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/post_realisation_round_outlet_realised.py
--rw-r--r--   0        0        0     2678 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_outlet_realised_id.py
--rw-r--r--   0        0        0     3341 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_proof_of_passage_id_ppra.py
--rw-r--r--   0        0        0     2690 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_update_container_collect_by_id_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/rotation_history/__init__.py
--rw-r--r--   0        0        0     3509 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/rotation_history/get_rotation_history.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/__init__.py
--rw-r--r--   0        0        0     2781 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/delete_round_id_round.py
--rw-r--r--   0        0        0     3392 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/delete_round_occurrence.py
--rw-r--r--   0        0        0     2970 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_availability_id_itinerary_date.py
--rw-r--r--   0        0        0     2837 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_planified_id_itinerary.py
--rw-r--r--   0        0        0     2836 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_realised_id_itinerary.py
--rw-r--r--   0        0        0     3709 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_track_id_geo_json_vehicle_profile.py
--rw-r--r--   0        0        0     3705 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_track_id_shp_vehicle_profile.py
--rw-r--r--   0        0        0     3393 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_occurrence_by_id.py
--rw-r--r--   0        0        0     3400 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_occurrence_details_by_id.py
--rw-r--r--   0        0        0     3474 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_route_parts_itinerary_id_geo_json.py
--rw-r--r--   0        0        0     3470 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_route_parts_itinerary_id_shp.py
--rw-r--r--   0        0        0     2546 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_team.py
--rw-r--r--   0        0        0     2695 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_itineraries_route_parts_type.py
--rw-r--r--   0        0        0     2685 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_itineraries_type.py
--rw-r--r--   0        0        0     2546 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_new.py
--rw-r--r--   0        0        0     2923 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_tracks.py
--rw-r--r--   0        0        0     2865 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round.py
--rw-r--r--   0        0        0     2947 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round_occurrence.py
--rw-r--r--   0        0        0     3170 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round_round_slots_id_round.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/route_parts/__init__.py
--rw-r--r--   0        0        0     3029 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/route_parts/post_route_parts_availabilities.py
--rw-r--r--   0        0        0     3104 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/route_parts/post_route_parts_producing_place_in_polygon.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/sector/__init__.py
--rw-r--r--   0        0        0     2727 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/sector/delete_sector_by_id_id.py
--rw-r--r--   0        0        0     2612 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/sector/get_sector_all.py
--rw-r--r--   0        0        0     2973 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/sector/post_sector_new.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/segment/__init__.py
--rw-r--r--   0        0        0     2725 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/segment/get_segment_by_id_id.py
--rw-r--r--   0        0        0     2623 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/segment/get_segment_filter_options.py
--rw-r--r--   0        0        0     2614 2024-05-15 07:41:29.485862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/segment/post_segment_all.py
--rw-r--r--   0        0        0     2636 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/segment/post_segment_territory_vehicle_profiles.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/stream/__init__.py
--rw-r--r--   0        0        0     2609 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/stream/get_stream.py
--rw-r--r--   0        0        0     2615 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/stream/get_stream_labels.py
--rw-r--r--   0        0        0     2907 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/stream/post_stream_new.py
--rw-r--r--   0        0        0     3034 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/stream/put_stream_by_id_id.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/street_service/__init__.py
--rw-r--r--   0        0        0     2567 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/street_service/post_street_service_compute_itinerary.py
--rw-r--r--   0        0        0     3427 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/street_service/put_street_service_transpose_realisation_id_realisation.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/__init__.py
--rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/get_unibac_current_user_info.py
--rw-r--r--   0        0        0     2989 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_login.py
--rw-r--r--   0        0        0     3054 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_reset_password.py
--rw-r--r--   0        0        0     2915 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_scan.py
--rw-r--r--   0        0        0     3054 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/put_unibac_change_password.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/__init__.py
--rw-r--r--   0        0        0     2638 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_container_sheet_params.py
--rw-r--r--   0        0        0     2632 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_logistic_params.py
--rw-r--r--   0        0        0     2639 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_operational_tabs_params.py
--rw-r--r--   0        0        0     2633 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_pdf_export_params.py
--rw-r--r--   0        0        0     2572 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_container_sheet_param.py
--rw-r--r--   0        0        0     3111 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_logistic_params_column.py
--rw-r--r--   0        0        0     2570 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_logistic_params_tab.py
--rw-r--r--   0        0        0     3118 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_operational_tabs_params.py
--rw-r--r--   0        0        0     3070 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_pdf_export_params.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/__init__.py
--rw-r--r--   0        0        0     2610 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle.py
--rw-r--r--   0        0        0     2631 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_environmental_criteria.py
--rw-r--r--   0        0        0     2623 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_filter_options.py
--rw-r--r--   0        0        0     2813 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_history_by_id_vehicle_id.py
--rw-r--r--   0        0        0     2809 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_info_by_id_vehicle_id.py
--rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_labels.py
--rw-r--r--   0        0        0     2623 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_labels_profile.py
--rw-r--r--   0        0        0     2622 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_loading_types.py
--rw-r--r--   0        0        0     2630 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_vehicle_profile_labels.py
--rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_vehicle_profiles.py
--rw-r--r--   0        0        0     3094 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_environmental_criterion_new.py
--rw-r--r--   0        0        0     3006 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_loading_type_new.py
--rw-r--r--   0        0        0     2548 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_new.py
--rw-r--r--   0        0        0     3030 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_vehicle_profile_new.py
--rw-r--r--   0        0        0     2972 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_archive_many.py
--rw-r--r--   0        0        0     3195 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_archive_vehicle_id.py
--rw-r--r--   0        0        0     2739 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_by_id_vehicle_id.py
--rw-r--r--   0        0        0     3110 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_environmental_criterion_update.py
--rw-r--r--   0        0        0     3022 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_loading_type_update.py
--rw-r--r--   0        0        0     3178 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_sectors_sector_id.py
--rw-r--r--   0        0        0     3046 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_vehicle_profile_update.py
--rw-r--r--   0        0        0        0 2024-05-15 12:37:40.841642 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/__init__.py
--rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/delete_waste_codes_id.py
--rw-r--r--   0        0        0     2613 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/get_waste_codes.py
--rw-r--r--   0        0        0     2548 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/post_waste_codes.py
--rw-r--r--   0        0        0     2657 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/put_waste_codes_id.py
--rw-r--r--   0        0        0    12417 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/client.py
--rw-r--r--   0        0        0      546 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/errors.py
--rw-r--r--   0        0        0     9568 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/__init__.py
--rw-r--r--   0        0        0     2133 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/changelog_response.py
--rw-r--r--   0        0        0     1963 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/client_response.py
--rw-r--r--   0        0        0     1930 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/current_user_response.py
--rw-r--r--   0        0        0     2396 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/login_choose_response.py
--rw-r--r--   0        0        0     1680 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/login_choose_response_clients_item.py
--rw-r--r--   0        0        0      174 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/login_choose_response_type.py
--rw-r--r--   0        0        0     2017 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/login_payload.py
--rw-r--r--   0        0        0     1833 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/login_token_response.py
--rw-r--r--   0        0        0      155 2024-05-15 07:41:29.489862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/login_token_response_type.py
--rw-r--r--   0        0        0     1603 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_auth_register_body.py
--rw-r--r--   0        0        0     1642 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_auth_reset_password_body.py
--rw-r--r--   0        0        0     2207 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_back_office_event_definition_email_subscription_body.py
--rw-r--r--   0        0        0     1602 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_comment_new_body.py
--rw-r--r--   0        0        0     1597 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_container_delete_many_body.py
--rw-r--r--   0        0        0     2632 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_container_new_many_body.py
--rw-r--r--   0        0        0     1543 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_custom_field_body.py
--rw-r--r--   0        0        0     1900 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_custom_field_option_id_custom_field_body.py
--rw-r--r--   0        0        0     1616 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_device_live_data_update_body.py
--rw-r--r--   0        0        0     1688 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_device_map_corrections_body.py
--rw-r--r--   0        0        0     2011 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_device_submit_check_in_body.py
--rw-r--r--   0        0        0     1712 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_error_report_device_crash_report_body.py
--rw-r--r--   0        0        0     1938 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_event_definition_category_new_body.py
--rw-r--r--   0        0        0     3398 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_event_definition_new_body.py
--rw-r--r--   0        0        0     1577 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_event_delete_many_body.py
--rw-r--r--   0        0        0     2156 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_external_button_collect_request_body.py
--rw-r--r--   0        0        0     1814 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_external_create_ifm_itinerary_id_realisation_body.py
--rw-r--r--   0        0        0     1631 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_external_live_vehicle_data_body.py
--rw-r--r--   0        0        0     2612 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_operational_layers_data_source_body.py
--rw-r--r--   0        0        0     1592 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producer_delete_many_body.py
--rw-r--r--   0        0        0     1643 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producer_id_uni_and_co_user_body.py
--rw-r--r--   0        0        0     2097 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_by_serial_numbers_body.py
--rw-r--r--   0        0        0     1625 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_delete_many_body.py
--rw-r--r--   0        0        0     2400 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_distinct_by_containers_ids_body.py
--rw-r--r--   0        0        0     2244 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_unique_stream_containers_total_by_ids_body.py
--rw-r--r--   0        0        0     1635 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_realisation_round_delete_many_body.py
--rw-r--r--   0        0        0     2130 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_realisation_round_outlet_realised_body.py
--rw-r--r--   0        0        0     1554 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_round_tracks_body.py
--rw-r--r--   0        0        0     2033 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_route_parts_availabilities_body.py
--rw-r--r--   0        0        0     2067 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_route_parts_producing_place_in_polygon_body.py
--rw-r--r--   0        0        0     1566 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_sector_new_body.py
--rw-r--r--   0        0        0     3103 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_stream_new_body.py
--rw-r--r--   0        0        0     1892 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_login_body.py
--rw-r--r--   0        0        0     1652 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_reset_password_body.py
--rw-r--r--   0        0        0     1810 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_scan_body.py
--rw-r--r--   0        0        0     1687 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_environmental_criterion_new_body.py
--rw-r--r--   0        0        0     1632 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_loading_type_new_body.py
--rw-r--r--   0        0        0     4414 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_vehicle_profile_new_body.py
--rw-r--r--   0        0        0     2487 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_auth_by_id_id_body.py
--rw-r--r--   0        0        0     1967 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_auth_change_password_body.py
--rw-r--r--   0        0        0     1985 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_calendar_settings_body.py
--rw-r--r--   0        0        0     1977 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_client_default_speed_on_segment_km_h_body.py
--rw-r--r--   0        0        0     1771 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_client_mapbox_body.py
--rw-r--r--   0        0        0     1743 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_client_show_deadheading_body.py
--rw-r--r--   0        0        0     1609 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_comment_by_id_id_body.py
--rw-r--r--   0        0        0     1919 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_constraint_body.py
--rw-r--r--   0        0        0     1658 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_container_update_state_by_id_id_body.py
--rw-r--r--   0        0        0     1615 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_employee_archive_id_body.py
--rw-r--r--   0        0        0     1592 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_employee_archive_many_body.py
--rw-r--r--   0        0        0     2185 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_employee_id_constraint_body.py
--rw-r--r--   0        0        0     1683 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_employee_sectors_id_body.py
--rw-r--r--   0        0        0     4636 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_event_definition_by_id_id_body.py
--rw-r--r--   0        0        0     1954 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_event_definition_category_by_id_id_body.py
--rw-r--r--   0        0        0     1636 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_intervention_id_planned_date_body.py
--rw-r--r--   0        0        0     1914 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_outlet_id_body.py
--rw-r--r--   0        0        0     3315 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_id_update_trackdechets_info_body.py
--rw-r--r--   0        0        0     2131 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_linked_producers_body.py
--rw-r--r--   0        0        0     1716 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_sectors_id_body.py
--rw-r--r--   0        0        0     2363 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_realisation_round_proof_of_passage_id_ppra_body.py
--rw-r--r--   0        0        0     1569 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_round_body.py
--rw-r--r--   0        0        0     1960 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_round_occurrence_body.py
--rw-r--r--   0        0        0     2079 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_round_round_slots_id_round_body.py
--rw-r--r--   0        0        0     3119 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_stream_by_id_id_body.py
--rw-r--r--   0        0        0     1926 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_street_service_transpose_realisation_id_realisation_body.py
--rw-r--r--   0        0        0     1977 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_unibac_change_password_body.py
--rw-r--r--   0        0        0     2045 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_logistic_params_column_body.py
--rw-r--r--   0        0        0     2335 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_operational_tabs_params_body.py
--rw-r--r--   0        0        0     2172 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_pdf_export_params_body.py
--rw-r--r--   0        0        0     1587 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_archive_many_body.py
--rw-r--r--   0        0        0     1648 2024-05-15 07:41:29.493862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_archive_vehicle_id_body.py
--rw-r--r--   0        0        0     1914 2024-05-15 07:41:29.497862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_environmental_criterion_update_body.py
--rw-r--r--   0        0        0     1859 2024-05-15 07:41:29.497862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_loading_type_update_body.py
--rw-r--r--   0        0        0     1711 2024-05-15 07:41:29.497862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_sectors_sector_id_body.py
--rw-r--r--   0        0        0     4641 2024-05-15 07:41:29.497862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_vehicle_profile_update_body.py
--rw-r--r--   0        0        0       25 2024-05-15 07:41:29.497862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/py.typed
--rw-r--r--   0        0        0      985 2024-05-15 07:41:29.497862 unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/types.py
--rw-r--r--   0        0        0     2309 2024-05-15 07:41:29.497862 unico_device_setuper-0.5.0/unico_device_setuper/lib/utils.py
--rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 unico_device_setuper-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/README.md
+-rw-r--r--   0        0        0     5084 2024-05-15 14:31:19.734485 unico_device_setuper-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-15 14:31:19.734485 unico_device_setuper-0.6.0/unico_device_setuper/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/cli/__init__.py
+-rw-r--r--   0        0        0     2191 2024-05-15 14:28:55.974128 unico_device_setuper-0.6.0/unico_device_setuper/cli/main.py
+-rw-r--r--   0        0        0     6102 2024-05-15 14:28:55.974128 unico_device_setuper-0.6.0/unico_device_setuper/cli/pkg.py
+-rw-r--r--   0        0        0     1632 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/cli/stp.py
+-rw-r--r--   0        0        0     1120 2024-05-15 12:52:44.596069 unico_device_setuper-0.6.0/unico_device_setuper/cli/unav.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/__init__.py
+-rw-r--r--   0        0        0     1354 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/aapt.py
+-rw-r--r--   0        0        0     1949 2024-05-15 12:52:44.596069 unico_device_setuper-0.6.0/unico_device_setuper/lib/adb.py
+-rw-r--r--   0        0        0     2951 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/auth.py
+-rw-r--r--   0        0        0     2013 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/cnsl.py
+-rw-r--r--   0        0        0      822 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/datadir.py
+-rw-r--r--   0        0        0     2834 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/dl.py
+-rw-r--r--   0        0        0    35108 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/__init__.py
+-rw-r--r--   0        0        0       45 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/__init__.py
+-rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/delete_attachment_id.py
+-rw-r--r--   0        0        0     2732 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_data_by_id_id.py
+-rw-r--r--   0        0        0     2795 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_event_images_id_event.py
+-rw-r--r--   0        0        0     2869 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_info_by_foreign_id_mode_id.py
+-rw-r--r--   0        0        0     2732 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_info_by_id_id.py
+-rw-r--r--   0        0        0     2904 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_producing_place_images_id_producing_place.py
+-rw-r--r--   0        0        0     2614 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/post_attachment.py
+-rw-r--r--   0        0        0     2933 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/put_attachment_is_visible_in_uni_and_co_id_is_visible.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/__init__.py
+-rw-r--r--   0        0        0     2720 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/delete_auth_id.py
+-rw-r--r--   0        0        0     2725 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/delete_auth_user_id.py
+-rw-r--r--   0        0        0     2607 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth.py
+-rw-r--r--   0        0        0     4107 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth_current_user_info.py
+-rw-r--r--   0        0        0     3338 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth_device_login.py
+-rw-r--r--   0        0        0     5755 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_login.py
+-rw-r--r--   0        0        0     2931 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_register.py
+-rw-r--r--   0        0        0     3038 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_reset_password.py
+-rw-r--r--   0        0        0     3084 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/put_auth_by_id_id.py
+-rw-r--r--   0        0        0     3038 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/put_auth_change_password.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/back_office/__init__.py
+-rw-r--r--   0        0        0     2649 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/back_office/get_back_office_event_definition_email_subscription_all.py
+-rw-r--r--   0        0        0     3184 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/back_office/post_back_office_event_definition_email_subscription.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/calendar/__init__.py
+-rw-r--r--   0        0        0     3824 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/calendar/get_calendar_calendar_occurrences.py
+-rw-r--r--   0        0        0     2956 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/calendar/put_calendar_settings.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/cartography/__init__.py
+-rw-r--r--   0        0        0     2628 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/cartography/get_cartography_map_corrections.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/__init__.py
+-rw-r--r--   0        0        0     4301 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/get_client.py
+-rw-r--r--   0        0        0     2633 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_default_speed_on_segment_km_h.py
+-rw-r--r--   0        0        0     2627 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_filling_rate_setting.py
+-rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_show_deadheading.py
+-rw-r--r--   0        0        0     2563 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/post_client_filling_rate_setting.py
+-rw-r--r--   0        0        0     2755 2024-05-15 07:41:29.469862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_color_color.py
+-rw-r--r--   0        0        0     3073 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_default_speed_on_segment_km_h.py
+-rw-r--r--   0        0        0     2990 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_mapbox.py
+-rw-r--r--   0        0        0     3063 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_show_deadheading.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/comment/__init__.py
+-rw-r--r--   0        0        0     2728 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/comment/delete_comment_by_id_id.py
+-rw-r--r--   0        0        0     2790 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/comment/get_comment_by_event_id_id_event.py
+-rw-r--r--   0        0        0     2981 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/comment/post_comment_new.py
+-rw-r--r--   0        0        0     3108 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/comment/put_comment_by_id_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/constraint/__init__.py
+-rw-r--r--   0        0        0     2657 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/constraint/get_constraint_id.py
+-rw-r--r--   0        0        0     2906 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/constraint/put_constraint.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/__init__.py
+-rw-r--r--   0        0        0     2730 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/delete_container_by_id_id.py
+-rw-r--r--   0        0        0     2612 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container.py
+-rw-r--r--   0        0        0     2626 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_all_definitions.py
+-rw-r--r--   0        0        0     2628 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_all_serial_numbers.py
+-rw-r--r--   0        0        0     2727 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_id_id.py
+-rw-r--r--   0        0        0     2901 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_id_producing_place_id_producing_place.py
+-rw-r--r--   0        0        0     2847 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_serial_number_serial_number.py
+-rw-r--r--   0        0        0     2637 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_containers_with_active_event.py
+-rw-r--r--   0        0        0     2735 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_custom_fields_id.py
+-rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_filter_options.py
+-rw-r--r--   0        0        0     2620 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_filtered.py
+-rw-r--r--   0        0        0     2735 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_history_by_id_id.py
+-rw-r--r--   0        0        0     3054 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_delete_many.py
+-rw-r--r--   0        0        0     2618 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_in_ids.py
+-rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_new.py
+-rw-r--r--   0        0        0     2964 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_new_many.py
+-rw-r--r--   0        0        0     2727 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/put_container_by_id_id.py
+-rw-r--r--   0        0        0     3214 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/put_container_update_state_by_id_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container_definition/__init__.py
+-rw-r--r--   0        0        0     2622 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container_definition/get_container_definition.py
+-rw-r--r--   0        0        0     2560 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container_definition/post_container_definition_new.py
+-rw-r--r--   0        0        0     2671 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container_definition/put_container_definition_by_id_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/__init__.py
+-rw-r--r--   0        0        0     2727 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/delete_custom_field_id.py
+-rw-r--r--   0        0        0     2804 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/delete_custom_field_option_id_option.py
+-rw-r--r--   0        0        0     2769 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/get_custom_field_many_target.py
+-rw-r--r--   0        0        0     2923 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/post_custom_field.py
+-rw-r--r--   0        0        0     3307 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/post_custom_field_option_id_custom_field.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/dashboard/__init__.py
+-rw-r--r--   0        0        0     3290 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/dashboard/get_dashboard_stats.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/__init__.py
+-rw-r--r--   0        0        0     2608 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot.py
+-rw-r--r--   0        0        0     2734 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_as_route_part_by_id_id.py
+-rw-r--r--   0        0        0     2760 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_as_route_part_label.py
+-rw-r--r--   0        0        0     2723 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_by_id_id.py
+-rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_details_id.py
+-rw-r--r--   0        0        0     2614 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_labels.py
+-rw-r--r--   0        0        0     2543 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/post_depot.py
+-rw-r--r--   0        0        0     2723 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/put_depot_by_id_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/__init__.py
+-rw-r--r--   0        0        0     2728 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/delete_device_event_id.py
+-rw-r--r--   0        0        0     2730 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_attachment_id.py
+-rw-r--r--   0        0        0     2620 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_check_in_form.py
+-rw-r--r--   0        0        0     2549 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_client.py
+-rw-r--r--   0        0        0     2902 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_client_dasri_allow_taken_producing_place_id.py
+-rw-r--r--   0        0        0     2854 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_container_by_serial_number_serial_number.py
+-rw-r--r--   0        0        0     2629 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_container_definitions.py
+-rw-r--r--   0        0        0     2749 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_containers_by_producing_place_id_id.py
+-rw-r--r--   0        0        0     2615 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_depots.py
+-rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_drivers.py
+-rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_event_definitions.py
+-rw-r--r--   0        0        0     2635 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_event_definitions_categories.py
+-rw-r--r--   0        0        0     3467 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_itinerary_id.py
+-rw-r--r--   0        0        0     2623 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_map_corrections.py
+-rw-r--r--   0        0        0     3503 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_near_by_producing_place.py
+-rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_outlets.py
+-rw-r--r--   0        0        0     2623 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_poi_definitions.py
+-rw-r--r--   0        0        0     2874 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_pois_id_poi_definition.py
+-rw-r--r--   0        0        0     3274 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_round_id_itinerary.py
+-rw-r--r--   0        0        0     3060 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_rounds_meta.py
+-rw-r--r--   0        0        0     3466 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_search_producing_place.py
+-rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.473862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_streams.py
+-rw-r--r--   0        0        0     4082 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_update_change_log.py
+-rw-r--r--   0        0        0     3470 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_v2_itinerary_id.py
+-rw-r--r--   0        0        0     3506 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_v_2_near_by_producing_place.py
+-rw-r--r--   0        0        0     2617 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_vehicles.py
+-rw-r--r--   0        0        0     2556 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_bsd_sign_many.py
+-rw-r--r--   0        0        0     2559 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_dasri_sign_many.py
+-rw-r--r--   0        0        0     2997 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_live_data_update.py
+-rw-r--r--   0        0        0     2996 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_map_corrections.py
+-rw-r--r--   0        0        0     2989 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_submit_check_in.py
+-rw-r--r--   0        0        0     2557 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_v2_bsd_create.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/driver/__init__.py
+-rw-r--r--   0        0        0     2609 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/driver/get_driver.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/__init__.py
+-rw-r--r--   0        0        0     2611 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee.py
+-rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_by_id_id.py
+-rw-r--r--   0        0        0     2820 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_employee_id_schedule.py
+-rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_filter_options.py
+-rw-r--r--   0        0        0     2666 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_id_constraint.py
+-rw-r--r--   0        0        0     2549 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/post_employee_new.py
+-rw-r--r--   0        0        0     3073 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_archive_id.py
+-rw-r--r--   0        0        0     2980 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_archive_many.py
+-rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_by_id_id.py
+-rw-r--r--   0        0        0     2754 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_employee_id_schedule.py
+-rw-r--r--   0        0        0     3097 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_id_constraint.py
+-rw-r--r--   0        0        0     3073 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_sectors_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/error_report/__init__.py
+-rw-r--r--   0        0        0     3062 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/error_report/post_error_report_device_crash_report.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.279192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/__init__.py
+-rw-r--r--   0        0        0     2548 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_active.py
+-rw-r--r--   0        0        0     2551 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_all_active.py
+-rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_all_unique_authors.py
+-rw-r--r--   0        0        0     2723 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_by_id_id.py
+-rw-r--r--   0        0        0     2924 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_count_by_id_round_realisation_id_round_realisation.py
+-rw-r--r--   0        0        0     2619 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_count_by_type.py
+-rw-r--r--   0        0        0     2615 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_def_all.py
+-rw-r--r--   0        0        0     2749 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_def_by_type_type.py
+-rw-r--r--   0        0        0     2731 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_detailed_by_id_id.py
+-rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_displayable_events.py
+-rw-r--r--   0        0        0     2621 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_filter_options.py
+-rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_filtered.py
+-rw-r--r--   0        0        0     2551 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_to_planify.py
+-rw-r--r--   0        0        0     3022 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/post_event_delete_many.py
+-rw-r--r--   0        0        0     2612 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/post_event_new.py
+-rw-r--r--   0        0        0     2664 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/put_event_update_by_id_id.py
+-rw-r--r--   0        0        0     2871 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/put_event_update_state_id_state.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition/__init__.py
+-rw-r--r--   0        0        0     2618 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition/get_event_definition.py
+-rw-r--r--   0        0        0     2980 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition/post_event_definition_new.py
+-rw-r--r--   0        0        0     3107 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition/put_event_definition_by_id_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/__init__.py
+-rw-r--r--   0        0        0     2626 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/get_event_definition_category.py
+-rw-r--r--   0        0        0     3045 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/post_event_definition_category_new.py
+-rw-r--r--   0        0        0     3172 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/put_event_definition_category_by_id_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/export_client/__init__.py
+-rw-r--r--   0        0        0     2860 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/export_client/get_export_client_reference_type.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/__init__.py
+-rw-r--r--   0        0        0     2635 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_alpes_mesure_filling_rate.py
+-rw-r--r--   0        0        0     3127 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_button_collect_request.py
+-rw-r--r--   0        0        0     3378 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_create_ifm_itinerary_id_realisation.py
+-rw-r--r--   0        0        0     2838 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_elise_work_orders_id_franchise.py
+-rw-r--r--   0        0        0     3021 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_live_vehicle_data.py
+-rw-r--r--   0        0        0     2717 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_v2_live_vehicle_data.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/icons/__init__.py
+-rw-r--r--   0        0        0     2929 2024-05-15 07:41:29.477862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/icons/get_icons.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/intervention/__init__.py
+-rw-r--r--   0        0        0     2725 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/intervention/get_intervention_id.py
+-rw-r--r--   0        0        0     2945 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/intervention/get_intervention_to_planify.py
+-rw-r--r--   0        0        0     3138 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/intervention/put_intervention_id_planned_date.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/logistic/__init__.py
+-rw-r--r--   0        0        0     2552 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_as_pois.py
+-rw-r--r--   0        0        0     2553 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_by_batch.py
+-rw-r--r--   0        0        0     2552 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_export.py
+-rw-r--r--   0        0        0     2556 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_total_count.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/mapbox/__init__.py
+-rw-r--r--   0        0        0     2609 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/mapbox/get_mapbox.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/message/__init__.py
+-rw-r--r--   0        0        0     2548 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/message/post_message_new.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/occurrence/__init__.py
+-rw-r--r--   0        0        0     3648 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_export_collect_points.py
+-rw-r--r--   0        0        0     3551 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_in_interval.py
+-rw-r--r--   0        0        0     3393 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_team_by_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operational/__init__.py
+-rw-r--r--   0        0        0     2628 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operational/get_operational_filter_options.py
+-rw-r--r--   0        0        0     3053 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operational/post_operational_layers_data_source.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operator/__init__.py
+-rw-r--r--   0        0        0     2611 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator.py
+-rw-r--r--   0        0        0     2736 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator_by_id_ids.py
+-rw-r--r--   0        0        0     2734 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator_history_by_id_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/__init__.py
+-rw-r--r--   0        0        0     2609 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet.py
+-rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_all_as_route_parts.py
+-rw-r--r--   0        0        0     2735 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_as_route_part_by_id_id.py
+-rw-r--r--   0        0        0     2761 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_as_route_part_label.py
+-rw-r--r--   0        0        0     2724 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_by_id_id.py
+-rw-r--r--   0        0        0     2727 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_details_id.py
+-rw-r--r--   0        0        0     2615 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_labels.py
+-rw-r--r--   0        0        0     2544 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/post_outlet.py
+-rw-r--r--   0        0        0     2724 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/put_outlet_by_id_id.py
+-rw-r--r--   0        0        0     2999 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/put_outlet_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/place/__init__.py
+-rw-r--r--   0        0        0     2723 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_by_id_id.py
+-rw-r--r--   0        0        0     3348 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_close_place.py
+-rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_operational_places.py
+-rw-r--r--   0        0        0     2638 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_with_displayable_producing_places.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/__init__.py
+-rw-r--r--   0        0        0     3117 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/delete_producer_unlink_producer_with_producing_place_id_producer_id_producing_place.py
+-rw-r--r--   0        0        0     2614 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_all.py
+-rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_by_id_id.py
+-rw-r--r--   0        0        0     2740 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_by_producing_place_id_id.py
+-rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_filter_options.py
+-rw-r--r--   0        0        0     2734 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_history_by_id_id.py
+-rw-r--r--   0        0        0     2627 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_with_active_event.py
+-rw-r--r--   0        0        0     3046 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_delete_many.py
+-rw-r--r--   0        0        0     3124 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_id_uni_and_co_user.py
+-rw-r--r--   0        0        0     2549 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_new.py
+-rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/put_producer_by_id_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/__init__.py
+-rw-r--r--   0        0        0     2738 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/delete_producing_place_anomaly_id.py
+-rw-r--r--   0        0        0     2732 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_by_id_id.py
+-rw-r--r--   0        0        0     2740 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_by_id_producer_id.py
+-rw-r--r--   0        0        0     3612 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_collectable_element_rounds_in_interval.py
+-rw-r--r--   0        0        0     2849 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_collection_planning_excel_by_id_producing_place_id.py
+-rw-r--r--   0        0        0     2740 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_custom_fields_id.py
+-rw-r--r--   0        0        0     2630 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_filter_options.py
+-rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_filtered.py
+-rw-r--r--   0        0        0     2740 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_history_by_id_id.py
+-rw-r--r--   0        0        0     2751 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_id_trackdechets_info_company.py
+-rw-r--r--   0        0        0     2896 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_producing_place_id_schedule.py
+-rw-r--r--   0        0        0     2835 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_producing_place_id_waste_register.py
+-rw-r--r--   0        0        0     2632 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_with_active_event.py
+-rw-r--r--   0        0        0     3070 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_by_serial_numbers.py
+-rw-r--r--   0        0        0     3095 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_delete_many.py
+-rw-r--r--   0        0        0     3201 2024-05-15 07:41:29.481862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_distinct_by_containers_ids.py
+-rw-r--r--   0        0        0     2644 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_distinct_ids_by_containers_ids.py
+-rw-r--r--   0        0        0     2621 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_new.py
+-rw-r--r--   0        0        0     3218 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_unique_stream_containers_total_by_ids.py
+-rw-r--r--   0        0        0     3244 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_id_update_trackdechets_info.py
+-rw-r--r--   0        0        0     2732 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_info_id.py
+-rw-r--r--   0        0        0     3061 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_linked_producers.py
+-rw-r--r--   0        0        0     2733 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_place_id.py
+-rw-r--r--   0        0        0     2830 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_producing_place_id_schedule.py
+-rw-r--r--   0        0        0     3122 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_sectors_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/__init__.py
+-rw-r--r--   0        0        0     2740 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/delete_producing_place_definition_id.py
+-rw-r--r--   0        0        0     2627 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/get_producing_place_definition.py
+-rw-r--r--   0        0        0     2737 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/get_producing_place_definition_id.py
+-rw-r--r--   0        0        0     2562 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/post_producing_place_definition.py
+-rw-r--r--   0        0        0     2671 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/put_producing_place_definition_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/__init__.py
+-rw-r--r--   0        0        0     2747 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/delete_realisation_round_outlet_realised_id.py
+-rw-r--r--   0        0        0     2734 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_by_id_id.py
+-rw-r--r--   0        0        0     3473 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_collect_report_by_id.py
+-rw-r--r--   0        0        0     2750 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_container_collect_by_id_id.py
+-rw-r--r--   0        0        0     2865 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_external_history_id_realisation.py
+-rw-r--r--   0        0        0     2867 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_external_itinerary_id_realisation.py
+-rw-r--r--   0        0        0     2632 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_filter_options.py
+-rw-r--r--   0        0        0     2737 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_history_id.py
+-rw-r--r--   0        0        0     2744 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_outlet_realised_id.py
+-rw-r--r--   0        0        0     2747 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_planned_vs_realised_id.py
+-rw-r--r--   0        0        0     2748 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_proof_of_passage_by_id_id.py
+-rw-r--r--   0        0        0     3086 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_related_external_realisation_vehicle_id_realisation_date.py
+-rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_stats.py
+-rw-r--r--   0        0        0     3111 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/post_realisation_round_delete_many.py
+-rw-r--r--   0        0        0     3077 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/post_realisation_round_outlet_realised.py
+-rw-r--r--   0        0        0     2678 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_outlet_realised_id.py
+-rw-r--r--   0        0        0     3341 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_proof_of_passage_id_ppra.py
+-rw-r--r--   0        0        0     2690 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_update_container_collect_by_id_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/rotation_history/__init__.py
+-rw-r--r--   0        0        0     3509 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/rotation_history/get_rotation_history.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/__init__.py
+-rw-r--r--   0        0        0     2781 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/delete_round_id_round.py
+-rw-r--r--   0        0        0     3392 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/delete_round_occurrence.py
+-rw-r--r--   0        0        0     2970 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_availability_id_itinerary_date.py
+-rw-r--r--   0        0        0     2837 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_planified_id_itinerary.py
+-rw-r--r--   0        0        0     2836 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_realised_id_itinerary.py
+-rw-r--r--   0        0        0     3709 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_track_id_geo_json_vehicle_profile.py
+-rw-r--r--   0        0        0     3705 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_track_id_shp_vehicle_profile.py
+-rw-r--r--   0        0        0     3393 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_occurrence_by_id.py
+-rw-r--r--   0        0        0     3400 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_occurrence_details_by_id.py
+-rw-r--r--   0        0        0     3474 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_route_parts_itinerary_id_geo_json.py
+-rw-r--r--   0        0        0     3470 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_route_parts_itinerary_id_shp.py
+-rw-r--r--   0        0        0     2546 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_team.py
+-rw-r--r--   0        0        0     2695 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_itineraries_route_parts_type.py
+-rw-r--r--   0        0        0     2685 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_itineraries_type.py
+-rw-r--r--   0        0        0     2546 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_new.py
+-rw-r--r--   0        0        0     2923 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_tracks.py
+-rw-r--r--   0        0        0     2865 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round.py
+-rw-r--r--   0        0        0     2947 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round_occurrence.py
+-rw-r--r--   0        0        0     3170 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round_round_slots_id_round.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/route_parts/__init__.py
+-rw-r--r--   0        0        0     3029 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/route_parts/post_route_parts_availabilities.py
+-rw-r--r--   0        0        0     3104 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/route_parts/post_route_parts_producing_place_in_polygon.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/sector/__init__.py
+-rw-r--r--   0        0        0     2727 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/sector/delete_sector_by_id_id.py
+-rw-r--r--   0        0        0     2612 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/sector/get_sector_all.py
+-rw-r--r--   0        0        0     2973 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/sector/post_sector_new.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/segment/__init__.py
+-rw-r--r--   0        0        0     2725 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/segment/get_segment_by_id_id.py
+-rw-r--r--   0        0        0     2623 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/segment/get_segment_filter_options.py
+-rw-r--r--   0        0        0     2614 2024-05-15 07:41:29.485862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/segment/post_segment_all.py
+-rw-r--r--   0        0        0     2636 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/segment/post_segment_territory_vehicle_profiles.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/stream/__init__.py
+-rw-r--r--   0        0        0     2609 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/stream/get_stream.py
+-rw-r--r--   0        0        0     2615 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/stream/get_stream_labels.py
+-rw-r--r--   0        0        0     2907 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/stream/post_stream_new.py
+-rw-r--r--   0        0        0     3034 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/stream/put_stream_by_id_id.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/street_service/__init__.py
+-rw-r--r--   0        0        0     2567 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/street_service/post_street_service_compute_itinerary.py
+-rw-r--r--   0        0        0     3427 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/street_service/put_street_service_transpose_realisation_id_realisation.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/__init__.py
+-rw-r--r--   0        0        0     2624 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/get_unibac_current_user_info.py
+-rw-r--r--   0        0        0     2989 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_login.py
+-rw-r--r--   0        0        0     3054 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_reset_password.py
+-rw-r--r--   0        0        0     2915 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_scan.py
+-rw-r--r--   0        0        0     3054 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/put_unibac_change_password.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/__init__.py
+-rw-r--r--   0        0        0     2638 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_container_sheet_params.py
+-rw-r--r--   0        0        0     2632 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_logistic_params.py
+-rw-r--r--   0        0        0     2639 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_operational_tabs_params.py
+-rw-r--r--   0        0        0     2633 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_pdf_export_params.py
+-rw-r--r--   0        0        0     2572 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_container_sheet_param.py
+-rw-r--r--   0        0        0     3111 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_logistic_params_column.py
+-rw-r--r--   0        0        0     2570 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_logistic_params_tab.py
+-rw-r--r--   0        0        0     3118 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_operational_tabs_params.py
+-rw-r--r--   0        0        0     3070 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_pdf_export_params.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/__init__.py
+-rw-r--r--   0        0        0     2610 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle.py
+-rw-r--r--   0        0        0     2631 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_environmental_criteria.py
+-rw-r--r--   0        0        0     2623 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_filter_options.py
+-rw-r--r--   0        0        0     2813 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_history_by_id_vehicle_id.py
+-rw-r--r--   0        0        0     2809 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_info_by_id_vehicle_id.py
+-rw-r--r--   0        0        0     2616 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_labels.py
+-rw-r--r--   0        0        0     2623 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_labels_profile.py
+-rw-r--r--   0        0        0     2622 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_loading_types.py
+-rw-r--r--   0        0        0     2630 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_vehicle_profile_labels.py
+-rw-r--r--   0        0        0     2625 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_vehicle_profiles.py
+-rw-r--r--   0        0        0     3094 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_environmental_criterion_new.py
+-rw-r--r--   0        0        0     3006 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_loading_type_new.py
+-rw-r--r--   0        0        0     2548 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_new.py
+-rw-r--r--   0        0        0     3030 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_vehicle_profile_new.py
+-rw-r--r--   0        0        0     2972 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_archive_many.py
+-rw-r--r--   0        0        0     3195 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_archive_vehicle_id.py
+-rw-r--r--   0        0        0     2739 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_by_id_vehicle_id.py
+-rw-r--r--   0        0        0     3110 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_environmental_criterion_update.py
+-rw-r--r--   0        0        0     3022 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_loading_type_update.py
+-rw-r--r--   0        0        0     3178 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_sectors_sector_id.py
+-rw-r--r--   0        0        0     3046 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_vehicle_profile_update.py
+-rw-r--r--   0        0        0        0 2024-05-15 14:36:04.283192 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/__init__.py
+-rw-r--r--   0        0        0     2726 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/delete_waste_codes_id.py
+-rw-r--r--   0        0        0     2613 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/get_waste_codes.py
+-rw-r--r--   0        0        0     2548 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/post_waste_codes.py
+-rw-r--r--   0        0        0     2657 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/put_waste_codes_id.py
+-rw-r--r--   0        0        0    12417 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/client.py
+-rw-r--r--   0        0        0      546 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/errors.py
+-rw-r--r--   0        0        0     9568 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/__init__.py
+-rw-r--r--   0        0        0     2133 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/changelog_response.py
+-rw-r--r--   0        0        0     1963 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/client_response.py
+-rw-r--r--   0        0        0     1930 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/current_user_response.py
+-rw-r--r--   0        0        0     2396 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/login_choose_response.py
+-rw-r--r--   0        0        0     1680 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/login_choose_response_clients_item.py
+-rw-r--r--   0        0        0      174 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/login_choose_response_type.py
+-rw-r--r--   0        0        0     2017 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/login_payload.py
+-rw-r--r--   0        0        0     1833 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/login_token_response.py
+-rw-r--r--   0        0        0      155 2024-05-15 07:41:29.489862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/login_token_response_type.py
+-rw-r--r--   0        0        0     1603 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_auth_register_body.py
+-rw-r--r--   0        0        0     1642 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_auth_reset_password_body.py
+-rw-r--r--   0        0        0     2207 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_back_office_event_definition_email_subscription_body.py
+-rw-r--r--   0        0        0     1602 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_comment_new_body.py
+-rw-r--r--   0        0        0     1597 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_container_delete_many_body.py
+-rw-r--r--   0        0        0     2632 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_container_new_many_body.py
+-rw-r--r--   0        0        0     1543 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_custom_field_body.py
+-rw-r--r--   0        0        0     1900 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_custom_field_option_id_custom_field_body.py
+-rw-r--r--   0        0        0     1616 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_device_live_data_update_body.py
+-rw-r--r--   0        0        0     1688 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_device_map_corrections_body.py
+-rw-r--r--   0        0        0     2011 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_device_submit_check_in_body.py
+-rw-r--r--   0        0        0     1712 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_error_report_device_crash_report_body.py
+-rw-r--r--   0        0        0     1938 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_event_definition_category_new_body.py
+-rw-r--r--   0        0        0     3398 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_event_definition_new_body.py
+-rw-r--r--   0        0        0     1577 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_event_delete_many_body.py
+-rw-r--r--   0        0        0     2156 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_external_button_collect_request_body.py
+-rw-r--r--   0        0        0     1814 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_external_create_ifm_itinerary_id_realisation_body.py
+-rw-r--r--   0        0        0     1631 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_external_live_vehicle_data_body.py
+-rw-r--r--   0        0        0     2612 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_operational_layers_data_source_body.py
+-rw-r--r--   0        0        0     1592 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producer_delete_many_body.py
+-rw-r--r--   0        0        0     1643 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producer_id_uni_and_co_user_body.py
+-rw-r--r--   0        0        0     2097 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_by_serial_numbers_body.py
+-rw-r--r--   0        0        0     1625 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_delete_many_body.py
+-rw-r--r--   0        0        0     2400 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_distinct_by_containers_ids_body.py
+-rw-r--r--   0        0        0     2244 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_unique_stream_containers_total_by_ids_body.py
+-rw-r--r--   0        0        0     1635 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_realisation_round_delete_many_body.py
+-rw-r--r--   0        0        0     2130 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_realisation_round_outlet_realised_body.py
+-rw-r--r--   0        0        0     1554 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_round_tracks_body.py
+-rw-r--r--   0        0        0     2033 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_route_parts_availabilities_body.py
+-rw-r--r--   0        0        0     2067 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_route_parts_producing_place_in_polygon_body.py
+-rw-r--r--   0        0        0     1566 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_sector_new_body.py
+-rw-r--r--   0        0        0     3103 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_stream_new_body.py
+-rw-r--r--   0        0        0     1892 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_login_body.py
+-rw-r--r--   0        0        0     1652 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_reset_password_body.py
+-rw-r--r--   0        0        0     1810 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_scan_body.py
+-rw-r--r--   0        0        0     1687 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_environmental_criterion_new_body.py
+-rw-r--r--   0        0        0     1632 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_loading_type_new_body.py
+-rw-r--r--   0        0        0     4414 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_vehicle_profile_new_body.py
+-rw-r--r--   0        0        0     2487 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_auth_by_id_id_body.py
+-rw-r--r--   0        0        0     1967 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_auth_change_password_body.py
+-rw-r--r--   0        0        0     1985 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_calendar_settings_body.py
+-rw-r--r--   0        0        0     1977 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_client_default_speed_on_segment_km_h_body.py
+-rw-r--r--   0        0        0     1771 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_client_mapbox_body.py
+-rw-r--r--   0        0        0     1743 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_client_show_deadheading_body.py
+-rw-r--r--   0        0        0     1609 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_comment_by_id_id_body.py
+-rw-r--r--   0        0        0     1919 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_constraint_body.py
+-rw-r--r--   0        0        0     1658 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_container_update_state_by_id_id_body.py
+-rw-r--r--   0        0        0     1615 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_employee_archive_id_body.py
+-rw-r--r--   0        0        0     1592 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_employee_archive_many_body.py
+-rw-r--r--   0        0        0     2185 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_employee_id_constraint_body.py
+-rw-r--r--   0        0        0     1683 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_employee_sectors_id_body.py
+-rw-r--r--   0        0        0     4636 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_event_definition_by_id_id_body.py
+-rw-r--r--   0        0        0     1954 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_event_definition_category_by_id_id_body.py
+-rw-r--r--   0        0        0     1636 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_intervention_id_planned_date_body.py
+-rw-r--r--   0        0        0     1914 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_outlet_id_body.py
+-rw-r--r--   0        0        0     3315 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_id_update_trackdechets_info_body.py
+-rw-r--r--   0        0        0     2131 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_linked_producers_body.py
+-rw-r--r--   0        0        0     1716 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_sectors_id_body.py
+-rw-r--r--   0        0        0     2363 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_realisation_round_proof_of_passage_id_ppra_body.py
+-rw-r--r--   0        0        0     1569 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_round_body.py
+-rw-r--r--   0        0        0     1960 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_round_occurrence_body.py
+-rw-r--r--   0        0        0     2079 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_round_round_slots_id_round_body.py
+-rw-r--r--   0        0        0     3119 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_stream_by_id_id_body.py
+-rw-r--r--   0        0        0     1926 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_street_service_transpose_realisation_id_realisation_body.py
+-rw-r--r--   0        0        0     1977 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_unibac_change_password_body.py
+-rw-r--r--   0        0        0     2045 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_logistic_params_column_body.py
+-rw-r--r--   0        0        0     2335 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_operational_tabs_params_body.py
+-rw-r--r--   0        0        0     2172 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_pdf_export_params_body.py
+-rw-r--r--   0        0        0     1587 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_archive_many_body.py
+-rw-r--r--   0        0        0     1648 2024-05-15 07:41:29.493862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_archive_vehicle_id_body.py
+-rw-r--r--   0        0        0     1914 2024-05-15 07:41:29.497862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_environmental_criterion_update_body.py
+-rw-r--r--   0        0        0     1859 2024-05-15 07:41:29.497862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_loading_type_update_body.py
+-rw-r--r--   0        0        0     1711 2024-05-15 07:41:29.497862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_sectors_sector_id_body.py
+-rw-r--r--   0        0        0     4641 2024-05-15 07:41:29.497862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_vehicle_profile_update_body.py
+-rw-r--r--   0        0        0       25 2024-05-15 07:41:29.497862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/py.typed
+-rw-r--r--   0        0        0      985 2024-05-15 07:41:29.497862 unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/types.py
+-rw-r--r--   0        0        0     2309 2024-05-15 07:41:29.497862 unico_device_setuper-0.6.0/unico_device_setuper/lib/utils.py
+-rw-r--r--   0        0        0      728 1970-01-01 00:00:00.000000 unico_device_setuper-0.6.0/PKG-INFO
```

### Comparing `unico_device_setuper-0.5.0/pyproject.toml` & `unico_device_setuper-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unico_device_setuper"
-version = '0.5.0'
+version = '0.6.0'
 description = ""
 authors = ["Florian Daude <floriandaude@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.12,<3.13"
```

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/cli/main.py` & `unico_device_setuper-0.6.0/unico_device_setuper/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 async def async_package(action: PackageAction, args: stp.Args):
     async with stp.Setup.make(args) as setup:
         match action:
             case PackageAction.LIST:
                 await pkg.list_packages(setup)
             case PackageAction.UNINSTALL:
-                await pkg.uninstall_list_packages(setup)
+                await pkg.uninstall_packages(setup)
 
 
 class UninavAction(enum.Enum):
     INSTALL = 'install'
 
 
 @APP.command()
```

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/cli/pkg.py` & `unico_device_setuper-0.6.0/unico_device_setuper/cli/pkg.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,42 +7,50 @@
 from unico_device_setuper.lib import cnsl, utils
 
 
 @dataclasses.dataclass
 class Package:
     label: str
     name: str
+    version: str | None = None
 
 
 async def get_package_from_apk_path(apk_path: str, name: str, setup: stp.Setup):
     output = await setup.aapt.dump('badging', apk_path, ignore_error=True)
 
+    package_prefix = 'package:'
     launchable_activity_prefix = 'launchable-activity:'
     base_label_prefix = 'application-label:'
     label_fr_prefix = 'application-label-fr:'
 
     launchable_activity_label = None
     base_label = None
     label_fr = None
+    version = None
     for line in output.splitlines():
         if line.startswith(launchable_activity_prefix):
             line_value = line.removeprefix(launchable_activity_prefix)
             _, _, label_and_after = line_value.partition('label=')
             label_value_and_space, _, _ = label_and_after.partition("='")
             launchable_activity_label = ' '.join(label_value_and_space.split()[:-1])[1:-1]
         if line.startswith(label_fr_prefix):
             label_fr = line.removeprefix(label_fr_prefix)[1:-1]
         if line.startswith(base_label_prefix):
             base_label = line.removeprefix(base_label_prefix)[1:-1]
+        if line.startswith(package_prefix):
+            line_value = line.removeprefix(package_prefix)
+            _, _, version_and_after = line_value.partition('versionName=')
+            version_and_space, _, _ = version_and_after.partition("='")
+            version = ' '.join(version_and_space.split()[:-1])[1:-1]
 
     label = launchable_activity_label or label_fr or base_label
     if label is None:
         return None
 
-    return Package(label=label, name=name)
+    return Package(label=label, name=name, version=version)
 
 
 def parse_package_list(output: str):
     prefix = 'package:'
     for line in output.splitlines():
         if line.startswith(prefix):
             yield line.removeprefix(prefix)
@@ -58,16 +66,22 @@
         package
         for name, path in tqdm.tqdm(package_apk_path_map.items())
         if (package := await get_package_from_apk_path(path, name, setup)) is not None
     ]
 
     max_label_length = max(len(p.label) for p in packages)
     for package in sorted(packages, key=lambda p: slugify.slugify(p.label)):
-        cnsl.print_blue(f' {package.label:<{max_label_length}}', end='')
-        cnsl.print(f' {package.name}')
+        cnsl.print(f' {package.label:<{max_label_length}}', end='')
+        cnsl.print_blue(f' {package.name}', end='')
+        cnsl.print_gray(f' ({package.version})' if package.version else '')
+
+
+async def uninstall_packages(setup: stp.Setup):
+    await uninstall_listed_packages(setup)
+    await clear_launcher_app_storage(setup)
 
 
 PACKAGE_TO_UNINSTALL: list[Package] = [
     Package('Chrome', name='com.android.chrome'),
     Package('Drive', name='com.google.android.apps.docs'),
     Package('Gmail', name='com.google.android.gm'),
     Package('Google', name='com.google.android.googlequicksearchbox'),
@@ -92,19 +106,24 @@
     Package('Samsung Flow', name='com.samsung.android.galaxycontinuity'),
     Package('AR Zone', name='com.samsung.android.arzone'),
     Package('Messages', name='com.samsung.android.messaging'),
     Package('Mes fichiers', name='com.sec.android.app.myfiles'),
     Package('Calendrier', name='com.samsung.android.calendar'),
     Package('Clock', name='com.sec.android.app.clockpackage'),
     Package('Netflix', name='com.netflix.mediaclient'),
+    Package('Mise à jour configuration', name='com.samsung.android.app.omcagent'),
 ]
 
 
-async def uninstall_list_packages(setup: stp.Setup):
-    installed_package_names = set(parse_package_list(await setup.adb.shell('pm list package')))
+async def get_installed_package_names(setup: stp.Setup):
+    return set(parse_package_list(await setup.adb.shell('pm list package')))
+
+
+async def uninstall_listed_packages(setup: stp.Setup):
+    installed_package_names = await get_installed_package_names(setup)
 
     await utils.gather(
         uninstall_package(package.name, installed_package_names, setup)
         for package in PACKAGE_TO_UNINSTALL
     )
 
 
@@ -113,7 +132,18 @@
         cnsl.print_gray(f'{package_name} déjà désinstallé')
         return
     try:
         await setup.adb.shell_uninstall(package_name)
         cnsl.print_greeen(f'{package_name} désinstallé avec succès')
     except RuntimeError:
         cnsl.print_red(f'Erreur lors de la désinstallation de {package_name}')
+
+
+LAUNCHER_APP_PACKAGE_NAMES = ['com.sec.android.app.launcher']
+
+
+async def clear_launcher_app_storage(setup: stp.Setup):
+    installed_package_names = await get_installed_package_names(setup)
+
+    for laucher_app_package_name in LAUNCHER_APP_PACKAGE_NAMES:
+        if laucher_app_package_name in installed_package_names:
+            await setup.adb.shell(f'pm clear {laucher_app_package_name}')
```

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/cli/stp.py` & `unico_device_setuper-0.6.0/unico_device_setuper/cli/stp.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/cli/unav.py` & `unico_device_setuper-0.6.0/unico_device_setuper/cli/unav.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 
 
 async def install_uninav(uninav_path: pathlib.Path, setup: stp.Setup):
     uninav_remote_path = pathlib.Path('/') / 'data' / 'local' / 'tmp' / 'uninav'
 
     await setup.adb.push(uninav_path, uninav_remote_path)
     with contextlib.suppress(RuntimeError):
-        await setup.adb.shell_uninstall('com.unico.dev.appmobile')
+        await setup.adb.uninstall_uninav()
     await setup.adb.shell_install(uninav_remote_path)
```

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/aapt.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/aapt.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/adb.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/adb.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 
     async def start_server(self):
         return await self._exec('start-server')
 
     async def kill_server(self):
         return await self._exec('kill-server')
 
+    async def uninstall_uninav(self):
+        return await self._exec('uninstall', 'com.unico.dev.appmobile')
+
     async def shell(self, cmd: str, *, ignore_error: bool = False):
         return await self._exec('shell', cmd, ignore_error=ignore_error)
 
     async def shell_uninstall(self, package_name: str):
         return await self.shell(f'pm uninstall -k --user 0 {package_name}')
 
     async def shell_disable(self, package_name: str):
```

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/auth.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/auth.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/cnsl.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/cnsl.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/datadir.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/datadir.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/dl.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/dl.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/__init__.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/__init__.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/delete_attachment_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/delete_attachment_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_data_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_data_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_event_images_id_event.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_event_images_id_event.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_info_by_foreign_id_mode_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_info_by_foreign_id_mode_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_info_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_info_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_producing_place_images_id_producing_place.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/get_attachment_producing_place_images_id_producing_place.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/post_attachment.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/post_attachment.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/attachment/put_attachment_is_visible_in_uni_and_co_id_is_visible.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/attachment/put_attachment_is_visible_in_uni_and_co_id_is_visible.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/delete_auth_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/delete_auth_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/delete_auth_user_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/delete_auth_user_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth_current_user_info.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth_current_user_info.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth_device_login.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/get_auth_device_login.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_login.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_login.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_register.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_register.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_reset_password.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/post_auth_reset_password.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/put_auth_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/put_auth_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/auth/put_auth_change_password.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/auth/put_auth_change_password.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/back_office/get_back_office_event_definition_email_subscription_all.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/back_office/get_back_office_event_definition_email_subscription_all.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/back_office/post_back_office_event_definition_email_subscription.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/back_office/post_back_office_event_definition_email_subscription.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/calendar/get_calendar_calendar_occurrences.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/calendar/get_calendar_calendar_occurrences.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/calendar/put_calendar_settings.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/calendar/put_calendar_settings.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/cartography/get_cartography_map_corrections.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/cartography/get_cartography_map_corrections.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/get_client.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/get_client.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_default_speed_on_segment_km_h.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_default_speed_on_segment_km_h.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_filling_rate_setting.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_filling_rate_setting.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_show_deadheading.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/get_client_show_deadheading.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/post_client_filling_rate_setting.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/post_client_filling_rate_setting.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_color_color.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_color_color.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_default_speed_on_segment_km_h.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_default_speed_on_segment_km_h.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_mapbox.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_mapbox.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_show_deadheading.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/client/put_client_show_deadheading.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/comment/delete_comment_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/comment/delete_comment_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/comment/get_comment_by_event_id_id_event.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/comment/get_comment_by_event_id_id_event.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/comment/post_comment_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/comment/post_comment_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/comment/put_comment_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/comment/put_comment_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/constraint/get_constraint_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/constraint/get_constraint_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/constraint/put_constraint.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/constraint/put_constraint.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/delete_container_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/delete_container_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_all_definitions.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_all_definitions.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_all_serial_numbers.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_all_serial_numbers.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_id_producing_place_id_producing_place.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_id_producing_place_id_producing_place.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_serial_number_serial_number.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_by_serial_number_serial_number.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_containers_with_active_event.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_containers_with_active_event.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_custom_fields_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_custom_fields_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_filter_options.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_filter_options.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_filtered.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_filtered.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_history_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/get_container_history_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_delete_many.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_delete_many.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_in_ids.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_in_ids.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_new_many.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/post_container_new_many.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/put_container_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/put_container_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container/put_container_update_state_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container/put_container_update_state_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container_definition/get_container_definition.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container_definition/get_container_definition.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container_definition/post_container_definition_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container_definition/post_container_definition_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/container_definition/put_container_definition_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/container_definition/put_container_definition_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/delete_custom_field_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/delete_custom_field_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/delete_custom_field_option_id_option.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/delete_custom_field_option_id_option.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/get_custom_field_many_target.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/get_custom_field_many_target.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/post_custom_field.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/post_custom_field.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/custom_field/post_custom_field_option_id_custom_field.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/custom_field/post_custom_field_option_id_custom_field.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/dashboard/get_dashboard_stats.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/dashboard/get_dashboard_stats.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_as_route_part_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_as_route_part_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_as_route_part_label.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_as_route_part_label.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_details_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_details_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_labels.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/get_depot_labels.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/post_depot.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/post_depot.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/depot/put_depot_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/depot/put_depot_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/delete_device_event_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/delete_device_event_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_attachment_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_attachment_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_check_in_form.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_check_in_form.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_client.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_client.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_client_dasri_allow_taken_producing_place_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_client_dasri_allow_taken_producing_place_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_container_by_serial_number_serial_number.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_container_by_serial_number_serial_number.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_container_definitions.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_container_definitions.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_containers_by_producing_place_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_containers_by_producing_place_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_depots.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_depots.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_drivers.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_drivers.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_event_definitions.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_event_definitions.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_event_definitions_categories.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_event_definitions_categories.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_itinerary_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_itinerary_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_map_corrections.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_map_corrections.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_near_by_producing_place.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_near_by_producing_place.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_outlets.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_outlets.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_poi_definitions.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_poi_definitions.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_pois_id_poi_definition.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_pois_id_poi_definition.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_round_id_itinerary.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_round_id_itinerary.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_rounds_meta.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_rounds_meta.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_search_producing_place.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_search_producing_place.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_streams.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_streams.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_update_change_log.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_update_change_log.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_v2_itinerary_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_v2_itinerary_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_v_2_near_by_producing_place.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_v_2_near_by_producing_place.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_vehicles.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/get_device_vehicles.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_bsd_sign_many.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_bsd_sign_many.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_dasri_sign_many.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_dasri_sign_many.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_live_data_update.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_live_data_update.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_map_corrections.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_map_corrections.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_submit_check_in.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_submit_check_in.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_v2_bsd_create.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/device/post_device_v2_bsd_create.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/driver/get_driver.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/driver/get_driver.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_employee_id_schedule.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_employee_id_schedule.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_filter_options.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_filter_options.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_id_constraint.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/get_employee_id_constraint.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/post_employee_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/post_employee_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_archive_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_archive_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_archive_many.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_archive_many.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_employee_id_schedule.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_employee_id_schedule.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_id_constraint.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_id_constraint.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_sectors_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/employee/put_employee_sectors_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/error_report/post_error_report_device_crash_report.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/error_report/post_error_report_device_crash_report.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_active.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_active.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_all_active.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_all_active.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_all_unique_authors.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_all_unique_authors.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_count_by_id_round_realisation_id_round_realisation.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_count_by_id_round_realisation_id_round_realisation.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_count_by_type.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_count_by_type.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_def_all.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_def_all.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_def_by_type_type.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_def_by_type_type.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_detailed_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_detailed_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_displayable_events.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_displayable_events.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_filter_options.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_filter_options.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_filtered.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_filtered.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_to_planify.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/get_event_to_planify.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/post_event_delete_many.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/post_event_delete_many.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/post_event_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/post_event_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/put_event_update_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/put_event_update_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event/put_event_update_state_id_state.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event/put_event_update_state_id_state.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition/get_event_definition.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition/get_event_definition.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition/post_event_definition_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition/post_event_definition_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition/put_event_definition_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition/put_event_definition_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/get_event_definition_category.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/get_event_definition_category.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/post_event_definition_category_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/post_event_definition_category_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/put_event_definition_category_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/event_definition_category/put_event_definition_category_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/export_client/get_export_client_reference_type.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/export_client/get_export_client_reference_type.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_alpes_mesure_filling_rate.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_alpes_mesure_filling_rate.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_button_collect_request.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_button_collect_request.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_create_ifm_itinerary_id_realisation.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_create_ifm_itinerary_id_realisation.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_elise_work_orders_id_franchise.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_elise_work_orders_id_franchise.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_live_vehicle_data.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_live_vehicle_data.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_v2_live_vehicle_data.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/external/post_external_v2_live_vehicle_data.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/icons/get_icons.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/icons/get_icons.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/intervention/get_intervention_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/intervention/get_intervention_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/intervention/get_intervention_to_planify.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/intervention/get_intervention_to_planify.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/intervention/put_intervention_id_planned_date.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/intervention/put_intervention_id_planned_date.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_as_pois.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_as_pois.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_by_batch.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_by_batch.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_export.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_export.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_total_count.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/logistic/post_logistic_total_count.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/mapbox/get_mapbox.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/mapbox/get_mapbox.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/message/post_message_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/message/post_message_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_export_collect_points.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_export_collect_points.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_in_interval.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_in_interval.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_team_by_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/occurrence/get_occurrence_team_by_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operational/get_operational_filter_options.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operational/get_operational_filter_options.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operational/post_operational_layers_data_source.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operational/post_operational_layers_data_source.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator_by_id_ids.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator_by_id_ids.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator_history_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/operator/get_operator_history_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_all_as_route_parts.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_all_as_route_parts.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_as_route_part_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_as_route_part_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_as_route_part_label.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_as_route_part_label.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_details_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_details_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_labels.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/get_outlet_labels.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/post_outlet.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/post_outlet.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/put_outlet_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/put_outlet_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/outlet/put_outlet_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/outlet/put_outlet_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_close_place.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_close_place.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_operational_places.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_operational_places.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_with_displayable_producing_places.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/place/get_place_with_displayable_producing_places.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/delete_producer_unlink_producer_with_producing_place_id_producer_id_producing_place.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/delete_producer_unlink_producer_with_producing_place_id_producer_id_producing_place.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_all.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_all.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_by_producing_place_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_by_producing_place_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_filter_options.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_filter_options.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_history_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_history_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_with_active_event.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/get_producer_with_active_event.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_delete_many.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_delete_many.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_id_uni_and_co_user.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_id_uni_and_co_user.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/post_producer_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producer/put_producer_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producer/put_producer_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/delete_producing_place_anomaly_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/delete_producing_place_anomaly_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_by_id_producer_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_by_id_producer_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_collectable_element_rounds_in_interval.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_collectable_element_rounds_in_interval.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_collection_planning_excel_by_id_producing_place_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_collection_planning_excel_by_id_producing_place_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_custom_fields_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_custom_fields_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_filter_options.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_filter_options.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_filtered.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_filtered.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_history_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_history_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_id_trackdechets_info_company.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_id_trackdechets_info_company.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_producing_place_id_schedule.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_producing_place_id_schedule.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_producing_place_id_waste_register.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_producing_place_id_waste_register.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_with_active_event.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/get_producing_place_with_active_event.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_by_serial_numbers.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_by_serial_numbers.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_delete_many.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_delete_many.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_distinct_by_containers_ids.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_distinct_by_containers_ids.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_distinct_ids_by_containers_ids.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_distinct_ids_by_containers_ids.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_unique_stream_containers_total_by_ids.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/post_producing_place_unique_stream_containers_total_by_ids.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_id_update_trackdechets_info.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_id_update_trackdechets_info.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_info_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_info_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_linked_producers.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_linked_producers.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_place_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_place_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_producing_place_id_schedule.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_producing_place_id_schedule.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_sectors_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place/put_producing_place_sectors_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/delete_producing_place_definition_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/delete_producing_place_definition_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/get_producing_place_definition.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/get_producing_place_definition.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/get_producing_place_definition_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/get_producing_place_definition_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/post_producing_place_definition.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/post_producing_place_definition.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/put_producing_place_definition_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/producing_place_definition/put_producing_place_definition_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/delete_realisation_round_outlet_realised_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/delete_realisation_round_outlet_realised_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_collect_report_by_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_collect_report_by_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_container_collect_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_container_collect_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_external_history_id_realisation.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_external_history_id_realisation.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_external_itinerary_id_realisation.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_external_itinerary_id_realisation.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_filter_options.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_filter_options.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_history_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_history_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_outlet_realised_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_outlet_realised_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_planned_vs_realised_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_planned_vs_realised_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_proof_of_passage_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_proof_of_passage_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_related_external_realisation_vehicle_id_realisation_date.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_related_external_realisation_vehicle_id_realisation_date.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_stats.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/get_realisation_round_stats.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/post_realisation_round_delete_many.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/post_realisation_round_delete_many.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/post_realisation_round_outlet_realised.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/post_realisation_round_outlet_realised.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_outlet_realised_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_outlet_realised_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_proof_of_passage_id_ppra.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_proof_of_passage_id_ppra.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_update_container_collect_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/realisation_round/put_realisation_round_update_container_collect_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/rotation_history/get_rotation_history.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/rotation_history/get_rotation_history.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/delete_round_id_round.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/delete_round_id_round.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/delete_round_occurrence.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/delete_round_occurrence.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_availability_id_itinerary_date.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_availability_id_itinerary_date.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_planified_id_itinerary.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_planified_id_itinerary.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_realised_id_itinerary.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_realised_id_itinerary.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_track_id_geo_json_vehicle_profile.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_track_id_geo_json_vehicle_profile.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_track_id_shp_vehicle_profile.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_itinerary_track_id_shp_vehicle_profile.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_occurrence_by_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_occurrence_by_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_occurrence_details_by_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_occurrence_details_by_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_route_parts_itinerary_id_geo_json.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_route_parts_itinerary_id_geo_json.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_route_parts_itinerary_id_shp.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_route_parts_itinerary_id_shp.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_team.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/get_round_team.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_itineraries_route_parts_type.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_itineraries_route_parts_type.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_itineraries_type.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_itineraries_type.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_tracks.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/post_round_tracks.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round_occurrence.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round_occurrence.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round_round_slots_id_round.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/round_/put_round_round_slots_id_round.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/route_parts/post_route_parts_availabilities.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/route_parts/post_route_parts_availabilities.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/route_parts/post_route_parts_producing_place_in_polygon.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/route_parts/post_route_parts_producing_place_in_polygon.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/sector/delete_sector_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/sector/delete_sector_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/sector/get_sector_all.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/sector/get_sector_all.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/sector/post_sector_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/sector/post_sector_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/segment/get_segment_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/segment/get_segment_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/segment/get_segment_filter_options.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/segment/get_segment_filter_options.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/segment/post_segment_all.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/segment/post_segment_all.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/segment/post_segment_territory_vehicle_profiles.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/segment/post_segment_territory_vehicle_profiles.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/stream/get_stream.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/stream/get_stream.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/stream/get_stream_labels.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/stream/get_stream_labels.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/stream/post_stream_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/stream/post_stream_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/stream/put_stream_by_id_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/stream/put_stream_by_id_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/street_service/post_street_service_compute_itinerary.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/street_service/post_street_service_compute_itinerary.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/street_service/put_street_service_transpose_realisation_id_realisation.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/street_service/put_street_service_transpose_realisation_id_realisation.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/get_unibac_current_user_info.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/get_unibac_current_user_info.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_login.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_login.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_reset_password.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_reset_password.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_scan.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/post_unibac_scan.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/unibac/put_unibac_change_password.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/unibac/put_unibac_change_password.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_container_sheet_params.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_container_sheet_params.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_logistic_params.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_logistic_params.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_operational_tabs_params.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_operational_tabs_params.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_pdf_export_params.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/get_user_preferences_pdf_export_params.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_container_sheet_param.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_container_sheet_param.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_logistic_params_column.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_logistic_params_column.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_logistic_params_tab.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_logistic_params_tab.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_operational_tabs_params.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_operational_tabs_params.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_pdf_export_params.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/user_preferences/put_user_preferences_pdf_export_params.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_environmental_criteria.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_environmental_criteria.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_filter_options.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_filter_options.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_history_by_id_vehicle_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_history_by_id_vehicle_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_info_by_id_vehicle_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_info_by_id_vehicle_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_labels.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_labels.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_labels_profile.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_labels_profile.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_loading_types.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_loading_types.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_vehicle_profile_labels.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_vehicle_profile_labels.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_vehicle_profiles.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/get_vehicle_vehicle_profiles.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_environmental_criterion_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_environmental_criterion_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_loading_type_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_loading_type_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_vehicle_profile_new.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/post_vehicle_vehicle_profile_new.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_archive_many.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_archive_many.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_archive_vehicle_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_archive_vehicle_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_by_id_vehicle_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_by_id_vehicle_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_environmental_criterion_update.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_environmental_criterion_update.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_loading_type_update.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_loading_type_update.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_sectors_sector_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_sectors_sector_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_vehicle_profile_update.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/vehicle/put_vehicle_vehicle_profile_update.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/delete_waste_codes_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/delete_waste_codes_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/get_waste_codes.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/get_waste_codes.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/post_waste_codes.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/post_waste_codes.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/put_waste_codes_id.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/api/waste_codes/put_waste_codes_id.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/client.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/client.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/errors.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/errors.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/__init__.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/changelog_response.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/changelog_response.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/client_response.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/client_response.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/current_user_response.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/current_user_response.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/login_choose_response.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/login_choose_response.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/login_choose_response_clients_item.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/login_choose_response_clients_item.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/login_payload.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/login_payload.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/login_token_response.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/login_token_response.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_auth_register_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_auth_register_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_auth_reset_password_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_auth_reset_password_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_back_office_event_definition_email_subscription_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_back_office_event_definition_email_subscription_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_comment_new_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_comment_new_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_container_delete_many_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_container_delete_many_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_container_new_many_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_container_new_many_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_custom_field_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_custom_field_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_custom_field_option_id_custom_field_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_custom_field_option_id_custom_field_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_device_live_data_update_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_device_live_data_update_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_device_map_corrections_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_device_map_corrections_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_device_submit_check_in_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_device_submit_check_in_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_error_report_device_crash_report_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_error_report_device_crash_report_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_event_definition_category_new_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_event_definition_category_new_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_event_definition_new_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_event_definition_new_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_event_delete_many_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_event_delete_many_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_external_button_collect_request_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_external_button_collect_request_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_external_create_ifm_itinerary_id_realisation_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_external_create_ifm_itinerary_id_realisation_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_external_live_vehicle_data_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_external_live_vehicle_data_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_operational_layers_data_source_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_operational_layers_data_source_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producer_delete_many_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producer_delete_many_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producer_id_uni_and_co_user_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producer_id_uni_and_co_user_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_by_serial_numbers_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_by_serial_numbers_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_delete_many_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_delete_many_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_distinct_by_containers_ids_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_distinct_by_containers_ids_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_unique_stream_containers_total_by_ids_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_producing_place_unique_stream_containers_total_by_ids_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_realisation_round_delete_many_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_realisation_round_delete_many_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_realisation_round_outlet_realised_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_realisation_round_outlet_realised_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_round_tracks_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_round_tracks_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_route_parts_availabilities_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_route_parts_availabilities_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_route_parts_producing_place_in_polygon_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_route_parts_producing_place_in_polygon_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_sector_new_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_sector_new_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_stream_new_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_stream_new_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_login_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_login_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_reset_password_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_reset_password_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_scan_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_unibac_scan_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_environmental_criterion_new_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_environmental_criterion_new_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_loading_type_new_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_loading_type_new_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_vehicle_profile_new_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/post_vehicle_vehicle_profile_new_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_auth_by_id_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_auth_by_id_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_auth_change_password_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_auth_change_password_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_calendar_settings_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_calendar_settings_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_client_default_speed_on_segment_km_h_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_client_default_speed_on_segment_km_h_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_client_mapbox_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_client_mapbox_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_client_show_deadheading_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_client_show_deadheading_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_comment_by_id_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_comment_by_id_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_constraint_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_constraint_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_container_update_state_by_id_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_container_update_state_by_id_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_employee_archive_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_employee_archive_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_employee_archive_many_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_employee_archive_many_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_employee_id_constraint_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_employee_id_constraint_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_employee_sectors_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_employee_sectors_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_event_definition_by_id_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_event_definition_by_id_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_event_definition_category_by_id_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_event_definition_category_by_id_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_intervention_id_planned_date_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_intervention_id_planned_date_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_outlet_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_outlet_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_id_update_trackdechets_info_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_id_update_trackdechets_info_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_linked_producers_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_linked_producers_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_sectors_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_producing_place_sectors_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_realisation_round_proof_of_passage_id_ppra_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_realisation_round_proof_of_passage_id_ppra_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_round_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_round_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_round_occurrence_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_round_occurrence_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_round_round_slots_id_round_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_round_round_slots_id_round_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_stream_by_id_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_stream_by_id_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_street_service_transpose_realisation_id_realisation_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_street_service_transpose_realisation_id_realisation_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_unibac_change_password_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_unibac_change_password_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_logistic_params_column_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_logistic_params_column_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_operational_tabs_params_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_operational_tabs_params_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_pdf_export_params_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_user_preferences_pdf_export_params_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_archive_many_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_archive_many_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_archive_vehicle_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_archive_vehicle_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_environmental_criterion_update_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_environmental_criterion_update_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_loading_type_update_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_loading_type_update_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_sectors_sector_id_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_sectors_sector_id_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_vehicle_profile_update_body.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/models/put_vehicle_vehicle_profile_update_body.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/unitech/impl/types.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/unitech/impl/types.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/unico_device_setuper/lib/utils.py` & `unico_device_setuper-0.6.0/unico_device_setuper/lib/utils.py`

 * *Files identical despite different names*

### Comparing `unico_device_setuper-0.5.0/PKG-INFO` & `unico_device_setuper-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unico_device_setuper
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 License: MIT
 Author: Florian Daude
 Author-email: floriandaude@hotmail.fr
 Requires-Python: >=3.12,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

