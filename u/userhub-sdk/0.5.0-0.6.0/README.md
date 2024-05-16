# Comparing `tmp/userhub_sdk-0.5.0.tar.gz` & `tmp/userhub_sdk-0.6.0.tar.gz`

## Comparing `userhub_sdk-0.5.0.tar` & `userhub_sdk-0.6.0.tar`

### file list

```diff
@@ -1,223 +1,220 @@
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/README.md
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/_internal/__init__.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/_internal/constants.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/_internal/http_transport.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/_internal/request.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/_internal/response.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/_internal/test_transport.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/_internal/transport.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/_internal/util.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminapi/__init__.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_client.py
--rw-r--r--   0        0        0    15413 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_flows.py
--rw-r--r--   0        0        0     6590 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_invoices.py
--rw-r--r--   0        0        0    41578 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_organizations.py
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_subscriptions.py
--rw-r--r--   0        0        0    35625 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_users.py
--rw-r--r--   0        0        0     7743 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/__init__.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_account_connection.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_account_subscription.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_account_subscription_plan.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_account_subscription_product.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_account_subscription_seat.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_auth0_connection.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_batch_create_triggers_response.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_batch_delete_triggers_response.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_batch_get_organizations_response.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_batch_get_triggers_response.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_batch_get_users_response.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_builtin_email_connection.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_card_payment_method.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_card_payment_method_expiration.py
--rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_connection.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_connection_delegate.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_connection_provider.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_create_api_session_response.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_create_payment_method_intent_response.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_create_portal_session_response.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_actor.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_api_key.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_connection.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_entity.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_organization.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_request.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_user.py
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_flow.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_google_cloud_identity_platform_connection.py
--rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_account.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_balance.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_change.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_item.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_preview.py
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_preview_item.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_join_organization_flow.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_connections_response.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_events_response.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_flows_response.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_invoices_response.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_members_response.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_organizations_response.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_plan_group_change_paths_response.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_plan_group_revisions_response.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_plan_group_tags_response.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_plan_groups_response.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_prices_response.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_products_response.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_roles_response.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_subscriptions_response.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_triggers_response.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_users_response.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_member.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_member_input.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_membership.py
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_organization.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_organization_input.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_organization_result.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_payment_intent.py
--rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_payment_method.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_payment_method_input.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan.py
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group.py
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_change_path.py
--rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_revision.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_revision_item.py
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_revision_plan.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_tag.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_trial.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_item.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_postmark_connection.py
--rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_price.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_price_fixed_price.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_price_tiered_price.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_price_transform_quantity.py
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_product.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_product_connection.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_role.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_search_members_response.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_search_organizations_response.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_search_users_response.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_signing_secret.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_signup_flow.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_stripe_connection.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_stripe_payment_intent.py
--rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_subscription.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_subscription_current_period.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_subscription_item.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_subscription_seat_info.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_subscription_trial.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_tiered_price_tier.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_trigger.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_trigger_result.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_update_subscription_items_request_item.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_user.py
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_user_input.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_user_result.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_webhook_connection.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/apiv1/__init__.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/apiv1/_empty_response.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/apiv1/_operation_info.py
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/apiv1/_status.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/apiv1/_status_details.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/commonv1/__init__.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/commonv1/_address.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/commonv1/_any.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/commonv1/_email.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/commonv1/_interval.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/commonv1/_period.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/__init__.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_challenge.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_custom_user.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_delete_custom_user_request.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_error_response.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_get_custom_user_request.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_list_custom_users_request.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_list_custom_users_response.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/__init__.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_event.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_flows_changed.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_members_changed.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_organizations_changed.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_subscriptions_changed.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_users_changed.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/operationsv1/__init__.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/operationsv1/_operation.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/operationsv1/_operation_error.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/types/__init__.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/types/_code.py
--rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/types/_error.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/types/_str_enum.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/types/_undefined.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userapi/__init__.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userapi/_client.py
--rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userapi/_flows.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userapi/_invoices.py
--rw-r--r--   0        0        0    14451 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userapi/_organizations.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userapi/_session.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/__init__.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_account_subscription.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_account_subscription_plan.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_account_subscription_seat.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_billing_account.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_card_payment_method.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_card_payment_method_expiration.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_flow.py
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_account.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_balance.py
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_change.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_item.py
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_preview.py
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_preview_item.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_join_organization_flow.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_flows_response.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_invoices_response.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_members_response.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_organizations_response.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_payment_methods_response.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_plan_groups_response.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_roles_response.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_subscriptions_response.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_member.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_membership.py
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_organization.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_organization_input.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_payment_intent.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_payment_method.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_payment_method_input.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_payment_method_intent.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_plan.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_plan_group.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_plan_group_change_path.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_plan_group_trial.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_plan_item.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_price.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_price_fixed_price.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_price_tiered_price.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_price_transform_quantity.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_product.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_role.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_session.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_signup_flow.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_stripe_payment_intent.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_stripe_payment_method_intent.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_subscription.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_subscription_current_period.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_subscription_item.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_subscription_seat_info.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_subscription_trial.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_tiered_price_tier.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/userv1/_user.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/webhook/__init__.py
--rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/webhook/_actions.py
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/webhook/_base.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/webhook/_handler.py
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/webhook/_http.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/src/userhub_sdk/webhook/_util.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/LICENSE
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 userhub_sdk-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/README.md
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/_internal/__init__.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/_internal/constants.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/_internal/http_transport.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/_internal/request.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/_internal/response.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/_internal/test_transport.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/_internal/transport.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/_internal/util.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminapi/__init__.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_client.py
+-rw-r--r--   0        0        0    16295 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_flows.py
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_invoices.py
+-rw-r--r--   0        0        0    44648 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_organizations.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_subscriptions.py
+-rw-r--r--   0        0        0    37141 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_users.py
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/__init__.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_account_connection.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_account_subscription.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_account_subscription_plan.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_account_subscription_product.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_account_subscription_seat.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_auth0_connection.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_batch_create_triggers_response.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_batch_delete_triggers_response.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_batch_get_organizations_response.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_batch_get_triggers_response.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_batch_get_users_response.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_builtin_email_connection.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_card_payment_method.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_card_payment_method_expiration.py
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_connection.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_connection_delegate.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_connection_provider.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_create_api_session_response.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_create_payment_method_intent_response.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_create_portal_session_response.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_actor.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_api_key.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_connection.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_entity.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_organization.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_request.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_user.py
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_flow.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_google_cloud_identity_platform_connection.py
+-rw-r--r--   0        0        0     9833 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_account.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_balance.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_change.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_item.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_preview.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_preview_item.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_join_organization_flow.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_connections_response.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_events_response.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_flows_response.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_invoices_response.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_members_response.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_organizations_response.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_plan_group_change_paths_response.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_plan_group_revisions_response.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_plan_group_tags_response.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_plan_groups_response.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_prices_response.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_products_response.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_roles_response.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_subscriptions_response.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_triggers_response.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_users_response.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_member.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_member_input.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_membership.py
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_organization.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_organization_input.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_organization_result.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_payment_intent.py
+-rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_payment_method.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_payment_method_input.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan.py
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_change_path.py
+-rw-r--r--   0        0        0     4598 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_revision.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_revision_item.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_revision_plan.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_tag.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_trial.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_item.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_postmark_connection.py
+-rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_price.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_price_fixed_price.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_price_tiered_price.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_price_transform_quantity.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_product.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_product_connection.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_role.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_signing_secret.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_signup_flow.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_stripe_connection.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_stripe_payment_intent.py
+-rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_subscription.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_subscription_current_period.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_subscription_item.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_subscription_seat_info.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_subscription_trial.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_tiered_price_tier.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_trigger.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_trigger_result.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_update_subscription_items_request_item.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_user.py
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_user_input.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_user_result.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_webhook_connection.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/apiv1/__init__.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/apiv1/_empty_response.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/apiv1/_operation_info.py
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/apiv1/_status.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/apiv1/_status_details.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/commonv1/__init__.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/commonv1/_address.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/commonv1/_any.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/commonv1/_email.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/commonv1/_interval.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/commonv1/_period.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/__init__.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_challenge.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_custom_user.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_delete_custom_user_request.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_error_response.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_get_custom_user_request.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_list_custom_users_request.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_list_custom_users_response.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/__init__.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_event.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_flows_changed.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_members_changed.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_organizations_changed.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_subscriptions_changed.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_users_changed.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/operationsv1/__init__.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/operationsv1/_operation.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/operationsv1/_operation_error.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/types/__init__.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/types/_code.py
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/types/_error.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/types/_str_enum.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/types/_undefined.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userapi/__init__.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userapi/_client.py
+-rw-r--r--   0        0        0    15360 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userapi/_flows.py
+-rw-r--r--   0        0        0     5089 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userapi/_invoices.py
+-rw-r--r--   0        0        0    14281 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userapi/_organizations.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userapi/_session.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/__init__.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_account_subscription.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_account_subscription_plan.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_account_subscription_seat.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_billing_account.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_card_payment_method.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_card_payment_method_expiration.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_flow.py
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_account.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_balance.py
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_change.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_item.py
+-rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_preview.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_preview_item.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_join_organization_flow.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_flows_response.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_invoices_response.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_members_response.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_organizations_response.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_payment_methods_response.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_plan_groups_response.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_roles_response.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_subscriptions_response.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_member.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_membership.py
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_organization.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_organization_input.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_payment_intent.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_payment_method.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_payment_method_input.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_payment_method_intent.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_plan.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_plan_group.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_plan_group_change_path.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_plan_group_trial.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_plan_item.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_price.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_price_fixed_price.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_price_tiered_price.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_price_transform_quantity.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_product.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_role.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_session.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_signup_flow.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_stripe_payment_intent.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_stripe_payment_method_intent.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_subscription.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_subscription_current_period.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_subscription_item.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_subscription_seat_info.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_subscription_trial.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_tiered_price_tier.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/userv1/_user.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/webhook/__init__.py
+-rw-r--r--   0        0        0    11432 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/webhook/_actions.py
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/webhook/_base.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/webhook/_handler.py
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/webhook/_http.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/src/userhub_sdk/webhook/_util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 userhub_sdk-0.6.0/PKG-INFO
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/_internal/constants.py` & `userhub_sdk-0.6.0/src/userhub_sdk/_internal/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Code generated. DO NOT EDIT.
 
 import datetime
 import sys
 
 API_BASE_URL = "https://api.userhub.com"
-USER_AGENT = "UserHub-Python/0.5.0"
-VERSION = "0.5.0"
+USER_AGENT = "UserHub-Python/0.6.0"
+VERSION = "0.6.0"
 
 AUTH_HEADER = "Authorization"
 API_KEY_HEADER = "UserHub-Api-Key"
 ADMIN_KEY_PREFIX = "sk_"
 USER_KEY_PREFIX = "pk_"
 
 WEBHOOK_ACTION_HEADER = "UserHub-Action"
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/_internal/http_transport.py` & `userhub_sdk-0.6.0/src/userhub_sdk/_internal/http_transport.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/_internal/request.py` & `userhub_sdk-0.6.0/src/userhub_sdk/_internal/request.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/_internal/response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/_internal/response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/_internal/test_transport.py` & `userhub_sdk-0.6.0/src/userhub_sdk/_internal/test_transport.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/_internal/transport.py` & `userhub_sdk-0.6.0/src/userhub_sdk/_internal/transport.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/_internal/util.py` & `userhub_sdk-0.6.0/src/userhub_sdk/_internal/util.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminapi/__init__.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminapi/__init__.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_client.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_client.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_flows.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_flows.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,61 +19,73 @@
 
     def list(
         self,
         *,
         organization_id: Optional[str] = None,
         user_id: Optional[str] = None,
         type: Optional[str] = None,
+        active: Optional[bool] = None,
+        creator_user_id: Optional[str] = None,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
         order_by: Optional[str] = None,
         view: Optional[str] = None,
     ) -> adminv1.ListFlowsResponse:
         """
         Lists flows.
 
         :param organization_id:
             Filter results by organization identifier.
         :param user_id:
             Filter results by user identifier.
         :param type:
             Filter the results by the specified flow type.
+        :param active:
+            Whether to filter out flows not in the `START_PENDING` or `STARTED`
+            state.
+        :param creator_user_id:
+            The identifier of the user that created the flow.
+
+            When this is specified only the flows created by the user are
+            returned.
         :param page_size:
             The maximum number of flows to return. The API may return fewer than
             this value.
 
             If unspecified, at most 20 flows will be returned.
             The maximum value is 100; values above 100 will be coerced to 100.
         :param page_token:
             A page token, received from a previous list flows call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list flows must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `type`
-            - `createTime`
+            Supports:
+            - `createTime desc`
         :param view:
             The Flow view to return in the results.
 
             This defaults to the `BASIC` view.
         """
         req = Request("admin.flows.list", "GET", "/admin/v1/flows")
         req.set_idempotent(True)
 
         if organization_id:
             req.set_query("organizationId", organization_id)
         if user_id:
             req.set_query("userId", user_id)
         if type:
             req.set_query("type", type)
+        if active:
+            req.set_query("active", active)
+        if creator_user_id:
+            req.set_query("creatorUserId", creator_user_id)
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
             req.set_query("pageToken", page_token)
         if order_by:
             req.set_query("orderBy", order_by)
         if view:
@@ -268,61 +280,73 @@
 
     async def list(
         self,
         *,
         organization_id: Optional[str] = None,
         user_id: Optional[str] = None,
         type: Optional[str] = None,
+        active: Optional[bool] = None,
+        creator_user_id: Optional[str] = None,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
         order_by: Optional[str] = None,
         view: Optional[str] = None,
     ) -> adminv1.ListFlowsResponse:
         """
         Lists flows.
 
         :param organization_id:
             Filter results by organization identifier.
         :param user_id:
             Filter results by user identifier.
         :param type:
             Filter the results by the specified flow type.
+        :param active:
+            Whether to filter out flows not in the `START_PENDING` or `STARTED`
+            state.
+        :param creator_user_id:
+            The identifier of the user that created the flow.
+
+            When this is specified only the flows created by the user are
+            returned.
         :param page_size:
             The maximum number of flows to return. The API may return fewer than
             this value.
 
             If unspecified, at most 20 flows will be returned.
             The maximum value is 100; values above 100 will be coerced to 100.
         :param page_token:
             A page token, received from a previous list flows call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list flows must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `type`
-            - `createTime`
+            Supports:
+            - `createTime desc`
         :param view:
             The Flow view to return in the results.
 
             This defaults to the `BASIC` view.
         """
         req = Request("admin.flows.list", "GET", "/admin/v1/flows")
         req.set_idempotent(True)
 
         if organization_id:
             req.set_query("organizationId", organization_id)
         if user_id:
             req.set_query("userId", user_id)
         if type:
             req.set_query("type", type)
+        if active:
+            req.set_query("active", active)
+        if creator_user_id:
+            req.set_query("creatorUserId", creator_user_id)
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
             req.set_query("pageToken", page_token)
         if order_by:
             req.set_query("orderBy", order_by)
         if view:
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_invoices.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_invoices.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,22 +45,19 @@
         :param page_token:
             A page token, received from a previous list invoices call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list invoices must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `state`
-            - `dueTime`
-            - `createTime`
-            - `updateTime`
+            Supports:
+            - `createTime asc`
+            - `createTime desc`
         """
         req = Request("admin.invoices.list", "GET", "/admin/v1/invoices")
         req.set_idempotent(True)
 
         if organization_id:
             req.set_query("organizationId", organization_id)
         if user_id:
@@ -147,22 +144,19 @@
         :param page_token:
             A page token, received from a previous list invoices call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list invoices must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `state`
-            - `dueTime`
-            - `createTime`
-            - `updateTime`
+            Supports:
+            - `createTime asc`
+            - `createTime desc`
         """
         req = Request("admin.invoices.list", "GET", "/admin/v1/invoices")
         req.set_idempotent(True)
 
         if organization_id:
             req.set_query("organizationId", organization_id)
         if user_id:
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_organizations.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_organizations.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,54 +17,76 @@
 
     def __init__(self, transport: Transport):
         self._transport = transport
 
     def list(
         self,
         *,
+        display_name: Optional[str] = None,
+        email: Optional[str] = None,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
         order_by: Optional[str] = None,
         show_deleted: Optional[bool] = None,
         view: Optional[str] = None,
     ) -> adminv1.ListOrganizationsResponse:
         """
         Lists organizations.
 
+        :param display_name:
+            Filter the results by display name.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
+        :param email:
+            Filter the results by email address.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
         :param page_size:
             The maximum number of organizations to return. The API may return fewer than
             this value.
 
             If unspecified, at most 20 organizations will be returned.
             The maximum value is 100; values above 100 will be coerced to 100.
         :param page_token:
             A page token, received from a previous list organizations call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list organizations must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `displayName`
-            - `email`
-            - `createTime`
-            - `deleteTime`
+            Supports:
+            - `displayName asc`
+            - `email asc`
+            - `signupTime desc`
+            - `createTime desc`
+            - `deleteTime desc`
         :param show_deleted:
             Whether to show deleted organizations.
         :param view:
             The organization view to return in the results.
 
             This defaults to the `BASIC` view.
         """
         req = Request("admin.organizations.list", "GET", "/admin/v1/organizations")
         req.set_idempotent(True)
 
+        if display_name:
+            req.set_query("displayName", display_name)
+        if email:
+            req.set_query("email", email)
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
             req.set_query("pageToken", page_token)
         if order_by:
             req.set_query("orderBy", order_by)
         if show_deleted:
@@ -442,50 +464,77 @@
 
         return res.decode_body(adminv1.Organization.__json_decode__)
 
     def list_members(
         self,
         organization_id: str,
         *,
+        display_name: Optional[str] = None,
+        email: Optional[str] = None,
+        role_id: Optional[str] = None,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
         order_by: Optional[str] = None,
     ) -> adminv1.ListMembersResponse:
         """
         Lists organization members.
 
         :param organization_id:
             The identifier of the organization.
+        :param display_name:
+            Filter the results by display name.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
+        :param email:
+            Filter the results by email address.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
+        :param role_id:
+            Filter the results by a role identifier.
         :param page_size:
             The maximum number of members to return. The API may return fewer than
             this value.
 
             If unspecified, at most 20 members will be returned.
             The maximum value is 100; values above 100 will be coerced to 100.
         :param page_token:
             A page token, received from a previous list members call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list members must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `createTime`
-            - `updateTime`
+            Supports:
+            - `displayName asc`
+            - `email asc`
+            - `createTime desc`
         """
         req = Request(
             "admin.organizations.listMembers",
             "GET",
             f"/admin/v1/organizations/{util.quote_path(organization_id)}/members",
         )
         req.set_idempotent(True)
 
+        if display_name:
+            req.set_query("displayName", display_name)
+        if email:
+            req.set_query("email", email)
+        if role_id:
+            req.set_query("roleId", role_id)
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
             req.set_query("pageToken", page_token)
         if order_by:
             req.set_query("orderBy", order_by)
 
@@ -505,16 +554,14 @@
 
         :param organization_id:
             The identifier of the organization.
         :param user_id:
             The identifier of the user.
         :param role_id:
             The identifier of the role.
-
-            This is currently limited to `member`, `admin`, and `owner`.
         """
         req = Request(
             "admin.organizations.addMember",
             "POST",
             f"/admin/v1/organizations/{util.quote_path(organization_id)}/members",
         )
         body: Dict[str, Any] = {}
@@ -567,16 +614,14 @@
 
         :param organization_id:
             The identifier of the organization.
         :param user_id:
             The identifier of the user.
         :param role_id:
             The identifier of the role.
-
-            This is currently limited to `member`, `admin`, and `owner`.
         :param allow_missing:
             If set to true, and the member is not found, a new member will be created.
         """
         req = Request(
             "admin.organizations.updateMember",
             "PATCH",
             f"/admin/v1/organizations/{util.quote_path(organization_id)}/members/{util.quote_path(user_id)}",
@@ -626,54 +671,76 @@
 
     def __init__(self, transport: AsyncTransport):
         self._transport = transport
 
     async def list(
         self,
         *,
+        display_name: Optional[str] = None,
+        email: Optional[str] = None,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
         order_by: Optional[str] = None,
         show_deleted: Optional[bool] = None,
         view: Optional[str] = None,
     ) -> adminv1.ListOrganizationsResponse:
         """
         Lists organizations.
 
+        :param display_name:
+            Filter the results by display name.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
+        :param email:
+            Filter the results by email address.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
         :param page_size:
             The maximum number of organizations to return. The API may return fewer than
             this value.
 
             If unspecified, at most 20 organizations will be returned.
             The maximum value is 100; values above 100 will be coerced to 100.
         :param page_token:
             A page token, received from a previous list organizations call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list organizations must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `displayName`
-            - `email`
-            - `createTime`
-            - `deleteTime`
+            Supports:
+            - `displayName asc`
+            - `email asc`
+            - `signupTime desc`
+            - `createTime desc`
+            - `deleteTime desc`
         :param show_deleted:
             Whether to show deleted organizations.
         :param view:
             The organization view to return in the results.
 
             This defaults to the `BASIC` view.
         """
         req = Request("admin.organizations.list", "GET", "/admin/v1/organizations")
         req.set_idempotent(True)
 
+        if display_name:
+            req.set_query("displayName", display_name)
+        if email:
+            req.set_query("email", email)
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
             req.set_query("pageToken", page_token)
         if order_by:
             req.set_query("orderBy", order_by)
         if show_deleted:
@@ -1051,50 +1118,77 @@
 
         return res.decode_body(adminv1.Organization.__json_decode__)
 
     async def list_members(
         self,
         organization_id: str,
         *,
+        display_name: Optional[str] = None,
+        email: Optional[str] = None,
+        role_id: Optional[str] = None,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
         order_by: Optional[str] = None,
     ) -> adminv1.ListMembersResponse:
         """
         Lists organization members.
 
         :param organization_id:
             The identifier of the organization.
+        :param display_name:
+            Filter the results by display name.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
+        :param email:
+            Filter the results by email address.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
+        :param role_id:
+            Filter the results by a role identifier.
         :param page_size:
             The maximum number of members to return. The API may return fewer than
             this value.
 
             If unspecified, at most 20 members will be returned.
             The maximum value is 100; values above 100 will be coerced to 100.
         :param page_token:
             A page token, received from a previous list members call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list members must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `createTime`
-            - `updateTime`
+            Supports:
+            - `displayName asc`
+            - `email asc`
+            - `createTime desc`
         """
         req = Request(
             "admin.organizations.listMembers",
             "GET",
             f"/admin/v1/organizations/{util.quote_path(organization_id)}/members",
         )
         req.set_idempotent(True)
 
+        if display_name:
+            req.set_query("displayName", display_name)
+        if email:
+            req.set_query("email", email)
+        if role_id:
+            req.set_query("roleId", role_id)
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
             req.set_query("pageToken", page_token)
         if order_by:
             req.set_query("orderBy", order_by)
 
@@ -1114,16 +1208,14 @@
 
         :param organization_id:
             The identifier of the organization.
         :param user_id:
             The identifier of the user.
         :param role_id:
             The identifier of the role.
-
-            This is currently limited to `member`, `admin`, and `owner`.
         """
         req = Request(
             "admin.organizations.addMember",
             "POST",
             f"/admin/v1/organizations/{util.quote_path(organization_id)}/members",
         )
         body: Dict[str, Any] = {}
@@ -1176,16 +1268,14 @@
 
         :param organization_id:
             The identifier of the organization.
         :param user_id:
             The identifier of the user.
         :param role_id:
             The identifier of the role.
-
-            This is currently limited to `member`, `admin`, and `owner`.
         :param allow_missing:
             If set to true, and the member is not found, a new member will be created.
         """
         req = Request(
             "admin.organizations.updateMember",
             "PATCH",
             f"/admin/v1/organizations/{util.quote_path(organization_id)}/members/{util.quote_path(user_id)}",
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_subscriptions.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,19 @@
         :param page_token:
             A page token, received from a previous list subscriptions call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list subscriptions must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `createTime`
+            Supports:
+            - `active desc`
+            - `createTime desc`
         :param view:
             The Subscription view to return in the results.
 
             This defaults to the `BASIC` view.
         """
         req = Request("admin.subscriptions.list", "GET", "/admin/v1/subscriptions")
         req.set_idempotent(True)
@@ -152,19 +152,19 @@
         :param page_token:
             A page token, received from a previous list subscriptions call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list subscriptions must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `createTime`
+            Supports:
+            - `active desc`
+            - `createTime desc`
         :param view:
             The Subscription view to return in the results.
 
             This defaults to the `BASIC` view.
         """
         req = Request("admin.subscriptions.list", "GET", "/admin/v1/subscriptions")
         req.set_idempotent(True)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminapi/_users.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminapi/_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,54 +17,76 @@
 
     def __init__(self, transport: Transport):
         self._transport = transport
 
     def list(
         self,
         *,
+        display_name: Optional[str] = None,
+        email: Optional[str] = None,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
         order_by: Optional[str] = None,
         show_deleted: Optional[bool] = None,
         view: Optional[str] = None,
     ) -> adminv1.ListUsersResponse:
         """
         Lists users.
 
+        :param display_name:
+            Filter the results by display name.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
+        :param email:
+            Filter the results by email address.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
         :param page_size:
             The maximum number of users to return. The API may return fewer than
             this value.
 
             If unspecified, at most 20 users will be returned.
             The maximum value is 100; values above 100 will be coerced to 100.
         :param page_token:
             A page token, received from a previous list users call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list users must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `displayName`
-            - `email`
-            - `createTime`
-            - `deleteTime`
+            Supports:
+            - `displayName asc`
+            - `email asc`
+            - `signupTime desc`
+            - `createTime desc`
+            - `deleteTime desc`
         :param show_deleted:
             Whether to show deleted users.
         :param view:
             The User view to return in the results.
 
             This defaults to the `BASIC` view.
         """
         req = Request("admin.users.list", "GET", "/admin/v1/users")
         req.set_idempotent(True)
 
+        if display_name:
+            req.set_query("displayName", display_name)
+        if email:
+            req.set_query("email", email)
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
             req.set_query("pageToken", page_token)
         if order_by:
             req.set_query("orderBy", order_by)
         if show_deleted:
@@ -554,54 +576,76 @@
 
     def __init__(self, transport: AsyncTransport):
         self._transport = transport
 
     async def list(
         self,
         *,
+        display_name: Optional[str] = None,
+        email: Optional[str] = None,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
         order_by: Optional[str] = None,
         show_deleted: Optional[bool] = None,
         view: Optional[str] = None,
     ) -> adminv1.ListUsersResponse:
         """
         Lists users.
 
+        :param display_name:
+            Filter the results by display name.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
+        :param email:
+            Filter the results by email address.
+
+            To enable prefix filtering append `*` to the end of the value
+            and ensure you provide at least 3 characters excluding the
+            wildcard.
+
+            This filter is case-insensitivity.
         :param page_size:
             The maximum number of users to return. The API may return fewer than
             this value.
 
             If unspecified, at most 20 users will be returned.
             The maximum value is 100; values above 100 will be coerced to 100.
         :param page_token:
             A page token, received from a previous list users call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list users must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `displayName`
-            - `email`
-            - `createTime`
-            - `deleteTime`
+            Supports:
+            - `displayName asc`
+            - `email asc`
+            - `signupTime desc`
+            - `createTime desc`
+            - `deleteTime desc`
         :param show_deleted:
             Whether to show deleted users.
         :param view:
             The User view to return in the results.
 
             This defaults to the `BASIC` view.
         """
         req = Request("admin.users.list", "GET", "/admin/v1/users")
         req.set_idempotent(True)
 
+        if display_name:
+            req.set_query("displayName", display_name)
+        if email:
+            req.set_query("email", email)
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
             req.set_query("pageToken", page_token)
         if order_by:
             req.set_query("orderBy", order_by)
         if show_deleted:
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/__init__.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,17 +78,14 @@
 from ._price import Price
 from ._price_fixed_price import PriceFixedPrice
 from ._price_tiered_price import PriceTieredPrice
 from ._price_transform_quantity import PriceTransformQuantity
 from ._product import Product
 from ._product_connection import ProductConnection
 from ._role import Role
-from ._search_members_response import SearchMembersResponse
-from ._search_organizations_response import SearchOrganizationsResponse
-from ._search_users_response import SearchUsersResponse
 from ._signing_secret import SigningSecret
 from ._signup_flow import SignupFlow
 from ._stripe_connection import StripeConnection
 from ._stripe_payment_intent import StripePaymentIntent
 from ._subscription import Subscription
 from ._subscription_current_period import SubscriptionCurrentPeriod
 from ._subscription_item import SubscriptionItem
@@ -180,17 +177,14 @@
     "Price",
     "PriceFixedPrice",
     "PriceTieredPrice",
     "PriceTransformQuantity",
     "Product",
     "ProductConnection",
     "Role",
-    "SearchMembersResponse",
-    "SearchOrganizationsResponse",
-    "SearchUsersResponse",
     "SigningSecret",
     "SignupFlow",
     "StripeConnection",
     "StripePaymentIntent",
     "Subscription",
     "SubscriptionCurrentPeriod",
     "SubscriptionItem",
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_account_connection.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_account_connection.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_account_subscription.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_account_subscription.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_account_subscription_plan.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_account_subscription_plan.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_account_subscription_product.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_account_subscription_product.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_account_subscription_seat.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_account_subscription_seat.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_auth0_connection.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_auth0_connection.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_batch_create_triggers_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_batch_create_triggers_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_batch_delete_triggers_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_batch_delete_triggers_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_batch_get_organizations_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_batch_get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_batch_get_triggers_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_batch_get_triggers_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_batch_get_users_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_batch_get_users_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_builtin_email_connection.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_builtin_email_connection.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_card_payment_method.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_card_payment_method.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_card_payment_method_expiration.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_card_payment_method_expiration.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_connection.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_connection.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_connection_delegate.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_connection_delegate.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_connection_provider.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_connection_provider.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_create_api_session_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_create_api_session_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_create_payment_method_intent_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_create_payment_method_intent_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_create_portal_session_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_create_portal_session_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_actor.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_actor.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_api_key.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_api_key.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_connection.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_connection.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_entity.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_entity.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_organization.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_organization.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_request.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_request.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_event_user.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_event_user.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_flow.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_flow.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_google_cloud_identity_platform_connection.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_google_cloud_identity_platform_connection.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_account.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_account.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_balance.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_balance.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_change.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_change.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_item.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_item.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_preview.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_preview.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_invoice_preview_item.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_invoice_preview_item.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_join_organization_flow.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_join_organization_flow.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_connections_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_connections_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_events_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_events_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_flows_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_flows_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_invoices_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_invoices_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_members_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_members_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_organizations_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_organizations_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_plan_group_change_paths_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_plan_group_change_paths_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_plan_group_revisions_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_plan_group_revisions_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_plan_group_tags_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_plan_group_tags_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_plan_groups_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_plan_groups_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_prices_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_prices_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_products_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_products_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_roles_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_roles_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_subscriptions_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_triggers_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_triggers_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_list_users_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_list_users_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_member.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_member.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_member_input.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_member_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     """
     Member input parameters.
     """
 
     #: The identifier of the user.
     user_id: str = ""
     #: The identifier of the role.
-    #:
-    #: This is currently limited to `member`, `admin`, and `owner`.
     role_id: str = ""
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
         if self.user_id is not None:
             data["userId"] = self.user_id
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_membership.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_membership.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_organization.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_organization.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_organization_input.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_organization_input.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_organization_result.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_organization_result.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_payment_intent.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_payment_intent.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_payment_method.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_payment_method.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_payment_method_input.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_payment_method_input.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_change_path.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_change_path.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_revision.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_revision.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_revision_item.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_revision_item.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_revision_plan.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_revision_plan.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_tag.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_tag.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_group_trial.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_group_trial.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_plan_item.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_plan_item.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_postmark_connection.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_postmark_connection.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_price.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_price.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_price_fixed_price.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_price_fixed_price.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_price_tiered_price.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_price_tiered_price.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_price_transform_quantity.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_price_transform_quantity.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_product.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_product.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_product_connection.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_product_connection.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_role.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_role.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_search_members_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_flows_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,55 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
 from typing import Any, Dict, List, Optional
 
-from ._member import Member
+from ._flow import Flow
 
 
 @dataclasses.dataclass
-class SearchMembersResponse:
+class ListFlowsResponse:
     """
-    Response message for SearchMembers.
+    Response message for ListFlows.
     """
 
-    #: The search of members.
-    members: List[Member] = dataclasses.field(default_factory=list)
+    #: The list of flows.
+    flows: List[Flow] = dataclasses.field(default_factory=list)
     #: A token, which can be sent as `pageToken` to retrieve the next page.
     #: If this field is omitted, there are no subsequent pages.
     next_page_token: str = ""
     #: A token, which can be sent as `pageToken` to retrieve the previous page.
     #: If this field is absent, there are no preceding pages. If this field is
     #: an empty string then the previous page is the first result.
     previous_page_token: Optional[str] = None
-    #: The estimated total count of matched members irrespective of pagination.
-    #:
-    #: This field is ignored if `show_total_size` is not true or `pageToken`
-    #: is not empty.
-    total_size: Optional[int] = None
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.members is not None:
-            data["members"] = [Member.__json_encode__(v) for v in self.members]
+        if self.flows is not None:
+            data["flows"] = [Flow.__json_encode__(v) for v in self.flows]
 
         if self.next_page_token is not None:
             data["nextPageToken"] = self.next_page_token
 
         if self.previous_page_token is not None:
             data["previousPageToken"] = self.previous_page_token
 
-        if self.total_size is not None:
-            data["totalSize"] = self.total_size
-
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "SearchMembersResponse":
+    def __json_decode__(data: Dict[str, Any]) -> "ListFlowsResponse":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("members") is not None:
-            kwargs["members"] = [Member.__json_decode__(v) for v in data["members"]]
+        if data.get("flows") is not None:
+            kwargs["flows"] = [Flow.__json_decode__(v) for v in data["flows"]]
 
         if data.get("nextPageToken") is not None:
             kwargs["next_page_token"] = data["nextPageToken"]
 
         if data.get("previousPageToken") is not None:
             kwargs["previous_page_token"] = data["previousPageToken"]
 
-        if data.get("totalSize") is not None:
-            kwargs["total_size"] = data["totalSize"]
-
-        return SearchMembersResponse(**kwargs)
+        return ListFlowsResponse(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_search_organizations_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_organizations_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 import dataclasses
 from typing import Any, Dict, List, Optional
 
 from ._organization import Organization
 
 
 @dataclasses.dataclass
-class SearchOrganizationsResponse:
+class ListOrganizationsResponse:
     """
-    Response message for SearchOrganizations.
+    Response message for ListOrganizations.
     """
 
-    #: The search of organizations.
-    organizations: List[Organization] = dataclasses.field(default_factory=list)
+    #: The list of organizations.
+    organizations: Optional[List[Organization]] = dataclasses.field(
+        default_factory=list
+    )
     #: A token, which can be sent as `pageToken` to retrieve the next page.
     #: If this field is omitted, there are no subsequent pages.
     next_page_token: str = ""
     #: A token, which can be sent as `pageToken` to retrieve the previous page.
     #: If this field is absent, there are no preceding pages. If this field is
     #: an empty string then the previous page is the first result.
     previous_page_token: Optional[str] = None
-    #: The estimated total count of matched organizations irrespective of pagination.
-    #:
-    #: This field is ignored if `show_total_size` is not true or `pageToken`
-    #: is not empty.
-    total_size: Optional[int] = None
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
         if self.organizations is not None:
             data["organizations"] = [
                 Organization.__json_encode__(v) for v in self.organizations
@@ -37,21 +34,18 @@
 
         if self.next_page_token is not None:
             data["nextPageToken"] = self.next_page_token
 
         if self.previous_page_token is not None:
             data["previousPageToken"] = self.previous_page_token
 
-        if self.total_size is not None:
-            data["totalSize"] = self.total_size
-
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "SearchOrganizationsResponse":
+    def __json_decode__(data: Dict[str, Any]) -> "ListOrganizationsResponse":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
         if data.get("organizations") is not None:
             kwargs["organizations"] = [
@@ -60,11 +54,8 @@
 
         if data.get("nextPageToken") is not None:
             kwargs["next_page_token"] = data["nextPageToken"]
 
         if data.get("previousPageToken") is not None:
             kwargs["previous_page_token"] = data["previousPageToken"]
 
-        if data.get("totalSize") is not None:
-            kwargs["total_size"] = data["totalSize"]
-
-        return SearchOrganizationsResponse(**kwargs)
+        return ListOrganizationsResponse(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_search_users_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_roles_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,55 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
 from typing import Any, Dict, List, Optional
 
-from ._user import User
+from ._role import Role
 
 
 @dataclasses.dataclass
-class SearchUsersResponse:
+class ListRolesResponse:
     """
-    Response message for SearchUsers.
+    Response message for ListRoles.
     """
 
-    #: The search of users.
-    users: List[User] = dataclasses.field(default_factory=list)
+    #: The list of roles.
+    roles: List[Role] = dataclasses.field(default_factory=list)
     #: A token, which can be sent as `pageToken` to retrieve the next page.
     #: If this field is omitted, there are no subsequent pages.
     next_page_token: str = ""
     #: A token, which can be sent as `pageToken` to retrieve the previous page.
     #: If this field is absent, there are no preceding pages. If this field is
     #: an empty string then the previous page is the first result.
     previous_page_token: Optional[str] = None
-    #: The estimated total count of matched users irrespective of pagination.
-    #:
-    #: This field is ignored if `show_total_size` is not true or `pageToken`
-    #: is not empty.
-    total_size: Optional[int] = None
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.users is not None:
-            data["users"] = [User.__json_encode__(v) for v in self.users]
+        if self.roles is not None:
+            data["roles"] = [Role.__json_encode__(v) for v in self.roles]
 
         if self.next_page_token is not None:
             data["nextPageToken"] = self.next_page_token
 
         if self.previous_page_token is not None:
             data["previousPageToken"] = self.previous_page_token
 
-        if self.total_size is not None:
-            data["totalSize"] = self.total_size
-
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "SearchUsersResponse":
+    def __json_decode__(data: Dict[str, Any]) -> "ListRolesResponse":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("users") is not None:
-            kwargs["users"] = [User.__json_decode__(v) for v in data["users"]]
+        if data.get("roles") is not None:
+            kwargs["roles"] = [Role.__json_decode__(v) for v in data["roles"]]
 
         if data.get("nextPageToken") is not None:
             kwargs["next_page_token"] = data["nextPageToken"]
 
         if data.get("previousPageToken") is not None:
             kwargs["previous_page_token"] = data["previousPageToken"]
 
-        if data.get("totalSize") is not None:
-            kwargs["total_size"] = data["totalSize"]
-
-        return SearchUsersResponse(**kwargs)
+        return ListRolesResponse(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_signing_secret.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_signing_secret.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_signup_flow.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_signup_flow.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_stripe_connection.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_stripe_connection.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_stripe_payment_intent.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_stripe_payment_intent.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_subscription.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_subscription.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_subscription_current_period.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_subscription_current_period.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_subscription_item.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_subscription_item.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_subscription_seat_info.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_subscription_seat_info.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_subscription_trial.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_subscription_trial.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_tiered_price_tier.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_tiered_price_tier.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_trigger.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_trigger.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_trigger_result.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_trigger_result.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_update_subscription_items_request_item.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_update_subscription_items_request_item.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_user.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_user.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_user_input.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_user_input.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_user_result.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_user_result.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/adminv1/_webhook_connection.py` & `userhub_sdk-0.6.0/src/userhub_sdk/adminv1/_webhook_connection.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/apiv1/_operation_info.py` & `userhub_sdk-0.6.0/src/userhub_sdk/apiv1/_operation_info.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/apiv1/_status.py` & `userhub_sdk-0.6.0/src/userhub_sdk/apiv1/_status.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/apiv1/_status_details.py` & `userhub_sdk-0.6.0/src/userhub_sdk/apiv1/_status_details.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/commonv1/_address.py` & `userhub_sdk-0.6.0/src/userhub_sdk/commonv1/_address.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/commonv1/_any.py` & `userhub_sdk-0.6.0/src/userhub_sdk/commonv1/_any.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/commonv1/_email.py` & `userhub_sdk-0.6.0/src/userhub_sdk/commonv1/_email.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/commonv1/_interval.py` & `userhub_sdk-0.6.0/src/userhub_sdk/commonv1/_interval.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/commonv1/_period.py` & `userhub_sdk-0.6.0/src/userhub_sdk/commonv1/_period.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/__init__.py` & `userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/__init__.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_challenge.py` & `userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_challenge.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_custom_user.py` & `userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_custom_user.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_delete_custom_user_request.py` & `userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_delete_custom_user_request.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_error_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_error_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_get_custom_user_request.py` & `userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_get_custom_user_request.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_list_custom_users_request.py` & `userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_list_custom_users_request.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/connectionsv1/_list_custom_users_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/connectionsv1/_list_custom_users_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_event.py` & `userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_event.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_flows_changed.py` & `userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_flows_changed.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_members_changed.py` & `userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_members_changed.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_organizations_changed.py` & `userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_organizations_changed.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_subscriptions_changed.py` & `userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_subscriptions_changed.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/eventsv1/_users_changed.py` & `userhub_sdk-0.6.0/src/userhub_sdk/eventsv1/_users_changed.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/operationsv1/_operation.py` & `userhub_sdk-0.6.0/src/userhub_sdk/operationsv1/_operation.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/operationsv1/_operation_error.py` & `userhub_sdk-0.6.0/src/userhub_sdk/operationsv1/_operation_error.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/types/_code.py` & `userhub_sdk-0.6.0/src/userhub_sdk/types/_code.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/types/_error.py` & `userhub_sdk-0.6.0/src/userhub_sdk/types/_error.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/types/_str_enum.py` & `userhub_sdk-0.6.0/src/userhub_sdk/types/_str_enum.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userapi/__init__.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userapi/__init__.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userapi/_client.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userapi/_client.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userapi/_flows.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userapi/_flows.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         self._transport = transport
 
     def list(
         self,
         *,
         organization_id: Optional[str] = None,
         type: Optional[str] = None,
+        active: Optional[bool] = None,
+        creator: Optional[bool] = None,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
         order_by: Optional[str] = None,
     ) -> userv1.ListFlowsResponse:
         """
         Lists flows.
 
@@ -33,41 +35,48 @@
 
             When not set the user's flows are returned.
 
             Otherwise if the user is an admin of the provided organization then
             the flows associated with that organization are returned.
         :param type:
             Filter the results by the specified flow type.
+        :param active:
+            Whether to filter out flows not in the `START_PENDING` or `STARTED`
+            state.
+        :param creator:
+            Whether to only return flows created by the authenticated user.
         :param page_size:
             The maximum number of flows to return. The API may return fewer than
             this value.
 
             If unspecified, at most 20 flows will be returned.
             The maximum value is 100; values above 100 will be coerced to 100.
         :param page_token:
             A page token, received from a previous list flows call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list flows must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `type`
-            - `createTime`
+            Supports:
+            - `createTime desc`
         """
         req = Request("user.flows.list", "GET", "/user/v1/flows")
         req.set_idempotent(True)
 
         if organization_id:
             req.set_query("organizationId", organization_id)
         if type:
             req.set_query("type", type)
+        if active:
+            req.set_query("active", active)
+        if creator:
+            req.set_query("creator", creator)
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
             req.set_query("pageToken", page_token)
         if order_by:
             req.set_query("orderBy", order_by)
 
@@ -270,14 +279,16 @@
         self._transport = transport
 
     async def list(
         self,
         *,
         organization_id: Optional[str] = None,
         type: Optional[str] = None,
+        active: Optional[bool] = None,
+        creator: Optional[bool] = None,
         page_size: Optional[int] = None,
         page_token: Optional[str] = None,
         order_by: Optional[str] = None,
     ) -> userv1.ListFlowsResponse:
         """
         Lists flows.
 
@@ -286,41 +297,48 @@
 
             When not set the user's flows are returned.
 
             Otherwise if the user is an admin of the provided organization then
             the flows associated with that organization are returned.
         :param type:
             Filter the results by the specified flow type.
+        :param active:
+            Whether to filter out flows not in the `START_PENDING` or `STARTED`
+            state.
+        :param creator:
+            Whether to only return flows created by the authenticated user.
         :param page_size:
             The maximum number of flows to return. The API may return fewer than
             this value.
 
             If unspecified, at most 20 flows will be returned.
             The maximum value is 100; values above 100 will be coerced to 100.
         :param page_token:
             A page token, received from a previous list flows call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list flows must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `type`
-            - `createTime`
+            Supports:
+            - `createTime desc`
         """
         req = Request("user.flows.list", "GET", "/user/v1/flows")
         req.set_idempotent(True)
 
         if organization_id:
             req.set_query("organizationId", organization_id)
         if type:
             req.set_query("type", type)
+        if active:
+            req.set_query("active", active)
+        if creator:
+            req.set_query("creator", creator)
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
             req.set_query("pageToken", page_token)
         if order_by:
             req.set_query("orderBy", order_by)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userapi/_invoices.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userapi/_invoices.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,22 +41,19 @@
         :param page_token:
             A page token, received from a previous list invoices call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list invoices must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `state`
-            - `dueTime`
-            - `createTime`
-            - `updateTime`
+            Supports:
+            - `createTime asc`
+            - `createTime desc`
         """
         req = Request("user.invoices.list", "GET", "/user/v1/invoices")
         req.set_idempotent(True)
 
         if organization_id:
             req.set_query("organizationId", organization_id)
         if page_size:
@@ -125,22 +122,19 @@
         :param page_token:
             A page token, received from a previous list invoices call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list invoices must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `state`
-            - `dueTime`
-            - `createTime`
-            - `updateTime`
+            Supports:
+            - `createTime asc`
+            - `createTime desc`
         """
         req = Request("user.invoices.list", "GET", "/user/v1/invoices")
         req.set_idempotent(True)
 
         if organization_id:
             req.set_query("organizationId", organization_id)
         if page_size:
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userapi/_organizations.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userapi/_organizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,19 @@
         :param page_token:
             A page token, received from a previous list organizations call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list organizations must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `displayName`
-            - `email`
+            Supports:
+            - `displayName asc`
+            - `email asc`
         """
         req = Request("user.organizations.list", "GET", "/user/v1/organizations")
         req.set_idempotent(True)
 
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
@@ -190,29 +189,29 @@
         res = self._transport.execute(req)
 
         return res.decode_body(userv1.Organization.__json_decode__)
 
     def delete(
         self,
         organization_id: str,
-    ) -> userv1.Organization:
+    ) -> apiv1.EmptyResponse:
         """
         Delete specified organization.
 
         :param organization_id:
             The identifier of the organization.
         """
         req = Request(
             "user.organizations.delete",
             "DELETE",
             f"/user/v1/organizations/{util.quote_path(organization_id)}",
         )
         res = self._transport.execute(req)
 
-        return res.decode_body(userv1.Organization.__json_decode__)
+        return res.decode_body(apiv1.EmptyResponse.__json_decode__)
 
     def leave(
         self,
         organization_id: str,
     ) -> apiv1.EmptyResponse:
         """
         Leave organization.
@@ -260,20 +259,19 @@
         :param page_token:
             A page token, received from a previous list organizations call.
             Provide this to retrieve the subsequent page.
 
             When paginating, all other parameters provided to list organizations must match
             the call that provided the page token.
         :param order_by:
-            A comma-separated list of fields to order by, sorted in ascending order.
-            Use `desc` after a field name for descending.
+            A comma-separated list of fields to order by.
 
-            Supported fields:
-            - `displayName`
-            - `email`
+            Supports:
+            - `displayName asc`
+            - `email asc`
         """
         req = Request("user.organizations.list", "GET", "/user/v1/organizations")
         req.set_idempotent(True)
 
         if page_size:
             req.set_query("pageSize", page_size)
         if page_token:
@@ -414,29 +412,29 @@
         res = await self._transport.execute(req)
 
         return res.decode_body(userv1.Organization.__json_decode__)
 
     async def delete(
         self,
         organization_id: str,
-    ) -> userv1.Organization:
+    ) -> apiv1.EmptyResponse:
         """
         Delete specified organization.
 
         :param organization_id:
             The identifier of the organization.
         """
         req = Request(
             "user.organizations.delete",
             "DELETE",
             f"/user/v1/organizations/{util.quote_path(organization_id)}",
         )
         res = await self._transport.execute(req)
 
-        return res.decode_body(userv1.Organization.__json_decode__)
+        return res.decode_body(apiv1.EmptyResponse.__json_decode__)
 
     async def leave(
         self,
         organization_id: str,
     ) -> apiv1.EmptyResponse:
         """
         Leave organization.
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userapi/_session.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userapi/_session.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/__init__.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/__init__.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_account_subscription.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_account_subscription.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_account_subscription_plan.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_account_subscription_plan.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_account_subscription_seat.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_account_subscription_seat.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_billing_account.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_billing_account.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_card_payment_method.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_card_payment_method.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_card_payment_method_expiration.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_card_payment_method_expiration.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_flow.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_flow.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_account.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_account.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_balance.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_balance.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_change.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_change.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_item.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_item.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_preview.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_preview.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_invoice_preview_item.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_invoice_preview_item.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_join_organization_flow.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_join_organization_flow.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_flows_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_invoices_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
 from typing import Any, Dict, List, Optional
 
-from ._flow import Flow
+from ._invoice import Invoice
 
 
 @dataclasses.dataclass
-class ListFlowsResponse:
+class ListInvoicesResponse:
     """
-    Response message for ListFlows.
+    Response message for ListInvoices.
     """
 
-    #: The list of flows.
-    flows: List[Flow] = dataclasses.field(default_factory=list)
+    #: The list of invoices.
+    invoices: List[Invoice] = dataclasses.field(default_factory=list)
     #: A token, which can be sent as `pageToken` to retrieve the next page.
     #: If this field is omitted, there are no subsequent pages.
     next_page_token: str = ""
     #: A token, which can be sent as `pageToken` to retrieve the previous page.
     #: If this field is absent, there are no preceding pages. If this field is
     #: an empty string then the previous page is the first result.
     previous_page_token: Optional[str] = None
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.flows is not None:
-            data["flows"] = [Flow.__json_encode__(v) for v in self.flows]
+        if self.invoices is not None:
+            data["invoices"] = [Invoice.__json_encode__(v) for v in self.invoices]
 
         if self.next_page_token is not None:
             data["nextPageToken"] = self.next_page_token
 
         if self.previous_page_token is not None:
             data["previousPageToken"] = self.previous_page_token
 
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "ListFlowsResponse":
+    def __json_decode__(data: Dict[str, Any]) -> "ListInvoicesResponse":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("flows") is not None:
-            kwargs["flows"] = [Flow.__json_decode__(v) for v in data["flows"]]
+        if data.get("invoices") is not None:
+            kwargs["invoices"] = [Invoice.__json_decode__(v) for v in data["invoices"]]
 
         if data.get("nextPageToken") is not None:
             kwargs["next_page_token"] = data["nextPageToken"]
 
         if data.get("previousPageToken") is not None:
             kwargs["previous_page_token"] = data["previousPageToken"]
 
-        return ListFlowsResponse(**kwargs)
+        return ListInvoicesResponse(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_invoices_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_members_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
 from typing import Any, Dict, List, Optional
 
-from ._invoice import Invoice
+from ._member import Member
 
 
 @dataclasses.dataclass
-class ListInvoicesResponse:
+class ListMembersResponse:
     """
-    Response message for ListInvoices.
+    Response message for ListMembers.
     """
 
-    #: The list of invoices.
-    invoices: List[Invoice] = dataclasses.field(default_factory=list)
+    #: The list of members.
+    members: Optional[List[Member]] = dataclasses.field(default_factory=list)
     #: A token, which can be sent as `pageToken` to retrieve the next page.
     #: If this field is omitted, there are no subsequent pages.
     next_page_token: str = ""
     #: A token, which can be sent as `pageToken` to retrieve the previous page.
     #: If this field is absent, there are no preceding pages. If this field is
     #: an empty string then the previous page is the first result.
     previous_page_token: Optional[str] = None
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.invoices is not None:
-            data["invoices"] = [Invoice.__json_encode__(v) for v in self.invoices]
+        if self.members is not None:
+            data["members"] = [Member.__json_encode__(v) for v in self.members]
 
         if self.next_page_token is not None:
             data["nextPageToken"] = self.next_page_token
 
         if self.previous_page_token is not None:
             data["previousPageToken"] = self.previous_page_token
 
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "ListInvoicesResponse":
+    def __json_decode__(data: Dict[str, Any]) -> "ListMembersResponse":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("invoices") is not None:
-            kwargs["invoices"] = [Invoice.__json_decode__(v) for v in data["invoices"]]
+        if data.get("members") is not None:
+            kwargs["members"] = [Member.__json_decode__(v) for v in data["members"]]
 
         if data.get("nextPageToken") is not None:
             kwargs["next_page_token"] = data["nextPageToken"]
 
         if data.get("previousPageToken") is not None:
             kwargs["previous_page_token"] = data["previousPageToken"]
 
-        return ListInvoicesResponse(**kwargs)
+        return ListMembersResponse(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_members_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_subscriptions_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
 from typing import Any, Dict, List, Optional
 
-from ._member import Member
+from ._subscription import Subscription
 
 
 @dataclasses.dataclass
-class ListMembersResponse:
+class ListSubscriptionsResponse:
     """
-    Response message for ListMembers.
+    Response message for ListSubscriptions.
     """
 
-    #: The list of members.
-    members: Optional[List[Member]] = dataclasses.field(default_factory=list)
+    #: The list of subscriptions.
+    subscriptions: List[Subscription] = dataclasses.field(default_factory=list)
     #: A token, which can be sent as `pageToken` to retrieve the next page.
     #: If this field is omitted, there are no subsequent pages.
     next_page_token: str = ""
     #: A token, which can be sent as `pageToken` to retrieve the previous page.
     #: If this field is absent, there are no preceding pages. If this field is
     #: an empty string then the previous page is the first result.
     previous_page_token: Optional[str] = None
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.members is not None:
-            data["members"] = [Member.__json_encode__(v) for v in self.members]
+        if self.subscriptions is not None:
+            data["subscriptions"] = [
+                Subscription.__json_encode__(v) for v in self.subscriptions
+            ]
 
         if self.next_page_token is not None:
             data["nextPageToken"] = self.next_page_token
 
         if self.previous_page_token is not None:
             data["previousPageToken"] = self.previous_page_token
 
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "ListMembersResponse":
+    def __json_decode__(data: Dict[str, Any]) -> "ListSubscriptionsResponse":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("members") is not None:
-            kwargs["members"] = [Member.__json_decode__(v) for v in data["members"]]
+        if data.get("subscriptions") is not None:
+            kwargs["subscriptions"] = [
+                Subscription.__json_decode__(v) for v in data["subscriptions"]
+            ]
 
         if data.get("nextPageToken") is not None:
             kwargs["next_page_token"] = data["nextPageToken"]
 
         if data.get("previousPageToken") is not None:
             kwargs["previous_page_token"] = data["previousPageToken"]
 
-        return ListMembersResponse(**kwargs)
+        return ListSubscriptionsResponse(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_organizations_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_payment_methods_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
 from typing import Any, Dict, List, Optional
 
-from ._organization import Organization
+from ._payment_method import PaymentMethod
 
 
 @dataclasses.dataclass
-class ListOrganizationsResponse:
+class ListPaymentMethodsResponse:
     """
-    Response message for ListOrganizations.
+    Response message for ListPaymentMethods.
     """
 
-    #: The list of organizations.
-    organizations: Optional[List[Organization]] = dataclasses.field(
-        default_factory=list
-    )
+    #: The list of payment methods.
+    payment_methods: List[PaymentMethod] = dataclasses.field(default_factory=list)
     #: A token, which can be sent as `pageToken` to retrieve the next page.
     #: If this field is omitted, there are no subsequent pages.
     next_page_token: str = ""
     #: A token, which can be sent as `pageToken` to retrieve the previous page.
     #: If this field is absent, there are no preceding pages. If this field is
     #: an empty string then the previous page is the first result.
     previous_page_token: Optional[str] = None
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.organizations is not None:
-            data["organizations"] = [
-                Organization.__json_encode__(v) for v in self.organizations
+        if self.payment_methods is not None:
+            data["paymentMethods"] = [
+                PaymentMethod.__json_encode__(v) for v in self.payment_methods
             ]
 
         if self.next_page_token is not None:
             data["nextPageToken"] = self.next_page_token
 
         if self.previous_page_token is not None:
             data["previousPageToken"] = self.previous_page_token
 
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "ListOrganizationsResponse":
+    def __json_decode__(data: Dict[str, Any]) -> "ListPaymentMethodsResponse":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("organizations") is not None:
-            kwargs["organizations"] = [
-                Organization.__json_decode__(v) for v in data["organizations"]
+        if data.get("paymentMethods") is not None:
+            kwargs["payment_methods"] = [
+                PaymentMethod.__json_decode__(v) for v in data["paymentMethods"]
             ]
 
         if data.get("nextPageToken") is not None:
             kwargs["next_page_token"] = data["nextPageToken"]
 
         if data.get("previousPageToken") is not None:
             kwargs["previous_page_token"] = data["previousPageToken"]
 
-        return ListOrganizationsResponse(**kwargs)
+        return ListPaymentMethodsResponse(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_plan_groups_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_list_plan_groups_response.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_roles_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_subscription_item.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Optional
 
-from ._role import Role
+from ._price import Price
+from ._product import Product
 
 
 @dataclasses.dataclass
-class ListRolesResponse:
+class SubscriptionItem:
     """
-    Response message for ListRoles.
+    The subscription items.
     """
 
-    #: The list of roles.
-    roles: List[Role] = dataclasses.field(default_factory=list)
-    #: A token, which can be sent as `pageToken` to retrieve the next page.
-    #: If this field is omitted, there are no subsequent pages.
-    next_page_token: str = ""
-    #: A token, which can be sent as `pageToken` to retrieve the previous page.
-    #: If this field is absent, there are no preceding pages. If this field is
-    #: an empty string then the previous page is the first result.
-    previous_page_token: Optional[str] = None
+    #: The identifier of the item.
+    id: str = ""
+    #: The details of the associated product.
+    product: Product = dataclasses.field(default_factory=Product)
+    #: The details of the associated price.
+    price: Optional[Price] = None
+    #: The quantity for the item.
+    quantity: int = 0
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.roles is not None:
-            data["roles"] = [Role.__json_encode__(v) for v in self.roles]
+        if self.id is not None:
+            data["id"] = self.id
 
-        if self.next_page_token is not None:
-            data["nextPageToken"] = self.next_page_token
+        if self.product is not None:
+            data["product"] = Product.__json_encode__(self.product)
 
-        if self.previous_page_token is not None:
-            data["previousPageToken"] = self.previous_page_token
+        if self.price is not None:
+            data["price"] = Price.__json_encode__(self.price)
+
+        if self.quantity is not None:
+            data["quantity"] = self.quantity
 
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "ListRolesResponse":
+    def __json_decode__(data: Dict[str, Any]) -> "SubscriptionItem":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("roles") is not None:
-            kwargs["roles"] = [Role.__json_decode__(v) for v in data["roles"]]
+        if data.get("id") is not None:
+            kwargs["id"] = data["id"]
+
+        if data.get("product") is not None:
+            kwargs["product"] = Product.__json_decode__(data["product"])
 
-        if data.get("nextPageToken") is not None:
-            kwargs["next_page_token"] = data["nextPageToken"]
+        if data.get("price") is not None:
+            kwargs["price"] = Price.__json_decode__(data["price"])
 
-        if data.get("previousPageToken") is not None:
-            kwargs["previous_page_token"] = data["previousPageToken"]
+        if data.get("quantity") is not None:
+            kwargs["quantity"] = data["quantity"]
 
-        return ListRolesResponse(**kwargs)
+        return SubscriptionItem(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_list_subscriptions_response.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_role.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,90 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
 from typing import Any, Dict, List, Optional
 
-from ._subscription import Subscription
-
 
 @dataclasses.dataclass
-class ListSubscriptionsResponse:
+class Role:
     """
-    Response message for ListSubscriptions.
+    A member's role within an organization.
     """
 
-    #: The list of subscriptions.
-    subscriptions: List[Subscription] = dataclasses.field(default_factory=list)
-    #: A token, which can be sent as `pageToken` to retrieve the next page.
-    #: If this field is omitted, there are no subsequent pages.
-    next_page_token: str = ""
-    #: A token, which can be sent as `pageToken` to retrieve the previous page.
-    #: If this field is absent, there are no preceding pages. If this field is
-    #: an empty string then the previous page is the first result.
-    previous_page_token: Optional[str] = None
+    #: The system-assigned identifier of the role.
+    id: str = ""
+    #: The client defined unique identifier of the role.
+    #:
+    #: It is restricted to letters, numbers, underscores, and hyphens,
+    #: with the first character a letter or a number, and a 255
+    #: character maximum.
+    #:
+    #: ID's starting with `role_` are reserved.
+    unique_id: str = ""
+    #: The human-readable display name of the role.
+    display_name: str = ""
+    #: The role type.
+    type: str = ""
+    #: The description of the role.
+    #:
+    #: The maximum length is 1000 characters.
+    description: Optional[str] = None
+    #: The additional permissions allowed by the role.
+    permission_sets: List[str] = dataclasses.field(default_factory=list)
+    #: Whether the role is the default for the tenant.
+    default: bool = False
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.subscriptions is not None:
-            data["subscriptions"] = [
-                Subscription.__json_encode__(v) for v in self.subscriptions
-            ]
+        if self.id is not None:
+            data["id"] = self.id
+
+        if self.unique_id is not None:
+            data["uniqueId"] = self.unique_id
+
+        if self.display_name is not None:
+            data["displayName"] = self.display_name
+
+        if self.type is not None:
+            data["type"] = self.type
+
+        if self.description is not None:
+            data["description"] = self.description
 
-        if self.next_page_token is not None:
-            data["nextPageToken"] = self.next_page_token
+        if self.permission_sets is not None:
+            data["permissionSets"] = self.permission_sets
 
-        if self.previous_page_token is not None:
-            data["previousPageToken"] = self.previous_page_token
+        if self.default is not None:
+            data["default"] = self.default
 
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "ListSubscriptionsResponse":
+    def __json_decode__(data: Dict[str, Any]) -> "Role":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("subscriptions") is not None:
-            kwargs["subscriptions"] = [
-                Subscription.__json_decode__(v) for v in data["subscriptions"]
-            ]
+        if data.get("id") is not None:
+            kwargs["id"] = data["id"]
+
+        if data.get("uniqueId") is not None:
+            kwargs["unique_id"] = data["uniqueId"]
+
+        if data.get("displayName") is not None:
+            kwargs["display_name"] = data["displayName"]
+
+        if data.get("type") is not None:
+            kwargs["type"] = data["type"]
+
+        if data.get("description") is not None:
+            kwargs["description"] = data["description"]
 
-        if data.get("nextPageToken") is not None:
-            kwargs["next_page_token"] = data["nextPageToken"]
+        if data.get("permissionSets") is not None:
+            kwargs["permission_sets"] = data["permissionSets"]
 
-        if data.get("previousPageToken") is not None:
-            kwargs["previous_page_token"] = data["previousPageToken"]
+        if data.get("default") is not None:
+            kwargs["default"] = data["default"]
 
-        return ListSubscriptionsResponse(**kwargs)
+        return Role(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_member.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_member.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_membership.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_membership.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_organization.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_organization.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_organization_input.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_organization_input.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_payment_intent.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_payment_intent.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_payment_method.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_payment_method.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_payment_method_input.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_payment_method_input.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_payment_method_intent.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_payment_method_intent.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_plan.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_plan.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_plan_group.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_plan_group.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_plan_group_change_path.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_plan_group_change_path.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_plan_group_trial.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_plan_group_trial.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_plan_item.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_plan_item.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_price.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_price.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_price_fixed_price.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_price_fixed_price.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_price_tiered_price.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_price_tiered_price.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_price_transform_quantity.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_price_transform_quantity.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_product.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_product.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_role.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_session.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,86 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
+import datetime
 from typing import Any, Dict, List, Optional
 
+from userhub_sdk._internal import util
+
+from ._account_subscription import AccountSubscription
+from ._membership import Membership
+from ._user import User
+
 
 @dataclasses.dataclass
-class Role:
+class Session:
     """
-    A member's role within an organization.
+    The session details.
     """
 
-    #: The system-assigned identifier of the role.
-    id: str = ""
-    #: The client defined unique identifier of the role.
-    #:
-    #: It is restricted to letters, numbers, underscores, and hyphens,
-    #: with the first character a letter or a number, and a 255
-    #: character maximum.
+    #: The authenticated user.
     #:
-    #: ID's starting with `role_` are reserved.
-    unique_id: str = ""
-    #: The human-readable display name of the role.
-    display_name: str = ""
-    #: The role type.
-    type: str = ""
-    #: The description of the role.
+    #: This will be null if the user is not authenticated.
+    user: Optional[User] = None
+    #: The authenticated user's organization memberships.
+    memberships: Optional[List[Membership]] = dataclasses.field(default_factory=list)
+    #: The user's default active individual subscription.
     #:
-    #: The maximum length is 1000 characters.
-    description: Optional[str] = None
-    #: The additional permissions allowed by the role.
-    permission_sets: List[str] = dataclasses.field(default_factory=list)
-    #: Whether the role is the default for the tenant.
-    default: bool = False
+    #: See memberships for organization subscription and
+    #: seat information.
+    subscription: Optional[AccountSubscription] = None
+    #: The expiration time for the current session.
+    expire_time: Optional[datetime.datetime] = None
+    #: The scopes available in the current session.
+    scopes: List[str] = dataclasses.field(default_factory=list)
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.id is not None:
-            data["id"] = self.id
-
-        if self.unique_id is not None:
-            data["uniqueId"] = self.unique_id
-
-        if self.display_name is not None:
-            data["displayName"] = self.display_name
+        if self.user is not None:
+            data["user"] = User.__json_encode__(self.user)
 
-        if self.type is not None:
-            data["type"] = self.type
+        if self.memberships is not None:
+            data["memberships"] = [
+                Membership.__json_encode__(v) for v in self.memberships
+            ]
+
+        if self.subscription is not None:
+            data["subscription"] = AccountSubscription.__json_encode__(
+                self.subscription
+            )
 
-        if self.description is not None:
-            data["description"] = self.description
+        if self.expire_time is not None:
+            data["expireTime"] = util.encode_datetime(self.expire_time)
 
-        if self.permission_sets is not None:
-            data["permissionSets"] = self.permission_sets
-
-        if self.default is not None:
-            data["default"] = self.default
+        if self.scopes is not None:
+            data["scopes"] = self.scopes
 
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "Role":
+    def __json_decode__(data: Dict[str, Any]) -> "Session":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("id") is not None:
-            kwargs["id"] = data["id"]
-
-        if data.get("uniqueId") is not None:
-            kwargs["unique_id"] = data["uniqueId"]
-
-        if data.get("displayName") is not None:
-            kwargs["display_name"] = data["displayName"]
-
-        if data.get("type") is not None:
-            kwargs["type"] = data["type"]
+        if data.get("user") is not None:
+            kwargs["user"] = User.__json_decode__(data["user"])
 
-        if data.get("description") is not None:
-            kwargs["description"] = data["description"]
+        if data.get("memberships") is not None:
+            kwargs["memberships"] = [
+                Membership.__json_decode__(v) for v in data["memberships"]
+            ]
+
+        if data.get("subscription") is not None:
+            kwargs["subscription"] = AccountSubscription.__json_decode__(
+                data["subscription"]
+            )
 
-        if data.get("permissionSets") is not None:
-            kwargs["permission_sets"] = data["permissionSets"]
+        if data.get("expireTime") is not None:
+            kwargs["expire_time"] = util.decode_datetime(data["expireTime"])
 
-        if data.get("default") is not None:
-            kwargs["default"] = data["default"]
+        if data.get("scopes") is not None:
+            kwargs["scopes"] = data["scopes"]
 
-        return Role(**kwargs)
+        return Session(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_session.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_subscription_trial.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,86 +1,68 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
 import datetime
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Optional
 
 from userhub_sdk._internal import util
 
-from ._account_subscription import AccountSubscription
-from ._membership import Membership
-from ._user import User
-
 
 @dataclasses.dataclass
-class Session:
+class SubscriptionTrial:
     """
-    The session details.
+    The trial information for the subscription.
     """
 
-    #: The authenticated user.
+    #: The time the trial started.
+    start_time: Optional[datetime.datetime] = None
+    #: The time the trial ended/ends.
+    end_time: Optional[datetime.datetime] = None
+    #: The number of days in the trial.
     #:
-    #: This will be null if the user is not authenticated.
-    user: Optional[User] = None
-    #: The authenticated user's organization memberships.
-    memberships: Optional[List[Membership]] = dataclasses.field(default_factory=list)
-    #: The user's default active individual subscription.
+    #: This number is rounded to the nearest whole number
+    #: of days.
+    days: int = 0
+    #: The number of days remaining in the trial.
     #:
-    #: See memberships for organization subscription and
-    #: seat information.
-    subscription: Optional[AccountSubscription] = None
-    #: The expiration time for the current session.
-    expire_time: Optional[datetime.datetime] = None
-    #: The scopes available in the current session.
-    scopes: List[str] = dataclasses.field(default_factory=list)
+    #: This number is rounded down, so will generally be
+    #: less than days. It will be zero on the last day
+    #: of the trial and null when the trial expires.
+    remaining_days: Optional[int] = None
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.user is not None:
-            data["user"] = User.__json_encode__(self.user)
+        if self.start_time is not None:
+            data["startTime"] = util.encode_datetime(self.start_time)
 
-        if self.memberships is not None:
-            data["memberships"] = [
-                Membership.__json_encode__(v) for v in self.memberships
-            ]
-
-        if self.subscription is not None:
-            data["subscription"] = AccountSubscription.__json_encode__(
-                self.subscription
-            )
+        if self.end_time is not None:
+            data["endTime"] = util.encode_datetime(self.end_time)
 
-        if self.expire_time is not None:
-            data["expireTime"] = util.encode_datetime(self.expire_time)
+        if self.days is not None:
+            data["days"] = self.days
 
-        if self.scopes is not None:
-            data["scopes"] = self.scopes
+        if self.remaining_days is not None:
+            data["remainingDays"] = self.remaining_days
 
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "Session":
+    def __json_decode__(data: Dict[str, Any]) -> "SubscriptionTrial":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("user") is not None:
-            kwargs["user"] = User.__json_decode__(data["user"])
+        if data.get("startTime") is not None:
+            kwargs["start_time"] = util.decode_datetime(data["startTime"])
 
-        if data.get("memberships") is not None:
-            kwargs["memberships"] = [
-                Membership.__json_decode__(v) for v in data["memberships"]
-            ]
-
-        if data.get("subscription") is not None:
-            kwargs["subscription"] = AccountSubscription.__json_decode__(
-                data["subscription"]
-            )
+        if data.get("endTime") is not None:
+            kwargs["end_time"] = util.decode_datetime(data["endTime"])
 
-        if data.get("expireTime") is not None:
-            kwargs["expire_time"] = util.decode_datetime(data["expireTime"])
+        if data.get("days") is not None:
+            kwargs["days"] = data["days"]
 
-        if data.get("scopes") is not None:
-            kwargs["scopes"] = data["scopes"]
+        if data.get("remainingDays") is not None:
+            kwargs["remaining_days"] = data["remainingDays"]
 
-        return Session(**kwargs)
+        return SubscriptionTrial(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_signup_flow.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_signup_flow.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_stripe_payment_intent.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_stripe_payment_intent.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_stripe_payment_method_intent.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_stripe_payment_method_intent.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_subscription.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_subscription.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_subscription_current_period.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_subscription_current_period.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_subscription_item.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_tiered_price_tier.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,50 @@
 # Code generated. DO NOT EDIT.
 
 import dataclasses
 from typing import Any, Dict, Optional
 
-from ._price import Price
-from ._product import Product
-
 
 @dataclasses.dataclass
-class SubscriptionItem:
+class TieredPriceTier:
     """
-    The subscription items.
+    A quantity range within the tiered price.
     """
 
-    #: The identifier of the item.
-    id: str = ""
-    #: The details of the associated product.
-    product: Product = dataclasses.field(default_factory=Product)
-    #: The details of the associated price.
-    price: Optional[Price] = None
-    #: The quantity for the item.
-    quantity: int = 0
+    #: The upper quantity for tier (inclusive).
+    upper: Optional[int] = None
+    #: The per quantity amount for the tier.
+    unit_amount: Optional[str] = None
+    #: The flat amount for the tier.
+    flat_amount: Optional[str] = None
 
     def __json_encode__(self) -> Dict[str, Any]:
         data: Dict[str, Any] = {}
 
-        if self.id is not None:
-            data["id"] = self.id
-
-        if self.product is not None:
-            data["product"] = Product.__json_encode__(self.product)
+        if self.upper is not None:
+            data["upper"] = self.upper
 
-        if self.price is not None:
-            data["price"] = Price.__json_encode__(self.price)
+        if self.unit_amount is not None:
+            data["unitAmount"] = self.unit_amount
 
-        if self.quantity is not None:
-            data["quantity"] = self.quantity
+        if self.flat_amount is not None:
+            data["flatAmount"] = self.flat_amount
 
         return data
 
     @staticmethod
-    def __json_decode__(data: Dict[str, Any]) -> "SubscriptionItem":
+    def __json_decode__(data: Dict[str, Any]) -> "TieredPriceTier":
         if data is None:
             data = {}
 
         kwargs: Dict[str, Any] = {}
 
-        if data.get("id") is not None:
-            kwargs["id"] = data["id"]
-
-        if data.get("product") is not None:
-            kwargs["product"] = Product.__json_decode__(data["product"])
+        if data.get("upper") is not None:
+            kwargs["upper"] = data["upper"]
 
-        if data.get("price") is not None:
-            kwargs["price"] = Price.__json_decode__(data["price"])
+        if data.get("unitAmount") is not None:
+            kwargs["unit_amount"] = data["unitAmount"]
 
-        if data.get("quantity") is not None:
-            kwargs["quantity"] = data["quantity"]
+        if data.get("flatAmount") is not None:
+            kwargs["flat_amount"] = data["flatAmount"]
 
-        return SubscriptionItem(**kwargs)
+        return TieredPriceTier(**kwargs)
```

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_subscription_seat_info.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_subscription_seat_info.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/userv1/_user.py` & `userhub_sdk-0.6.0/src/userhub_sdk/userv1/_user.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/webhook/_actions.py` & `userhub_sdk-0.6.0/src/userhub_sdk/webhook/_actions.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/webhook/_base.py` & `userhub_sdk-0.6.0/src/userhub_sdk/webhook/_base.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/webhook/_handler.py` & `userhub_sdk-0.6.0/src/userhub_sdk/webhook/_handler.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/webhook/_http.py` & `userhub_sdk-0.6.0/src/userhub_sdk/webhook/_http.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/src/userhub_sdk/webhook/_util.py` & `userhub_sdk-0.6.0/src/userhub_sdk/webhook/_util.py`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/LICENSE` & `userhub_sdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/pyproject.toml` & `userhub_sdk-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `userhub_sdk-0.5.0/PKG-INFO` & `userhub_sdk-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: userhub-sdk
-Version: 0.5.0
+Version: 0.6.0
 Summary: UserHub Python SDK
 Project-URL: Homepage, https://userhub.com
 Project-URL: Source, https://github.com/userhubdev/python-sdk
 Author-email: UserHub <hello@userhub.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

