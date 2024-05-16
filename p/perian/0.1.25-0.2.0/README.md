# Comparing `tmp/perian-0.1.25.tar.gz` & `tmp/perian-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perian-0.1.25.tar", last modified: Wed Feb 28 14:39:34 2024, max compression
+gzip compressed data, was "perian-0.2.0.tar", last modified: Thu May 16 09:03:22 2024, max compression
```

## Comparing `perian-0.1.25.tar` & `perian-0.2.0.tar`

### file list

```diff
@@ -1,257 +1,367 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 14:39:34.355718 perian-0.1.25/
--rw-r--r--   0 root         (0) root         (0)      489 2024-02-28 14:39:34.355718 perian-0.1.25/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6241 2024-02-28 14:39:12.000000 perian-0.1.25/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 14:39:34.323716 perian-0.1.25/perian/
--rw-r--r--   0 root         (0) root         (0)     7980 2024-02-28 14:39:34.000000 perian-0.1.25/perian/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 14:39:34.323716 perian-0.1.25/perian/api/
--rw-r--r--   0 root         (0) root         (0)      342 2024-02-28 14:39:34.000000 perian-0.1.25/perian/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12056 2024-02-28 14:39:33.000000 perian-0.1.25/perian/api/admin_api.py
--rw-r--r--   0 root         (0) root         (0)    14610 2024-02-28 14:39:34.000000 perian-0.1.25/perian/api/instance_type_api.py
--rw-r--r--   0 root         (0) root         (0)    21713 2024-02-28 14:39:34.000000 perian-0.1.25/perian/api/job_api.py
--rw-r--r--   0 root         (0) root         (0)    12199 2024-02-28 14:39:34.000000 perian-0.1.25/perian/api/organization_api.py
--rw-r--r--   0 root         (0) root         (0)    12353 2024-02-28 14:39:34.000000 perian-0.1.25/perian/api/service_account_api.py
--rw-r--r--   0 root         (0) root         (0)    11735 2024-02-28 14:39:34.000000 perian-0.1.25/perian/api/user_api.py
--rw-r--r--   0 root         (0) root         (0)    25745 2024-02-28 14:39:34.000000 perian-0.1.25/perian/api_client.py
--rw-r--r--   0 root         (0) root         (0)      652 2024-02-28 14:39:34.000000 perian-0.1.25/perian/api_response.py
--rw-r--r--   0 root         (0) root         (0)    14459 2024-02-28 14:39:34.000000 perian-0.1.25/perian/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5973 2024-02-28 14:39:34.000000 perian-0.1.25/perian/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 14:39:34.339717 perian-0.1.25/perian/models/
--rw-r--r--   0 root         (0) root         (0)     7213 2024-02-28 14:39:34.000000 perian-0.1.25/perian/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3542 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/accelerator_data_view.py
--rw-r--r--   0 root         (0) root         (0)     1274 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/accelerator_name.py
--rw-r--r--   0 root         (0) root         (0)     5380 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/accelerator_query.py
--rw-r--r--   0 root         (0) root         (0)     4895 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/accelerator_query_memory.py
--rw-r--r--   0 root         (0) root         (0)     4861 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/accelerator_query_operator.py
--rw-r--r--   0 root         (0) root         (0)     4916 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/accelerator_query_options.py
--rw-r--r--   0 root         (0) root         (0)     3152 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/accelerator_type_view.py
--rw-r--r--   0 root         (0) root         (0)      807 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/accelerator_vendor.py
--rw-r--r--   0 root         (0) root         (0)     2711 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/availability.py
--rw-r--r--   0 root         (0) root         (0)     3382 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/availability_query.py
--rw-r--r--   0 root         (0) root         (0)      806 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/availability_source.py
--rw-r--r--   0 root         (0) root         (0)     3224 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/bandwidth.py
--rw-r--r--   0 root         (0) root         (0)      795 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/bandwidth_limits.py
--rw-r--r--   0 root         (0) root         (0)      848 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/bandwidth_sla.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/bandwidth_units.py
--rw-r--r--   0 root         (0) root         (0)     4809 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/command.py
--rw-r--r--   0 root         (0) root         (0)      882 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/compute_billing_period.py
--rw-r--r--   0 root         (0) root         (0)      881 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/compute_instance_type.py
--rw-r--r--   0 root         (0) root         (0)     2963 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/cpu.py
--rw-r--r--   0 root         (0) root         (0)     3220 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/cpu_data.py
--rw-r--r--   0 root         (0) root         (0)     3622 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/cpu_query.py
--rw-r--r--   0 root         (0) root         (0)     3108 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_admin_success.py
--rw-r--r--   0 root         (0) root         (0)     3091 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_global_admin_request.py
--rw-r--r--   0 root         (0) root         (0)     4238 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_job_request.py
--rw-r--r--   0 root         (0) root         (0)     5220 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_job_request_docker_registry_credentials.py
--rw-r--r--   0 root         (0) root         (0)     3091 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_job_success.py
--rw-r--r--   0 root         (0) root         (0)     2915 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_organization_request.py
--rw-r--r--   0 root         (0) root         (0)     3542 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_organization_success.py
--rw-r--r--   0 root         (0) root         (0)     2748 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_service_account_request.py
--rw-r--r--   0 root         (0) root         (0)     3458 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_service_account_success.py
--rw-r--r--   0 root         (0) root         (0)     3233 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_user_request.py
--rw-r--r--   0 root         (0) root         (0)     3088 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/create_user_success.py
--rw-r--r--   0 root         (0) root         (0)      770 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/currency.py
--rw-r--r--   0 root         (0) root         (0)     3066 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/default_client_error.py
--rw-r--r--   0 root         (0) root         (0)     3066 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/default_server_error.py
--rw-r--r--   0 root         (0) root         (0)     5508 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/description.py
--rw-r--r--   0 root         (0) root         (0)     2841 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/docker_registry_credentials.py
--rw-r--r--   0 root         (0) root         (0)     3313 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/docker_run_parameters.py
--rw-r--r--   0 root         (0) root         (0)     4877 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/done_at.py
--rw-r--r--   0 root         (0) root         (0)     3917 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/get_instance_types_success.py
--rw-r--r--   0 root         (0) root         (0)     3508 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/get_jobs_success.py
--rw-r--r--   0 root         (0) root         (0)     2963 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/http_validation_error.py
--rw-r--r--   0 root         (0) root         (0)     5451 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/id.py
--rw-r--r--   0 root         (0) root         (0)     4815 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/image_tag.py
--rw-r--r--   0 root         (0) root         (0)     3198 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_blocked_error.py
--rw-r--r--   0 root         (0) root         (0)     9076 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query.py
--rw-r--r--   0 root         (0) root         (0)     5006 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_accelerator.py
--rw-r--r--   0 root         (0) root         (0)     5027 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_availability.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_cpu.py
--rw-r--r--   0 root         (0) root         (0)     4859 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_name.py
--rw-r--r--   0 root         (0) root         (0)     4922 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_network.py
--rw-r--r--   0 root         (0) root         (0)     4880 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_price.py
--rw-r--r--   0 root         (0) root         (0)     4943 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_provider.py
--rw-r--r--   0 root         (0) root         (0)     5007 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_reference_id.py
--rw-r--r--   0 root         (0) root         (0)     4901 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_region.py
--rw-r--r--   0 root         (0) root         (0)     4922 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_storage.py
--rw-r--r--   0 root         (0) root         (0)     4859 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_type.py
--rw-r--r--   0 root         (0) root         (0)     4859 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_query_zone.py
--rw-r--r--   0 root         (0) root         (0)     6409 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/instance_type_view.py
--rw-r--r--   0 root         (0) root         (0)      843 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/job_status.py
--rw-r--r--   0 root         (0) root         (0)     3308 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/job_view.py
--rw-r--r--   0 root         (0) root         (0)     1200 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/location.py
--rw-r--r--   0 root         (0) root         (0)     4791 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/logs.py
--rw-r--r--   0 root         (0) root         (0)     3181 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/memory.py
--rw-r--r--   0 root         (0) root         (0)      761 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/memory_interface.py
--rw-r--r--   0 root         (0) root         (0)     3376 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/memory_query.py
--rw-r--r--   0 root         (0) root         (0)      742 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/memory_unit.py
--rw-r--r--   0 root         (0) root         (0)     4791 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/name.py
--rw-r--r--   0 root         (0) root         (0)     3328 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/name_query.py
--rw-r--r--   0 root         (0) root         (0)     3061 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/network.py
--rw-r--r--   0 root         (0) root         (0)     3558 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/network_query.py
--rw-r--r--   0 root         (0) root         (0)     3114 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/no_job_found_error.py
--rw-r--r--   0 root         (0) root         (0)      770 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/operator.py
--rw-r--r--   0 root         (0) root         (0)     2479 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/organization.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/organization_name_error.py
--rw-r--r--   0 root         (0) root         (0)     3246 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/organization_name_exists_error.py
--rw-r--r--   0 root         (0) root         (0)     2526 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/os_storage_config.py
--rw-r--r--   0 root         (0) root         (0)     2639 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/price.py
--rw-r--r--   0 root         (0) root         (0)     3048 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/price_data.py
--rw-r--r--   0 root         (0) root         (0)     3607 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/price_query.py
--rw-r--r--   0 root         (0) root         (0)     4118 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/provider.py
--rw-r--r--   0 root         (0) root         (0)      782 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/provider_capabilities.py
--rw-r--r--   0 root         (0) root         (0)      976 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/provider_name.py
--rw-r--r--   0 root         (0) root         (0)     2645 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/provider_properties.py
--rw-r--r--   0 root         (0) root         (0)     3931 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/provider_query.py
--rw-r--r--   0 root         (0) root         (0)     4873 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/provider_specific_name.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/query_options.py
--rw-r--r--   0 root         (0) root         (0)     4821 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/reference.py
--rw-r--r--   0 root         (0) root         (0)     3348 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/reference_id_query.py
--rw-r--r--   0 root         (0) root         (0)     3547 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/region.py
--rw-r--r--   0 root         (0) root         (0)     3940 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/region_query.py
--rw-r--r--   0 root         (0) root         (0)     5122 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/response400_create_global_admin_admin_post.py
--rw-r--r--   0 root         (0) root         (0)     6204 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/response400_create_organization_organization_post.py
--rw-r--r--   0 root         (0) root         (0)     5225 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/response400_create_service_account_service_account_post.py
--rw-r--r--   0 root         (0) root         (0)     5105 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/response400_create_user_user_post.py
--rw-r--r--   0 root         (0) root         (0)     4961 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/response_get_job_job_get.py
--rw-r--r--   0 root         (0) root         (0)     3122 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/role_not_valid_error.py
--rw-r--r--   0 root         (0) root         (0)     3124 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/setup_token_error.py
--rw-r--r--   0 root         (0) root         (0)      764 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/status.py
--rw-r--r--   0 root         (0) root         (0)     3176 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/storage.py
--rw-r--r--   0 root         (0) root         (0)     3524 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/storage_data.py
--rw-r--r--   0 root         (0) root         (0)      803 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/storage_included.py
--rw-r--r--   0 root         (0) root         (0)     3751 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/storage_query.py
--rw-r--r--   0 root         (0) root         (0)      781 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/storage_type.py
--rw-r--r--   0 root         (0) root         (0)     3328 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/type_query.py
--rw-r--r--   0 root         (0) root         (0)     3064 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/validation_error.py
--rw-r--r--   0 root         (0) root         (0)     4890 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/validation_error_loc_inner.py
--rw-r--r--   0 root         (0) root         (0)     4803 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/vendor.py
--rw-r--r--   0 root         (0) root         (0)     2648 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/zone.py
--rw-r--r--   0 root         (0) root         (0)     3711 2024-02-28 14:39:33.000000 perian-0.1.25/perian/models/zone_query.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-02-28 14:39:34.000000 perian-0.1.25/perian/py.typed
--rw-r--r--   0 root         (0) root         (0)     9225 2024-02-28 14:39:34.000000 perian-0.1.25/perian/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 14:39:34.355718 perian-0.1.25/perian.egg-info/
--rw-r--r--   0 root         (0) root         (0)      489 2024-02-28 14:39:34.000000 perian-0.1.25/perian.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8170 2024-02-28 14:39:34.000000 perian-0.1.25/perian.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 14:39:34.000000 perian-0.1.25/perian.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-02-28 14:39:34.000000 perian-0.1.25/perian.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-28 14:39:34.000000 perian-0.1.25/perian.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      702 2024-02-28 14:39:12.000000 perian-0.1.25/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       69 2024-02-28 14:39:34.355718 perian-0.1.25/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1306 2024-02-28 14:39:34.000000 perian-0.1.25/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 14:39:34.355718 perian-0.1.25/test/
--rw-r--r--   0 root         (0) root         (0)     1925 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_accelerator_data_view.py
--rw-r--r--   0 root         (0) root         (0)      711 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_accelerator_name.py
--rw-r--r--   0 root         (0) root         (0)     1633 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_accelerator_query.py
--rw-r--r--   0 root         (0) root         (0)     1536 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_accelerator_query_memory.py
--rw-r--r--   0 root         (0) root         (0)     1467 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_accelerator_query_operator.py
--rw-r--r--   0 root         (0) root         (0)     1549 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_accelerator_query_options.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_accelerator_type_view.py
--rw-r--r--   0 root         (0) root         (0)      725 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_accelerator_vendor.py
--rw-r--r--   0 root         (0) root         (0)      779 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_admin_api.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_availability.py
--rw-r--r--   0 root         (0) root         (0)     1480 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_availability_query.py
--rw-r--r--   0 root         (0) root         (0)      732 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_availability_source.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_bandwidth.py
--rw-r--r--   0 root         (0) root         (0)      711 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_bandwidth_limits.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_bandwidth_sla.py
--rw-r--r--   0 root         (0) root         (0)      704 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_bandwidth_units.py
--rw-r--r--   0 root         (0) root         (0)     1261 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_command.py
--rw-r--r--   0 root         (0) root         (0)      747 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_compute_billing_period.py
--rw-r--r--   0 root         (0) root         (0)      740 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_compute_instance_type.py
--rw-r--r--   0 root         (0) root         (0)     1545 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_cpu.py
--rw-r--r--   0 root         (0) root         (0)     1551 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_cpu_data.py
--rw-r--r--   0 root         (0) root         (0)     1452 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_cpu_query.py
--rw-r--r--   0 root         (0) root         (0)     1580 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_admin_success.py
--rw-r--r--   0 root         (0) root         (0)     1630 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_global_admin_request.py
--rw-r--r--   0 root         (0) root         (0)     1793 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_job_request.py
--rw-r--r--   0 root         (0) root         (0)     1767 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_job_request_docker_registry_credentials.py
--rw-r--r--   0 root         (0) root         (0)     1573 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_job_success.py
--rw-r--r--   0 root         (0) root         (0)     1539 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_organization_request.py
--rw-r--r--   0 root         (0) root         (0)     1876 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_organization_success.py
--rw-r--r--   0 root         (0) root         (0)     1618 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_service_account_request.py
--rw-r--r--   0 root         (0) root         (0)     1760 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_service_account_success.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_create_user_success.py
--rw-r--r--   0 root         (0) root         (0)      661 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_currency.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_default_client_error.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_default_server_error.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_description.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_docker_registry_credentials.py
--rw-r--r--   0 root         (0) root         (0)     1505 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_docker_run_parameters.py
--rw-r--r--   0 root         (0) root         (0)     1250 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_done_at.py
--rw-r--r--   0 root         (0) root         (0)     2305 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_get_instance_types_success.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_get_jobs_success.py
--rw-r--r--   0 root         (0) root         (0)     1693 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_http_validation_error.py
--rw-r--r--   0 root         (0) root         (0)     1201 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_id.py
--rw-r--r--   0 root         (0) root         (0)     1274 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_image_tag.py
--rw-r--r--   0 root         (0) root         (0)      823 2024-02-28 14:39:34.000000 perian-0.1.25/test/test_instance_type_api.py
--rw-r--r--   0 root         (0) root         (0)     1686 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_blocked_error.py
--rw-r--r--   0 root         (0) root         (0)     1885 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query.py
--rw-r--r--   0 root         (0) root         (0)     1781 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_accelerator.py
--rw-r--r--   0 root         (0) root         (0)     1626 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_availability.py
--rw-r--r--   0 root         (0) root         (0)     1603 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_cpu.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_name.py
--rw-r--r--   0 root         (0) root         (0)     1609 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_network.py
--rw-r--r--   0 root         (0) root         (0)     1605 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_price.py
--rw-r--r--   0 root         (0) root         (0)     1699 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_provider.py
--rw-r--r--   0 root         (0) root         (0)     1608 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_reference_id.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_region.py
--rw-r--r--   0 root         (0) root         (0)     1680 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_storage.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_type.py
--rw-r--r--   0 root         (0) root         (0)     1583 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_query_zone.py
--rw-r--r--   0 root         (0) root         (0)     5189 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_instance_type_view.py
--rw-r--r--   0 root         (0) root         (0)      866 2024-02-28 14:39:34.000000 perian-0.1.25/test/test_job_api.py
--rw-r--r--   0 root         (0) root         (0)      669 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_job_status.py
--rw-r--r--   0 root         (0) root         (0)     1382 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_job_view.py
--rw-r--r--   0 root         (0) root         (0)      661 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_location.py
--rw-r--r--   0 root         (0) root         (0)     1225 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_logs.py
--rw-r--r--   0 root         (0) root         (0)     1622 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_memory.py
--rw-r--r--   0 root         (0) root         (0)      711 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_memory_interface.py
--rw-r--r--   0 root         (0) root         (0)     1404 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_memory_query.py
--rw-r--r--   0 root         (0) root         (0)      676 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_memory_unit.py
--rw-r--r--   0 root         (0) root         (0)     1225 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_name.py
--rw-r--r--   0 root         (0) root         (0)     1377 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_name_query.py
--rw-r--r--   0 root         (0) root         (0)     1815 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_network.py
--rw-r--r--   0 root         (0) root         (0)     1465 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_network_query.py
--rw-r--r--   0 root         (0) root         (0)     1554 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_no_job_found_error.py
--rw-r--r--   0 root         (0) root         (0)      661 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_operator.py
--rw-r--r--   0 root         (0) root         (0)     1347 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_organization.py
--rw-r--r--   0 root         (0) root         (0)      828 2024-02-28 14:39:34.000000 perian-0.1.25/test/test_organization_api.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_organization_name_error.py
--rw-r--r--   0 root         (0) root         (0)     1740 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_organization_name_exists_error.py
--rw-r--r--   0 root         (0) root         (0)     1385 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_os_storage_config.py
--rw-r--r--   0 root         (0) root         (0)     1300 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_price.py
--rw-r--r--   0 root         (0) root         (0)     1500 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_price_data.py
--rw-r--r--   0 root         (0) root         (0)     1459 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_price_query.py
--rw-r--r--   0 root         (0) root         (0)     2257 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_provider.py
--rw-r--r--   0 root         (0) root         (0)      746 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_provider_capabilities.py
--rw-r--r--   0 root         (0) root         (0)      690 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_provider_name.py
--rw-r--r--   0 root         (0) root         (0)     1448 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_provider_properties.py
--rw-r--r--   0 root         (0) root         (0)     1545 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_provider_query.py
--rw-r--r--   0 root         (0) root         (0)     1419 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_provider_specific_name.py
--rw-r--r--   0 root         (0) root         (0)     1414 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_query_options.py
--rw-r--r--   0 root         (0) root         (0)     1285 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_reference.py
--rw-r--r--   0 root         (0) root         (0)     1460 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_reference_id_query.py
--rw-r--r--   0 root         (0) root         (0)     1636 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_region.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_region_query.py
--rw-r--r--   0 root         (0) root         (0)     1755 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_response400_create_global_admin_admin_post.py
--rw-r--r--   0 root         (0) root         (0)     1850 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_response400_create_organization_organization_post.py
--rw-r--r--   0 root         (0) root         (0)     1900 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_response400_create_service_account_service_account_post.py
--rw-r--r--   0 root         (0) root         (0)     1658 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_response400_create_user_user_post.py
--rw-r--r--   0 root         (0) root         (0)     1608 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_response_get_job_job_get.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_role_not_valid_error.py
--rw-r--r--   0 root         (0) root         (0)      854 2024-02-28 14:39:34.000000 perian-0.1.25/test/test_service_account_api.py
--rw-r--r--   0 root         (0) root         (0)     1558 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_setup_token_error.py
--rw-r--r--   0 root         (0) root         (0)      647 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_status.py
--rw-r--r--   0 root         (0) root         (0)     1767 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_storage.py
--rw-r--r--   0 root         (0) root         (0)     1794 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_storage_data.py
--rw-r--r--   0 root         (0) root         (0)      711 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_storage_included.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_storage_query.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_storage_type.py
--rw-r--r--   0 root         (0) root         (0)     1377 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_type_query.py
--rw-r--r--   0 root         (0) root         (0)      748 2024-02-28 14:39:34.000000 perian-0.1.25/test/test_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1607 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_validation_error.py
--rw-r--r--   0 root         (0) root         (0)     1456 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_validation_error_loc_inner.py
--rw-r--r--   0 root         (0) root         (0)     1249 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_vendor.py
--rw-r--r--   0 root         (0) root         (0)     1311 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_zone.py
--rw-r--r--   0 root         (0) root         (0)     1433 2024-02-28 14:39:33.000000 perian-0.1.25/test/test_zone_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 09:03:22.237855 perian-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)      488 2024-05-16 09:03:22.237855 perian-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6241 2024-05-16 09:02:49.000000 perian-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 09:03:22.125855 perian-0.2.0/perian/
+-rw-r--r--   0 root         (0) root         (0)    11921 2024-05-16 09:03:21.000000 perian-0.2.0/perian/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 09:03:22.129855 perian-0.2.0/perian/api/
+-rw-r--r--   0 root         (0) root         (0)      252 2024-05-16 09:03:21.000000 perian-0.2.0/perian/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31701 2024-05-16 09:03:21.000000 perian-0.2.0/perian/api/accelerator_type_api.py
+-rw-r--r--   0 root         (0) root         (0)    13762 2024-05-16 09:03:21.000000 perian-0.2.0/perian/api/billing_api.py
+-rw-r--r--   0 root         (0) root         (0)    25075 2024-05-16 09:03:21.000000 perian-0.2.0/perian/api/instance_type_api.py
+-rw-r--r--   0 root         (0) root         (0)    42150 2024-05-16 09:03:21.000000 perian-0.2.0/perian/api/job_api.py
+-rw-r--r--   0 root         (0) root         (0)    25744 2024-05-16 09:03:21.000000 perian-0.2.0/perian/api_client.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-05-16 09:03:21.000000 perian-0.2.0/perian/api_response.py
+-rw-r--r--   0 root         (0) root         (0)    14458 2024-05-16 09:03:21.000000 perian-0.2.0/perian/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5973 2024-05-16 09:03:21.000000 perian-0.2.0/perian/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 09:03:22.181855 perian-0.2.0/perian/models/
+-rw-r--r--   0 root         (0) root         (0)    11245 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_data_view.py
+-rw-r--r--   0 root         (0) root         (0)     5671 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     5001 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_query_input_memory.py
+-rw-r--r--   0 root         (0) root         (0)     4891 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_query_input_operator.py
+-rw-r--r--   0 root         (0) root         (0)     4946 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_query_input_options.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     5022 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_query_output_memory.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_type_not_found_error.py
+-rw-r--r--   0 root         (0) root         (0)     5960 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_type_query.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_type_view.py
+-rw-r--r--   0 root         (0) root         (0)      807 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/accelerator_vendor.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/api_router_accelerator_type_incorrect_parameter_error.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/api_router_instance_type_incorrect_parameter_error.py
+-rw-r--r--   0 root         (0) root         (0)     3258 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/api_router_instance_type_instance_type_not_found_error.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/api_router_job_instance_type_not_found_error.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/availability.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/availability_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/availability_query_output.py
+-rw-r--r--   0 root         (0) root         (0)      806 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/availability_source.py
+-rw-r--r--   0 root         (0) root         (0)     4843 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/available.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/bandwidth.py
+-rw-r--r--   0 root         (0) root         (0)      795 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/bandwidth_limits.py
+-rw-r--r--   0 root         (0) root         (0)      848 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/bandwidth_sla.py
+-rw-r--r--   0 root         (0) root         (0)      862 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/bandwidth_units.py
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/bill.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/bill_item.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/billing_granularity.py
+-rw-r--r--   0 root         (0) root         (0)     4809 2024-05-16 09:03:19.000000 perian-0.2.0/perian/models/command.py
+-rw-r--r--   0 root         (0) root         (0)      881 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/compute_instance_type.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/cores.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     3220 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/cpu_data.py
+-rw-r--r--   0 root         (0) root         (0)     4608 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/cpu_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     4377 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/cpu_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     5309 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/create_job_request.py
+-rw-r--r--   0 root         (0) root         (0)     5220 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/create_job_request_docker_registry_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/create_job_request_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/create_job_success.py
+-rw-r--r--   0 root         (0) root         (0)      770 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/currency.py
+-rw-r--r--   0 root         (0) root         (0)     4820 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/currency1.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/default_client_error.py
+-rw-r--r--   0 root         (0) root         (0)     3066 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/default_server_error.py
+-rw-r--r--   0 root         (0) root         (0)     3026 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/default_success.py
+-rw-r--r--   0 root         (0) root         (0)     5508 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/description.py
+-rw-r--r--   0 root         (0) root         (0)     3607 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/docker_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/docker_registry_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/docker_run_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     4877 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/done_at.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/end_time.py
+-rw-r--r--   0 root         (0) root         (0)     4803 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/get_accelerator_type_request.py
+-rw-r--r--   0 root         (0) root         (0)     4276 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/get_accelerator_types_success.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/get_instance_type_request.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/get_instance_types_success.py
+-rw-r--r--   0 root         (0) root         (0)     4184 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/get_jobs_success.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/http_validation_error.py
+-rw-r--r--   0 root         (0) root         (0)     5451 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/id.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/id1.py
+-rw-r--r--   0 root         (0) root         (0)     4815 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/image_tag.py
+-rw-r--r--   0 root         (0) root         (0)     5614 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/inbound_speed.py
+-rw-r--r--   0 root         (0) root         (0)     4815 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/included.py
+-rw-r--r--   0 root         (0) root         (0)     3276 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/incorrect_create_job_parameter_error.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_id.py
+-rw-r--r--   0 root         (0) root         (0)     9231 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     5112 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input_accelerator.py
+-rw-r--r--   0 root         (0) root         (0)     5133 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input_availability.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input_cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5028 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input_network.py
+-rw-r--r--   0 root         (0) root         (0)     4986 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input_price.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input_provider.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input_reference_id.py
+-rw-r--r--   0 root         (0) root         (0)     5007 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input_region.py
+-rw-r--r--   0 root         (0) root         (0)     5028 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input_storage.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_input_zone.py
+-rw-r--r--   0 root         (0) root         (0)     9279 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     5133 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output_accelerator.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output_availability.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output_cpu.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output_network.py
+-rw-r--r--   0 root         (0) root         (0)     5007 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output_price.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output_provider.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output_reference_id.py
+-rw-r--r--   0 root         (0) root         (0)     5028 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output_region.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output_storage.py
+-rw-r--r--   0 root         (0) root         (0)     4986 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_query_output_zone.py
+-rw-r--r--   0 root         (0) root         (0)     6409 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_type_view.py
+-rw-r--r--   0 root         (0) root         (0)     8256 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/instance_typer_query_view.py
+-rw-r--r--   0 root         (0) root         (0)     3176 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/job_already_done_error.py
+-rw-r--r--   0 root         (0) root         (0)      911 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/job_status.py
+-rw-r--r--   0 root         (0) root         (0)     5941 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/job_view.py
+-rw-r--r--   0 root         (0) root         (0)     4934 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/job_view_docker_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     5039 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/job_view_requirement_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     4955 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/job_view_runtime_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/limit.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/location.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/location1.py
+-rw-r--r--   0 root         (0) root         (0)     4791 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/logs.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/memory.py
+-rw-r--r--   0 root         (0) root         (0)      761 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/memory_interface.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/memory_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     3402 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/memory_query_output.py
+-rw-r--r--   0 root         (0) root         (0)      742 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/memory_unit.py
+-rw-r--r--   0 root         (0) root         (0)     5466 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/name.py
+-rw-r--r--   0 root         (0) root         (0)     4797 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/name1.py
+-rw-r--r--   0 root         (0) root         (0)     4821 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/name_short.py
+-rw-r--r--   0 root         (0) root         (0)     3061 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/network.py
+-rw-r--r--   0 root         (0) root         (0)     4188 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/network_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     3564 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/network_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/next_page.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/no.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/no_job_found_error.py
+-rw-r--r--   0 root         (0) root         (0)     3122 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/no_parameter_error.py
+-rw-r--r--   0 root         (0) root         (0)     4814 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/offset.py
+-rw-r--r--   0 root         (0) root         (0)      770 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/operator.py
+-rw-r--r--   0 root         (0) root         (0)      762 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/order_criterion.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/os_storage_config.py
+-rw-r--r--   0 root         (0) root         (0)     5620 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/outbound_speed.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/pagination_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/previous_page.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/price_data.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/price_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/price_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/provider.py
+-rw-r--r--   0 root         (0) root         (0)      782 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/provider_capabilities.py
+-rw-r--r--   0 root         (0) root         (0)      976 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/provider_name.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/provider_properties.py
+-rw-r--r--   0 root         (0) root         (0)     5047 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/provider_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/provider_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/provider_specific_name.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/query_options.py
+-rw-r--r--   0 root         (0) root         (0)     3622 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/reference_id_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     3626 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/reference_id_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/region.py
+-rw-r--r--   0 root         (0) root         (0)     5055 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/region_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     5059 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/region_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2024-05-16 09:03:20.000000 perian-0.2.0/perian/models/requirement_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     5131 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/requirement_metadata_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     5845 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/response400_cancel_job.py
+-rw-r--r--   0 root         (0) root         (0)     6375 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/response400_create_job.py
+-rw-r--r--   0 root         (0) root         (0)     6542 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/response400_get_accelerator_type_by_id.py
+-rw-r--r--   0 root         (0) root         (0)     6602 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/response400_get_accelerator_type_by_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/response400_get_instance_type_by_id.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/response400_get_instance_type_by_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/response400_get_job_by_id.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/runtime_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     5566 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/size.py
+-rw-r--r--   0 root         (0) root         (0)     5572 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/speed.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/start_time.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/started_at.py
+-rw-r--r--   0 root         (0) root         (0)      764 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/status.py
+-rw-r--r--   0 root         (0) root         (0)     4809 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/status1.py
+-rw-r--r--   0 root         (0) root         (0)     3176 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/storage.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/storage_data.py
+-rw-r--r--   0 root         (0) root         (0)      803 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/storage_included.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/storage_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/storage_query_output.py
+-rw-r--r--   0 root         (0) root         (0)      781 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/storage_type.py
+-rw-r--r--   0 root         (0) root         (0)     4855 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/sustainable.py
+-rw-r--r--   0 root         (0) root         (0)     4820 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/threads.py
+-rw-r--r--   0 root         (0) root         (0)     4791 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/type.py
+-rw-r--r--   0 root         (0) root         (0)     5596 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/unit_price.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)     4890 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/validation_error_loc_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4803 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/vendor.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/zone.py
+-rw-r--r--   0 root         (0) root         (0)     4262 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/zone_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2024-05-16 09:03:21.000000 perian-0.2.0/perian/models/zone_query_output.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 09:03:21.000000 perian-0.2.0/perian/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9225 2024-05-16 09:03:21.000000 perian-0.2.0/perian/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 09:03:22.237855 perian-0.2.0/perian.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      488 2024-05-16 09:03:22.000000 perian-0.2.0/perian.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12474 2024-05-16 09:03:22.000000 perian-0.2.0/perian.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 09:03:22.000000 perian-0.2.0/perian.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-16 09:03:22.000000 perian-0.2.0/perian.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-16 09:03:22.000000 perian-0.2.0/perian.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-05-16 09:02:49.000000 perian-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-16 09:03:22.237855 perian-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-05-16 09:03:21.000000 perian-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 09:03:22.237855 perian-0.2.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1931 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_data_view.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_query_input_memory.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_query_input_operator.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_query_input_options.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     1609 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_query_output_memory.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_accelerator_type_api.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_type_not_found_error.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_type_query.py
+-rw-r--r--   0 root         (0) root         (0)     1704 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_type_view.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_accelerator_vendor.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_api_router_accelerator_type_incorrect_parameter_error.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_api_router_instance_type_incorrect_parameter_error.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_api_router_instance_type_instance_type_not_found_error.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_api_router_job_instance_type_not_found_error.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_availability.py
+-rw-r--r--   0 root         (0) root         (0)     1541 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_availability_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_availability_query_output.py
+-rw-r--r--   0 root         (0) root         (0)      732 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_availability_source.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_available.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_bandwidth.py
+-rw-r--r--   0 root         (0) root         (0)      711 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_bandwidth_limits.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_bandwidth_sla.py
+-rw-r--r--   0 root         (0) root         (0)      704 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_bandwidth_units.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_bill.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_bill_item.py
+-rw-r--r--   0 root         (0) root         (0)      749 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_billing_api.py
+-rw-r--r--   0 root         (0) root         (0)      732 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_billing_granularity.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-05-16 09:03:19.000000 perian-0.2.0/test/test_command.py
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_compute_instance_type.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_cores.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_cpu.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_cpu_data.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_cpu_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_cpu_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_create_job_request.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_create_job_request_docker_registry_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     2018 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_create_job_request_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_create_job_success.py
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_currency.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_currency1.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_default_client_error.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_default_server_error.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_default_success.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_description.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_docker_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_docker_registry_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_docker_run_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_done_at.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_end_time.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_get_accelerator_type_request.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_get_accelerator_types_success.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_get_instance_type_request.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_get_instance_types_success.py
+-rw-r--r--   0 root         (0) root         (0)     2409 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_get_jobs_success.py
+-rw-r--r--   0 root         (0) root         (0)     1693 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_http_validation_error.py
+-rw-r--r--   0 root         (0) root         (0)     1201 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_id.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_id1.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_image_tag.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_inbound_speed.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_included.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_incorrect_create_job_parameter_error.py
+-rw-r--r--   0 root         (0) root         (0)      995 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_instance_type_api.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_id.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input_accelerator.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input_availability.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input_cpu.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input_network.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input_price.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input_reference_id.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input_region.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_input_zone.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output_accelerator.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output_availability.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output_cpu.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output_network.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output_price.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output_reference_id.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output_region.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_query_output_zone.py
+-rw-r--r--   0 root         (0) root         (0)     5132 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_type_view.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_instance_typer_query_view.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_job_already_done_error.py
+-rw-r--r--   0 root         (0) root         (0)     1098 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_job_api.py
+-rw-r--r--   0 root         (0) root         (0)      669 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_job_status.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_job_view.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_job_view_docker_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1647 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_job_view_requirement_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_job_view_runtime_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_limit.py
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_location.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_location1.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_logs.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_memory.py
+-rw-r--r--   0 root         (0) root         (0)      711 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_memory_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_memory_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_memory_query_output.py
+-rw-r--r--   0 root         (0) root         (0)      676 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_memory_unit.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_name.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_name1.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_name_short.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_network.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_network_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1532 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_network_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_next_page.py
+-rw-r--r--   0 root         (0) root         (0)     1201 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_no.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_no_job_found_error.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_no_parameter_error.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_offset.py
+-rw-r--r--   0 root         (0) root         (0)      661 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_operator.py
+-rw-r--r--   0 root         (0) root         (0)      704 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_order_criterion.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_os_storage_config.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_outbound_speed.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_pagination_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_previous_page.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_price_data.py
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_price_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_price_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_provider.py
+-rw-r--r--   0 root         (0) root         (0)      746 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_provider_capabilities.py
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_provider_name.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_provider_properties.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_provider_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_provider_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_provider_specific_name.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_query_options.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_reference_id_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_reference_id_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_region.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_region_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_region_query_output.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2024-05-16 09:03:20.000000 perian-0.2.0/test/test_requirement_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_requirement_metadata_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_response400_cancel_job.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_response400_create_job.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_response400_get_accelerator_type_by_id.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_response400_get_accelerator_type_by_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_response400_get_instance_type_by_id.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_response400_get_instance_type_by_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_response400_get_job_by_id.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_runtime_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_size.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_speed.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_start_time.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_started_at.py
+-rw-r--r--   0 root         (0) root         (0)      647 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_status.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_status1.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_storage_data.py
+-rw-r--r--   0 root         (0) root         (0)      711 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_storage_included.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_storage_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_storage_query_output.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_storage_type.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_sustainable.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_threads.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_type.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_unit_price.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_validation_error.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_validation_error_loc_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_vendor.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_zone.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_zone_query_input.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2024-05-16 09:03:21.000000 perian-0.2.0/test/test_zone_query_output.py
```

### Comparing `perian-0.1.25/README.md` & `perian-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/__init__.py` & `perian-0.2.0/perian/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,139 +10,194 @@
     The version of the OpenAPI document: 0.1.24
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.1.25"
+__version__ = "0.2.0"
 
 # import apis into sdk package
-from perian.api.admin_api import AdminApi
+from perian.api.accelerator_type_api import AcceleratorTypeApi
+from perian.api.billing_api import BillingApi
 from perian.api.instance_type_api import InstanceTypeApi
 from perian.api.job_api import JobApi
-from perian.api.organization_api import OrganizationApi
-from perian.api.service_account_api import ServiceAccountApi
-from perian.api.user_api import UserApi
 
 # import ApiClient
 from perian.api_response import ApiResponse
 from perian.api_client import ApiClient
 from perian.configuration import Configuration
 from perian.exceptions import OpenApiException
 from perian.exceptions import ApiTypeError
 from perian.exceptions import ApiValueError
 from perian.exceptions import ApiKeyError
 from perian.exceptions import ApiAttributeError
 from perian.exceptions import ApiException
 
 # import models into sdk package
 from perian.models.accelerator_data_view import AcceleratorDataView
-from perian.models.accelerator_name import AcceleratorName
-from perian.models.accelerator_query import AcceleratorQuery
-from perian.models.accelerator_query_memory import AcceleratorQueryMemory
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input import AcceleratorQueryInput
+from perian.models.accelerator_query_input_memory import AcceleratorQueryInputMemory
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
+from perian.models.accelerator_query_output import AcceleratorQueryOutput
+from perian.models.accelerator_query_output_memory import AcceleratorQueryOutputMemory
+from perian.models.accelerator_type_not_found_error import AcceleratorTypeNotFoundError
+from perian.models.accelerator_type_query import AcceleratorTypeQuery
 from perian.models.accelerator_type_view import AcceleratorTypeView
 from perian.models.accelerator_vendor import AcceleratorVendor
+from perian.models.api_router_accelerator_type_incorrect_parameter_error import ApiRouterAcceleratorTypeIncorrectParameterError
+from perian.models.api_router_instance_type_incorrect_parameter_error import ApiRouterInstanceTypeIncorrectParameterError
+from perian.models.api_router_instance_type_instance_type_not_found_error import ApiRouterInstanceTypeInstanceTypeNotFoundError
+from perian.models.api_router_job_instance_type_not_found_error import ApiRouterJobInstanceTypeNotFoundError
 from perian.models.availability import Availability
-from perian.models.availability_query import AvailabilityQuery
+from perian.models.availability_query_input import AvailabilityQueryInput
+from perian.models.availability_query_output import AvailabilityQueryOutput
 from perian.models.availability_source import AvailabilitySource
+from perian.models.available import Available
 from perian.models.bandwidth import Bandwidth
 from perian.models.bandwidth_limits import BandwidthLimits
 from perian.models.bandwidth_sla import BandwidthSla
 from perian.models.bandwidth_units import BandwidthUnits
+from perian.models.bill import Bill
+from perian.models.bill_item import BillItem
+from perian.models.billing_granularity import BillingGranularity
 from perian.models.command import Command
-from perian.models.compute_billing_period import ComputeBillingPeriod
 from perian.models.compute_instance_type import ComputeInstanceType
+from perian.models.cores import Cores
 from perian.models.cpu import Cpu
 from perian.models.cpu_data import CpuData
-from perian.models.cpu_query import CpuQuery
-from perian.models.create_admin_success import CreateAdminSuccess
-from perian.models.create_global_admin_request import CreateGlobalAdminRequest
+from perian.models.cpu_query_input import CpuQueryInput
+from perian.models.cpu_query_output import CpuQueryOutput
 from perian.models.create_job_request import CreateJobRequest
 from perian.models.create_job_request_docker_registry_credentials import CreateJobRequestDockerRegistryCredentials
+from perian.models.create_job_request_requirements import CreateJobRequestRequirements
 from perian.models.create_job_success import CreateJobSuccess
-from perian.models.create_organization_request import CreateOrganizationRequest
-from perian.models.create_organization_success import CreateOrganizationSuccess
-from perian.models.create_service_account_request import CreateServiceAccountRequest
-from perian.models.create_service_account_success import CreateServiceAccountSuccess
-from perian.models.create_user_request import CreateUserRequest
-from perian.models.create_user_success import CreateUserSuccess
 from perian.models.currency import Currency
+from perian.models.currency1 import Currency1
 from perian.models.default_client_error import DefaultClientError
 from perian.models.default_server_error import DefaultServerError
+from perian.models.default_success import DefaultSuccess
 from perian.models.description import Description
+from perian.models.docker_metadata import DockerMetadata
 from perian.models.docker_registry_credentials import DockerRegistryCredentials
 from perian.models.docker_run_parameters import DockerRunParameters
 from perian.models.done_at import DoneAt
+from perian.models.end_time import EndTime
+from perian.models.errors import Errors
+from perian.models.get_accelerator_type_request import GetAcceleratorTypeRequest
+from perian.models.get_accelerator_types_success import GetAcceleratorTypesSuccess
+from perian.models.get_instance_type_request import GetInstanceTypeRequest
 from perian.models.get_instance_types_success import GetInstanceTypesSuccess
 from perian.models.get_jobs_success import GetJobsSuccess
 from perian.models.http_validation_error import HTTPValidationError
 from perian.models.id import Id
+from perian.models.id1 import Id1
 from perian.models.image_tag import ImageTag
-from perian.models.instance_type_blocked_error import InstanceTypeBlockedError
-from perian.models.instance_type_query import InstanceTypeQuery
-from perian.models.instance_type_query_accelerator import InstanceTypeQueryAccelerator
-from perian.models.instance_type_query_availability import InstanceTypeQueryAvailability
-from perian.models.instance_type_query_cpu import InstanceTypeQueryCpu
-from perian.models.instance_type_query_name import InstanceTypeQueryName
-from perian.models.instance_type_query_network import InstanceTypeQueryNetwork
-from perian.models.instance_type_query_price import InstanceTypeQueryPrice
-from perian.models.instance_type_query_provider import InstanceTypeQueryProvider
-from perian.models.instance_type_query_reference_id import InstanceTypeQueryReferenceId
-from perian.models.instance_type_query_region import InstanceTypeQueryRegion
-from perian.models.instance_type_query_storage import InstanceTypeQueryStorage
-from perian.models.instance_type_query_type import InstanceTypeQueryType
-from perian.models.instance_type_query_zone import InstanceTypeQueryZone
+from perian.models.inbound_speed import InboundSpeed
+from perian.models.included import Included
+from perian.models.incorrect_create_job_parameter_error import IncorrectCreateJobParameterError
+from perian.models.instance_type_id import InstanceTypeId
+from perian.models.instance_type_query_input import InstanceTypeQueryInput
+from perian.models.instance_type_query_input_accelerator import InstanceTypeQueryInputAccelerator
+from perian.models.instance_type_query_input_availability import InstanceTypeQueryInputAvailability
+from perian.models.instance_type_query_input_cpu import InstanceTypeQueryInputCpu
+from perian.models.instance_type_query_input_network import InstanceTypeQueryInputNetwork
+from perian.models.instance_type_query_input_price import InstanceTypeQueryInputPrice
+from perian.models.instance_type_query_input_provider import InstanceTypeQueryInputProvider
+from perian.models.instance_type_query_input_reference_id import InstanceTypeQueryInputReferenceId
+from perian.models.instance_type_query_input_region import InstanceTypeQueryInputRegion
+from perian.models.instance_type_query_input_storage import InstanceTypeQueryInputStorage
+from perian.models.instance_type_query_input_zone import InstanceTypeQueryInputZone
+from perian.models.instance_type_query_output import InstanceTypeQueryOutput
+from perian.models.instance_type_query_output_accelerator import InstanceTypeQueryOutputAccelerator
+from perian.models.instance_type_query_output_availability import InstanceTypeQueryOutputAvailability
+from perian.models.instance_type_query_output_cpu import InstanceTypeQueryOutputCpu
+from perian.models.instance_type_query_output_network import InstanceTypeQueryOutputNetwork
+from perian.models.instance_type_query_output_price import InstanceTypeQueryOutputPrice
+from perian.models.instance_type_query_output_provider import InstanceTypeQueryOutputProvider
+from perian.models.instance_type_query_output_reference_id import InstanceTypeQueryOutputReferenceId
+from perian.models.instance_type_query_output_region import InstanceTypeQueryOutputRegion
+from perian.models.instance_type_query_output_storage import InstanceTypeQueryOutputStorage
+from perian.models.instance_type_query_output_zone import InstanceTypeQueryOutputZone
 from perian.models.instance_type_view import InstanceTypeView
+from perian.models.instance_typer_query_view import InstanceTyperQueryView
+from perian.models.job_already_done_error import JobAlreadyDoneError
 from perian.models.job_status import JobStatus
 from perian.models.job_view import JobView
+from perian.models.job_view_docker_metadata import JobViewDockerMetadata
+from perian.models.job_view_requirement_metadata import JobViewRequirementMetadata
+from perian.models.job_view_runtime_metadata import JobViewRuntimeMetadata
+from perian.models.limit import Limit
 from perian.models.location import Location
+from perian.models.location1 import Location1
 from perian.models.logs import Logs
 from perian.models.memory import Memory
 from perian.models.memory_interface import MemoryInterface
-from perian.models.memory_query import MemoryQuery
+from perian.models.memory_query_input import MemoryQueryInput
+from perian.models.memory_query_output import MemoryQueryOutput
 from perian.models.memory_unit import MemoryUnit
 from perian.models.name import Name
-from perian.models.name_query import NameQuery
+from perian.models.name1 import Name1
+from perian.models.name_short import NameShort
 from perian.models.network import Network
-from perian.models.network_query import NetworkQuery
+from perian.models.network_query_input import NetworkQueryInput
+from perian.models.network_query_output import NetworkQueryOutput
+from perian.models.next_page import NextPage
+from perian.models.no import No
 from perian.models.no_job_found_error import NoJobFoundError
+from perian.models.no_parameter_error import NoParameterError
 from perian.models.os_storage_config import OSStorageConfig
+from perian.models.offset import Offset
 from perian.models.operator import Operator
-from perian.models.organization import Organization
-from perian.models.organization_name_error import OrganizationNameError
-from perian.models.organization_name_exists_error import OrganizationNameExistsError
-from perian.models.price import Price
+from perian.models.order_criterion import OrderCriterion
+from perian.models.outbound_speed import OutboundSpeed
+from perian.models.pagination_metadata import PaginationMetadata
+from perian.models.previous_page import PreviousPage
 from perian.models.price_data import PriceData
-from perian.models.price_query import PriceQuery
+from perian.models.price_query_input import PriceQueryInput
+from perian.models.price_query_output import PriceQueryOutput
 from perian.models.provider import Provider
 from perian.models.provider_capabilities import ProviderCapabilities
 from perian.models.provider_name import ProviderName
 from perian.models.provider_properties import ProviderProperties
-from perian.models.provider_query import ProviderQuery
+from perian.models.provider_query_input import ProviderQueryInput
+from perian.models.provider_query_output import ProviderQueryOutput
 from perian.models.provider_specific_name import ProviderSpecificName
 from perian.models.query_options import QueryOptions
-from perian.models.reference import Reference
-from perian.models.reference_id_query import ReferenceIdQuery
+from perian.models.reference_id_query_input import ReferenceIdQueryInput
+from perian.models.reference_id_query_output import ReferenceIdQueryOutput
 from perian.models.region import Region
-from perian.models.region_query import RegionQuery
-from perian.models.response400_create_global_admin_admin_post import Response400CreateGlobalAdminAdminPost
-from perian.models.response400_create_organization_organization_post import Response400CreateOrganizationOrganizationPost
-from perian.models.response400_create_service_account_service_account_post import Response400CreateServiceAccountServiceAccountPost
-from perian.models.response400_create_user_user_post import Response400CreateUserUserPost
-from perian.models.response_get_job_job_get import ResponseGetJobJobGet
-from perian.models.role_not_valid_error import RoleNotValidError
-from perian.models.setup_token_error import SetupTokenError
+from perian.models.region_query_input import RegionQueryInput
+from perian.models.region_query_output import RegionQueryOutput
+from perian.models.requirement_metadata import RequirementMetadata
+from perian.models.requirement_metadata_requirements import RequirementMetadataRequirements
+from perian.models.response400_cancel_job import Response400CancelJob
+from perian.models.response400_create_job import Response400CreateJob
+from perian.models.response400_get_accelerator_type_by_id import Response400GetAcceleratorTypeById
+from perian.models.response400_get_accelerator_type_by_requirements import Response400GetAcceleratorTypeByRequirements
+from perian.models.response400_get_instance_type_by_id import Response400GetInstanceTypeById
+from perian.models.response400_get_instance_type_by_requirements import Response400GetInstanceTypeByRequirements
+from perian.models.response400_get_job_by_id import Response400GetJobById
+from perian.models.runtime_metadata import RuntimeMetadata
+from perian.models.size import Size
+from perian.models.speed import Speed
+from perian.models.start_time import StartTime
+from perian.models.started_at import StartedAt
 from perian.models.status import Status
+from perian.models.status1 import Status1
 from perian.models.storage import Storage
 from perian.models.storage_data import StorageData
 from perian.models.storage_included import StorageIncluded
-from perian.models.storage_query import StorageQuery
+from perian.models.storage_query_input import StorageQueryInput
+from perian.models.storage_query_output import StorageQueryOutput
 from perian.models.storage_type import StorageType
-from perian.models.type_query import TypeQuery
+from perian.models.sustainable import Sustainable
+from perian.models.threads import Threads
+from perian.models.type import Type
+from perian.models.unit_price import UnitPrice
 from perian.models.validation_error import ValidationError
 from perian.models.validation_error_loc_inner import ValidationErrorLocInner
 from perian.models.vendor import Vendor
 from perian.models.zone import Zone
-from perian.models.zone_query import ZoneQuery
+from perian.models.zone_query_input import ZoneQueryInput
+from perian.models.zone_query_output import ZoneQueryOutput
```

### Comparing `perian-0.1.25/perian/api/admin_api.py` & `perian-0.2.0/perian/api/billing_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,57 +12,69 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from perian.models.create_admin_success import CreateAdminSuccess
-from perian.models.create_global_admin_request import CreateGlobalAdminRequest
+from pydantic import Field, StrictStr
+from typing import Any, Optional
+from typing_extensions import Annotated
+from perian.models.bill import Bill
 
 from perian.api_client import ApiClient, RequestSerialized
 from perian.api_response import ApiResponse
 from perian.rest import RESTResponseType
 
 
-class AdminApi:
+class BillingApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def create_global_admin_admin_post(
+    def generate_bill(
         self,
-        create_global_admin_request: CreateGlobalAdminRequest,
+        organization: Annotated[StrictStr, Field(description="Name of the organization")],
+        currency: Annotated[Optional[Any], Field(description="Currency")] = None,
+        start_time: Annotated[Optional[Any], Field(description="Start time - defaults to the beginning of the last month")] = None,
+        end_time: Annotated[Optional[Any], Field(description="End time - defaults to the end of the last month")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CreateAdminSuccess:
-        """Create Global Admin
+    ) -> Bill:
+        """Generate Bill
 
+        Endpoint to generate a bill for the organization
 
-        :param create_global_admin_request: (required)
-        :type create_global_admin_request: CreateGlobalAdminRequest
+        :param organization: Name of the organization (required)
+        :type organization: str
+        :param currency: Currency
+        :type currency: Currency1
+        :param start_time: Start time - defaults to the beginning of the last month
+        :type start_time: StartTime
+        :param end_time: End time - defaults to the end of the last month
+        :type end_time: EndTime
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -77,61 +89,72 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_global_admin_admin_post_serialize(
-            create_global_admin_request=create_global_admin_request,
+        _param = self._generate_bill_serialize(
+            organization=organization,
+            currency=currency,
+            start_time=start_time,
+            end_time=end_time,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateAdminSuccess",
-            '400': "Response400CreateGlobalAdminAdminPost",
-            '500': "DefaultServerError",
+            '200': "Bill",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_global_admin_admin_post_with_http_info(
+    def generate_bill_with_http_info(
         self,
-        create_global_admin_request: CreateGlobalAdminRequest,
+        organization: Annotated[StrictStr, Field(description="Name of the organization")],
+        currency: Annotated[Optional[Any], Field(description="Currency")] = None,
+        start_time: Annotated[Optional[Any], Field(description="Start time - defaults to the beginning of the last month")] = None,
+        end_time: Annotated[Optional[Any], Field(description="End time - defaults to the end of the last month")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CreateAdminSuccess]:
-        """Create Global Admin
+    ) -> ApiResponse[Bill]:
+        """Generate Bill
 
+        Endpoint to generate a bill for the organization
 
-        :param create_global_admin_request: (required)
-        :type create_global_admin_request: CreateGlobalAdminRequest
+        :param organization: Name of the organization (required)
+        :type organization: str
+        :param currency: Currency
+        :type currency: Currency1
+        :param start_time: Start time - defaults to the beginning of the last month
+        :type start_time: StartTime
+        :param end_time: End time - defaults to the end of the last month
+        :type end_time: EndTime
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -146,61 +169,72 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_global_admin_admin_post_serialize(
-            create_global_admin_request=create_global_admin_request,
+        _param = self._generate_bill_serialize(
+            organization=organization,
+            currency=currency,
+            start_time=start_time,
+            end_time=end_time,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateAdminSuccess",
-            '400': "Response400CreateGlobalAdminAdminPost",
-            '500': "DefaultServerError",
+            '200': "Bill",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_global_admin_admin_post_without_preload_content(
+    def generate_bill_without_preload_content(
         self,
-        create_global_admin_request: CreateGlobalAdminRequest,
+        organization: Annotated[StrictStr, Field(description="Name of the organization")],
+        currency: Annotated[Optional[Any], Field(description="Currency")] = None,
+        start_time: Annotated[Optional[Any], Field(description="Start time - defaults to the beginning of the last month")] = None,
+        end_time: Annotated[Optional[Any], Field(description="End time - defaults to the end of the last month")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create Global Admin
+        """Generate Bill
 
+        Endpoint to generate a bill for the organization
 
-        :param create_global_admin_request: (required)
-        :type create_global_admin_request: CreateGlobalAdminRequest
+        :param organization: Name of the organization (required)
+        :type organization: str
+        :param currency: Currency
+        :type currency: Currency1
+        :param start_time: Start time - defaults to the beginning of the last month
+        :type start_time: StartTime
+        :param end_time: End time - defaults to the end of the last month
+        :type end_time: EndTime
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -215,38 +249,42 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_global_admin_admin_post_serialize(
-            create_global_admin_request=create_global_admin_request,
+        _param = self._generate_bill_serialize(
+            organization=organization,
+            currency=currency,
+            start_time=start_time,
+            end_time=end_time,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateAdminSuccess",
-            '400': "Response400CreateGlobalAdminAdminPost",
-            '500': "DefaultServerError",
+            '200': "Bill",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_global_admin_admin_post_serialize(
+    def _generate_bill_serialize(
         self,
-        create_global_admin_request,
+        organization,
+        currency,
+        start_time,
+        end_time,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -259,49 +297,50 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if organization is not None:
+            
+            _query_params.append(('organization', organization))
+            
+        if currency is not None:
+            
+            _query_params.append(('currency', currency))
+            
+        if start_time is not None:
+            
+            _query_params.append(('start_time', start_time))
+            
+        if end_time is not None:
+            
+            _query_params.append(('end_time', end_time))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if create_global_admin_request is not None:
-            _body_params = create_global_admin_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/admin',
+            method='GET',
+            resource_path='/billing/generate',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `perian-0.1.25/perian/api/job_api.py` & `perian-0.2.0/perian/api/instance_type_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,61 +12,60 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictStr
-from typing import Optional
+from pydantic import Field, StrictInt, StrictStr
+from typing import Any, Optional
 from typing_extensions import Annotated
-from perian.models.create_job_request import CreateJobRequest
-from perian.models.create_job_success import CreateJobSuccess
-from perian.models.response_get_job_job_get import ResponseGetJobJobGet
+from perian.models.get_instance_type_request import GetInstanceTypeRequest
+from perian.models.get_instance_types_success import GetInstanceTypesSuccess
 
 from perian.api_client import ApiClient, RequestSerialized
 from perian.api_response import ApiResponse
 from perian.rest import RESTResponseType
 
 
-class JobApi:
+class InstanceTypeApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def create_job_job_post(
+    def get_instance_type_by_id(
         self,
-        create_job_request: CreateJobRequest,
+        instance_type_id: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> CreateJobSuccess:
-        """Create Job
+    ) -> GetInstanceTypesSuccess:
+        """Get Instance Type By Id
 
 
-        :param create_job_request: (required)
-        :type create_job_request: CreateJobRequest
+        :param instance_type_id: (required)
+        :type instance_type_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -81,61 +80,61 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_job_job_post_serialize(
-            create_job_request=create_job_request,
+        _param = self._get_instance_type_by_id_serialize(
+            instance_type_id=instance_type_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateJobSuccess",
-            '400': "DefaultClientError",
-            '500': "InstanceTypeBlockedError",
+            '200': "GetInstanceTypesSuccess",
+            '400': "Response400GetInstanceTypeById",
+            '500': "DefaultServerError",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def create_job_job_post_with_http_info(
+    def get_instance_type_by_id_with_http_info(
         self,
-        create_job_request: CreateJobRequest,
+        instance_type_id: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[CreateJobSuccess]:
-        """Create Job
+    ) -> ApiResponse[GetInstanceTypesSuccess]:
+        """Get Instance Type By Id
 
 
-        :param create_job_request: (required)
-        :type create_job_request: CreateJobRequest
+        :param instance_type_id: (required)
+        :type instance_type_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -150,61 +149,61 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_job_job_post_serialize(
-            create_job_request=create_job_request,
+        _param = self._get_instance_type_by_id_serialize(
+            instance_type_id=instance_type_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateJobSuccess",
-            '400': "DefaultClientError",
-            '500': "InstanceTypeBlockedError",
+            '200': "GetInstanceTypesSuccess",
+            '400': "Response400GetInstanceTypeById",
+            '500': "DefaultServerError",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def create_job_job_post_without_preload_content(
+    def get_instance_type_by_id_without_preload_content(
         self,
-        create_job_request: CreateJobRequest,
+        instance_type_id: StrictStr,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Create Job
+        """Get Instance Type By Id
 
 
-        :param create_job_request: (required)
-        :type create_job_request: CreateJobRequest
+        :param instance_type_id: (required)
+        :type instance_type_id: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -219,38 +218,38 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._create_job_job_post_serialize(
-            create_job_request=create_job_request,
+        _param = self._get_instance_type_by_id_serialize(
+            instance_type_id=instance_type_id,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "CreateJobSuccess",
-            '400': "DefaultClientError",
-            '500': "InstanceTypeBlockedError",
+            '200': "GetInstanceTypesSuccess",
+            '400': "Response400GetInstanceTypeById",
+            '500': "DefaultServerError",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _create_job_job_post_serialize(
+    def _get_instance_type_by_id_serialize(
         self,
-        create_job_request,
+        instance_type_id,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -262,50 +261,37 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if instance_type_id is not None:
+            _path_params['instance_type_id'] = instance_type_id
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
-        if create_job_request is not None:
-            _body_params = create_job_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
-        # set the HTTP header `Content-Type`
-        if _content_type:
-            _header_params['Content-Type'] = _content_type
-        else:
-            _default_content_type = (
-                self.api_client.select_header_content_type(
-                    [
-                        'application/json'
-                    ]
-                )
-            )
-            if _default_content_type is not None:
-                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
         ]
 
         return self.api_client.param_serialize(
-            method='POST',
-            resource_path='/job',
+            method='GET',
+            resource_path='/instance-type/{instance_type_id}',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
@@ -314,35 +300,44 @@
             _request_auth=_request_auth
         )
 
 
 
 
     @validate_call
-    def get_job_job_get(
+    def get_instance_type_by_requirements(
         self,
-        id: Annotated[Optional[StrictStr], Field(description="Provide an ID to only get this specific job")] = None,
+        get_instance_type_request: GetInstanceTypeRequest,
+        limit: Annotated[Optional[StrictInt], Field(description="Limit the number of instance types to return")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="Number of requested result page")] = None,
+        criterion: Annotated[Optional[Any], Field(description="Select a specific criterion to optimize for. Currently available options: PRICE")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ResponseGetJobJobGet:
-        """Get Job
+    ) -> GetInstanceTypesSuccess:
+        """Get Instance Type By Requirements
 
 
-        :param id: Provide an ID to only get this specific job
-        :type id: str
+        :param get_instance_type_request: (required)
+        :type get_instance_type_request: GetInstanceTypeRequest
+        :param limit: Limit the number of instance types to return
+        :type limit: int
+        :param page: Number of requested result page
+        :type page: int
+        :param criterion: Select a specific criterion to optimize for. Currently available options: PRICE
+        :type criterion: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -357,59 +352,73 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_job_job_get_serialize(
-            id=id,
+        _param = self._get_instance_type_by_requirements_serialize(
+            get_instance_type_request=get_instance_type_request,
+            limit=limit,
+            page=page,
+            criterion=criterion,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ResponseGetJobJobGet",
+            '200': "GetInstanceTypesSuccess",
+            '400': "Response400GetInstanceTypeByRequirements",
+            '500': "DefaultServerError",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_job_job_get_with_http_info(
+    def get_instance_type_by_requirements_with_http_info(
         self,
-        id: Annotated[Optional[StrictStr], Field(description="Provide an ID to only get this specific job")] = None,
+        get_instance_type_request: GetInstanceTypeRequest,
+        limit: Annotated[Optional[StrictInt], Field(description="Limit the number of instance types to return")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="Number of requested result page")] = None,
+        criterion: Annotated[Optional[Any], Field(description="Select a specific criterion to optimize for. Currently available options: PRICE")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[ResponseGetJobJobGet]:
-        """Get Job
+    ) -> ApiResponse[GetInstanceTypesSuccess]:
+        """Get Instance Type By Requirements
 
 
-        :param id: Provide an ID to only get this specific job
-        :type id: str
+        :param get_instance_type_request: (required)
+        :type get_instance_type_request: GetInstanceTypeRequest
+        :param limit: Limit the number of instance types to return
+        :type limit: int
+        :param page: Number of requested result page
+        :type page: int
+        :param criterion: Select a specific criterion to optimize for. Currently available options: PRICE
+        :type criterion: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -424,59 +433,73 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_job_job_get_serialize(
-            id=id,
+        _param = self._get_instance_type_by_requirements_serialize(
+            get_instance_type_request=get_instance_type_request,
+            limit=limit,
+            page=page,
+            criterion=criterion,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ResponseGetJobJobGet",
+            '200': "GetInstanceTypesSuccess",
+            '400': "Response400GetInstanceTypeByRequirements",
+            '500': "DefaultServerError",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_job_job_get_without_preload_content(
+    def get_instance_type_by_requirements_without_preload_content(
         self,
-        id: Annotated[Optional[StrictStr], Field(description="Provide an ID to only get this specific job")] = None,
+        get_instance_type_request: GetInstanceTypeRequest,
+        limit: Annotated[Optional[StrictInt], Field(description="Limit the number of instance types to return")] = None,
+        page: Annotated[Optional[StrictInt], Field(description="Number of requested result page")] = None,
+        criterion: Annotated[Optional[Any], Field(description="Select a specific criterion to optimize for. Currently available options: PRICE")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get Job
+        """Get Instance Type By Requirements
 
 
-        :param id: Provide an ID to only get this specific job
-        :type id: str
+        :param get_instance_type_request: (required)
+        :type get_instance_type_request: GetInstanceTypeRequest
+        :param limit: Limit the number of instance types to return
+        :type limit: int
+        :param page: Number of requested result page
+        :type page: int
+        :param criterion: Select a specific criterion to optimize for. Currently available options: PRICE
+        :type criterion: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -491,36 +514,44 @@
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
-        _param = self._get_job_job_get_serialize(
-            id=id,
+        _param = self._get_instance_type_by_requirements_serialize(
+            get_instance_type_request=get_instance_type_request,
+            limit=limit,
+            page=page,
+            criterion=criterion,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "ResponseGetJobJobGet",
+            '200': "GetInstanceTypesSuccess",
+            '400': "Response400GetInstanceTypeByRequirements",
+            '500': "DefaultServerError",
             '422': "HTTPValidationError",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_job_job_get_serialize(
+    def _get_instance_type_by_requirements_serialize(
         self,
-        id,
+        get_instance_type_request,
+        limit,
+        page,
+        criterion,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -533,38 +564,61 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
-        if id is not None:
+        if limit is not None:
+            
+            _query_params.append(('limit', limit))
+            
+        if page is not None:
             
-            _query_params.append(('id', id))
+            _query_params.append(('page', page))
+            
+        if criterion is not None:
+            
+            _query_params.append(('criterion', criterion))
             
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if get_instance_type_request is not None:
+            _body_params = get_instance_type_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/job',
+            method='POST',
+            resource_path='/instance-type',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `perian-0.1.25/perian/api_client.py` & `perian-0.2.0/perian/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.25/python'
+        self.user_agent = 'OpenAPI-Generator/0.2.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `perian-0.1.25/perian/api_response.py` & `perian-0.2.0/perian/api_response.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/configuration.py` & `perian-0.2.0/perian/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.24\n"\
-               "SDK Package Version: 0.1.25".\
+               "SDK Package Version: 0.2.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `perian-0.1.25/perian/exceptions.py` & `perian-0.2.0/perian/exceptions.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/__init__.py` & `perian-0.2.0/perian/models/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,116 +11,173 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from perian.models.accelerator_data_view import AcceleratorDataView
-from perian.models.accelerator_name import AcceleratorName
-from perian.models.accelerator_query import AcceleratorQuery
-from perian.models.accelerator_query_memory import AcceleratorQueryMemory
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input import AcceleratorQueryInput
+from perian.models.accelerator_query_input_memory import AcceleratorQueryInputMemory
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
+from perian.models.accelerator_query_output import AcceleratorQueryOutput
+from perian.models.accelerator_query_output_memory import AcceleratorQueryOutputMemory
+from perian.models.accelerator_type_not_found_error import AcceleratorTypeNotFoundError
+from perian.models.accelerator_type_query import AcceleratorTypeQuery
 from perian.models.accelerator_type_view import AcceleratorTypeView
 from perian.models.accelerator_vendor import AcceleratorVendor
+from perian.models.api_router_accelerator_type_incorrect_parameter_error import ApiRouterAcceleratorTypeIncorrectParameterError
+from perian.models.api_router_instance_type_incorrect_parameter_error import ApiRouterInstanceTypeIncorrectParameterError
+from perian.models.api_router_instance_type_instance_type_not_found_error import ApiRouterInstanceTypeInstanceTypeNotFoundError
+from perian.models.api_router_job_instance_type_not_found_error import ApiRouterJobInstanceTypeNotFoundError
 from perian.models.availability import Availability
-from perian.models.availability_query import AvailabilityQuery
+from perian.models.availability_query_input import AvailabilityQueryInput
+from perian.models.availability_query_output import AvailabilityQueryOutput
 from perian.models.availability_source import AvailabilitySource
+from perian.models.available import Available
 from perian.models.bandwidth import Bandwidth
 from perian.models.bandwidth_limits import BandwidthLimits
 from perian.models.bandwidth_sla import BandwidthSla
 from perian.models.bandwidth_units import BandwidthUnits
+from perian.models.bill import Bill
+from perian.models.bill_item import BillItem
+from perian.models.billing_granularity import BillingGranularity
 from perian.models.command import Command
-from perian.models.compute_billing_period import ComputeBillingPeriod
 from perian.models.compute_instance_type import ComputeInstanceType
+from perian.models.cores import Cores
 from perian.models.cpu import Cpu
 from perian.models.cpu_data import CpuData
-from perian.models.cpu_query import CpuQuery
-from perian.models.create_admin_success import CreateAdminSuccess
-from perian.models.create_global_admin_request import CreateGlobalAdminRequest
+from perian.models.cpu_query_input import CpuQueryInput
+from perian.models.cpu_query_output import CpuQueryOutput
 from perian.models.create_job_request import CreateJobRequest
 from perian.models.create_job_request_docker_registry_credentials import CreateJobRequestDockerRegistryCredentials
+from perian.models.create_job_request_requirements import CreateJobRequestRequirements
 from perian.models.create_job_success import CreateJobSuccess
-from perian.models.create_organization_request import CreateOrganizationRequest
-from perian.models.create_organization_success import CreateOrganizationSuccess
-from perian.models.create_service_account_request import CreateServiceAccountRequest
-from perian.models.create_service_account_success import CreateServiceAccountSuccess
-from perian.models.create_user_request import CreateUserRequest
-from perian.models.create_user_success import CreateUserSuccess
 from perian.models.currency import Currency
+from perian.models.currency1 import Currency1
 from perian.models.default_client_error import DefaultClientError
 from perian.models.default_server_error import DefaultServerError
+from perian.models.default_success import DefaultSuccess
 from perian.models.description import Description
+from perian.models.docker_metadata import DockerMetadata
 from perian.models.docker_registry_credentials import DockerRegistryCredentials
 from perian.models.docker_run_parameters import DockerRunParameters
 from perian.models.done_at import DoneAt
+from perian.models.end_time import EndTime
+from perian.models.errors import Errors
+from perian.models.get_accelerator_type_request import GetAcceleratorTypeRequest
+from perian.models.get_accelerator_types_success import GetAcceleratorTypesSuccess
+from perian.models.get_instance_type_request import GetInstanceTypeRequest
 from perian.models.get_instance_types_success import GetInstanceTypesSuccess
 from perian.models.get_jobs_success import GetJobsSuccess
 from perian.models.http_validation_error import HTTPValidationError
 from perian.models.id import Id
+from perian.models.id1 import Id1
 from perian.models.image_tag import ImageTag
-from perian.models.instance_type_blocked_error import InstanceTypeBlockedError
-from perian.models.instance_type_query import InstanceTypeQuery
-from perian.models.instance_type_query_accelerator import InstanceTypeQueryAccelerator
-from perian.models.instance_type_query_availability import InstanceTypeQueryAvailability
-from perian.models.instance_type_query_cpu import InstanceTypeQueryCpu
-from perian.models.instance_type_query_name import InstanceTypeQueryName
-from perian.models.instance_type_query_network import InstanceTypeQueryNetwork
-from perian.models.instance_type_query_price import InstanceTypeQueryPrice
-from perian.models.instance_type_query_provider import InstanceTypeQueryProvider
-from perian.models.instance_type_query_reference_id import InstanceTypeQueryReferenceId
-from perian.models.instance_type_query_region import InstanceTypeQueryRegion
-from perian.models.instance_type_query_storage import InstanceTypeQueryStorage
-from perian.models.instance_type_query_type import InstanceTypeQueryType
-from perian.models.instance_type_query_zone import InstanceTypeQueryZone
+from perian.models.inbound_speed import InboundSpeed
+from perian.models.included import Included
+from perian.models.incorrect_create_job_parameter_error import IncorrectCreateJobParameterError
+from perian.models.instance_type_id import InstanceTypeId
+from perian.models.instance_type_query_input import InstanceTypeQueryInput
+from perian.models.instance_type_query_input_accelerator import InstanceTypeQueryInputAccelerator
+from perian.models.instance_type_query_input_availability import InstanceTypeQueryInputAvailability
+from perian.models.instance_type_query_input_cpu import InstanceTypeQueryInputCpu
+from perian.models.instance_type_query_input_network import InstanceTypeQueryInputNetwork
+from perian.models.instance_type_query_input_price import InstanceTypeQueryInputPrice
+from perian.models.instance_type_query_input_provider import InstanceTypeQueryInputProvider
+from perian.models.instance_type_query_input_reference_id import InstanceTypeQueryInputReferenceId
+from perian.models.instance_type_query_input_region import InstanceTypeQueryInputRegion
+from perian.models.instance_type_query_input_storage import InstanceTypeQueryInputStorage
+from perian.models.instance_type_query_input_zone import InstanceTypeQueryInputZone
+from perian.models.instance_type_query_output import InstanceTypeQueryOutput
+from perian.models.instance_type_query_output_accelerator import InstanceTypeQueryOutputAccelerator
+from perian.models.instance_type_query_output_availability import InstanceTypeQueryOutputAvailability
+from perian.models.instance_type_query_output_cpu import InstanceTypeQueryOutputCpu
+from perian.models.instance_type_query_output_network import InstanceTypeQueryOutputNetwork
+from perian.models.instance_type_query_output_price import InstanceTypeQueryOutputPrice
+from perian.models.instance_type_query_output_provider import InstanceTypeQueryOutputProvider
+from perian.models.instance_type_query_output_reference_id import InstanceTypeQueryOutputReferenceId
+from perian.models.instance_type_query_output_region import InstanceTypeQueryOutputRegion
+from perian.models.instance_type_query_output_storage import InstanceTypeQueryOutputStorage
+from perian.models.instance_type_query_output_zone import InstanceTypeQueryOutputZone
 from perian.models.instance_type_view import InstanceTypeView
+from perian.models.instance_typer_query_view import InstanceTyperQueryView
+from perian.models.job_already_done_error import JobAlreadyDoneError
 from perian.models.job_status import JobStatus
 from perian.models.job_view import JobView
+from perian.models.job_view_docker_metadata import JobViewDockerMetadata
+from perian.models.job_view_requirement_metadata import JobViewRequirementMetadata
+from perian.models.job_view_runtime_metadata import JobViewRuntimeMetadata
+from perian.models.limit import Limit
 from perian.models.location import Location
+from perian.models.location1 import Location1
 from perian.models.logs import Logs
 from perian.models.memory import Memory
 from perian.models.memory_interface import MemoryInterface
-from perian.models.memory_query import MemoryQuery
+from perian.models.memory_query_input import MemoryQueryInput
+from perian.models.memory_query_output import MemoryQueryOutput
 from perian.models.memory_unit import MemoryUnit
 from perian.models.name import Name
-from perian.models.name_query import NameQuery
+from perian.models.name1 import Name1
+from perian.models.name_short import NameShort
 from perian.models.network import Network
-from perian.models.network_query import NetworkQuery
+from perian.models.network_query_input import NetworkQueryInput
+from perian.models.network_query_output import NetworkQueryOutput
+from perian.models.next_page import NextPage
+from perian.models.no import No
 from perian.models.no_job_found_error import NoJobFoundError
+from perian.models.no_parameter_error import NoParameterError
 from perian.models.os_storage_config import OSStorageConfig
+from perian.models.offset import Offset
 from perian.models.operator import Operator
-from perian.models.organization import Organization
-from perian.models.organization_name_error import OrganizationNameError
-from perian.models.organization_name_exists_error import OrganizationNameExistsError
-from perian.models.price import Price
+from perian.models.order_criterion import OrderCriterion
+from perian.models.outbound_speed import OutboundSpeed
+from perian.models.pagination_metadata import PaginationMetadata
+from perian.models.previous_page import PreviousPage
 from perian.models.price_data import PriceData
-from perian.models.price_query import PriceQuery
+from perian.models.price_query_input import PriceQueryInput
+from perian.models.price_query_output import PriceQueryOutput
 from perian.models.provider import Provider
 from perian.models.provider_capabilities import ProviderCapabilities
 from perian.models.provider_name import ProviderName
 from perian.models.provider_properties import ProviderProperties
-from perian.models.provider_query import ProviderQuery
+from perian.models.provider_query_input import ProviderQueryInput
+from perian.models.provider_query_output import ProviderQueryOutput
 from perian.models.provider_specific_name import ProviderSpecificName
 from perian.models.query_options import QueryOptions
-from perian.models.reference import Reference
-from perian.models.reference_id_query import ReferenceIdQuery
+from perian.models.reference_id_query_input import ReferenceIdQueryInput
+from perian.models.reference_id_query_output import ReferenceIdQueryOutput
 from perian.models.region import Region
-from perian.models.region_query import RegionQuery
-from perian.models.response400_create_global_admin_admin_post import Response400CreateGlobalAdminAdminPost
-from perian.models.response400_create_organization_organization_post import Response400CreateOrganizationOrganizationPost
-from perian.models.response400_create_service_account_service_account_post import Response400CreateServiceAccountServiceAccountPost
-from perian.models.response400_create_user_user_post import Response400CreateUserUserPost
-from perian.models.response_get_job_job_get import ResponseGetJobJobGet
-from perian.models.role_not_valid_error import RoleNotValidError
-from perian.models.setup_token_error import SetupTokenError
+from perian.models.region_query_input import RegionQueryInput
+from perian.models.region_query_output import RegionQueryOutput
+from perian.models.requirement_metadata import RequirementMetadata
+from perian.models.requirement_metadata_requirements import RequirementMetadataRequirements
+from perian.models.response400_cancel_job import Response400CancelJob
+from perian.models.response400_create_job import Response400CreateJob
+from perian.models.response400_get_accelerator_type_by_id import Response400GetAcceleratorTypeById
+from perian.models.response400_get_accelerator_type_by_requirements import Response400GetAcceleratorTypeByRequirements
+from perian.models.response400_get_instance_type_by_id import Response400GetInstanceTypeById
+from perian.models.response400_get_instance_type_by_requirements import Response400GetInstanceTypeByRequirements
+from perian.models.response400_get_job_by_id import Response400GetJobById
+from perian.models.runtime_metadata import RuntimeMetadata
+from perian.models.size import Size
+from perian.models.speed import Speed
+from perian.models.start_time import StartTime
+from perian.models.started_at import StartedAt
 from perian.models.status import Status
+from perian.models.status1 import Status1
 from perian.models.storage import Storage
 from perian.models.storage_data import StorageData
 from perian.models.storage_included import StorageIncluded
-from perian.models.storage_query import StorageQuery
+from perian.models.storage_query_input import StorageQueryInput
+from perian.models.storage_query_output import StorageQueryOutput
 from perian.models.storage_type import StorageType
-from perian.models.type_query import TypeQuery
+from perian.models.sustainable import Sustainable
+from perian.models.threads import Threads
+from perian.models.type import Type
+from perian.models.unit_price import UnitPrice
 from perian.models.validation_error import ValidationError
 from perian.models.validation_error_loc_inner import ValidationErrorLocInner
 from perian.models.vendor import Vendor
 from perian.models.zone import Zone
-from perian.models.zone_query import ZoneQuery
+from perian.models.zone_query_input import ZoneQueryInput
+from perian.models.zone_query_output import ZoneQueryOutput
```

### Comparing `perian-0.1.25/perian/models/accelerator_data_view.py` & `perian-0.2.0/perian/models/accelerator_data_view.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/accelerator_query.py` & `perian-0.2.0/perian/models/accelerator_type_query.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,39 +13,42 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.accelerator_query_memory import AcceleratorQueryMemory
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input_memory import AcceleratorQueryInputMemory
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
 from perian.models.description import Description
+from perian.models.id import Id
 from perian.models.name import Name
+from perian.models.no import No
 from perian.models.provider_specific_name import ProviderSpecificName
 from perian.models.vendor import Vendor
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AcceleratorQuery(BaseModel):
+class AcceleratorTypeQuery(BaseModel):
     """
-    AcceleratorQuery
+    AcceleratorTypeQuery
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    no: Optional[StrictInt] = None
-    memory: Optional[AcceleratorQueryMemory] = None
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    no: Optional[No] = None
+    memory: Optional[AcceleratorQueryInputMemory] = None
     vendor: Optional[Vendor] = None
     name: Optional[Name] = None
     description: Optional[Description] = None
     provider_specific_name: Optional[ProviderSpecificName] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "no", "memory", "vendor", "name", "description", "provider_specific_name"]
+    id: Optional[Id] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "no", "memory", "vendor", "name", "description", "provider_specific_name", "id"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -57,15 +60,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AcceleratorQuery from a JSON string"""
+        """Create an instance of AcceleratorTypeQuery from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -84,14 +87,17 @@
         )
         # override the default output from pydantic by calling `to_dict()` of operator
         if self.operator:
             _dict['operator'] = self.operator.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of no
+        if self.no:
+            _dict['no'] = self.no.to_dict()
         # override the default output from pydantic by calling `to_dict()` of memory
         if self.memory:
             _dict['memory'] = self.memory.to_dict()
         # override the default output from pydantic by calling `to_dict()` of vendor
         if self.vendor:
             _dict['vendor'] = self.vendor.to_dict()
         # override the default output from pydantic by calling `to_dict()` of name
@@ -99,31 +105,35 @@
             _dict['name'] = self.name.to_dict()
         # override the default output from pydantic by calling `to_dict()` of description
         if self.description:
             _dict['description'] = self.description.to_dict()
         # override the default output from pydantic by calling `to_dict()` of provider_specific_name
         if self.provider_specific_name:
             _dict['provider_specific_name'] = self.provider_specific_name.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of id
+        if self.id:
+            _dict['id'] = self.id.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AcceleratorQuery from a dict"""
+        """Create an instance of AcceleratorTypeQuery from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
-            "no": obj.get("no"),
-            "memory": AcceleratorQueryMemory.from_dict(obj["memory"]) if obj.get("memory") is not None else None,
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "no": No.from_dict(obj["no"]) if obj.get("no") is not None else None,
+            "memory": AcceleratorQueryInputMemory.from_dict(obj["memory"]) if obj.get("memory") is not None else None,
             "vendor": Vendor.from_dict(obj["vendor"]) if obj.get("vendor") is not None else None,
             "name": Name.from_dict(obj["name"]) if obj.get("name") is not None else None,
             "description": Description.from_dict(obj["description"]) if obj.get("description") is not None else None,
-            "provider_specific_name": ProviderSpecificName.from_dict(obj["provider_specific_name"]) if obj.get("provider_specific_name") is not None else None
+            "provider_specific_name": ProviderSpecificName.from_dict(obj["provider_specific_name"]) if obj.get("provider_specific_name") is not None else None,
+            "id": Id.from_dict(obj["id"]) if obj.get("id") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/accelerator_query_memory.py` & `perian-0.2.0/perian/models/accelerator_query_input_memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.memory_query import MemoryQuery
+from perian.models.memory_query_input import MemoryQueryInput
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-ACCELERATORQUERYMEMORY_ANY_OF_SCHEMAS = ["MemoryQuery", "object"]
+ACCELERATORQUERYINPUTMEMORY_ANY_OF_SCHEMAS = ["MemoryQueryInput", "object"]
 
-class AcceleratorQueryMemory(BaseModel):
+class AcceleratorQueryInputMemory(BaseModel):
     """
-    AcceleratorQueryMemory
+    AcceleratorQueryInputMemory
     """
 
-    # data type: MemoryQuery
-    anyof_schema_1_validator: Optional[MemoryQuery] = None
+    # data type: MemoryQueryInput
+    anyof_schema_1_validator: Optional[MemoryQueryInput] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[MemoryQuery, object]] = None
+        actual_instance: Optional[Union[MemoryQueryInput, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["MemoryQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["MemoryQueryInput", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,46 +54,46 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = AcceleratorQueryMemory.model_construct()
+        instance = AcceleratorQueryInputMemory.model_construct()
         error_messages = []
-        # validate data type: MemoryQuery
-        if not isinstance(v, MemoryQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `MemoryQuery`")
+        # validate data type: MemoryQueryInput
+        if not isinstance(v, MemoryQueryInput):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `MemoryQueryInput`")
         else:
             return v
 
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in AcceleratorQueryMemory with anyOf schemas: MemoryQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in AcceleratorQueryInputMemory with anyOf schemas: MemoryQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[MemoryQuery] = None
+        # anyof_schema_1_validator: Optional[MemoryQueryInput] = None
         try:
-            instance.actual_instance = MemoryQuery.from_json(json_str)
+            instance.actual_instance = MemoryQueryInput.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
@@ -101,29 +101,29 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into AcceleratorQueryMemory with anyOf schemas: MemoryQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into AcceleratorQueryInputMemory with anyOf schemas: MemoryQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], MemoryQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], MemoryQueryInput, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/accelerator_query_operator.py` & `perian-0.2.0/perian/models/name_short.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,35 +15,34 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.operator import Operator
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-ACCELERATORQUERYOPERATOR_ANY_OF_SCHEMAS = ["Operator", "object"]
+NAMESHORT_ANY_OF_SCHEMAS = ["object", "str"]
 
-class AcceleratorQueryOperator(BaseModel):
+class NameShort(BaseModel):
     """
-    AcceleratorQueryOperator
+    NameShort
     """
 
-    # data type: Operator
-    anyof_schema_1_validator: Optional[Operator] = None
+    # data type: str
+    anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[Operator, object]] = None
+        actual_instance: Optional[Union[object, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["Operator", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["object", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,76 +53,79 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = AcceleratorQueryOperator.model_construct()
+        instance = NameShort.model_construct()
         error_messages = []
-        # validate data type: Operator
-        if not isinstance(v, Operator):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `Operator`")
-        else:
+        # validate data type: str
+        try:
+            instance.anyof_schema_1_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in AcceleratorQueryOperator with anyOf schemas: Operator, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in NameShort with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[Operator] = None
+        # deserialize data into str
         try:
-            instance.actual_instance = Operator.from_json(json_str)
+            # validation
+            instance.anyof_schema_1_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into AcceleratorQueryOperator with anyOf schemas: Operator, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into NameShort with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], Operator, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], object, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/accelerator_query_options.py` & `perian-0.2.0/perian/models/accelerator_query_input_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
 from perian.models.query_options import QueryOptions
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-ACCELERATORQUERYOPTIONS_ANY_OF_SCHEMAS = ["QueryOptions", "object"]
+ACCELERATORQUERYINPUTOPTIONS_ANY_OF_SCHEMAS = ["QueryOptions", "object"]
 
-class AcceleratorQueryOptions(BaseModel):
+class AcceleratorQueryInputOptions(BaseModel):
     """
-    AcceleratorQueryOptions
+    AcceleratorQueryInputOptions
     """
 
     # data type: QueryOptions
     anyof_schema_1_validator: Optional[QueryOptions] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
@@ -54,15 +54,15 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = AcceleratorQueryOptions.model_construct()
+        instance = AcceleratorQueryInputOptions.model_construct()
         error_messages = []
         # validate data type: QueryOptions
         if not isinstance(v, QueryOptions):
             error_messages.append(f"Error! Input type `{type(v)}` is not `QueryOptions`")
         else:
             return v
 
@@ -70,15 +70,15 @@
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in AcceleratorQueryOptions with anyOf schemas: QueryOptions, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in AcceleratorQueryInputOptions with anyOf schemas: QueryOptions, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
@@ -101,15 +101,15 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into AcceleratorQueryOptions with anyOf schemas: QueryOptions, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into AcceleratorQueryInputOptions with anyOf schemas: QueryOptions, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
```

### Comparing `perian-0.1.25/perian/models/accelerator_type_view.py` & `perian-0.2.0/perian/models/accelerator_type_view.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,29 +15,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.accelerator_name import AcceleratorName
 from perian.models.accelerator_vendor import AcceleratorVendor
 from perian.models.memory import Memory
 from typing import Optional, Set
 from typing_extensions import Self
 
 class AcceleratorTypeView(BaseModel):
     """
     AcceleratorTypeView
     """ # noqa: E501
+    display_name: Optional[StrictStr] = None
     id: Optional[StrictStr] = None
-    name: Optional[AcceleratorName] = None
     vendor: Optional[AcceleratorVendor] = None
     memory: Optional[Memory] = None
-    __properties: ClassVar[List[str]] = ["id", "name", "vendor", "memory"]
+    __properties: ClassVar[List[str]] = ["display_name", "id", "vendor", "memory"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -85,15 +84,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "display_name": obj.get("display_name"),
             "id": obj.get("id"),
-            "name": obj.get("name"),
             "vendor": obj.get("vendor"),
             "memory": Memory.from_dict(obj["memory"]) if obj.get("memory") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/accelerator_vendor.py` & `perian-0.2.0/perian/models/accelerator_vendor.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/availability.py` & `perian-0.2.0/perian/models/availability.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/availability_query.py` & `perian-0.2.0/perian/models/reference_id_query_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictBool
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
+from perian.models.id1 import Id1
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AvailabilityQuery(BaseModel):
+class ReferenceIdQueryOutput(BaseModel):
     """
-    AvailabilityQuery
+    ReferenceIdQueryOutput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    available: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "available"]
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    id: Optional[Id1] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "id"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -47,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AvailabilityQuery from a JSON string"""
+        """Create an instance of ReferenceIdQueryOutput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,26 +75,29 @@
         )
         # override the default output from pydantic by calling `to_dict()` of operator
         if self.operator:
             _dict['operator'] = self.operator.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of id
+        if self.id:
+            _dict['id'] = self.id.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AvailabilityQuery from a dict"""
+        """Create an instance of ReferenceIdQueryOutput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
-            "available": obj.get("available")
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "id": Id1.from_dict(obj["id"]) if obj.get("id") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/availability_source.py` & `perian-0.2.0/perian/models/availability_source.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/bandwidth.py` & `perian-0.2.0/perian/models/bandwidth.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/bandwidth_limits.py` & `perian-0.2.0/perian/models/bandwidth_limits.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/bandwidth_sla.py` & `perian-0.2.0/perian/models/bandwidth_sla.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/bandwidth_units.py` & `perian-0.2.0/perian/models/bandwidth_units.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/command.py` & `perian-0.2.0/perian/models/command.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/compute_billing_period.py` & `perian-0.2.0/perian/models/status.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class ComputeBillingPeriod(str, Enum):
+class Status(str, Enum):
     """
-    ComputeBillingPeriod
+    Status
     """
 
     """
     allowed enum values
     """
-    PER_SECOND = 'PER_SECOND'
-    PER_MINUTE = 'PER_MINUTE'
-    PER_HOUR = 'PER_HOUR'
-    PER_10_MINUTES = 'PER_10_MINUTES'
-    UNDEFINED = 'UNDEFINED'
+    ACTIVE = 'Active'
+    INACTIVE = 'Inactive'
+    UNDEFINED = 'Undefined'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of ComputeBillingPeriod from a JSON string"""
+        """Create an instance of Status from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `perian-0.1.25/perian/models/compute_instance_type.py` & `perian-0.2.0/perian/models/compute_instance_type.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/cpu.py` & `perian-0.2.0/perian/models/cpu.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/cpu_data.py` & `perian-0.2.0/perian/models/cpu_data.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/cpu_query.py` & `perian-0.2.0/perian/models/price_query_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,32 +13,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictFloat, StrictInt
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from pydantic import BaseModel
+from typing import Any, ClassVar, Dict, List, Optional
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
+from perian.models.unit_price import UnitPrice
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CpuQuery(BaseModel):
+class PriceQueryInput(BaseModel):
     """
-    CpuQuery
+    PriceQueryInput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    no: Optional[StrictInt] = None
-    cores: Optional[StrictInt] = None
-    threads: Optional[StrictInt] = None
-    speed: Optional[Union[StrictFloat, StrictInt]] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "no", "cores", "threads", "speed"]
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    unit_price: Optional[UnitPrice] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "unit_price"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -50,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CpuQuery from a JSON string"""
+        """Create an instance of PriceQueryInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -77,29 +75,29 @@
         )
         # override the default output from pydantic by calling `to_dict()` of operator
         if self.operator:
             _dict['operator'] = self.operator.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of unit_price
+        if self.unit_price:
+            _dict['unit_price'] = self.unit_price.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CpuQuery from a dict"""
+        """Create an instance of PriceQueryInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
-            "no": obj.get("no"),
-            "cores": obj.get("cores"),
-            "threads": obj.get("threads"),
-            "speed": obj.get("speed")
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "unit_price": UnitPrice.from_dict(obj["unit_price"]) if obj.get("unit_price") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/create_admin_success.py` & `perian-0.2.0/perian/models/default_success.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateAdminSuccess(BaseModel):
+class DefaultSuccess(BaseModel):
     """
-    CreateAdminSuccess
+    DefaultSuccess
     """ # noqa: E501
     status: Optional[StrictStr] = 'Success'
     message: Optional[StrictStr] = 'Operation was successful'
-    detail: Optional[StrictStr] = 'Global admin created successfully'
+    detail: Optional[StrictStr] = ''
     status_code: Optional[StrictInt] = 200
     __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateAdminSuccess from a JSON string"""
+        """Create an instance of DefaultSuccess from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,23 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateAdminSuccess from a dict"""
+        """Create an instance of DefaultSuccess from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status") if obj.get("status") is not None else 'Success',
             "message": obj.get("message") if obj.get("message") is not None else 'Operation was successful',
-            "detail": obj.get("detail") if obj.get("detail") is not None else 'Global admin created successfully',
+            "detail": obj.get("detail") if obj.get("detail") is not None else '',
             "status_code": obj.get("status_code") if obj.get("status_code") is not None else 200
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/create_global_admin_request.py` & `perian-0.2.0/perian/models/create_job_success.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateGlobalAdminRequest(BaseModel):
+class CreateJobSuccess(BaseModel):
     """
-    CreateGlobalAdminRequest
+    CreateJobSuccess
     """ # noqa: E501
-    mail_address: Optional[StrictStr] = None
-    setup_token: Optional[StrictStr] = None
-    password: Optional[StrictStr] = ''
-    firstname: Optional[StrictStr] = ''
-    lastname: Optional[StrictStr] = ''
-    __properties: ClassVar[List[str]] = ["mail_address", "setup_token", "password", "firstname", "lastname"]
+    status: Optional[StrictStr] = 'Success'
+    message: Optional[StrictStr] = 'Job created successfully'
+    detail: Optional[StrictStr] = ''
+    status_code: Optional[StrictInt] = 200
+    id: StrictStr
+    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code", "id"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateGlobalAdminRequest from a JSON string"""
+        """Create an instance of CreateJobSuccess from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,24 +72,24 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateGlobalAdminRequest from a dict"""
+        """Create an instance of CreateJobSuccess from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "mail_address": obj.get("mail_address"),
-            "setup_token": obj.get("setup_token"),
-            "password": obj.get("password") if obj.get("password") is not None else '',
-            "firstname": obj.get("firstname") if obj.get("firstname") is not None else '',
-            "lastname": obj.get("lastname") if obj.get("lastname") is not None else ''
+            "status": obj.get("status") if obj.get("status") is not None else 'Success',
+            "message": obj.get("message") if obj.get("message") is not None else 'Job created successfully',
+            "detail": obj.get("detail") if obj.get("detail") is not None else '',
+            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 200,
+            "id": obj.get("id")
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/create_job_request.py` & `perian-0.2.0/perian/models/create_job_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,31 +13,35 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
 from perian.models.create_job_request_docker_registry_credentials import CreateJobRequestDockerRegistryCredentials
+from perian.models.create_job_request_requirements import CreateJobRequestRequirements
 from perian.models.docker_run_parameters import DockerRunParameters
+from perian.models.instance_type_id import InstanceTypeId
 from perian.models.os_storage_config import OSStorageConfig
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateJobRequest(BaseModel):
     """
     CreateJobRequest
     """ # noqa: E501
-    instance_type_id: Optional[StrictStr] = None
+    instance_type_id: Optional[InstanceTypeId] = None
+    auto_failover_instance_type: Optional[StrictBool] = False
     os_storage_config: Optional[OSStorageConfig] = None
+    requirements: Optional[CreateJobRequestRequirements] = None
     docker_run_parameters: Optional[DockerRunParameters] = None
     docker_registry_credentials: Optional[CreateJobRequestDockerRegistryCredentials] = None
-    __properties: ClassVar[List[str]] = ["instance_type_id", "os_storage_config", "docker_run_parameters", "docker_registry_credentials"]
+    __properties: ClassVar[List[str]] = ["instance_type_id", "auto_failover_instance_type", "os_storage_config", "requirements", "docker_run_parameters", "docker_registry_credentials"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -70,17 +74,23 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of instance_type_id
+        if self.instance_type_id:
+            _dict['instance_type_id'] = self.instance_type_id.to_dict()
         # override the default output from pydantic by calling `to_dict()` of os_storage_config
         if self.os_storage_config:
             _dict['os_storage_config'] = self.os_storage_config.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of requirements
+        if self.requirements:
+            _dict['requirements'] = self.requirements.to_dict()
         # override the default output from pydantic by calling `to_dict()` of docker_run_parameters
         if self.docker_run_parameters:
             _dict['docker_run_parameters'] = self.docker_run_parameters.to_dict()
         # override the default output from pydantic by calling `to_dict()` of docker_registry_credentials
         if self.docker_registry_credentials:
             _dict['docker_registry_credentials'] = self.docker_registry_credentials.to_dict()
         return _dict
@@ -91,15 +101,17 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "instance_type_id": obj.get("instance_type_id"),
+            "instance_type_id": InstanceTypeId.from_dict(obj["instance_type_id"]) if obj.get("instance_type_id") is not None else None,
+            "auto_failover_instance_type": obj.get("auto_failover_instance_type") if obj.get("auto_failover_instance_type") is not None else False,
             "os_storage_config": OSStorageConfig.from_dict(obj["os_storage_config"]) if obj.get("os_storage_config") is not None else None,
+            "requirements": CreateJobRequestRequirements.from_dict(obj["requirements"]) if obj.get("requirements") is not None else None,
             "docker_run_parameters": DockerRunParameters.from_dict(obj["docker_run_parameters"]) if obj.get("docker_run_parameters") is not None else None,
             "docker_registry_credentials": CreateJobRequestDockerRegistryCredentials.from_dict(obj["docker_registry_credentials"]) if obj.get("docker_registry_credentials") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/create_job_request_docker_registry_credentials.py` & `perian-0.2.0/perian/models/create_job_request_docker_registry_credentials.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/create_job_success.py` & `perian-0.2.0/perian/models/default_server_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,24 +18,23 @@
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateJobSuccess(BaseModel):
+class DefaultServerError(BaseModel):
     """
-    CreateJobSuccess
+    DefaultServerError
     """ # noqa: E501
-    status: Optional[StrictStr] = 'Success'
-    message: Optional[StrictStr] = 'Job created successfully'
+    status: Optional[StrictStr] = 'Error'
+    message: Optional[StrictStr] = 'Operation failed due to a server error'
     detail: Optional[StrictStr] = ''
-    status_code: Optional[StrictInt] = 200
-    id: StrictStr
-    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code", "id"]
+    status_code: Optional[StrictInt] = 500
+    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -47,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateJobSuccess from a JSON string"""
+        """Create an instance of DefaultServerError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,24 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateJobSuccess from a dict"""
+        """Create an instance of DefaultServerError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "status": obj.get("status") if obj.get("status") is not None else 'Success',
-            "message": obj.get("message") if obj.get("message") is not None else 'Job created successfully',
+            "status": obj.get("status") if obj.get("status") is not None else 'Error',
+            "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a server error',
             "detail": obj.get("detail") if obj.get("detail") is not None else '',
-            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 200,
-            "id": obj.get("id")
+            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 500
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/create_organization_request.py` & `perian-0.2.0/perian/models/zone.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,25 +15,26 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.reference import Reference
+from perian.models.status import Status
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateOrganizationRequest(BaseModel):
+class Zone(BaseModel):
     """
-    CreateOrganizationRequest
+    Zone
     """ # noqa: E501
+    id: Optional[StrictStr] = None
     name: Optional[StrictStr] = None
-    reference: Optional[Reference] = None
-    __properties: ClassVar[List[str]] = ["name", "reference"]
+    status: Optional[Status] = None
+    __properties: ClassVar[List[str]] = ["id", "name", "status"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -45,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateOrganizationRequest from a JSON string"""
+        """Create an instance of Zone from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,28 +67,26 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of reference
-        if self.reference:
-            _dict['reference'] = self.reference.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateOrganizationRequest from a dict"""
+        """Create an instance of Zone from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "id": obj.get("id"),
             "name": obj.get("name"),
-            "reference": Reference.from_dict(obj["reference"]) if obj.get("reference") is not None else None
+            "status": obj.get("status")
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/create_organization_success.py` & `perian-0.2.0/perian/models/api_router_instance_type_incorrect_parameter_error.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.organization import Organization
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateOrganizationSuccess(BaseModel):
+class ApiRouterInstanceTypeIncorrectParameterError(BaseModel):
     """
-    CreateOrganizationSuccess
+    ApiRouterInstanceTypeIncorrectParameterError
     """ # noqa: E501
-    status: Optional[StrictStr] = 'Success'
-    message: Optional[StrictStr] = 'Operation was successful'
-    detail: Optional[StrictStr] = 'Organization created successfully'
-    status_code: Optional[StrictInt] = 200
-    organization: Organization
-    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code", "organization"]
+    status: Optional[StrictStr] = 'Error'
+    message: Optional[StrictStr] = 'Operation failed due to a client error'
+    detail: Optional[StrictStr] = 'Please either provide a specific instance_type ID or a query'
+    status_code: Optional[StrictInt] = 400
+    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -48,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateOrganizationSuccess from a JSON string"""
+        """Create an instance of ApiRouterInstanceTypeIncorrectParameterError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,31 +67,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of organization
-        if self.organization:
-            _dict['organization'] = self.organization.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateOrganizationSuccess from a dict"""
+        """Create an instance of ApiRouterInstanceTypeIncorrectParameterError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "status": obj.get("status") if obj.get("status") is not None else 'Success',
-            "message": obj.get("message") if obj.get("message") is not None else 'Operation was successful',
-            "detail": obj.get("detail") if obj.get("detail") is not None else 'Organization created successfully',
-            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 200,
-            "organization": Organization.from_dict(obj["organization"]) if obj.get("organization") is not None else None
+            "status": obj.get("status") if obj.get("status") is not None else 'Error',
+            "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
+            "detail": obj.get("detail") if obj.get("detail") is not None else 'Please either provide a specific instance_type ID or a query',
+            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/create_service_account_request.py` & `perian-0.2.0/perian/models/provider_properties.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
+from perian.models.billing_granularity import BillingGranularity
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateServiceAccountRequest(BaseModel):
+class ProviderProperties(BaseModel):
     """
-    CreateServiceAccountRequest
+    ProviderProperties
     """ # noqa: E501
-    service_account_name: Optional[StrictStr] = ''
-    roles: Optional[List[StrictStr]] = None
-    __properties: ClassVar[List[str]] = ["service_account_name", "roles"]
+    compute_billing_granularity: Optional[BillingGranularity] = None
+    __properties: ClassVar[List[str]] = ["compute_billing_granularity"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -44,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateServiceAccountRequest from a JSON string"""
+        """Create an instance of ProviderProperties from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,21 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateServiceAccountRequest from a dict"""
+        """Create an instance of ProviderProperties from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "service_account_name": obj.get("service_account_name") if obj.get("service_account_name") is not None else '',
-            "roles": obj.get("roles")
+            "compute_billing_granularity": obj.get("compute_billing_granularity")
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/create_service_account_success.py` & `perian-0.2.0/perian/models/incorrect_create_job_parameter_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,25 +18,23 @@
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateServiceAccountSuccess(BaseModel):
+class IncorrectCreateJobParameterError(BaseModel):
     """
-    CreateServiceAccountSuccess
+    IncorrectCreateJobParameterError
     """ # noqa: E501
-    status: Optional[StrictStr] = 'Success'
-    message: Optional[StrictStr] = 'Operation was successful'
-    detail: Optional[StrictStr] = 'Service account created successfully'
-    status_code: Optional[StrictInt] = 200
-    client_id: Optional[StrictStr] = ''
-    client_secret: Optional[StrictStr] = ''
-    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code", "client_id", "client_secret"]
+    status: Optional[StrictStr] = 'Error'
+    message: Optional[StrictStr] = 'Operation failed due to a client error'
+    detail: Optional[StrictStr] = 'Please either provide a specific instance type ID or requirements for the job'
+    status_code: Optional[StrictInt] = 400
+    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -48,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateServiceAccountSuccess from a JSON string"""
+        """Create an instance of IncorrectCreateJobParameterError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,25 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateServiceAccountSuccess from a dict"""
+        """Create an instance of IncorrectCreateJobParameterError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "status": obj.get("status") if obj.get("status") is not None else 'Success',
-            "message": obj.get("message") if obj.get("message") is not None else 'Operation was successful',
-            "detail": obj.get("detail") if obj.get("detail") is not None else 'Service account created successfully',
-            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 200,
-            "client_id": obj.get("client_id") if obj.get("client_id") is not None else '',
-            "client_secret": obj.get("client_secret") if obj.get("client_secret") is not None else ''
+            "status": obj.get("status") if obj.get("status") is not None else 'Error',
+            "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
+            "detail": obj.get("detail") if obj.get("detail") is not None else 'Please either provide a specific instance type ID or requirements for the job',
+            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/create_user_request.py` & `perian-0.2.0/perian/models/job_already_done_error.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,30 +13,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateUserRequest(BaseModel):
+class JobAlreadyDoneError(BaseModel):
     """
-    CreateUserRequest
+    JobAlreadyDoneError
     """ # noqa: E501
-    username: Optional[StrictStr] = ''
-    mail_address: Optional[StrictStr] = ''
-    password: Optional[StrictStr] = ''
-    firstname: Optional[StrictStr] = ''
-    lastname: Optional[StrictStr] = '[]'
-    roles: Optional[List[StrictStr]] = None
-    __properties: ClassVar[List[str]] = ["username", "mail_address", "password", "firstname", "lastname", "roles"]
+    status: Optional[StrictStr] = 'Error'
+    message: Optional[StrictStr] = 'Operation failed due to a client error'
+    detail: Optional[StrictStr] = 'The job you are trying to cancel is already complete.'
+    status_code: Optional[StrictInt] = 400
+    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -48,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateUserRequest from a JSON string"""
+        """Create an instance of JobAlreadyDoneError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,25 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateUserRequest from a dict"""
+        """Create an instance of JobAlreadyDoneError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "username": obj.get("username") if obj.get("username") is not None else '',
-            "mail_address": obj.get("mail_address") if obj.get("mail_address") is not None else '',
-            "password": obj.get("password") if obj.get("password") is not None else '',
-            "firstname": obj.get("firstname") if obj.get("firstname") is not None else '',
-            "lastname": obj.get("lastname") if obj.get("lastname") is not None else '[]',
-            "roles": obj.get("roles")
+            "status": obj.get("status") if obj.get("status") is not None else 'Error',
+            "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
+            "detail": obj.get("detail") if obj.get("detail") is not None else 'The job you are trying to cancel is already complete.',
+            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/create_user_success.py` & `perian-0.2.0/perian/models/no_job_found_error.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateUserSuccess(BaseModel):
+class NoJobFoundError(BaseModel):
     """
-    CreateUserSuccess
+    NoJobFoundError
     """ # noqa: E501
-    status: Optional[StrictStr] = 'Success'
-    message: Optional[StrictStr] = 'Operation was successful'
-    detail: Optional[StrictStr] = 'User created successfully'
-    status_code: Optional[StrictInt] = 200
+    status: Optional[StrictStr] = 'Error'
+    message: Optional[StrictStr] = 'Operation failed due to a client error'
+    detail: Optional[StrictStr] = 'No job found with specified ID'
+    status_code: Optional[StrictInt] = 400
     __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateUserSuccess from a JSON string"""
+        """Create an instance of NoJobFoundError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,23 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateUserSuccess from a dict"""
+        """Create an instance of NoJobFoundError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "status": obj.get("status") if obj.get("status") is not None else 'Success',
-            "message": obj.get("message") if obj.get("message") is not None else 'Operation was successful',
-            "detail": obj.get("detail") if obj.get("detail") is not None else 'User created successfully',
-            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 200
+            "status": obj.get("status") if obj.get("status") is not None else 'Error',
+            "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
+            "detail": obj.get("detail") if obj.get("detail") is not None else 'No job found with specified ID',
+            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/currency.py` & `perian-0.2.0/perian/models/currency.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/default_client_error.py` & `perian-0.2.0/perian/models/default_client_error.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/default_server_error.py` & `perian-0.2.0/perian/models/accelerator_type_not_found_error.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class DefaultServerError(BaseModel):
+class AcceleratorTypeNotFoundError(BaseModel):
     """
-    DefaultServerError
+    AcceleratorTypeNotFoundError
     """ # noqa: E501
     status: Optional[StrictStr] = 'Error'
-    message: Optional[StrictStr] = 'Operation failed due to a server error'
-    detail: Optional[StrictStr] = ''
-    status_code: Optional[StrictInt] = 500
+    message: Optional[StrictStr] = 'Operation failed due to a client error'
+    detail: Optional[StrictStr] = 'No accelerator type found'
+    status_code: Optional[StrictInt] = 400
     __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of DefaultServerError from a JSON string"""
+        """Create an instance of AcceleratorTypeNotFoundError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,23 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of DefaultServerError from a dict"""
+        """Create an instance of AcceleratorTypeNotFoundError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status") if obj.get("status") is not None else 'Error',
-            "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a server error',
-            "detail": obj.get("detail") if obj.get("detail") is not None else '',
-            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 500
+            "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
+            "detail": obj.get("detail") if obj.get("detail") is not None else 'No accelerator type found',
+            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/description.py` & `perian-0.2.0/perian/models/description.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/docker_registry_credentials.py` & `perian-0.2.0/perian/models/docker_registry_credentials.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/docker_run_parameters.py` & `perian-0.2.0/perian/models/docker_run_parameters.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/done_at.py` & `perian-0.2.0/perian/models/done_at.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/get_instance_types_success.py` & `perian-0.2.0/perian/models/get_instance_types_success.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,31 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from perian.models.instance_type_view import InstanceTypeView
+from perian.models.pagination_metadata import PaginationMetadata
 from typing import Optional, Set
 from typing_extensions import Self
 
 class GetInstanceTypesSuccess(BaseModel):
     """
     GetInstanceTypesSuccess
     """ # noqa: E501
     status: Optional[StrictStr] = 'Success'
     message: Optional[StrictStr] = 'Operation was successful'
     detail: Optional[StrictStr] = ''
     status_code: Optional[StrictInt] = 200
     limit: Optional[StrictInt] = 0
     no: Optional[StrictInt] = 0
     instance_types: Optional[List[InstanceTypeView]] = None
-    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code", "limit", "no", "instance_types"]
+    pagination: Optional[PaginationMetadata] = None
+    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code", "limit", "no", "instance_types", "pagination"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -78,14 +80,17 @@
         # override the default output from pydantic by calling `to_dict()` of each item in instance_types (list)
         _items = []
         if self.instance_types:
             for _item in self.instance_types:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['instance_types'] = _items
+        # override the default output from pydantic by calling `to_dict()` of pagination
+        if self.pagination:
+            _dict['pagination'] = self.pagination.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of GetInstanceTypesSuccess from a dict"""
         if obj is None:
             return None
@@ -96,12 +101,13 @@
         _obj = cls.model_validate({
             "status": obj.get("status") if obj.get("status") is not None else 'Success',
             "message": obj.get("message") if obj.get("message") is not None else 'Operation was successful',
             "detail": obj.get("detail") if obj.get("detail") is not None else '',
             "status_code": obj.get("status_code") if obj.get("status_code") is not None else 200,
             "limit": obj.get("limit") if obj.get("limit") is not None else 0,
             "no": obj.get("no") if obj.get("no") is not None else 0,
-            "instance_types": [InstanceTypeView.from_dict(_item) for _item in obj["instance_types"]] if obj.get("instance_types") is not None else None
+            "instance_types": [InstanceTypeView.from_dict(_item) for _item in obj["instance_types"]] if obj.get("instance_types") is not None else None,
+            "pagination": PaginationMetadata.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/get_jobs_success.py` & `perian-0.2.0/perian/models/api_router_job_instance_type_not_found_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.job_view import JobView
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GetJobsSuccess(BaseModel):
+class ApiRouterJobInstanceTypeNotFoundError(BaseModel):
     """
-    GetJobsSuccess
+    ApiRouterJobInstanceTypeNotFoundError
     """ # noqa: E501
-    status: Optional[StrictStr] = 'Success'
-    message: Optional[StrictStr] = 'Operation was successful'
-    detail: Optional[StrictStr] = ''
-    status_code: Optional[StrictInt] = 200
-    jobs: List[JobView]
-    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code", "jobs"]
+    status: Optional[StrictStr] = 'Error'
+    message: Optional[StrictStr] = 'Operation failed due to a client error'
+    detail: Optional[StrictStr] = 'The selected Instance Type was not found'
+    status_code: Optional[StrictInt] = 400
+    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -48,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GetJobsSuccess from a JSON string"""
+        """Create an instance of ApiRouterJobInstanceTypeNotFoundError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,35 +67,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in jobs (list)
-        _items = []
-        if self.jobs:
-            for _item in self.jobs:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['jobs'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GetJobsSuccess from a dict"""
+        """Create an instance of ApiRouterJobInstanceTypeNotFoundError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "status": obj.get("status") if obj.get("status") is not None else 'Success',
-            "message": obj.get("message") if obj.get("message") is not None else 'Operation was successful',
-            "detail": obj.get("detail") if obj.get("detail") is not None else '',
-            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 200,
-            "jobs": [JobView.from_dict(_item) for _item in obj["jobs"]] if obj.get("jobs") is not None else None
+            "status": obj.get("status") if obj.get("status") is not None else 'Error',
+            "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
+            "detail": obj.get("detail") if obj.get("detail") is not None else 'The selected Instance Type was not found',
+            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/http_validation_error.py` & `perian-0.2.0/perian/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/id.py` & `perian-0.2.0/perian/models/id.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/image_tag.py` & `perian-0.2.0/perian/models/image_tag.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/instance_type_blocked_error.py` & `perian-0.2.0/perian/models/no_parameter_error.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class InstanceTypeBlockedError(BaseModel):
+class NoParameterError(BaseModel):
     """
-    InstanceTypeBlockedError
+    NoParameterError
     """ # noqa: E501
     status: Optional[StrictStr] = 'Error'
     message: Optional[StrictStr] = 'Operation failed due to a client error'
-    detail: Optional[StrictStr] = 'The selected Instance Type is blocked for your account'
+    detail: Optional[StrictStr] = 'Please provide a specific job ID'
     status_code: Optional[StrictInt] = 400
     __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of InstanceTypeBlockedError from a JSON string"""
+        """Create an instance of NoParameterError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,23 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of InstanceTypeBlockedError from a dict"""
+        """Create an instance of NoParameterError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status") if obj.get("status") is not None else 'Error',
             "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
-            "detail": obj.get("detail") if obj.get("detail") is not None else 'The selected Instance Type is blocked for your account',
+            "detail": obj.get("detail") if obj.get("detail") is not None else 'Please provide a specific job ID',
             "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/instance_type_query.py` & `perian-0.2.0/perian/models/instance_type_query_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,54 +15,54 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.accelerator_query_memory import AcceleratorQueryMemory
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input_memory import AcceleratorQueryInputMemory
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
 from perian.models.id import Id
-from perian.models.instance_type_query_accelerator import InstanceTypeQueryAccelerator
-from perian.models.instance_type_query_availability import InstanceTypeQueryAvailability
-from perian.models.instance_type_query_cpu import InstanceTypeQueryCpu
-from perian.models.instance_type_query_name import InstanceTypeQueryName
-from perian.models.instance_type_query_network import InstanceTypeQueryNetwork
-from perian.models.instance_type_query_price import InstanceTypeQueryPrice
-from perian.models.instance_type_query_provider import InstanceTypeQueryProvider
-from perian.models.instance_type_query_reference_id import InstanceTypeQueryReferenceId
-from perian.models.instance_type_query_region import InstanceTypeQueryRegion
-from perian.models.instance_type_query_storage import InstanceTypeQueryStorage
-from perian.models.instance_type_query_type import InstanceTypeQueryType
-from perian.models.instance_type_query_zone import InstanceTypeQueryZone
+from perian.models.instance_type_query_input_accelerator import InstanceTypeQueryInputAccelerator
+from perian.models.instance_type_query_input_availability import InstanceTypeQueryInputAvailability
+from perian.models.instance_type_query_input_cpu import InstanceTypeQueryInputCpu
+from perian.models.instance_type_query_input_network import InstanceTypeQueryInputNetwork
+from perian.models.instance_type_query_input_price import InstanceTypeQueryInputPrice
+from perian.models.instance_type_query_input_provider import InstanceTypeQueryInputProvider
+from perian.models.instance_type_query_input_reference_id import InstanceTypeQueryInputReferenceId
+from perian.models.instance_type_query_input_region import InstanceTypeQueryInputRegion
+from perian.models.instance_type_query_input_storage import InstanceTypeQueryInputStorage
+from perian.models.instance_type_query_input_zone import InstanceTypeQueryInputZone
+from perian.models.name1 import Name1
+from perian.models.type import Type
 from typing import Optional, Set
 from typing_extensions import Self
 
-class InstanceTypeQuery(BaseModel):
+class InstanceTypeQueryInput(BaseModel):
     """
-    InstanceTypeQuery
+    InstanceTypeQueryInput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
     id: Optional[Id] = None
-    provider: Optional[InstanceTypeQueryProvider] = None
-    region: Optional[InstanceTypeQueryRegion] = None
-    zone: Optional[InstanceTypeQueryZone] = None
-    reference_id: Optional[InstanceTypeQueryReferenceId] = None
-    name: Optional[InstanceTypeQueryName] = None
-    cpu: Optional[InstanceTypeQueryCpu] = None
-    accelerator: Optional[InstanceTypeQueryAccelerator] = None
-    ram: Optional[AcceleratorQueryMemory] = None
-    storage: Optional[InstanceTypeQueryStorage] = None
-    network: Optional[InstanceTypeQueryNetwork] = None
-    price: Optional[InstanceTypeQueryPrice] = None
-    availability: Optional[InstanceTypeQueryAvailability] = None
-    type: Optional[InstanceTypeQueryType] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "id", "provider", "region", "zone", "reference_id", "name", "cpu", "accelerator", "ram", "storage", "network", "price", "availability", "type"]
+    region: Optional[InstanceTypeQueryInputRegion] = None
+    zone: Optional[InstanceTypeQueryInputZone] = None
+    name: Optional[Name1] = None
+    cpu: Optional[InstanceTypeQueryInputCpu] = None
+    accelerator: Optional[InstanceTypeQueryInputAccelerator] = None
+    ram: Optional[AcceleratorQueryInputMemory] = None
+    storage: Optional[InstanceTypeQueryInputStorage] = None
+    network: Optional[InstanceTypeQueryInputNetwork] = None
+    price: Optional[InstanceTypeQueryInputPrice] = None
+    availability: Optional[InstanceTypeQueryInputAvailability] = None
+    type: Optional[Type] = None
+    provider: Optional[InstanceTypeQueryInputProvider] = None
+    reference_id: Optional[InstanceTypeQueryInputReferenceId] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "id", "region", "zone", "name", "cpu", "accelerator", "ram", "storage", "network", "price", "availability", "type", "provider", "reference_id"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -74,15 +74,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of InstanceTypeQuery from a JSON string"""
+        """Create an instance of InstanceTypeQueryInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -104,26 +104,20 @@
             _dict['operator'] = self.operator.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
         # override the default output from pydantic by calling `to_dict()` of id
         if self.id:
             _dict['id'] = self.id.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of provider
-        if self.provider:
-            _dict['provider'] = self.provider.to_dict()
         # override the default output from pydantic by calling `to_dict()` of region
         if self.region:
             _dict['region'] = self.region.to_dict()
         # override the default output from pydantic by calling `to_dict()` of zone
         if self.zone:
             _dict['zone'] = self.zone.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of reference_id
-        if self.reference_id:
-            _dict['reference_id'] = self.reference_id.to_dict()
         # override the default output from pydantic by calling `to_dict()` of name
         if self.name:
             _dict['name'] = self.name.to_dict()
         # override the default output from pydantic by calling `to_dict()` of cpu
         if self.cpu:
             _dict['cpu'] = self.cpu.to_dict()
         # override the default output from pydantic by calling `to_dict()` of accelerator
@@ -143,39 +137,45 @@
             _dict['price'] = self.price.to_dict()
         # override the default output from pydantic by calling `to_dict()` of availability
         if self.availability:
             _dict['availability'] = self.availability.to_dict()
         # override the default output from pydantic by calling `to_dict()` of type
         if self.type:
             _dict['type'] = self.type.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of provider
+        if self.provider:
+            _dict['provider'] = self.provider.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of reference_id
+        if self.reference_id:
+            _dict['reference_id'] = self.reference_id.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of InstanceTypeQuery from a dict"""
+        """Create an instance of InstanceTypeQueryInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
             "id": Id.from_dict(obj["id"]) if obj.get("id") is not None else None,
-            "provider": InstanceTypeQueryProvider.from_dict(obj["provider"]) if obj.get("provider") is not None else None,
-            "region": InstanceTypeQueryRegion.from_dict(obj["region"]) if obj.get("region") is not None else None,
-            "zone": InstanceTypeQueryZone.from_dict(obj["zone"]) if obj.get("zone") is not None else None,
-            "reference_id": InstanceTypeQueryReferenceId.from_dict(obj["reference_id"]) if obj.get("reference_id") is not None else None,
-            "name": InstanceTypeQueryName.from_dict(obj["name"]) if obj.get("name") is not None else None,
-            "cpu": InstanceTypeQueryCpu.from_dict(obj["cpu"]) if obj.get("cpu") is not None else None,
-            "accelerator": InstanceTypeQueryAccelerator.from_dict(obj["accelerator"]) if obj.get("accelerator") is not None else None,
-            "ram": AcceleratorQueryMemory.from_dict(obj["ram"]) if obj.get("ram") is not None else None,
-            "storage": InstanceTypeQueryStorage.from_dict(obj["storage"]) if obj.get("storage") is not None else None,
-            "network": InstanceTypeQueryNetwork.from_dict(obj["network"]) if obj.get("network") is not None else None,
-            "price": InstanceTypeQueryPrice.from_dict(obj["price"]) if obj.get("price") is not None else None,
-            "availability": InstanceTypeQueryAvailability.from_dict(obj["availability"]) if obj.get("availability") is not None else None,
-            "type": InstanceTypeQueryType.from_dict(obj["type"]) if obj.get("type") is not None else None
+            "region": InstanceTypeQueryInputRegion.from_dict(obj["region"]) if obj.get("region") is not None else None,
+            "zone": InstanceTypeQueryInputZone.from_dict(obj["zone"]) if obj.get("zone") is not None else None,
+            "name": Name1.from_dict(obj["name"]) if obj.get("name") is not None else None,
+            "cpu": InstanceTypeQueryInputCpu.from_dict(obj["cpu"]) if obj.get("cpu") is not None else None,
+            "accelerator": InstanceTypeQueryInputAccelerator.from_dict(obj["accelerator"]) if obj.get("accelerator") is not None else None,
+            "ram": AcceleratorQueryInputMemory.from_dict(obj["ram"]) if obj.get("ram") is not None else None,
+            "storage": InstanceTypeQueryInputStorage.from_dict(obj["storage"]) if obj.get("storage") is not None else None,
+            "network": InstanceTypeQueryInputNetwork.from_dict(obj["network"]) if obj.get("network") is not None else None,
+            "price": InstanceTypeQueryInputPrice.from_dict(obj["price"]) if obj.get("price") is not None else None,
+            "availability": InstanceTypeQueryInputAvailability.from_dict(obj["availability"]) if obj.get("availability") is not None else None,
+            "type": Type.from_dict(obj["type"]) if obj.get("type") is not None else None,
+            "provider": InstanceTypeQueryInputProvider.from_dict(obj["provider"]) if obj.get("provider") is not None else None,
+            "reference_id": InstanceTypeQueryInputReferenceId.from_dict(obj["reference_id"]) if obj.get("reference_id") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_accelerator.py` & `perian-0.2.0/perian/models/accelerator_query_input_operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.accelerator_query import AcceleratorQuery
+from perian.models.operator import Operator
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYACCELERATOR_ANY_OF_SCHEMAS = ["AcceleratorQuery", "object"]
+ACCELERATORQUERYINPUTOPERATOR_ANY_OF_SCHEMAS = ["Operator", "object"]
 
-class InstanceTypeQueryAccelerator(BaseModel):
+class AcceleratorQueryInputOperator(BaseModel):
     """
-    InstanceTypeQueryAccelerator
+    AcceleratorQueryInputOperator
     """
 
-    # data type: AcceleratorQuery
-    anyof_schema_1_validator: Optional[AcceleratorQuery] = None
+    # data type: Operator
+    anyof_schema_1_validator: Optional[Operator] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[AcceleratorQuery, object]] = None
+        actual_instance: Optional[Union[Operator, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["AcceleratorQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["Operator", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,46 +54,46 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryAccelerator.model_construct()
+        instance = AcceleratorQueryInputOperator.model_construct()
         error_messages = []
-        # validate data type: AcceleratorQuery
-        if not isinstance(v, AcceleratorQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `AcceleratorQuery`")
+        # validate data type: Operator
+        if not isinstance(v, Operator):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `Operator`")
         else:
             return v
 
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryAccelerator with anyOf schemas: AcceleratorQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in AcceleratorQueryInputOperator with anyOf schemas: Operator, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[AcceleratorQuery] = None
+        # anyof_schema_1_validator: Optional[Operator] = None
         try:
-            instance.actual_instance = AcceleratorQuery.from_json(json_str)
+            instance.actual_instance = Operator.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
@@ -101,29 +101,29 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryAccelerator with anyOf schemas: AcceleratorQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into AcceleratorQueryInputOperator with anyOf schemas: Operator, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], AcceleratorQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], Operator, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_availability.py` & `perian-0.2.0/perian/models/instance_type_query_input_availability.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.availability_query import AvailabilityQuery
+from perian.models.availability_query_input import AvailabilityQueryInput
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYAVAILABILITY_ANY_OF_SCHEMAS = ["AvailabilityQuery", "object"]
+INSTANCETYPEQUERYINPUTAVAILABILITY_ANY_OF_SCHEMAS = ["AvailabilityQueryInput", "object"]
 
-class InstanceTypeQueryAvailability(BaseModel):
+class InstanceTypeQueryInputAvailability(BaseModel):
     """
-    InstanceTypeQueryAvailability
+    InstanceTypeQueryInputAvailability
     """
 
-    # data type: AvailabilityQuery
-    anyof_schema_1_validator: Optional[AvailabilityQuery] = None
+    # data type: AvailabilityQueryInput
+    anyof_schema_1_validator: Optional[AvailabilityQueryInput] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[AvailabilityQuery, object]] = None
+        actual_instance: Optional[Union[AvailabilityQueryInput, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["AvailabilityQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["AvailabilityQueryInput", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,46 +54,46 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryAvailability.model_construct()
+        instance = InstanceTypeQueryInputAvailability.model_construct()
         error_messages = []
-        # validate data type: AvailabilityQuery
-        if not isinstance(v, AvailabilityQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `AvailabilityQuery`")
+        # validate data type: AvailabilityQueryInput
+        if not isinstance(v, AvailabilityQueryInput):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `AvailabilityQueryInput`")
         else:
             return v
 
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryAvailability with anyOf schemas: AvailabilityQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryInputAvailability with anyOf schemas: AvailabilityQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[AvailabilityQuery] = None
+        # anyof_schema_1_validator: Optional[AvailabilityQueryInput] = None
         try:
-            instance.actual_instance = AvailabilityQuery.from_json(json_str)
+            instance.actual_instance = AvailabilityQueryInput.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
@@ -101,29 +101,29 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryAvailability with anyOf schemas: AvailabilityQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryInputAvailability with anyOf schemas: AvailabilityQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], AvailabilityQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], AvailabilityQueryInput, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_cpu.py` & `perian-0.2.0/perian/models/instance_type_query_input_cpu.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.cpu_query import CpuQuery
+from perian.models.cpu_query_input import CpuQueryInput
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYCPU_ANY_OF_SCHEMAS = ["CpuQuery", "object"]
+INSTANCETYPEQUERYINPUTCPU_ANY_OF_SCHEMAS = ["CpuQueryInput", "object"]
 
-class InstanceTypeQueryCpu(BaseModel):
+class InstanceTypeQueryInputCpu(BaseModel):
     """
-    InstanceTypeQueryCpu
+    InstanceTypeQueryInputCpu
     """
 
-    # data type: CpuQuery
-    anyof_schema_1_validator: Optional[CpuQuery] = None
+    # data type: CpuQueryInput
+    anyof_schema_1_validator: Optional[CpuQueryInput] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[CpuQuery, object]] = None
+        actual_instance: Optional[Union[CpuQueryInput, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["CpuQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["CpuQueryInput", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,46 +54,46 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryCpu.model_construct()
+        instance = InstanceTypeQueryInputCpu.model_construct()
         error_messages = []
-        # validate data type: CpuQuery
-        if not isinstance(v, CpuQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `CpuQuery`")
+        # validate data type: CpuQueryInput
+        if not isinstance(v, CpuQueryInput):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `CpuQueryInput`")
         else:
             return v
 
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryCpu with anyOf schemas: CpuQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryInputCpu with anyOf schemas: CpuQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[CpuQuery] = None
+        # anyof_schema_1_validator: Optional[CpuQueryInput] = None
         try:
-            instance.actual_instance = CpuQuery.from_json(json_str)
+            instance.actual_instance = CpuQueryInput.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
@@ -101,29 +101,29 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryCpu with anyOf schemas: CpuQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryInputCpu with anyOf schemas: CpuQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], CpuQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], CpuQueryInput, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_name.py` & `perian-0.2.0/perian/models/sustainable.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,37 +13,36 @@
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
-from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
+from pydantic import BaseModel, Field, StrictBool, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.name_query import NameQuery
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYNAME_ANY_OF_SCHEMAS = ["NameQuery", "object"]
+SUSTAINABLE_ANY_OF_SCHEMAS = ["bool", "object"]
 
-class InstanceTypeQueryName(BaseModel):
+class Sustainable(BaseModel):
     """
-    InstanceTypeQueryName
+    Sustainable
     """
 
-    # data type: NameQuery
-    anyof_schema_1_validator: Optional[NameQuery] = None
+    # data type: bool
+    anyof_schema_1_validator: Optional[StrictBool] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[NameQuery, object]] = None
+        actual_instance: Optional[Union[bool, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["NameQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["bool", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,76 +53,79 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryName.model_construct()
+        instance = Sustainable.model_construct()
         error_messages = []
-        # validate data type: NameQuery
-        if not isinstance(v, NameQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `NameQuery`")
-        else:
+        # validate data type: bool
+        try:
+            instance.anyof_schema_1_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryName with anyOf schemas: NameQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Sustainable with anyOf schemas: bool, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[NameQuery] = None
+        # deserialize data into bool
         try:
-            instance.actual_instance = NameQuery.from_json(json_str)
+            # validation
+            instance.anyof_schema_1_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryName with anyOf schemas: NameQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Sustainable with anyOf schemas: bool, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], NameQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], bool, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_network.py` & `perian-0.2.0/perian/models/instance_type_query_input_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.network_query import NetworkQuery
+from perian.models.network_query_input import NetworkQueryInput
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYNETWORK_ANY_OF_SCHEMAS = ["NetworkQuery", "object"]
+INSTANCETYPEQUERYINPUTNETWORK_ANY_OF_SCHEMAS = ["NetworkQueryInput", "object"]
 
-class InstanceTypeQueryNetwork(BaseModel):
+class InstanceTypeQueryInputNetwork(BaseModel):
     """
-    InstanceTypeQueryNetwork
+    InstanceTypeQueryInputNetwork
     """
 
-    # data type: NetworkQuery
-    anyof_schema_1_validator: Optional[NetworkQuery] = None
+    # data type: NetworkQueryInput
+    anyof_schema_1_validator: Optional[NetworkQueryInput] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[NetworkQuery, object]] = None
+        actual_instance: Optional[Union[NetworkQueryInput, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["NetworkQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["NetworkQueryInput", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,46 +54,46 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryNetwork.model_construct()
+        instance = InstanceTypeQueryInputNetwork.model_construct()
         error_messages = []
-        # validate data type: NetworkQuery
-        if not isinstance(v, NetworkQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `NetworkQuery`")
+        # validate data type: NetworkQueryInput
+        if not isinstance(v, NetworkQueryInput):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `NetworkQueryInput`")
         else:
             return v
 
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryNetwork with anyOf schemas: NetworkQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryInputNetwork with anyOf schemas: NetworkQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[NetworkQuery] = None
+        # anyof_schema_1_validator: Optional[NetworkQueryInput] = None
         try:
-            instance.actual_instance = NetworkQuery.from_json(json_str)
+            instance.actual_instance = NetworkQueryInput.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
@@ -101,29 +101,29 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryNetwork with anyOf schemas: NetworkQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryInputNetwork with anyOf schemas: NetworkQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], NetworkQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], NetworkQueryInput, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_price.py` & `perian-0.2.0/perian/models/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,35 +15,34 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.price_query import PriceQuery
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYPRICE_ANY_OF_SCHEMAS = ["PriceQuery", "object"]
+ERRORS_ANY_OF_SCHEMAS = ["object", "str"]
 
-class InstanceTypeQueryPrice(BaseModel):
+class Errors(BaseModel):
     """
-    InstanceTypeQueryPrice
+    Errors
     """
 
-    # data type: PriceQuery
-    anyof_schema_1_validator: Optional[PriceQuery] = None
+    # data type: str
+    anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[PriceQuery, object]] = None
+        actual_instance: Optional[Union[object, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["PriceQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["object", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,76 +53,79 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryPrice.model_construct()
+        instance = Errors.model_construct()
         error_messages = []
-        # validate data type: PriceQuery
-        if not isinstance(v, PriceQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `PriceQuery`")
-        else:
+        # validate data type: str
+        try:
+            instance.anyof_schema_1_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryPrice with anyOf schemas: PriceQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Errors with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[PriceQuery] = None
+        # deserialize data into str
         try:
-            instance.actual_instance = PriceQuery.from_json(json_str)
+            # validation
+            instance.anyof_schema_1_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryPrice with anyOf schemas: PriceQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Errors with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], PriceQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], object, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_provider.py` & `perian-0.2.0/perian/models/instance_type_query_input_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.provider_query import ProviderQuery
+from perian.models.provider_query_input import ProviderQueryInput
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYPROVIDER_ANY_OF_SCHEMAS = ["ProviderQuery", "object"]
+INSTANCETYPEQUERYINPUTPROVIDER_ANY_OF_SCHEMAS = ["ProviderQueryInput", "object"]
 
-class InstanceTypeQueryProvider(BaseModel):
+class InstanceTypeQueryInputProvider(BaseModel):
     """
-    InstanceTypeQueryProvider
+    InstanceTypeQueryInputProvider
     """
 
-    # data type: ProviderQuery
-    anyof_schema_1_validator: Optional[ProviderQuery] = None
+    # data type: ProviderQueryInput
+    anyof_schema_1_validator: Optional[ProviderQueryInput] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[ProviderQuery, object]] = None
+        actual_instance: Optional[Union[ProviderQueryInput, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["ProviderQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["ProviderQueryInput", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,46 +54,46 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryProvider.model_construct()
+        instance = InstanceTypeQueryInputProvider.model_construct()
         error_messages = []
-        # validate data type: ProviderQuery
-        if not isinstance(v, ProviderQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `ProviderQuery`")
+        # validate data type: ProviderQueryInput
+        if not isinstance(v, ProviderQueryInput):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `ProviderQueryInput`")
         else:
             return v
 
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryProvider with anyOf schemas: ProviderQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryInputProvider with anyOf schemas: ProviderQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[ProviderQuery] = None
+        # anyof_schema_1_validator: Optional[ProviderQueryInput] = None
         try:
-            instance.actual_instance = ProviderQuery.from_json(json_str)
+            instance.actual_instance = ProviderQueryInput.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
@@ -101,29 +101,29 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryProvider with anyOf schemas: ProviderQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryInputProvider with anyOf schemas: ProviderQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], ProviderQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], ProviderQueryInput, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_reference_id.py` & `perian-0.2.0/perian/models/instance_type_query_input_reference_id.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.reference_id_query import ReferenceIdQuery
+from perian.models.reference_id_query_input import ReferenceIdQueryInput
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYREFERENCEID_ANY_OF_SCHEMAS = ["ReferenceIdQuery", "object"]
+INSTANCETYPEQUERYINPUTREFERENCEID_ANY_OF_SCHEMAS = ["ReferenceIdQueryInput", "object"]
 
-class InstanceTypeQueryReferenceId(BaseModel):
+class InstanceTypeQueryInputReferenceId(BaseModel):
     """
-    InstanceTypeQueryReferenceId
+    InstanceTypeQueryInputReferenceId
     """
 
-    # data type: ReferenceIdQuery
-    anyof_schema_1_validator: Optional[ReferenceIdQuery] = None
+    # data type: ReferenceIdQueryInput
+    anyof_schema_1_validator: Optional[ReferenceIdQueryInput] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[ReferenceIdQuery, object]] = None
+        actual_instance: Optional[Union[ReferenceIdQueryInput, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["ReferenceIdQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["ReferenceIdQueryInput", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,46 +54,46 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryReferenceId.model_construct()
+        instance = InstanceTypeQueryInputReferenceId.model_construct()
         error_messages = []
-        # validate data type: ReferenceIdQuery
-        if not isinstance(v, ReferenceIdQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `ReferenceIdQuery`")
+        # validate data type: ReferenceIdQueryInput
+        if not isinstance(v, ReferenceIdQueryInput):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `ReferenceIdQueryInput`")
         else:
             return v
 
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryReferenceId with anyOf schemas: ReferenceIdQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryInputReferenceId with anyOf schemas: ReferenceIdQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[ReferenceIdQuery] = None
+        # anyof_schema_1_validator: Optional[ReferenceIdQueryInput] = None
         try:
-            instance.actual_instance = ReferenceIdQuery.from_json(json_str)
+            instance.actual_instance = ReferenceIdQueryInput.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
@@ -101,29 +101,29 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryReferenceId with anyOf schemas: ReferenceIdQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryInputReferenceId with anyOf schemas: ReferenceIdQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], ReferenceIdQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], ReferenceIdQueryInput, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_region.py` & `perian-0.2.0/perian/models/instance_type_query_input_region.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.region_query import RegionQuery
+from perian.models.region_query_input import RegionQueryInput
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYREGION_ANY_OF_SCHEMAS = ["RegionQuery", "object"]
+INSTANCETYPEQUERYINPUTREGION_ANY_OF_SCHEMAS = ["RegionQueryInput", "object"]
 
-class InstanceTypeQueryRegion(BaseModel):
+class InstanceTypeQueryInputRegion(BaseModel):
     """
-    InstanceTypeQueryRegion
+    InstanceTypeQueryInputRegion
     """
 
-    # data type: RegionQuery
-    anyof_schema_1_validator: Optional[RegionQuery] = None
+    # data type: RegionQueryInput
+    anyof_schema_1_validator: Optional[RegionQueryInput] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[RegionQuery, object]] = None
+        actual_instance: Optional[Union[RegionQueryInput, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["RegionQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["RegionQueryInput", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,46 +54,46 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryRegion.model_construct()
+        instance = InstanceTypeQueryInputRegion.model_construct()
         error_messages = []
-        # validate data type: RegionQuery
-        if not isinstance(v, RegionQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `RegionQuery`")
+        # validate data type: RegionQueryInput
+        if not isinstance(v, RegionQueryInput):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `RegionQueryInput`")
         else:
             return v
 
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryRegion with anyOf schemas: RegionQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryInputRegion with anyOf schemas: RegionQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[RegionQuery] = None
+        # anyof_schema_1_validator: Optional[RegionQueryInput] = None
         try:
-            instance.actual_instance = RegionQuery.from_json(json_str)
+            instance.actual_instance = RegionQueryInput.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
@@ -101,29 +101,29 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryRegion with anyOf schemas: RegionQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryInputRegion with anyOf schemas: RegionQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], RegionQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], RegionQueryInput, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_storage.py` & `perian-0.2.0/perian/models/instance_type_query_input_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.storage_query import StorageQuery
+from perian.models.storage_query_input import StorageQueryInput
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYSTORAGE_ANY_OF_SCHEMAS = ["StorageQuery", "object"]
+INSTANCETYPEQUERYINPUTSTORAGE_ANY_OF_SCHEMAS = ["StorageQueryInput", "object"]
 
-class InstanceTypeQueryStorage(BaseModel):
+class InstanceTypeQueryInputStorage(BaseModel):
     """
-    InstanceTypeQueryStorage
+    InstanceTypeQueryInputStorage
     """
 
-    # data type: StorageQuery
-    anyof_schema_1_validator: Optional[StorageQuery] = None
+    # data type: StorageQueryInput
+    anyof_schema_1_validator: Optional[StorageQueryInput] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[StorageQuery, object]] = None
+        actual_instance: Optional[Union[StorageQueryInput, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["StorageQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["StorageQueryInput", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,46 +54,46 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryStorage.model_construct()
+        instance = InstanceTypeQueryInputStorage.model_construct()
         error_messages = []
-        # validate data type: StorageQuery
-        if not isinstance(v, StorageQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `StorageQuery`")
+        # validate data type: StorageQueryInput
+        if not isinstance(v, StorageQueryInput):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `StorageQueryInput`")
         else:
             return v
 
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryStorage with anyOf schemas: StorageQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryInputStorage with anyOf schemas: StorageQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[StorageQuery] = None
+        # anyof_schema_1_validator: Optional[StorageQueryInput] = None
         try:
-            instance.actual_instance = StorageQuery.from_json(json_str)
+            instance.actual_instance = StorageQueryInput.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
@@ -101,29 +101,29 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryStorage with anyOf schemas: StorageQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryInputStorage with anyOf schemas: StorageQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], StorageQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], StorageQueryInput, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_type.py` & `perian-0.2.0/perian/models/name.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,35 +15,36 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
-from perian.models.type_query import TypeQuery
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYTYPE_ANY_OF_SCHEMAS = ["TypeQuery", "object"]
+NAME_ANY_OF_SCHEMAS = ["object", "str"]
 
-class InstanceTypeQueryType(BaseModel):
+class Name(BaseModel):
     """
-    InstanceTypeQueryType
+    Name
     """
 
-    # data type: TypeQuery
-    anyof_schema_1_validator: Optional[TypeQuery] = None
+    # data type: str
+    anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
+    # data type: object
+    anyof_schema_3_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[TypeQuery, object]] = None
+        actual_instance: Optional[Union[object, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["TypeQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["object", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,76 +55,94 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryType.model_construct()
+        instance = Name.model_construct()
         error_messages = []
-        # validate data type: TypeQuery
-        if not isinstance(v, TypeQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `TypeQuery`")
-        else:
+        # validate data type: str
+        try:
+            instance.anyof_schema_1_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
+        # validate data type: object
+        try:
+            instance.anyof_schema_3_validator = v
+            return v
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryType with anyOf schemas: TypeQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Name with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[TypeQuery] = None
+        # deserialize data into str
         try:
-            instance.actual_instance = TypeQuery.from_json(json_str)
+            # validation
+            instance.anyof_schema_1_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
+        # deserialize data into object
+        try:
+            # validation
+            instance.anyof_schema_3_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_3_validator
+            return instance
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryType with anyOf schemas: TypeQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Name with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], TypeQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], object, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_query_zone.py` & `perian-0.2.0/perian/models/provider_specific_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,36 +14,35 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
-from typing import Any, Optional
-from perian.models.zone_query import ZoneQuery
+from typing import Any, Dict, Optional
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-INSTANCETYPEQUERYZONE_ANY_OF_SCHEMAS = ["ZoneQuery", "object"]
+PROVIDERSPECIFICNAME_ANY_OF_SCHEMAS = ["object"]
 
-class InstanceTypeQueryZone(BaseModel):
+class ProviderSpecificName(BaseModel):
     """
-    InstanceTypeQueryZone
+    ProviderSpecificName
     """
 
-    # data type: ZoneQuery
-    anyof_schema_1_validator: Optional[ZoneQuery] = None
+    # data type: object
+    anyof_schema_1_validator: Optional[Dict[str, Any]] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[ZoneQuery, object]] = None
+        actual_instance: Optional[Union[object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["ZoneQuery", "object"])
+    any_of_schemas: List[str] = Field(default=Literal["object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -54,76 +53,79 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = InstanceTypeQueryZone.model_construct()
+        instance = ProviderSpecificName.model_construct()
         error_messages = []
-        # validate data type: ZoneQuery
-        if not isinstance(v, ZoneQuery):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `ZoneQuery`")
-        else:
+        # validate data type: object
+        try:
+            instance.anyof_schema_1_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in InstanceTypeQueryZone with anyOf schemas: ZoneQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in ProviderSpecificName with anyOf schemas: object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[ZoneQuery] = None
+        # deserialize data into object
         try:
-            instance.actual_instance = ZoneQuery.from_json(json_str)
+            # validation
+            instance.anyof_schema_1_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
         # deserialize data into object
         try:
             # validation
             instance.anyof_schema_2_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into InstanceTypeQueryZone with anyOf schemas: ZoneQuery, object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into ProviderSpecificName with anyOf schemas: object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], ZoneQuery, object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/instance_type_view.py` & `perian-0.2.0/perian/models/instance_type_view.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/job_status.py` & `perian-0.2.0/perian/models/order_criterion.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,28 +14,24 @@
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class JobStatus(str, Enum):
+class OrderCriterion(str, Enum):
     """
-    JobStatus
+    OrderCriterion
     """
 
     """
     allowed enum values
     """
-    QUEUED = 'Queued'
-    INITIALIZING = 'Initializing'
-    RUNNING = 'Running'
-    DONE = 'Done'
-    ERROR = 'Error'
-    UNDEFINED = 'Undefined'
+    PRICE = 'PRICE'
+    CREATED_AT = 'CREATED_AT'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of JobStatus from a JSON string"""
+        """Create an instance of OrderCriterion from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `perian-0.1.25/perian/models/job_view.py` & `perian-0.2.0/perian/models/network.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,31 +13,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.done_at import DoneAt
-from perian.models.job_status import JobStatus
-from perian.models.logs import Logs
+from perian.models.bandwidth import Bandwidth
 from typing import Optional, Set
 from typing_extensions import Self
 
-class JobView(BaseModel):
+class Network(BaseModel):
     """
-    Limited View on Model representation of a perian job.
+    Network
     """ # noqa: E501
-    id: Optional[StrictStr] = None
-    status: Optional[JobStatus] = None
-    done_at: Optional[DoneAt] = None
-    logs: Optional[Logs] = None
-    __properties: ClassVar[List[str]] = ["id", "status", "done_at", "logs"]
+    inbound: Optional[Bandwidth] = None
+    outbound: Optional[Bandwidth] = None
+    __properties: ClassVar[List[str]] = ["inbound", "outbound"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -49,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of JobView from a JSON string"""
+        """Create an instance of Network from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,33 +66,31 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of done_at
-        if self.done_at:
-            _dict['done_at'] = self.done_at.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of logs
-        if self.logs:
-            _dict['logs'] = self.logs.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of inbound
+        if self.inbound:
+            _dict['inbound'] = self.inbound.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of outbound
+        if self.outbound:
+            _dict['outbound'] = self.outbound.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of JobView from a dict"""
+        """Create an instance of Network from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "status": obj.get("status"),
-            "done_at": DoneAt.from_dict(obj["done_at"]) if obj.get("done_at") is not None else None,
-            "logs": Logs.from_dict(obj["logs"]) if obj.get("logs") is not None else None
+            "inbound": Bandwidth.from_dict(obj["inbound"]) if obj.get("inbound") is not None else None,
+            "outbound": Bandwidth.from_dict(obj["outbound"]) if obj.get("outbound") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/location.py` & `perian-0.2.0/perian/models/location.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/logs.py` & `perian-0.2.0/perian/models/logs.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/memory.py` & `perian-0.2.0/perian/models/memory.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/memory_interface.py` & `perian-0.2.0/perian/models/memory_interface.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/memory_query.py` & `perian-0.2.0/perian/models/memory_query_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictFloat, StrictInt
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
 from typing import Optional, Set
 from typing_extensions import Self
 
-class MemoryQuery(BaseModel):
+class MemoryQueryOutput(BaseModel):
     """
-    MemoryQuery
+    MemoryQueryOutput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    size: Optional[Union[StrictFloat, StrictInt]] = None
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    size: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["operator", "options", "size"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of MemoryQuery from a JSON string"""
+        """Create an instance of MemoryQueryOutput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,22 +78,22 @@
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of MemoryQuery from a dict"""
+        """Create an instance of MemoryQueryOutput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
             "size": obj.get("size")
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/memory_unit.py` & `perian-0.2.0/perian/models/memory_unit.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/name.py` & `perian-0.2.0/perian/models/name1.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-NAME_ANY_OF_SCHEMAS = ["object", "str"]
+NAME1_ANY_OF_SCHEMAS = ["object", "str"]
 
-class Name(BaseModel):
+class Name1(BaseModel):
     """
-    Name
+    Name1
     """
 
     # data type: str
     anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
@@ -53,15 +53,15 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Name.model_construct()
+        instance = Name1.model_construct()
         error_messages = []
         # validate data type: str
         try:
             instance.anyof_schema_1_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
@@ -69,15 +69,15 @@
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Name with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Name1 with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
@@ -103,15 +103,15 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Name with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Name1 with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
```

### Comparing `perian-0.1.25/perian/models/name_query.py` & `perian-0.2.0/perian/models/memory_query_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
+from perian.models.size import Size
 from typing import Optional, Set
 from typing_extensions import Self
 
-class NameQuery(BaseModel):
+class MemoryQueryInput(BaseModel):
     """
-    NameQuery
+    MemoryQueryInput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    name: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "name"]
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    size: Optional[Size] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "size"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -47,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of NameQuery from a JSON string"""
+        """Create an instance of MemoryQueryInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,26 +75,29 @@
         )
         # override the default output from pydantic by calling `to_dict()` of operator
         if self.operator:
             _dict['operator'] = self.operator.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of size
+        if self.size:
+            _dict['size'] = self.size.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of NameQuery from a dict"""
+        """Create an instance of MemoryQueryInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
-            "name": obj.get("name")
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "size": Size.from_dict(obj["size"]) if obj.get("size") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/network.py` & `perian-0.2.0/perian/models/get_accelerator_type_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.bandwidth import Bandwidth
+from perian.models.accelerator_type_query import AcceleratorTypeQuery
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Network(BaseModel):
+class GetAcceleratorTypeRequest(BaseModel):
     """
-    Network
+    GetAcceleratorTypeRequest
     """ # noqa: E501
-    inbound: Optional[Bandwidth] = None
-    outbound: Optional[Bandwidth] = None
-    __properties: ClassVar[List[str]] = ["inbound", "outbound"]
+    accelerator_type_query: Optional[AcceleratorTypeQuery] = None
+    __properties: ClassVar[List[str]] = ["accelerator_type_query"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -45,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Network from a JSON string"""
+        """Create an instance of GetAcceleratorTypeRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,31 +65,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of inbound
-        if self.inbound:
-            _dict['inbound'] = self.inbound.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of outbound
-        if self.outbound:
-            _dict['outbound'] = self.outbound.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of accelerator_type_query
+        if self.accelerator_type_query:
+            _dict['accelerator_type_query'] = self.accelerator_type_query.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Network from a dict"""
+        """Create an instance of GetAcceleratorTypeRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "inbound": Bandwidth.from_dict(obj["inbound"]) if obj.get("inbound") is not None else None,
-            "outbound": Bandwidth.from_dict(obj["outbound"]) if obj.get("outbound") is not None else None
+            "accelerator_type_query": AcceleratorTypeQuery.from_dict(obj["accelerator_type_query"]) if obj.get("accelerator_type_query") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/network_query.py` & `perian-0.2.0/perian/models/network_query_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictFloat, StrictInt
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
 from typing import Optional, Set
 from typing_extensions import Self
 
-class NetworkQuery(BaseModel):
+class NetworkQueryOutput(BaseModel):
     """
-    NetworkQuery
+    NetworkQueryOutput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    inbound_speed: Optional[Union[StrictFloat, StrictInt]] = None
-    outbound_speed: Optional[Union[StrictFloat, StrictInt]] = None
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    inbound_speed: Optional[StrictStr] = None
+    outbound_speed: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["operator", "options", "inbound_speed", "outbound_speed"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -48,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of NetworkQuery from a JSON string"""
+        """Create an instance of NetworkQueryOutput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,23 +79,23 @@
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of NetworkQuery from a dict"""
+        """Create an instance of NetworkQueryOutput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
             "inbound_speed": obj.get("inbound_speed"),
             "outbound_speed": obj.get("outbound_speed")
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/no_job_found_error.py` & `perian-0.2.0/perian/models/api_router_accelerator_type_incorrect_parameter_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class NoJobFoundError(BaseModel):
+class ApiRouterAcceleratorTypeIncorrectParameterError(BaseModel):
     """
-    NoJobFoundError
+    ApiRouterAcceleratorTypeIncorrectParameterError
     """ # noqa: E501
     status: Optional[StrictStr] = 'Error'
     message: Optional[StrictStr] = 'Operation failed due to a client error'
-    detail: Optional[StrictStr] = 'No job found with specified ID'
+    detail: Optional[StrictStr] = ''
     status_code: Optional[StrictInt] = 400
     __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of NoJobFoundError from a JSON string"""
+        """Create an instance of ApiRouterAcceleratorTypeIncorrectParameterError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,23 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of NoJobFoundError from a dict"""
+        """Create an instance of ApiRouterAcceleratorTypeIncorrectParameterError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status") if obj.get("status") is not None else 'Error',
             "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
-            "detail": obj.get("detail") if obj.get("detail") is not None else 'No job found with specified ID',
+            "detail": obj.get("detail") if obj.get("detail") is not None else '',
             "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/operator.py` & `perian-0.2.0/perian/models/operator.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/organization.py` & `perian-0.2.0/perian/models/query_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,25 +13,31 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictBool
 from typing import Any, ClassVar, Dict, List, Optional
+from perian.models.limit import Limit
+from perian.models.offset import Offset
+from perian.models.order_criterion import OrderCriterion
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Organization(BaseModel):
+class QueryOptions(BaseModel):
     """
-    Organization
+    QueryOptions
     """ # noqa: E501
-    name: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["name"]
+    limit: Optional[Limit] = None
+    offset: Optional[Offset] = None
+    order: Optional[OrderCriterion] = None
+    lazy_loading: Optional[StrictBool] = False
+    __properties: ClassVar[List[str]] = ["limit", "offset", "order", "lazy_loading"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -43,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Organization from a JSON string"""
+        """Create an instance of QueryOptions from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -64,24 +70,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of limit
+        if self.limit:
+            _dict['limit'] = self.limit.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of offset
+        if self.offset:
+            _dict['offset'] = self.offset.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Organization from a dict"""
+        """Create an instance of QueryOptions from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name")
+            "limit": Limit.from_dict(obj["limit"]) if obj.get("limit") is not None else None,
+            "offset": Offset.from_dict(obj["offset"]) if obj.get("offset") is not None else None,
+            "order": obj.get("order"),
+            "lazy_loading": obj.get("lazy_loading") if obj.get("lazy_loading") is not None else False
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/organization_name_error.py` & `perian-0.2.0/perian/models/api_router_instance_type_instance_type_not_found_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 import json
 
 from pydantic import BaseModel, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OrganizationNameError(BaseModel):
+class ApiRouterInstanceTypeInstanceTypeNotFoundError(BaseModel):
     """
-    OrganizationNameError
+    ApiRouterInstanceTypeInstanceTypeNotFoundError
     """ # noqa: E501
     status: Optional[StrictStr] = 'Error'
     message: Optional[StrictStr] = 'Operation failed due to a client error'
-    detail: Optional[StrictStr] = 'The provided organization name is not valid'
+    detail: Optional[StrictStr] = 'No instance type found with specified ID'
     status_code: Optional[StrictInt] = 400
     __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OrganizationNameError from a JSON string"""
+        """Create an instance of ApiRouterInstanceTypeInstanceTypeNotFoundError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,23 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OrganizationNameError from a dict"""
+        """Create an instance of ApiRouterInstanceTypeInstanceTypeNotFoundError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "status": obj.get("status") if obj.get("status") is not None else 'Error',
             "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
-            "detail": obj.get("detail") if obj.get("detail") is not None else 'The provided organization name is not valid',
+            "detail": obj.get("detail") if obj.get("detail") is not None else 'No instance type found with specified ID',
             "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/organization_name_exists_error.py` & `perian-0.2.0/perian/models/region.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,28 +13,34 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from perian.models.location import Location
+from perian.models.status import Status
+from perian.models.zone import Zone
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OrganizationNameExistsError(BaseModel):
+class Region(BaseModel):
     """
-    OrganizationNameExistsError
+    Region
     """ # noqa: E501
-    status: Optional[StrictStr] = 'Error'
-    message: Optional[StrictStr] = 'Operation failed due to a client error'
-    detail: Optional[StrictStr] = 'The provided organization name already exists. Please choose another one'
-    status_code: Optional[StrictInt] = 400
-    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
+    id: Optional[StrictStr] = None
+    name: Optional[StrictStr] = None
+    city: Optional[StrictStr] = None
+    location: Optional[Location] = None
+    sustainable: Optional[StrictBool] = False
+    status: Optional[Status] = None
+    zones: Optional[List[Zone]] = None
+    __properties: ClassVar[List[str]] = ["id", "name", "city", "location", "sustainable", "status", "zones"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -46,15 +52,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OrganizationNameExistsError from a JSON string"""
+        """Create an instance of Region from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,27 +73,37 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in zones (list)
+        _items = []
+        if self.zones:
+            for _item in self.zones:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['zones'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OrganizationNameExistsError from a dict"""
+        """Create an instance of Region from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "status": obj.get("status") if obj.get("status") is not None else 'Error',
-            "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
-            "detail": obj.get("detail") if obj.get("detail") is not None else 'The provided organization name already exists. Please choose another one',
-            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
+            "id": obj.get("id"),
+            "name": obj.get("name"),
+            "city": obj.get("city"),
+            "location": obj.get("location"),
+            "sustainable": obj.get("sustainable") if obj.get("sustainable") is not None else False,
+            "status": obj.get("status"),
+            "zones": [Zone.from_dict(_item) for _item in obj["zones"]] if obj.get("zones") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/os_storage_config.py` & `perian-0.2.0/perian/models/os_storage_config.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/price.py` & `perian-0.2.0/perian/models/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.currency import Currency
+from perian.models.bandwidth import Bandwidth
+from perian.models.memory import Memory
+from perian.models.storage_type import StorageType
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Price(BaseModel):
+class Storage(BaseModel):
     """
-    Price
+    Storage
     """ # noqa: E501
-    per_hour: Optional[StrictStr] = '0.0'
-    unit: Optional[Currency] = None
-    __properties: ClassVar[List[str]] = ["per_hour", "unit"]
+    type: Optional[StorageType] = None
+    size: Optional[Memory] = None
+    speed: Optional[Bandwidth] = None
+    __properties: ClassVar[List[str]] = ["type", "size", "speed"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -45,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Price from a JSON string"""
+        """Create an instance of Storage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,25 +69,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of size
+        if self.size:
+            _dict['size'] = self.size.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of speed
+        if self.speed:
+            _dict['speed'] = self.speed.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Price from a dict"""
+        """Create an instance of Storage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "per_hour": obj.get("per_hour") if obj.get("per_hour") is not None else '0.0',
-            "unit": obj.get("unit")
+            "type": obj.get("type"),
+            "size": Memory.from_dict(obj["size"]) if obj.get("size") is not None else None,
+            "speed": Bandwidth.from_dict(obj["speed"]) if obj.get("speed") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/price_data.py` & `perian-0.2.0/perian/models/price_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,25 +15,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.price import Price
+from perian.models.billing_granularity import BillingGranularity
+from perian.models.currency import Currency
 from typing import Optional, Set
 from typing_extensions import Self
 
 class PriceData(BaseModel):
     """
     PriceData
     """ # noqa: E501
-    euro_price: Optional[StrictStr] = '0.0'
-    prices: Optional[List[Price]] = None
-    __properties: ClassVar[List[str]] = ["euro_price", "prices"]
+    unit_price: Optional[StrictStr] = '0.0'
+    currency: Optional[Currency] = None
+    granularity: Optional[BillingGranularity] = None
+    provider_billing_granularity: Optional[BillingGranularity] = None
+    __properties: ClassVar[List[str]] = ["unit_price", "currency", "granularity", "provider_billing_granularity"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -66,32 +69,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in prices (list)
-        _items = []
-        if self.prices:
-            for _item in self.prices:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['prices'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
         """Create an instance of PriceData from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "euro_price": obj.get("euro_price") if obj.get("euro_price") is not None else '0.0',
-            "prices": [Price.from_dict(_item) for _item in obj["prices"]] if obj.get("prices") is not None else None
+            "unit_price": obj.get("unit_price") if obj.get("unit_price") is not None else '0.0',
+            "currency": obj.get("currency"),
+            "granularity": obj.get("granularity"),
+            "provider_billing_granularity": obj.get("provider_billing_granularity")
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/price_query.py` & `perian-0.2.0/perian/models/price_query_output.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,31 +13,29 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PriceQuery(BaseModel):
+class PriceQueryOutput(BaseModel):
     """
-    PriceQuery
+    PriceQueryOutput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    euro_price: Optional[Union[StrictFloat, StrictInt]] = None
-    unit: Optional[StrictStr] = None
-    per_hour: Optional[Union[StrictFloat, StrictInt]] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "euro_price", "unit", "per_hour"]
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    unit_price: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "unit_price"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -49,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PriceQuery from a JSON string"""
+        """Create an instance of PriceQueryOutput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,24 +78,22 @@
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PriceQuery from a dict"""
+        """Create an instance of PriceQueryOutput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
-            "euro_price": obj.get("euro_price"),
-            "unit": obj.get("unit"),
-            "per_hour": obj.get("per_hour")
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "unit_price": obj.get("unit_price")
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/provider.py` & `perian-0.2.0/perian/models/provider.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/provider_capabilities.py` & `perian-0.2.0/perian/models/provider_capabilities.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/provider_name.py` & `perian-0.2.0/perian/models/provider_name.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/provider_properties.py` & `perian-0.2.0/perian/models/runtime_metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel
+from pydantic import BaseModel, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.compute_billing_period import ComputeBillingPeriod
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ProviderProperties(BaseModel):
+class RuntimeMetadata(BaseModel):
     """
-    ProviderProperties
+    RuntimeMetadata
     """ # noqa: E501
-    compute_billing_period: Optional[ComputeBillingPeriod] = None
-    __properties: ClassVar[List[str]] = ["compute_billing_period"]
+    instance_type_id: Optional[StrictStr] = None
+    auto_failover_instance_type: Optional[StrictBool] = False
+    __properties: ClassVar[List[str]] = ["instance_type_id", "auto_failover_instance_type"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -44,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ProviderProperties from a JSON string"""
+        """Create an instance of RuntimeMetadata from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +69,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ProviderProperties from a dict"""
+        """Create an instance of RuntimeMetadata from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "compute_billing_period": obj.get("compute_billing_period")
+            "instance_type_id": obj.get("instance_type_id"),
+            "auto_failover_instance_type": obj.get("auto_failover_instance_type") if obj.get("auto_failover_instance_type") is not None else False
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/provider_query.py` & `perian-0.2.0/perian/models/zone_query_output.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,34 +13,34 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
 from perian.models.id import Id
+from perian.models.name1 import Name1
+from perian.models.status1 import Status1
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ProviderQuery(BaseModel):
+class ZoneQueryOutput(BaseModel):
     """
-    ProviderQuery
+    ZoneQueryOutput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
     id: Optional[Id] = None
-    name: Optional[StrictStr] = None
-    name_short: Optional[StrictStr] = None
-    location: Optional[StrictStr] = None
-    status: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "id", "name", "name_short", "location", "status"]
+    name: Optional[Name1] = None
+    status: Optional[Status1] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "id", "name", "status"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -52,15 +52,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ProviderQuery from a JSON string"""
+        """Create an instance of ZoneQueryOutput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,30 +82,34 @@
             _dict['operator'] = self.operator.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
         # override the default output from pydantic by calling `to_dict()` of id
         if self.id:
             _dict['id'] = self.id.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of name
+        if self.name:
+            _dict['name'] = self.name.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of status
+        if self.status:
+            _dict['status'] = self.status.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ProviderQuery from a dict"""
+        """Create an instance of ZoneQueryOutput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
             "id": Id.from_dict(obj["id"]) if obj.get("id") is not None else None,
-            "name": obj.get("name"),
-            "name_short": obj.get("name_short"),
-            "location": obj.get("location"),
-            "status": obj.get("status")
+            "name": Name1.from_dict(obj["name"]) if obj.get("name") is not None else None,
+            "status": Status1.from_dict(obj["status"]) if obj.get("status") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/provider_specific_name.py` & `perian-0.2.0/perian/models/cores.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,36 +13,36 @@
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
-from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
-from typing import Any, Dict, Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr, ValidationError, field_validator
+from typing import Any, Optional
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-PROVIDERSPECIFICNAME_ANY_OF_SCHEMAS = ["object"]
+CORES_ANY_OF_SCHEMAS = ["int", "object"]
 
-class ProviderSpecificName(BaseModel):
+class Cores(BaseModel):
     """
-    ProviderSpecificName
+    Cores
     """
 
-    # data type: object
-    anyof_schema_1_validator: Optional[Dict[str, Any]] = None
+    # data type: int
+    anyof_schema_1_validator: Optional[StrictInt] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[object]] = None
+        actual_instance: Optional[Union[int, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["object"])
+    any_of_schemas: List[str] = Field(default=Literal["int", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -53,44 +53,44 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = ProviderSpecificName.model_construct()
+        instance = Cores.model_construct()
         error_messages = []
-        # validate data type: object
+        # validate data type: int
         try:
             instance.anyof_schema_1_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         # validate data type: object
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in ProviderSpecificName with anyOf schemas: object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Cores with anyOf schemas: int, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # deserialize data into object
+        # deserialize data into int
         try:
             # validation
             instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
@@ -103,29 +103,29 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into ProviderSpecificName with anyOf schemas: object. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Cores with anyOf schemas: int, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], object]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], int, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/query_options.py` & `perian-0.2.0/perian/models/validation_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,27 +13,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictBool, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List
+from perian.models.validation_error_loc_inner import ValidationErrorLocInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class QueryOptions(BaseModel):
+class ValidationError(BaseModel):
     """
-    QueryOptions
+    ValidationError
     """ # noqa: E501
-    limit: Optional[StrictInt] = 25
-    order: Optional[StrictStr] = None
-    lazy_loading: Optional[StrictBool] = False
-    __properties: ClassVar[List[str]] = ["limit", "order", "lazy_loading"]
+    loc: List[ValidationErrorLocInner]
+    msg: StrictStr
+    type: StrictStr
+    __properties: ClassVar[List[str]] = ["loc", "msg", "type"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -45,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of QueryOptions from a JSON string"""
+        """Create an instance of ValidationError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,26 +67,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in loc (list)
+        _items = []
+        if self.loc:
+            for _item in self.loc:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['loc'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of QueryOptions from a dict"""
+        """Create an instance of ValidationError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "limit": obj.get("limit") if obj.get("limit") is not None else 25,
-            "order": obj.get("order"),
-            "lazy_loading": obj.get("lazy_loading") if obj.get("lazy_loading") is not None else False
+            "loc": [ValidationErrorLocInner.from_dict(_item) for _item in obj["loc"]] if obj.get("loc") is not None else None,
+            "msg": obj.get("msg"),
+            "type": obj.get("type")
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/reference.py` & `perian-0.2.0/perian/models/id1.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
 from typing import Any, Optional
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-REFERENCE_ANY_OF_SCHEMAS = ["object", "str"]
+ID1_ANY_OF_SCHEMAS = ["object", "str"]
 
-class Reference(BaseModel):
+class Id1(BaseModel):
     """
-    Reference
+    Id1
     """
 
     # data type: str
     anyof_schema_1_validator: Optional[StrictStr] = None
     # data type: object
     anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
@@ -53,15 +53,15 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Reference.model_construct()
+        instance = Id1.model_construct()
         error_messages = []
         # validate data type: str
         try:
             instance.anyof_schema_1_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
@@ -69,15 +69,15 @@
         try:
             instance.anyof_schema_2_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Reference with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Id1 with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
@@ -103,15 +103,15 @@
             instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Reference with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Id1 with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
```

### Comparing `perian-0.1.25/perian/models/reference_id_query.py` & `perian-0.2.0/perian/models/reference_id_query_input.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,28 +13,29 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
+from perian.models.id1 import Id1
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ReferenceIdQuery(BaseModel):
+class ReferenceIdQueryInput(BaseModel):
     """
-    ReferenceIdQuery
+    ReferenceIdQueryInput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    id: Optional[StrictStr] = None
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    id: Optional[Id1] = None
     __properties: ClassVar[List[str]] = ["operator", "options", "id"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
@@ -47,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ReferenceIdQuery from a JSON string"""
+        """Create an instance of ReferenceIdQueryInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,26 +75,29 @@
         )
         # override the default output from pydantic by calling `to_dict()` of operator
         if self.operator:
             _dict['operator'] = self.operator.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of id
+        if self.id:
+            _dict['id'] = self.id.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ReferenceIdQuery from a dict"""
+        """Create an instance of ReferenceIdQueryInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
-            "id": obj.get("id")
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "id": Id1.from_dict(obj["id"]) if obj.get("id") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/region.py` & `perian-0.2.0/perian/models/bill.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,34 +13,34 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictBool, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.location import Location
-from perian.models.status import Status
-from perian.models.zone import Zone
+from datetime import datetime
+from pydantic import BaseModel, StrictStr
+from typing import Any, ClassVar, Dict, List
+from perian.models.bill_item import BillItem
+from perian.models.currency import Currency
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Region(BaseModel):
+class Bill(BaseModel):
     """
-    Region
+    A total bill for a single organization.
     """ # noqa: E501
-    id: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    city: Optional[StrictStr] = None
-    location: Optional[Location] = None
-    sustainable: Optional[StrictBool] = False
-    status: Optional[Status] = None
-    zones: Optional[List[Zone]] = None
-    __properties: ClassVar[List[str]] = ["id", "name", "city", "location", "sustainable", "status", "zones"]
+    organization_id: StrictStr
+    start_time: datetime
+    end_time: datetime
+    total_price: StrictStr
+    currency: Currency
+    margin_multiplier: StrictStr
+    items: List[BillItem]
+    __properties: ClassVar[List[str]] = ["organization_id", "start_time", "end_time", "total_price", "currency", "margin_multiplier", "items"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -52,15 +52,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Region from a JSON string"""
+        """Create an instance of Bill from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,37 +73,37 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in zones (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in items (list)
         _items = []
-        if self.zones:
-            for _item in self.zones:
+        if self.items:
+            for _item in self.items:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['zones'] = _items
+            _dict['items'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Region from a dict"""
+        """Create an instance of Bill from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "name": obj.get("name"),
-            "city": obj.get("city"),
-            "location": obj.get("location"),
-            "sustainable": obj.get("sustainable") if obj.get("sustainable") is not None else False,
-            "status": obj.get("status"),
-            "zones": [Zone.from_dict(_item) for _item in obj["zones"]] if obj.get("zones") is not None else None
+            "organization_id": obj.get("organization_id"),
+            "start_time": obj.get("start_time"),
+            "end_time": obj.get("end_time"),
+            "total_price": obj.get("total_price"),
+            "currency": obj.get("currency"),
+            "margin_multiplier": obj.get("margin_multiplier"),
+            "items": [BillItem.from_dict(_item) for _item in obj["items"]] if obj.get("items") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/region_query.py` & `perian-0.2.0/perian/models/zone_query_input.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,34 +13,34 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictBool, StrictStr
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
 from perian.models.id import Id
+from perian.models.name1 import Name1
+from perian.models.status1 import Status1
 from typing import Optional, Set
 from typing_extensions import Self
 
-class RegionQuery(BaseModel):
+class ZoneQueryInput(BaseModel):
     """
-    RegionQuery
+    ZoneQueryInput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
     id: Optional[Id] = None
-    name: Optional[StrictStr] = None
-    location: Optional[StrictStr] = None
-    sustainable: Optional[StrictBool] = None
-    status: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "id", "name", "location", "sustainable", "status"]
+    name: Optional[Name1] = None
+    status: Optional[Status1] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "id", "name", "status"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -52,15 +52,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RegionQuery from a JSON string"""
+        """Create an instance of ZoneQueryInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,30 +82,34 @@
             _dict['operator'] = self.operator.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
         # override the default output from pydantic by calling `to_dict()` of id
         if self.id:
             _dict['id'] = self.id.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of name
+        if self.name:
+            _dict['name'] = self.name.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of status
+        if self.status:
+            _dict['status'] = self.status.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RegionQuery from a dict"""
+        """Create an instance of ZoneQueryInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
             "id": Id.from_dict(obj["id"]) if obj.get("id") is not None else None,
-            "name": obj.get("name"),
-            "location": obj.get("location"),
-            "sustainable": obj.get("sustainable"),
-            "status": obj.get("status")
+            "name": Name1.from_dict(obj["name"]) if obj.get("name") is not None else None,
+            "status": Status1.from_dict(obj["status"]) if obj.get("status") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/response400_create_global_admin_admin_post.py` & `perian-0.2.0/perian/models/create_job_request_requirements.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,37 +14,36 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
-from typing import Optional
-from perian.models.default_client_error import DefaultClientError
-from perian.models.setup_token_error import SetupTokenError
+from typing import Any, Optional
+from perian.models.instance_type_query_input import InstanceTypeQueryInput
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-RESPONSE400CREATEGLOBALADMINADMINPOST_ANY_OF_SCHEMAS = ["DefaultClientError", "SetupTokenError"]
+CREATEJOBREQUESTREQUIREMENTS_ANY_OF_SCHEMAS = ["InstanceTypeQueryInput", "object"]
 
-class Response400CreateGlobalAdminAdminPost(BaseModel):
+class CreateJobRequestRequirements(BaseModel):
     """
-    Response400CreateGlobalAdminAdminPost
+    CreateJobRequestRequirements
     """
 
-    # data type: DefaultClientError
-    anyof_schema_1_validator: Optional[DefaultClientError] = None
-    # data type: SetupTokenError
-    anyof_schema_2_validator: Optional[SetupTokenError] = None
+    # data type: InstanceTypeQueryInput
+    anyof_schema_1_validator: Optional[InstanceTypeQueryInput] = None
+    # data type: object
+    anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[DefaultClientError, SetupTokenError]] = None
+        actual_instance: Optional[Union[InstanceTypeQueryInput, object]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["DefaultClientError", "SetupTokenError"])
+    any_of_schemas: List[str] = Field(default=Literal["InstanceTypeQueryInput", "object"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -55,73 +54,76 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Response400CreateGlobalAdminAdminPost.model_construct()
+        instance = CreateJobRequestRequirements.model_construct()
         error_messages = []
-        # validate data type: DefaultClientError
-        if not isinstance(v, DefaultClientError):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `DefaultClientError`")
+        # validate data type: InstanceTypeQueryInput
+        if not isinstance(v, InstanceTypeQueryInput):
+            error_messages.append(f"Error! Input type `{type(v)}` is not `InstanceTypeQueryInput`")
         else:
             return v
 
-        # validate data type: SetupTokenError
-        if not isinstance(v, SetupTokenError):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `SetupTokenError`")
-        else:
+        # validate data type: object
+        try:
+            instance.anyof_schema_2_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Response400CreateGlobalAdminAdminPost with anyOf schemas: DefaultClientError, SetupTokenError. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in CreateJobRequestRequirements with anyOf schemas: InstanceTypeQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[DefaultClientError] = None
+        # anyof_schema_1_validator: Optional[InstanceTypeQueryInput] = None
         try:
-            instance.actual_instance = DefaultClientError.from_json(json_str)
+            instance.actual_instance = InstanceTypeQueryInput.from_json(json_str)
             return instance
         except (ValidationError, ValueError) as e:
              error_messages.append(str(e))
-        # anyof_schema_2_validator: Optional[SetupTokenError] = None
+        # deserialize data into object
         try:
-            instance.actual_instance = SetupTokenError.from_json(json_str)
+            # validation
+            instance.anyof_schema_2_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Response400CreateGlobalAdminAdminPost with anyOf schemas: DefaultClientError, SetupTokenError. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into CreateJobRequestRequirements with anyOf schemas: InstanceTypeQueryInput, object. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], DefaultClientError, SetupTokenError]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], InstanceTypeQueryInput, object]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/response400_create_organization_organization_post.py` & `perian-0.2.0/perian/models/outbound_speed.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,41 +13,38 @@
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
-from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
-from typing import Optional
-from perian.models.default_client_error import DefaultClientError
-from perian.models.organization_name_error import OrganizationNameError
-from perian.models.organization_name_exists_error import OrganizationNameExistsError
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, ValidationError, field_validator
+from typing import Any, Optional, Union
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-RESPONSE400CREATEORGANIZATIONORGANIZATIONPOST_ANY_OF_SCHEMAS = ["DefaultClientError", "OrganizationNameError", "OrganizationNameExistsError"]
+OUTBOUNDSPEED_ANY_OF_SCHEMAS = ["float", "object", "str"]
 
-class Response400CreateOrganizationOrganizationPost(BaseModel):
+class OutboundSpeed(BaseModel):
     """
-    Response400CreateOrganizationOrganizationPost
+    OutboundSpeed
     """
 
-    # data type: DefaultClientError
-    anyof_schema_1_validator: Optional[DefaultClientError] = None
-    # data type: OrganizationNameError
-    anyof_schema_2_validator: Optional[OrganizationNameError] = None
-    # data type: OrganizationNameExistsError
-    anyof_schema_3_validator: Optional[OrganizationNameExistsError] = None
+    # data type: str
+    anyof_schema_1_validator: Optional[StrictStr] = None
+    # data type: float
+    anyof_schema_2_validator: Optional[Union[StrictFloat, StrictInt]] = None
+    # data type: object
+    anyof_schema_3_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[DefaultClientError, OrganizationNameError, OrganizationNameExistsError]] = None
+        actual_instance: Optional[Union[float, object, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["DefaultClientError", "OrganizationNameError", "OrganizationNameExistsError"])
+    any_of_schemas: List[str] = Field(default=Literal["float", "object", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -58,85 +55,94 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Response400CreateOrganizationOrganizationPost.model_construct()
+        instance = OutboundSpeed.model_construct()
         error_messages = []
-        # validate data type: DefaultClientError
-        if not isinstance(v, DefaultClientError):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `DefaultClientError`")
-        else:
+        # validate data type: str
+        try:
+            instance.anyof_schema_1_validator = v
             return v
-
-        # validate data type: OrganizationNameError
-        if not isinstance(v, OrganizationNameError):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `OrganizationNameError`")
-        else:
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
+        # validate data type: float
+        try:
+            instance.anyof_schema_2_validator = v
             return v
-
-        # validate data type: OrganizationNameExistsError
-        if not isinstance(v, OrganizationNameExistsError):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `OrganizationNameExistsError`")
-        else:
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
+        # validate data type: object
+        try:
+            instance.anyof_schema_3_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Response400CreateOrganizationOrganizationPost with anyOf schemas: DefaultClientError, OrganizationNameError, OrganizationNameExistsError. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in OutboundSpeed with anyOf schemas: float, object, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[DefaultClientError] = None
+        # deserialize data into str
         try:
-            instance.actual_instance = DefaultClientError.from_json(json_str)
+            # validation
+            instance.anyof_schema_1_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_2_validator: Optional[OrganizationNameError] = None
+            error_messages.append(str(e))
+        # deserialize data into float
         try:
-            instance.actual_instance = OrganizationNameError.from_json(json_str)
+            # validation
+            instance.anyof_schema_2_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_3_validator: Optional[OrganizationNameExistsError] = None
+            error_messages.append(str(e))
+        # deserialize data into object
         try:
-            instance.actual_instance = OrganizationNameExistsError.from_json(json_str)
+            # validation
+            instance.anyof_schema_3_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_3_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Response400CreateOrganizationOrganizationPost with anyOf schemas: DefaultClientError, OrganizationNameError, OrganizationNameExistsError. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into OutboundSpeed with anyOf schemas: float, object, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], DefaultClientError, OrganizationNameError, OrganizationNameExistsError]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], float, object, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/response400_create_service_account_service_account_post.py` & `perian-0.2.0/perian/models/currency1.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,37 +14,35 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
-from typing import Optional
-from perian.models.default_client_error import DefaultClientError
-from perian.models.role_not_valid_error import RoleNotValidError
+from typing import Any, Optional
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-RESPONSE400CREATESERVICEACCOUNTSERVICEACCOUNTPOST_ANY_OF_SCHEMAS = ["DefaultClientError", "RoleNotValidError"]
+CURRENCY1_ANY_OF_SCHEMAS = ["object", "str"]
 
-class Response400CreateServiceAccountServiceAccountPost(BaseModel):
+class Currency1(BaseModel):
     """
-    Response400CreateServiceAccountServiceAccountPost
+    Currency
     """
 
-    # data type: DefaultClientError
-    anyof_schema_1_validator: Optional[DefaultClientError] = None
-    # data type: RoleNotValidError
-    anyof_schema_2_validator: Optional[RoleNotValidError] = None
+    # data type: str
+    anyof_schema_1_validator: Optional[StrictStr] = None
+    # data type: object
+    anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[DefaultClientError, RoleNotValidError]] = None
+        actual_instance: Optional[Union[object, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["DefaultClientError", "RoleNotValidError"])
+    any_of_schemas: List[str] = Field(default=Literal["object", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -55,73 +53,79 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Response400CreateServiceAccountServiceAccountPost.model_construct()
+        instance = Currency1.model_construct()
         error_messages = []
-        # validate data type: DefaultClientError
-        if not isinstance(v, DefaultClientError):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `DefaultClientError`")
-        else:
+        # validate data type: str
+        try:
+            instance.anyof_schema_1_validator = v
             return v
-
-        # validate data type: RoleNotValidError
-        if not isinstance(v, RoleNotValidError):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `RoleNotValidError`")
-        else:
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
+        # validate data type: object
+        try:
+            instance.anyof_schema_2_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Response400CreateServiceAccountServiceAccountPost with anyOf schemas: DefaultClientError, RoleNotValidError. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Currency1 with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[DefaultClientError] = None
+        # deserialize data into str
         try:
-            instance.actual_instance = DefaultClientError.from_json(json_str)
+            # validation
+            instance.anyof_schema_1_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_2_validator: Optional[RoleNotValidError] = None
+            error_messages.append(str(e))
+        # deserialize data into object
         try:
-            instance.actual_instance = RoleNotValidError.from_json(json_str)
+            # validation
+            instance.anyof_schema_2_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Response400CreateServiceAccountServiceAccountPost with anyOf schemas: DefaultClientError, RoleNotValidError. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Currency1 with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], DefaultClientError, RoleNotValidError]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], object, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/response400_create_user_user_post.py` & `perian-0.2.0/perian/models/status1.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,37 +14,35 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
-from typing import Optional
-from perian.models.default_client_error import DefaultClientError
-from perian.models.role_not_valid_error import RoleNotValidError
+from typing import Any, Optional
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-RESPONSE400CREATEUSERUSERPOST_ANY_OF_SCHEMAS = ["DefaultClientError", "RoleNotValidError"]
+STATUS1_ANY_OF_SCHEMAS = ["object", "str"]
 
-class Response400CreateUserUserPost(BaseModel):
+class Status1(BaseModel):
     """
-    Response400CreateUserUserPost
+    Status1
     """
 
-    # data type: DefaultClientError
-    anyof_schema_1_validator: Optional[DefaultClientError] = None
-    # data type: RoleNotValidError
-    anyof_schema_2_validator: Optional[RoleNotValidError] = None
+    # data type: str
+    anyof_schema_1_validator: Optional[StrictStr] = None
+    # data type: object
+    anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[DefaultClientError, RoleNotValidError]] = None
+        actual_instance: Optional[Union[object, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["DefaultClientError", "RoleNotValidError"])
+    any_of_schemas: List[str] = Field(default=Literal["object", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -55,73 +53,79 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = Response400CreateUserUserPost.model_construct()
+        instance = Status1.model_construct()
         error_messages = []
-        # validate data type: DefaultClientError
-        if not isinstance(v, DefaultClientError):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `DefaultClientError`")
-        else:
+        # validate data type: str
+        try:
+            instance.anyof_schema_1_validator = v
             return v
-
-        # validate data type: RoleNotValidError
-        if not isinstance(v, RoleNotValidError):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `RoleNotValidError`")
-        else:
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
+        # validate data type: object
+        try:
+            instance.anyof_schema_2_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in Response400CreateUserUserPost with anyOf schemas: DefaultClientError, RoleNotValidError. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Status1 with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[DefaultClientError] = None
+        # deserialize data into str
         try:
-            instance.actual_instance = DefaultClientError.from_json(json_str)
+            # validation
+            instance.anyof_schema_1_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_2_validator: Optional[RoleNotValidError] = None
+            error_messages.append(str(e))
+        # deserialize data into object
         try:
-            instance.actual_instance = RoleNotValidError.from_json(json_str)
+            # validation
+            instance.anyof_schema_2_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into Response400CreateUserUserPost with anyOf schemas: DefaultClientError, RoleNotValidError. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Status1 with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], DefaultClientError, RoleNotValidError]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], object, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/response_get_job_job_get.py` & `perian-0.2.0/perian/models/location1.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,37 +14,35 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
-from typing import Optional
-from perian.models.get_jobs_success import GetJobsSuccess
-from perian.models.no_job_found_error import NoJobFoundError
+from typing import Any, Optional
 from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-RESPONSEGETJOBJOBGET_ANY_OF_SCHEMAS = ["GetJobsSuccess", "NoJobFoundError"]
+LOCATION1_ANY_OF_SCHEMAS = ["object", "str"]
 
-class ResponseGetJobJobGet(BaseModel):
+class Location1(BaseModel):
     """
-    ResponseGetJobJobGet
+    Location1
     """
 
-    # data type: GetJobsSuccess
-    anyof_schema_1_validator: Optional[GetJobsSuccess] = None
-    # data type: NoJobFoundError
-    anyof_schema_2_validator: Optional[NoJobFoundError] = None
+    # data type: str
+    anyof_schema_1_validator: Optional[StrictStr] = None
+    # data type: object
+    anyof_schema_2_validator: Optional[Any] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[GetJobsSuccess, NoJobFoundError]] = None
+        actual_instance: Optional[Union[object, str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["GetJobsSuccess", "NoJobFoundError"])
+    any_of_schemas: List[str] = Field(default=Literal["object", "str"])
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -55,73 +53,79 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = ResponseGetJobJobGet.model_construct()
+        instance = Location1.model_construct()
         error_messages = []
-        # validate data type: GetJobsSuccess
-        if not isinstance(v, GetJobsSuccess):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `GetJobsSuccess`")
-        else:
+        # validate data type: str
+        try:
+            instance.anyof_schema_1_validator = v
             return v
-
-        # validate data type: NoJobFoundError
-        if not isinstance(v, NoJobFoundError):
-            error_messages.append(f"Error! Input type `{type(v)}` is not `NoJobFoundError`")
-        else:
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
+        # validate data type: object
+        try:
+            instance.anyof_schema_2_validator = v
             return v
-
+        except (ValidationError, ValueError) as e:
+            error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in ResponseGetJobJobGet with anyOf schemas: GetJobsSuccess, NoJobFoundError. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in Location1 with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # anyof_schema_1_validator: Optional[GetJobsSuccess] = None
+        # deserialize data into str
         try:
-            instance.actual_instance = GetJobsSuccess.from_json(json_str)
+            # validation
+            instance.anyof_schema_1_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
-        # anyof_schema_2_validator: Optional[NoJobFoundError] = None
+            error_messages.append(str(e))
+        # deserialize data into object
         try:
-            instance.actual_instance = NoJobFoundError.from_json(json_str)
+            # validation
+            instance.anyof_schema_2_validator = json.loads(json_str)
+            # assign value to actual_instance
+            instance.actual_instance = instance.anyof_schema_2_validator
             return instance
         except (ValidationError, ValueError) as e:
-             error_messages.append(str(e))
+            error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into ResponseGetJobJobGet with anyOf schemas: GetJobsSuccess, NoJobFoundError. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into Location1 with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], GetJobsSuccess, NoJobFoundError]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], object, str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `perian-0.1.25/perian/models/setup_token_error.py` & `perian-0.2.0/perian/models/storage_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,28 +13,31 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
+from perian.models.memory import Memory
+from perian.models.storage import Storage
+from perian.models.storage_included import StorageIncluded
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SetupTokenError(BaseModel):
+class StorageData(BaseModel):
     """
-    SetupTokenError
+    StorageData
     """ # noqa: E501
-    status: Optional[StrictStr] = 'Error'
-    message: Optional[StrictStr] = 'Operation failed due to a client error'
-    detail: Optional[StrictStr] = 'The provided setup token is invalid'
-    status_code: Optional[StrictInt] = 400
-    __properties: ClassVar[List[str]] = ["status", "message", "detail", "status_code"]
+    no: Optional[StrictInt] = 0
+    size: Optional[Memory] = None
+    included: Optional[StorageIncluded] = None
+    storages: Optional[List[Storage]] = None
+    __properties: ClassVar[List[str]] = ["no", "size", "included", "storages"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -46,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SetupTokenError from a JSON string"""
+        """Create an instance of StorageData from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,27 +70,37 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of size
+        if self.size:
+            _dict['size'] = self.size.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in storages (list)
+        _items = []
+        if self.storages:
+            for _item in self.storages:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['storages'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SetupTokenError from a dict"""
+        """Create an instance of StorageData from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "status": obj.get("status") if obj.get("status") is not None else 'Error',
-            "message": obj.get("message") if obj.get("message") is not None else 'Operation failed due to a client error',
-            "detail": obj.get("detail") if obj.get("detail") is not None else 'The provided setup token is invalid',
-            "status_code": obj.get("status_code") if obj.get("status_code") is not None else 400
+            "no": obj.get("no") if obj.get("no") is not None else 0,
+            "size": Memory.from_dict(obj["size"]) if obj.get("size") is not None else None,
+            "included": obj.get("included"),
+            "storages": [Storage.from_dict(_item) for _item in obj["storages"]] if obj.get("storages") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/status.py` & `perian-0.2.0/perian/models/storage_included.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,25 +14,25 @@
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class Status(str, Enum):
+class StorageIncluded(str, Enum):
     """
-    Status
+    StorageIncluded
     """
 
     """
     allowed enum values
     """
-    ACTIVE = 'Active'
-    INACTIVE = 'Inactive'
-    UNDEFINED = 'Undefined'
+    UNDEFINED = 'UNDEFINED'
+    INCLUDED = 'INCLUDED'
+    NOT_INCLUDED = 'NOT_INCLUDED'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of Status from a JSON string"""
+        """Create an instance of StorageIncluded from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `perian-0.1.25/perian/models/storage.py` & `perian-0.2.0/perian/models/availability_query_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.bandwidth import Bandwidth
-from perian.models.memory import Memory
-from perian.models.storage_type import StorageType
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
+from perian.models.available import Available
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Storage(BaseModel):
+class AvailabilityQueryOutput(BaseModel):
     """
-    Storage
+    AvailabilityQueryOutput
     """ # noqa: E501
-    type: Optional[StorageType] = None
-    size: Optional[Memory] = None
-    speed: Optional[Bandwidth] = None
-    __properties: ClassVar[List[str]] = ["type", "size", "speed"]
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    available: Optional[Available] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "available"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -48,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Storage from a JSON string"""
+        """Create an instance of AvailabilityQueryOutput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,32 +69,35 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of size
-        if self.size:
-            _dict['size'] = self.size.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of speed
-        if self.speed:
-            _dict['speed'] = self.speed.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of operator
+        if self.operator:
+            _dict['operator'] = self.operator.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of options
+        if self.options:
+            _dict['options'] = self.options.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of available
+        if self.available:
+            _dict['available'] = self.available.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Storage from a dict"""
+        """Create an instance of AvailabilityQueryOutput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "type": obj.get("type"),
-            "size": Memory.from_dict(obj["size"]) if obj.get("size") is not None else None,
-            "speed": Bandwidth.from_dict(obj["speed"]) if obj.get("speed") is not None else None
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "available": Available.from_dict(obj["available"]) if obj.get("available") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/storage_data.py` & `perian-0.2.0/perian/models/availability_query_input.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,31 +13,30 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.memory import Memory
-from perian.models.storage import Storage
-from perian.models.storage_included import StorageIncluded
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
+from perian.models.available import Available
 from typing import Optional, Set
 from typing_extensions import Self
 
-class StorageData(BaseModel):
+class AvailabilityQueryInput(BaseModel):
     """
-    StorageData
+    AvailabilityQueryInput
     """ # noqa: E501
-    no: Optional[StrictInt] = 0
-    size: Optional[Memory] = None
-    included: Optional[StorageIncluded] = None
-    storages: Optional[List[Storage]] = None
-    __properties: ClassVar[List[str]] = ["no", "size", "included", "storages"]
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    available: Optional[Available] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "available"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -49,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of StorageData from a JSON string"""
+        """Create an instance of AvailabilityQueryInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,37 +69,35 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of size
-        if self.size:
-            _dict['size'] = self.size.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in storages (list)
-        _items = []
-        if self.storages:
-            for _item in self.storages:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['storages'] = _items
+        # override the default output from pydantic by calling `to_dict()` of operator
+        if self.operator:
+            _dict['operator'] = self.operator.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of options
+        if self.options:
+            _dict['options'] = self.options.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of available
+        if self.available:
+            _dict['available'] = self.available.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of StorageData from a dict"""
+        """Create an instance of AvailabilityQueryInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "no": obj.get("no") if obj.get("no") is not None else 0,
-            "size": Memory.from_dict(obj["size"]) if obj.get("size") is not None else None,
-            "included": obj.get("included"),
-            "storages": [Storage.from_dict(_item) for _item in obj["storages"]] if obj.get("storages") is not None else None
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "available": Available.from_dict(obj["available"]) if obj.get("available") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/storage_included.py` & `perian-0.2.0/perian/models/storage_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class StorageIncluded(str, Enum):
+class StorageType(str, Enum):
     """
-    StorageIncluded
+    StorageType
     """
 
     """
     allowed enum values
     """
+    NVME = 'NVME'
+    SSD = 'SSD'
+    HDD = 'HDD'
     UNDEFINED = 'UNDEFINED'
-    INCLUDED = 'INCLUDED'
-    NOT_INCLUDED = 'NOT_INCLUDED'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of StorageIncluded from a JSON string"""
+        """Create an instance of StorageType from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `perian-0.1.25/perian/models/storage_query.py` & `perian-0.2.0/perian/models/pagination_metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,33 +13,32 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from pydantic import BaseModel, StrictInt
+from typing import Any, ClassVar, Dict, List, Optional
+from perian.models.next_page import NextPage
+from perian.models.previous_page import PreviousPage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class StorageQuery(BaseModel):
+class PaginationMetadata(BaseModel):
     """
-    StorageQuery
+    PaginationMetadata
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    no: Optional[StrictInt] = None
-    size: Optional[Union[StrictFloat, StrictInt]] = None
-    type: Optional[StrictStr] = None
-    speed: Optional[Union[StrictFloat, StrictInt]] = None
-    included: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "no", "size", "type", "speed", "included"]
+    total_items: Optional[StrictInt] = 0
+    items_per_page: Optional[StrictInt] = 25
+    current_page: Optional[StrictInt] = 1
+    total_pages: Optional[StrictInt] = 1
+    next_page: Optional[NextPage] = None
+    previous_page: Optional[PreviousPage] = None
+    __properties: ClassVar[List[str]] = ["total_items", "items_per_page", "current_page", "total_pages", "next_page", "previous_page"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -51,15 +50,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of StorageQuery from a JSON string"""
+        """Create an instance of PaginationMetadata from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,36 +71,35 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of operator
-        if self.operator:
-            _dict['operator'] = self.operator.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of options
-        if self.options:
-            _dict['options'] = self.options.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of next_page
+        if self.next_page:
+            _dict['next_page'] = self.next_page.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of previous_page
+        if self.previous_page:
+            _dict['previous_page'] = self.previous_page.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of StorageQuery from a dict"""
+        """Create an instance of PaginationMetadata from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
-            "no": obj.get("no"),
-            "size": obj.get("size"),
-            "type": obj.get("type"),
-            "speed": obj.get("speed"),
-            "included": obj.get("included")
+            "total_items": obj.get("total_items") if obj.get("total_items") is not None else 0,
+            "items_per_page": obj.get("items_per_page") if obj.get("items_per_page") is not None else 25,
+            "current_page": obj.get("current_page") if obj.get("current_page") is not None else 1,
+            "total_pages": obj.get("total_pages") if obj.get("total_pages") is not None else 1,
+            "next_page": NextPage.from_dict(obj["next_page"]) if obj.get("next_page") is not None else None,
+            "previous_page": PreviousPage.from_dict(obj["previous_page"]) if obj.get("previous_page") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/type_query.py` & `perian-0.2.0/perian/models/storage_query_output.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,27 +15,34 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
+from perian.models.included import Included
+from perian.models.no import No
+from perian.models.type import Type
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TypeQuery(BaseModel):
+class StorageQueryOutput(BaseModel):
     """
-    TypeQuery
+    StorageQueryOutput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    type: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "type"]
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    no: Optional[No] = None
+    size: Optional[StrictStr] = None
+    type: Optional[Type] = None
+    speed: Optional[StrictStr] = None
+    included: Optional[Included] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "no", "size", "type", "speed", "included"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -47,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TypeQuery from a JSON string"""
+        """Create an instance of StorageQueryOutput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,26 +81,39 @@
         )
         # override the default output from pydantic by calling `to_dict()` of operator
         if self.operator:
             _dict['operator'] = self.operator.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of no
+        if self.no:
+            _dict['no'] = self.no.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of type
+        if self.type:
+            _dict['type'] = self.type.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of included
+        if self.included:
+            _dict['included'] = self.included.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TypeQuery from a dict"""
+        """Create an instance of StorageQueryOutput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
-            "type": obj.get("type")
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "no": No.from_dict(obj["no"]) if obj.get("no") is not None else None,
+            "size": obj.get("size"),
+            "type": Type.from_dict(obj["type"]) if obj.get("type") is not None else None,
+            "speed": obj.get("speed"),
+            "included": Included.from_dict(obj["included"]) if obj.get("included") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/validation_error.py` & `perian-0.2.0/perian/models/bill_item.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,26 +15,29 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, StrictStr
 from typing import Any, ClassVar, Dict, List
-from perian.models.validation_error_loc_inner import ValidationErrorLocInner
+from perian.models.currency import Currency
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ValidationError(BaseModel):
+class BillItem(BaseModel):
     """
-    ValidationError
+    A single item on a bill corresponding to one Job.
     """ # noqa: E501
-    loc: List[ValidationErrorLocInner]
-    msg: StrictStr
-    type: StrictStr
-    __properties: ClassVar[List[str]] = ["loc", "msg", "type"]
+    job_id: StrictStr
+    price: StrictStr
+    currency: Currency
+    original_price: StrictStr
+    original_currency: Currency
+    exchange_rate: StrictStr
+    __properties: ClassVar[List[str]] = ["job_id", "price", "currency", "original_price", "original_currency", "exchange_rate"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -46,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ValidationError from a JSON string"""
+        """Create an instance of BillItem from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,33 +70,29 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in loc (list)
-        _items = []
-        if self.loc:
-            for _item in self.loc:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['loc'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ValidationError from a dict"""
+        """Create an instance of BillItem from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "loc": [ValidationErrorLocInner.from_dict(_item) for _item in obj["loc"]] if obj.get("loc") is not None else None,
-            "msg": obj.get("msg"),
-            "type": obj.get("type")
+            "job_id": obj.get("job_id"),
+            "price": obj.get("price"),
+            "currency": obj.get("currency"),
+            "original_price": obj.get("original_price"),
+            "original_currency": obj.get("original_currency"),
+            "exchange_rate": obj.get("exchange_rate")
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/validation_error_loc_inner.py` & `perian-0.2.0/perian/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/vendor.py` & `perian-0.2.0/perian/models/vendor.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/perian/models/zone.py` & `perian-0.2.0/perian/models/docker_metadata.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.status import Status
+from perian.models.create_job_request_docker_registry_credentials import CreateJobRequestDockerRegistryCredentials
+from perian.models.docker_run_parameters import DockerRunParameters
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Zone(BaseModel):
+class DockerMetadata(BaseModel):
     """
-    Zone
+    DockerMetadata
     """ # noqa: E501
-    id: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    status: Optional[Status] = None
-    __properties: ClassVar[List[str]] = ["id", "name", "status"]
+    docker_run_parameters: Optional[DockerRunParameters] = None
+    docker_registry_credentials: Optional[CreateJobRequestDockerRegistryCredentials] = None
+    __properties: ClassVar[List[str]] = ["docker_run_parameters", "docker_registry_credentials"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Zone from a JSON string"""
+        """Create an instance of DockerMetadata from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,26 +67,31 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of docker_run_parameters
+        if self.docker_run_parameters:
+            _dict['docker_run_parameters'] = self.docker_run_parameters.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of docker_registry_credentials
+        if self.docker_registry_credentials:
+            _dict['docker_registry_credentials'] = self.docker_registry_credentials.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Zone from a dict"""
+        """Create an instance of DockerMetadata from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "name": obj.get("name"),
-            "status": obj.get("status")
+            "docker_run_parameters": DockerRunParameters.from_dict(obj["docker_run_parameters"]) if obj.get("docker_run_parameters") is not None else None,
+            "docker_registry_credentials": CreateJobRequestDockerRegistryCredentials.from_dict(obj["docker_registry_credentials"]) if obj.get("docker_registry_credentials") is not None else None
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/models/zone_query.py` & `perian-0.2.0/perian/models/cpu_query_output.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,30 +15,33 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
-from perian.models.id import Id
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
+from perian.models.cores import Cores
+from perian.models.no import No
+from perian.models.threads import Threads
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ZoneQuery(BaseModel):
+class CpuQueryOutput(BaseModel):
     """
-    ZoneQuery
+    CpuQueryOutput
     """ # noqa: E501
-    operator: Optional[AcceleratorQueryOperator] = None
-    options: Optional[AcceleratorQueryOptions] = None
-    id: Optional[Id] = None
-    name: Optional[StrictStr] = None
-    status: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["operator", "options", "id", "name", "status"]
+    operator: Optional[AcceleratorQueryInputOperator] = None
+    options: Optional[AcceleratorQueryInputOptions] = None
+    no: Optional[No] = None
+    cores: Optional[Cores] = None
+    threads: Optional[Threads] = None
+    speed: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["operator", "options", "no", "cores", "threads", "speed"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -50,15 +53,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ZoneQuery from a JSON string"""
+        """Create an instance of CpuQueryOutput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -77,31 +80,38 @@
         )
         # override the default output from pydantic by calling `to_dict()` of operator
         if self.operator:
             _dict['operator'] = self.operator.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict['options'] = self.options.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of id
-        if self.id:
-            _dict['id'] = self.id.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of no
+        if self.no:
+            _dict['no'] = self.no.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of cores
+        if self.cores:
+            _dict['cores'] = self.cores.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of threads
+        if self.threads:
+            _dict['threads'] = self.threads.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ZoneQuery from a dict"""
+        """Create an instance of CpuQueryOutput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "operator": AcceleratorQueryOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
-            "options": AcceleratorQueryOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
-            "id": Id.from_dict(obj["id"]) if obj.get("id") is not None else None,
-            "name": obj.get("name"),
-            "status": obj.get("status")
+            "operator": AcceleratorQueryInputOperator.from_dict(obj["operator"]) if obj.get("operator") is not None else None,
+            "options": AcceleratorQueryInputOptions.from_dict(obj["options"]) if obj.get("options") is not None else None,
+            "no": No.from_dict(obj["no"]) if obj.get("no") is not None else None,
+            "cores": Cores.from_dict(obj["cores"]) if obj.get("cores") is not None else None,
+            "threads": Threads.from_dict(obj["threads"]) if obj.get("threads") is not None else None,
+            "speed": obj.get("speed")
         })
         return _obj
```

### Comparing `perian-0.1.25/perian/rest.py` & `perian-0.2.0/perian/rest.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/pyproject.toml` & `perian-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/setup.py` & `perian-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "perian"
-VERSION = "0.1.25"
+VERSION = "0.2.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `perian-0.1.25/test/test_accelerator_data_view.py` & `perian-0.2.0/test/test_accelerator_data_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,16 +39,16 @@
                 memory = perian.models.memory.Memory(
                     size = '0.0', 
                     unit = null, 
                     bandwidth = null, 
                     interface = null, ),
                 accelerator_types = [
                     perian.models.accelerator_type_view.AcceleratorTypeView(
+                        display_name = '', 
                         id = '', 
-                        name = null, 
                         vendor = null, 
                         memory = null, )
                     ]
             )
         else:
             return AcceleratorDataView(
         )
```

### Comparing `perian-0.1.25/test/test_accelerator_name.py` & `perian-0.2.0/test/test_accelerator_vendor.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.accelerator_name import AcceleratorName
+from perian.models.accelerator_vendor import AcceleratorVendor
 
-class TestAcceleratorName(unittest.TestCase):
-    """AcceleratorName unit test stubs"""
+class TestAcceleratorVendor(unittest.TestCase):
+    """AcceleratorVendor unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAcceleratorName(self):
-        """Test AcceleratorName"""
-        # inst = AcceleratorName()
+    def testAcceleratorVendor(self):
+        """Test AcceleratorVendor"""
+        # inst = AcceleratorVendor()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_accelerator_query.py` & `perian-0.2.0/test/test_accelerator_type_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,49 +10,50 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.accelerator_query import AcceleratorQuery
+from perian.models.accelerator_type_query import AcceleratorTypeQuery
 
-class TestAcceleratorQuery(unittest.TestCase):
-    """AcceleratorQuery unit test stubs"""
+class TestAcceleratorTypeQuery(unittest.TestCase):
+    """AcceleratorTypeQuery unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> AcceleratorQuery:
-        """Test AcceleratorQuery
+    def make_instance(self, include_optional) -> AcceleratorTypeQuery:
+        """Test AcceleratorTypeQuery
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AcceleratorQuery`
+        # uncomment below to create an instance of `AcceleratorTypeQuery`
         """
-        model = AcceleratorQuery()
+        model = AcceleratorTypeQuery()
         if include_optional:
-            return AcceleratorQuery(
+            return AcceleratorTypeQuery(
                 operator = None,
                 options = None,
-                no = 56,
+                no = None,
                 memory = None,
                 vendor = None,
                 name = None,
                 description = None,
-                provider_specific_name = None
+                provider_specific_name = None,
+                id = None
             )
         else:
-            return AcceleratorQuery(
+            return AcceleratorTypeQuery(
         )
         """
 
-    def testAcceleratorQuery(self):
-        """Test AcceleratorQuery"""
+    def testAcceleratorTypeQuery(self):
+        """Test AcceleratorTypeQuery"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_accelerator_query_memory.py` & `perian-0.2.0/test/test_accelerator_query_input_memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,44 +10,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.accelerator_query_memory import AcceleratorQueryMemory
+from perian.models.accelerator_query_input_memory import AcceleratorQueryInputMemory
 
-class TestAcceleratorQueryMemory(unittest.TestCase):
-    """AcceleratorQueryMemory unit test stubs"""
+class TestAcceleratorQueryInputMemory(unittest.TestCase):
+    """AcceleratorQueryInputMemory unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> AcceleratorQueryMemory:
-        """Test AcceleratorQueryMemory
+    def make_instance(self, include_optional) -> AcceleratorQueryInputMemory:
+        """Test AcceleratorQueryInputMemory
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AcceleratorQueryMemory`
+        # uncomment below to create an instance of `AcceleratorQueryInputMemory`
         """
-        model = AcceleratorQueryMemory()
+        model = AcceleratorQueryInputMemory()
         if include_optional:
-            return AcceleratorQueryMemory(
+            return AcceleratorQueryInputMemory(
                 operator = None,
                 options = None,
                 size = None
             )
         else:
-            return AcceleratorQueryMemory(
+            return AcceleratorQueryInputMemory(
         )
         """
 
-    def testAcceleratorQueryMemory(self):
-        """Test AcceleratorQueryMemory"""
+    def testAcceleratorQueryInputMemory(self):
+        """Test AcceleratorQueryInputMemory"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_accelerator_query_operator.py` & `perian-0.2.0/test/test_accelerator_query_input_operator.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,41 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.accelerator_query_operator import AcceleratorQueryOperator
+from perian.models.accelerator_query_input_operator import AcceleratorQueryInputOperator
 
-class TestAcceleratorQueryOperator(unittest.TestCase):
-    """AcceleratorQueryOperator unit test stubs"""
+class TestAcceleratorQueryInputOperator(unittest.TestCase):
+    """AcceleratorQueryInputOperator unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> AcceleratorQueryOperator:
-        """Test AcceleratorQueryOperator
+    def make_instance(self, include_optional) -> AcceleratorQueryInputOperator:
+        """Test AcceleratorQueryInputOperator
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AcceleratorQueryOperator`
+        # uncomment below to create an instance of `AcceleratorQueryInputOperator`
         """
-        model = AcceleratorQueryOperator()
+        model = AcceleratorQueryInputOperator()
         if include_optional:
-            return AcceleratorQueryOperator(
+            return AcceleratorQueryInputOperator(
             )
         else:
-            return AcceleratorQueryOperator(
+            return AcceleratorQueryInputOperator(
         )
         """
 
-    def testAcceleratorQueryOperator(self):
-        """Test AcceleratorQueryOperator"""
+    def testAcceleratorQueryInputOperator(self):
+        """Test AcceleratorQueryInputOperator"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_accelerator_query_options.py` & `perian-0.2.0/test/test_accelerator_query_input_options.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,44 +10,45 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.accelerator_query_options import AcceleratorQueryOptions
+from perian.models.accelerator_query_input_options import AcceleratorQueryInputOptions
 
-class TestAcceleratorQueryOptions(unittest.TestCase):
-    """AcceleratorQueryOptions unit test stubs"""
+class TestAcceleratorQueryInputOptions(unittest.TestCase):
+    """AcceleratorQueryInputOptions unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> AcceleratorQueryOptions:
-        """Test AcceleratorQueryOptions
+    def make_instance(self, include_optional) -> AcceleratorQueryInputOptions:
+        """Test AcceleratorQueryInputOptions
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AcceleratorQueryOptions`
+        # uncomment below to create an instance of `AcceleratorQueryInputOptions`
         """
-        model = AcceleratorQueryOptions()
+        model = AcceleratorQueryInputOptions()
         if include_optional:
-            return AcceleratorQueryOptions(
+            return AcceleratorQueryInputOptions(
                 limit = None,
-                order = '',
+                offset = None,
+                order = 'PRICE',
                 lazy_loading = None
             )
         else:
-            return AcceleratorQueryOptions(
+            return AcceleratorQueryInputOptions(
         )
         """
 
-    def testAcceleratorQueryOptions(self):
-        """Test AcceleratorQueryOptions"""
+    def testAcceleratorQueryInputOptions(self):
+        """Test AcceleratorQueryInputOptions"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_accelerator_type_view.py` & `perian-0.2.0/test/test_accelerator_type_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `AcceleratorTypeView`
         """
         model = AcceleratorTypeView()
         if include_optional:
             return AcceleratorTypeView(
+                display_name = '',
                 id = '',
-                name = 'NVIDIA_H100_80',
                 vendor = 'NVIDIA',
                 memory = perian.models.memory.Memory(
                     size = '0.0', 
                     unit = null, 
                     bandwidth = null, 
                     interface = null, )
             )
```

### Comparing `perian-0.1.25/test/test_accelerator_vendor.py` & `perian-0.2.0/test/test_operator.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.accelerator_vendor import AcceleratorVendor
+from perian.models.operator import Operator
 
-class TestAcceleratorVendor(unittest.TestCase):
-    """AcceleratorVendor unit test stubs"""
+class TestOperator(unittest.TestCase):
+    """Operator unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAcceleratorVendor(self):
-        """Test AcceleratorVendor"""
-        # inst = AcceleratorVendor()
+    def testOperator(self):
+        """Test Operator"""
+        # inst = Operator()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_admin_api.py` & `perian-0.2.0/test/test_memory_unit.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,29 +10,24 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.api.admin_api import AdminApi
+from perian.models.memory_unit import MemoryUnit
 
+class TestMemoryUnit(unittest.TestCase):
+    """MemoryUnit unit test stubs"""
 
-class TestAdminApi(unittest.TestCase):
-    """AdminApi unit test stubs"""
-
-    def setUp(self) -> None:
-        self.api = AdminApi()
-
-    def tearDown(self) -> None:
+    def setUp(self):
         pass
 
-    def test_create_global_admin_admin_post(self) -> None:
-        """Test case for create_global_admin_admin_post
-
-        Create Global Admin
-        """
+    def tearDown(self):
         pass
 
+    def testMemoryUnit(self):
+        """Test MemoryUnit"""
+        # inst = MemoryUnit()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_availability.py` & `perian-0.2.0/test/test_availability.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_availability_query.py` & `perian-0.2.0/test/test_availability_query_input.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,44 +10,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.availability_query import AvailabilityQuery
+from perian.models.availability_query_input import AvailabilityQueryInput
 
-class TestAvailabilityQuery(unittest.TestCase):
-    """AvailabilityQuery unit test stubs"""
+class TestAvailabilityQueryInput(unittest.TestCase):
+    """AvailabilityQueryInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> AvailabilityQuery:
-        """Test AvailabilityQuery
+    def make_instance(self, include_optional) -> AvailabilityQueryInput:
+        """Test AvailabilityQueryInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AvailabilityQuery`
+        # uncomment below to create an instance of `AvailabilityQueryInput`
         """
-        model = AvailabilityQuery()
+        model = AvailabilityQueryInput()
         if include_optional:
-            return AvailabilityQuery(
+            return AvailabilityQueryInput(
                 operator = None,
                 options = None,
-                available = True
+                available = None
             )
         else:
-            return AvailabilityQuery(
+            return AvailabilityQueryInput(
         )
         """
 
-    def testAvailabilityQuery(self):
-        """Test AvailabilityQuery"""
+    def testAvailabilityQueryInput(self):
+        """Test AvailabilityQueryInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_availability_source.py` & `perian-0.2.0/test/test_availability_source.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_bandwidth.py` & `perian-0.2.0/test/test_bandwidth.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_bandwidth_limits.py` & `perian-0.2.0/test/test_bandwidth_limits.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_bandwidth_sla.py` & `perian-0.2.0/test/test_bandwidth_sla.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_bandwidth_units.py` & `perian-0.2.0/test/test_bandwidth_units.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_command.py` & `perian-0.2.0/test/test_command.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_compute_billing_period.py` & `perian-0.2.0/test/test_location.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.compute_billing_period import ComputeBillingPeriod
+from perian.models.location import Location
 
-class TestComputeBillingPeriod(unittest.TestCase):
-    """ComputeBillingPeriod unit test stubs"""
+class TestLocation(unittest.TestCase):
+    """Location unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testComputeBillingPeriod(self):
-        """Test ComputeBillingPeriod"""
-        # inst = ComputeBillingPeriod()
+    def testLocation(self):
+        """Test Location"""
+        # inst = Location()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_compute_instance_type.py` & `perian-0.2.0/test/test_compute_instance_type.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_cpu.py` & `perian-0.2.0/test/test_cpu.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_cpu_data.py` & `perian-0.2.0/test/test_cpu_data.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_cpu_query.py` & `perian-0.2.0/test/test_zone.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,47 +10,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.cpu_query import CpuQuery
+from perian.models.zone import Zone
 
-class TestCpuQuery(unittest.TestCase):
-    """CpuQuery unit test stubs"""
+class TestZone(unittest.TestCase):
+    """Zone unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CpuQuery:
-        """Test CpuQuery
+    def make_instance(self, include_optional) -> Zone:
+        """Test Zone
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CpuQuery`
+        # uncomment below to create an instance of `Zone`
         """
-        model = CpuQuery()
+        model = Zone()
         if include_optional:
-            return CpuQuery(
-                operator = None,
-                options = None,
-                no = 56,
-                cores = 56,
-                threads = 56,
-                speed = 1.337
+            return Zone(
+                id = '',
+                name = '',
+                status = 'Active'
             )
         else:
-            return CpuQuery(
+            return Zone(
         )
         """
 
-    def testCpuQuery(self):
-        """Test CpuQuery"""
+    def testZone(self):
+        """Test Zone"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_create_admin_success.py` & `perian-0.2.0/test/test_create_job_success.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,45 +10,47 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.create_admin_success import CreateAdminSuccess
+from perian.models.create_job_success import CreateJobSuccess
 
-class TestCreateAdminSuccess(unittest.TestCase):
-    """CreateAdminSuccess unit test stubs"""
+class TestCreateJobSuccess(unittest.TestCase):
+    """CreateJobSuccess unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateAdminSuccess:
-        """Test CreateAdminSuccess
+    def make_instance(self, include_optional) -> CreateJobSuccess:
+        """Test CreateJobSuccess
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateAdminSuccess`
+        # uncomment below to create an instance of `CreateJobSuccess`
         """
-        model = CreateAdminSuccess()
+        model = CreateJobSuccess()
         if include_optional:
-            return CreateAdminSuccess(
+            return CreateJobSuccess(
                 status = 'Success',
-                message = 'Operation was successful',
-                detail = 'Global admin created successfully',
-                status_code = 56
+                message = 'Job created successfully',
+                detail = '',
+                status_code = 56,
+                id = ''
             )
         else:
-            return CreateAdminSuccess(
+            return CreateJobSuccess(
+                id = '',
         )
         """
 
-    def testCreateAdminSuccess(self):
-        """Test CreateAdminSuccess"""
+    def testCreateJobSuccess(self):
+        """Test CreateJobSuccess"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_create_global_admin_request.py` & `perian-0.2.0/test/test_create_job_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,46 +10,51 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.create_global_admin_request import CreateGlobalAdminRequest
+from perian.models.create_job_request import CreateJobRequest
 
-class TestCreateGlobalAdminRequest(unittest.TestCase):
-    """CreateGlobalAdminRequest unit test stubs"""
+class TestCreateJobRequest(unittest.TestCase):
+    """CreateJobRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateGlobalAdminRequest:
-        """Test CreateGlobalAdminRequest
+    def make_instance(self, include_optional) -> CreateJobRequest:
+        """Test CreateJobRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateGlobalAdminRequest`
+        # uncomment below to create an instance of `CreateJobRequest`
         """
-        model = CreateGlobalAdminRequest()
+        model = CreateJobRequest()
         if include_optional:
-            return CreateGlobalAdminRequest(
-                mail_address = '',
-                setup_token = '',
-                password = '',
-                firstname = '',
-                lastname = ''
+            return CreateJobRequest(
+                instance_type_id = None,
+                auto_failover_instance_type = True,
+                os_storage_config = perian.models.os_storage_config.OSStorageConfig(
+                    size = 56, ),
+                requirements = None,
+                docker_run_parameters = perian.models.docker_run_parameters.DockerRunParameters(
+                    image_name = '', 
+                    image_tag = null, 
+                    command = null, ),
+                docker_registry_credentials = None
             )
         else:
-            return CreateGlobalAdminRequest(
+            return CreateJobRequest(
         )
         """
 
-    def testCreateGlobalAdminRequest(self):
-        """Test CreateGlobalAdminRequest"""
+    def testCreateJobRequest(self):
+        """Test CreateJobRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_create_job_request.py` & `perian-0.2.0/test/test_memory_query_input.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,49 +10,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.create_job_request import CreateJobRequest
+from perian.models.memory_query_input import MemoryQueryInput
 
-class TestCreateJobRequest(unittest.TestCase):
-    """CreateJobRequest unit test stubs"""
+class TestMemoryQueryInput(unittest.TestCase):
+    """MemoryQueryInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateJobRequest:
-        """Test CreateJobRequest
+    def make_instance(self, include_optional) -> MemoryQueryInput:
+        """Test MemoryQueryInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateJobRequest`
+        # uncomment below to create an instance of `MemoryQueryInput`
         """
-        model = CreateJobRequest()
+        model = MemoryQueryInput()
         if include_optional:
-            return CreateJobRequest(
-                instance_type_id = '',
-                os_storage_config = perian.models.os_storage_config.OSStorageConfig(
-                    size = 56, ),
-                docker_run_parameters = perian.models.docker_run_parameters.DockerRunParameters(
-                    image_name = '', 
-                    image_tag = null, 
-                    command = null, ),
-                docker_registry_credentials = None
+            return MemoryQueryInput(
+                operator = None,
+                options = None,
+                size = None
             )
         else:
-            return CreateJobRequest(
+            return MemoryQueryInput(
         )
         """
 
-    def testCreateJobRequest(self):
-        """Test CreateJobRequest"""
+    def testMemoryQueryInput(self):
+        """Test MemoryQueryInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_create_job_request_docker_registry_credentials.py` & `perian-0.2.0/test/test_create_job_request_docker_registry_credentials.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_create_job_success.py` & `perian-0.2.0/test/test_pagination_metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,47 +10,47 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.create_job_success import CreateJobSuccess
+from perian.models.pagination_metadata import PaginationMetadata
 
-class TestCreateJobSuccess(unittest.TestCase):
-    """CreateJobSuccess unit test stubs"""
+class TestPaginationMetadata(unittest.TestCase):
+    """PaginationMetadata unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateJobSuccess:
-        """Test CreateJobSuccess
+    def make_instance(self, include_optional) -> PaginationMetadata:
+        """Test PaginationMetadata
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateJobSuccess`
+        # uncomment below to create an instance of `PaginationMetadata`
         """
-        model = CreateJobSuccess()
+        model = PaginationMetadata()
         if include_optional:
-            return CreateJobSuccess(
-                status = 'Success',
-                message = 'Job created successfully',
-                detail = '',
-                status_code = 56,
-                id = ''
+            return PaginationMetadata(
+                total_items = 56,
+                items_per_page = 56,
+                current_page = 56,
+                total_pages = 56,
+                next_page = None,
+                previous_page = None
             )
         else:
-            return CreateJobSuccess(
-                id = '',
+            return PaginationMetadata(
         )
         """
 
-    def testCreateJobSuccess(self):
-        """Test CreateJobSuccess"""
+    def testPaginationMetadata(self):
+        """Test PaginationMetadata"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_create_organization_request.py` & `perian-0.2.0/test/test_query_options.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,43 +10,45 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.create_organization_request import CreateOrganizationRequest
+from perian.models.query_options import QueryOptions
 
-class TestCreateOrganizationRequest(unittest.TestCase):
-    """CreateOrganizationRequest unit test stubs"""
+class TestQueryOptions(unittest.TestCase):
+    """QueryOptions unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateOrganizationRequest:
-        """Test CreateOrganizationRequest
+    def make_instance(self, include_optional) -> QueryOptions:
+        """Test QueryOptions
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateOrganizationRequest`
+        # uncomment below to create an instance of `QueryOptions`
         """
-        model = CreateOrganizationRequest()
+        model = QueryOptions()
         if include_optional:
-            return CreateOrganizationRequest(
-                name = '',
-                reference = None
+            return QueryOptions(
+                limit = None,
+                offset = None,
+                order = 'PRICE',
+                lazy_loading = True
             )
         else:
-            return CreateOrganizationRequest(
+            return QueryOptions(
         )
         """
 
-    def testCreateOrganizationRequest(self):
-        """Test CreateOrganizationRequest"""
+    def testQueryOptions(self):
+        """Test QueryOptions"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_create_organization_success.py` & `perian-0.2.0/test/test_location1.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,49 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.create_organization_success import CreateOrganizationSuccess
+from perian.models.location1 import Location1
 
-class TestCreateOrganizationSuccess(unittest.TestCase):
-    """CreateOrganizationSuccess unit test stubs"""
+class TestLocation1(unittest.TestCase):
+    """Location1 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateOrganizationSuccess:
-        """Test CreateOrganizationSuccess
+    def make_instance(self, include_optional) -> Location1:
+        """Test Location1
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateOrganizationSuccess`
+        # uncomment below to create an instance of `Location1`
         """
-        model = CreateOrganizationSuccess()
+        model = Location1()
         if include_optional:
-            return CreateOrganizationSuccess(
-                status = 'Success',
-                message = 'Operation was successful',
-                detail = 'Organization created successfully',
-                status_code = 56,
-                organization = perian.models.organization.Organization(
-                    name = '', )
+            return Location1(
             )
         else:
-            return CreateOrganizationSuccess(
-                organization = perian.models.organization.Organization(
-                    name = '', ),
+            return Location1(
         )
         """
 
-    def testCreateOrganizationSuccess(self):
-        """Test CreateOrganizationSuccess"""
+    def testLocation1(self):
+        """Test Location1"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_create_service_account_request.py` & `perian-0.2.0/test/test_vendor.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,45 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.create_service_account_request import CreateServiceAccountRequest
+from perian.models.vendor import Vendor
 
-class TestCreateServiceAccountRequest(unittest.TestCase):
-    """CreateServiceAccountRequest unit test stubs"""
+class TestVendor(unittest.TestCase):
+    """Vendor unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateServiceAccountRequest:
-        """Test CreateServiceAccountRequest
+    def make_instance(self, include_optional) -> Vendor:
+        """Test Vendor
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateServiceAccountRequest`
+        # uncomment below to create an instance of `Vendor`
         """
-        model = CreateServiceAccountRequest()
+        model = Vendor()
         if include_optional:
-            return CreateServiceAccountRequest(
-                service_account_name = '',
-                roles = [
-                    ''
-                    ]
+            return Vendor(
             )
         else:
-            return CreateServiceAccountRequest(
+            return Vendor(
         )
         """
 
-    def testCreateServiceAccountRequest(self):
-        """Test CreateServiceAccountRequest"""
+    def testVendor(self):
+        """Test Vendor"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_create_service_account_success.py` & `perian-0.2.0/test/test_no.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,47 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.create_service_account_success import CreateServiceAccountSuccess
+from perian.models.no import No
 
-class TestCreateServiceAccountSuccess(unittest.TestCase):
-    """CreateServiceAccountSuccess unit test stubs"""
+class TestNo(unittest.TestCase):
+    """No unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateServiceAccountSuccess:
-        """Test CreateServiceAccountSuccess
+    def make_instance(self, include_optional) -> No:
+        """Test No
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateServiceAccountSuccess`
+        # uncomment below to create an instance of `No`
         """
-        model = CreateServiceAccountSuccess()
+        model = No()
         if include_optional:
-            return CreateServiceAccountSuccess(
-                status = 'Success',
-                message = 'Operation was successful',
-                detail = 'Service account created successfully',
-                status_code = 56,
-                client_id = '',
-                client_secret = ''
+            return No(
             )
         else:
-            return CreateServiceAccountSuccess(
+            return No(
         )
         """
 
-    def testCreateServiceAccountSuccess(self):
-        """Test CreateServiceAccountSuccess"""
+    def testNo(self):
+        """Test No"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_create_user_request.py` & `perian-0.2.0/test/test_threads.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,49 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.create_user_request import CreateUserRequest
+from perian.models.threads import Threads
 
-class TestCreateUserRequest(unittest.TestCase):
-    """CreateUserRequest unit test stubs"""
+class TestThreads(unittest.TestCase):
+    """Threads unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateUserRequest:
-        """Test CreateUserRequest
+    def make_instance(self, include_optional) -> Threads:
+        """Test Threads
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateUserRequest`
+        # uncomment below to create an instance of `Threads`
         """
-        model = CreateUserRequest()
+        model = Threads()
         if include_optional:
-            return CreateUserRequest(
-                username = '',
-                mail_address = '',
-                password = '',
-                firstname = '',
-                lastname = '[]',
-                roles = [
-                    ''
-                    ]
+            return Threads(
             )
         else:
-            return CreateUserRequest(
+            return Threads(
         )
         """
 
-    def testCreateUserRequest(self):
-        """Test CreateUserRequest"""
+    def testThreads(self):
+        """Test Threads"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_create_user_success.py` & `perian-0.2.0/test/test_provider_properties.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,45 +10,42 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.create_user_success import CreateUserSuccess
+from perian.models.provider_properties import ProviderProperties
 
-class TestCreateUserSuccess(unittest.TestCase):
-    """CreateUserSuccess unit test stubs"""
+class TestProviderProperties(unittest.TestCase):
+    """ProviderProperties unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateUserSuccess:
-        """Test CreateUserSuccess
+    def make_instance(self, include_optional) -> ProviderProperties:
+        """Test ProviderProperties
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateUserSuccess`
+        # uncomment below to create an instance of `ProviderProperties`
         """
-        model = CreateUserSuccess()
+        model = ProviderProperties()
         if include_optional:
-            return CreateUserSuccess(
-                status = 'Success',
-                message = 'Operation was successful',
-                detail = 'User created successfully',
-                status_code = 56
+            return ProviderProperties(
+                compute_billing_granularity = 'PER_SECOND'
             )
         else:
-            return CreateUserSuccess(
+            return ProviderProperties(
         )
         """
 
-    def testCreateUserSuccess(self):
-        """Test CreateUserSuccess"""
+    def testProviderProperties(self):
+        """Test ProviderProperties"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_currency.py` & `perian-0.2.0/test/test_currency.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_default_client_error.py` & `perian-0.2.0/test/test_default_client_error.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_default_server_error.py` & `perian-0.2.0/test/test_default_server_error.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_description.py` & `perian-0.2.0/test/test_description.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_docker_registry_credentials.py` & `perian-0.2.0/test/test_docker_registry_credentials.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_docker_run_parameters.py` & `perian-0.2.0/test/test_docker_run_parameters.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_done_at.py` & `perian-0.2.0/test/test_done_at.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_get_instance_types_success.py` & `perian-0.2.0/test/test_get_instance_types_success.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,22 @@
                         cpu = null, 
                         accelerator = null, 
                         ram = null, 
                         storage = null, 
                         network = null, 
                         price = null, 
                         availability = null, )
-                    ]
+                    ],
+                pagination = perian.models.pagination_metadata.PaginationMetadata(
+                    total_items = 56, 
+                    items_per_page = 56, 
+                    current_page = 56, 
+                    total_pages = 56, 
+                    next_page = null, 
+                    previous_page = null, )
             )
         else:
             return GetInstanceTypesSuccess(
         )
         """
 
     def testGetInstanceTypesSuccess(self):
```

### Comparing `perian-0.1.25/test/test_get_jobs_success.py` & `perian-0.2.0/test/test_get_jobs_success.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,31 +35,39 @@
         model = GetJobsSuccess()
         if include_optional:
             return GetJobsSuccess(
                 status = 'Success',
                 message = 'Operation was successful',
                 detail = '',
                 status_code = 56,
+                limit = 56,
+                no = 56,
                 jobs = [
                     perian.models.job_view.JobView(
                         id = '', 
                         status = null, 
+                        started_at = null, 
                         done_at = null, 
-                        logs = null, )
-                    ]
+                        logs = null, 
+                        errors = null, 
+                        price = null, 
+                        docker_metadata = null, 
+                        requirement_metadata = null, 
+                        runtime_metadata = null, )
+                    ],
+                pagination = perian.models.pagination_metadata.PaginationMetadata(
+                    total_items = 56, 
+                    items_per_page = 56, 
+                    current_page = 56, 
+                    total_pages = 56, 
+                    next_page = null, 
+                    previous_page = null, )
             )
         else:
             return GetJobsSuccess(
-                jobs = [
-                    perian.models.job_view.JobView(
-                        id = '', 
-                        status = null, 
-                        done_at = null, 
-                        logs = null, )
-                    ],
         )
         """
 
     def testGetJobsSuccess(self):
         """Test GetJobsSuccess"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `perian-0.1.25/test/test_http_validation_error.py` & `perian-0.2.0/test/test_http_validation_error.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_id.py` & `perian-0.2.0/test/test_id.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_image_tag.py` & `perian-0.2.0/test/test_image_tag.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_instance_type_api.py` & `perian-0.2.0/test/test_instance_type_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,17 +22,24 @@
 
     def setUp(self) -> None:
         self.api = InstanceTypeApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_get_instance_type_instance_type_get(self) -> None:
-        """Test case for get_instance_type_instance_type_get
+    def test_get_instance_type_by_id(self) -> None:
+        """Test case for get_instance_type_by_id
 
-        Get Instance Type
+        Get Instance Type By Id
+        """
+        pass
+
+    def test_get_instance_type_by_requirements(self) -> None:
+        """Test case for get_instance_type_by_requirements
+
+        Get Instance Type By Requirements
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_blocked_error.py` & `perian-0.2.0/test/test_instance_type_query_output_zone.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,45 +10,46 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_blocked_error import InstanceTypeBlockedError
+from perian.models.instance_type_query_output_zone import InstanceTypeQueryOutputZone
 
-class TestInstanceTypeBlockedError(unittest.TestCase):
-    """InstanceTypeBlockedError unit test stubs"""
+class TestInstanceTypeQueryOutputZone(unittest.TestCase):
+    """InstanceTypeQueryOutputZone unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeBlockedError:
-        """Test InstanceTypeBlockedError
+    def make_instance(self, include_optional) -> InstanceTypeQueryOutputZone:
+        """Test InstanceTypeQueryOutputZone
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeBlockedError`
+        # uncomment below to create an instance of `InstanceTypeQueryOutputZone`
         """
-        model = InstanceTypeBlockedError()
+        model = InstanceTypeQueryOutputZone()
         if include_optional:
-            return InstanceTypeBlockedError(
-                status = 'Error',
-                message = 'Operation failed due to a client error',
-                detail = 'The selected Instance Type is blocked for your account',
-                status_code = 56
+            return InstanceTypeQueryOutputZone(
+                operator = None,
+                options = None,
+                id = None,
+                name = None,
+                status = None
             )
         else:
-            return InstanceTypeBlockedError(
+            return InstanceTypeQueryOutputZone(
         )
         """
 
-    def testInstanceTypeBlockedError(self):
-        """Test InstanceTypeBlockedError"""
+    def testInstanceTypeQueryOutputZone(self):
+        """Test InstanceTypeQueryOutputZone"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query.py` & `perian-0.2.0/test/test_instance_type_query_output.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,57 +10,57 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query import InstanceTypeQuery
+from perian.models.instance_type_query_output import InstanceTypeQueryOutput
 
-class TestInstanceTypeQuery(unittest.TestCase):
-    """InstanceTypeQuery unit test stubs"""
+class TestInstanceTypeQueryOutput(unittest.TestCase):
+    """InstanceTypeQueryOutput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQuery:
-        """Test InstanceTypeQuery
+    def make_instance(self, include_optional) -> InstanceTypeQueryOutput:
+        """Test InstanceTypeQueryOutput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQuery`
+        # uncomment below to create an instance of `InstanceTypeQueryOutput`
         """
-        model = InstanceTypeQuery()
+        model = InstanceTypeQueryOutput()
         if include_optional:
-            return InstanceTypeQuery(
+            return InstanceTypeQueryOutput(
                 operator = None,
                 options = None,
                 id = None,
-                provider = None,
                 region = None,
                 zone = None,
-                reference_id = None,
                 name = None,
                 cpu = None,
                 accelerator = None,
                 ram = None,
                 storage = None,
                 network = None,
                 price = None,
                 availability = None,
-                type = None
+                type = None,
+                provider = None,
+                reference_id = None
             )
         else:
-            return InstanceTypeQuery(
+            return InstanceTypeQueryOutput(
         )
         """
 
-    def testInstanceTypeQuery(self):
-        """Test InstanceTypeQuery"""
+    def testInstanceTypeQueryOutput(self):
+        """Test InstanceTypeQueryOutput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_accelerator.py` & `perian-0.2.0/test/test_instance_type_query_output_accelerator.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,49 +10,49 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_accelerator import InstanceTypeQueryAccelerator
+from perian.models.instance_type_query_output_accelerator import InstanceTypeQueryOutputAccelerator
 
-class TestInstanceTypeQueryAccelerator(unittest.TestCase):
-    """InstanceTypeQueryAccelerator unit test stubs"""
+class TestInstanceTypeQueryOutputAccelerator(unittest.TestCase):
+    """InstanceTypeQueryOutputAccelerator unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryAccelerator:
-        """Test InstanceTypeQueryAccelerator
+    def make_instance(self, include_optional) -> InstanceTypeQueryOutputAccelerator:
+        """Test InstanceTypeQueryOutputAccelerator
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryAccelerator`
+        # uncomment below to create an instance of `InstanceTypeQueryOutputAccelerator`
         """
-        model = InstanceTypeQueryAccelerator()
+        model = InstanceTypeQueryOutputAccelerator()
         if include_optional:
-            return InstanceTypeQueryAccelerator(
+            return InstanceTypeQueryOutputAccelerator(
                 operator = None,
                 options = None,
                 no = None,
                 memory = None,
                 vendor = None,
                 name = None,
                 description = None,
                 provider_specific_name = None
             )
         else:
-            return InstanceTypeQueryAccelerator(
+            return InstanceTypeQueryOutputAccelerator(
         )
         """
 
-    def testInstanceTypeQueryAccelerator(self):
-        """Test InstanceTypeQueryAccelerator"""
+    def testInstanceTypeQueryOutputAccelerator(self):
+        """Test InstanceTypeQueryOutputAccelerator"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_availability.py` & `perian-0.2.0/test/test_instance_type_query_output_price.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,44 +10,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_availability import InstanceTypeQueryAvailability
+from perian.models.instance_type_query_output_price import InstanceTypeQueryOutputPrice
 
-class TestInstanceTypeQueryAvailability(unittest.TestCase):
-    """InstanceTypeQueryAvailability unit test stubs"""
+class TestInstanceTypeQueryOutputPrice(unittest.TestCase):
+    """InstanceTypeQueryOutputPrice unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryAvailability:
-        """Test InstanceTypeQueryAvailability
+    def make_instance(self, include_optional) -> InstanceTypeQueryOutputPrice:
+        """Test InstanceTypeQueryOutputPrice
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryAvailability`
+        # uncomment below to create an instance of `InstanceTypeQueryOutputPrice`
         """
-        model = InstanceTypeQueryAvailability()
+        model = InstanceTypeQueryOutputPrice()
         if include_optional:
-            return InstanceTypeQueryAvailability(
+            return InstanceTypeQueryOutputPrice(
                 operator = None,
                 options = None,
-                available = None
+                unit_price = None
             )
         else:
-            return InstanceTypeQueryAvailability(
+            return InstanceTypeQueryOutputPrice(
         )
         """
 
-    def testInstanceTypeQueryAvailability(self):
-        """Test InstanceTypeQueryAvailability"""
+    def testInstanceTypeQueryOutputPrice(self):
+        """Test InstanceTypeQueryOutputPrice"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_cpu.py` & `perian-0.2.0/test/test_instance_type_query_input_region.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,47 +10,48 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_cpu import InstanceTypeQueryCpu
+from perian.models.instance_type_query_input_region import InstanceTypeQueryInputRegion
 
-class TestInstanceTypeQueryCpu(unittest.TestCase):
-    """InstanceTypeQueryCpu unit test stubs"""
+class TestInstanceTypeQueryInputRegion(unittest.TestCase):
+    """InstanceTypeQueryInputRegion unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryCpu:
-        """Test InstanceTypeQueryCpu
+    def make_instance(self, include_optional) -> InstanceTypeQueryInputRegion:
+        """Test InstanceTypeQueryInputRegion
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryCpu`
+        # uncomment below to create an instance of `InstanceTypeQueryInputRegion`
         """
-        model = InstanceTypeQueryCpu()
+        model = InstanceTypeQueryInputRegion()
         if include_optional:
-            return InstanceTypeQueryCpu(
+            return InstanceTypeQueryInputRegion(
                 operator = None,
                 options = None,
-                no = None,
-                cores = None,
-                threads = None,
-                speed = None
+                id = None,
+                name = None,
+                location = None,
+                sustainable = None,
+                status = None
             )
         else:
-            return InstanceTypeQueryCpu(
+            return InstanceTypeQueryInputRegion(
         )
         """
 
-    def testInstanceTypeQueryCpu(self):
-        """Test InstanceTypeQueryCpu"""
+    def testInstanceTypeQueryInputRegion(self):
+        """Test InstanceTypeQueryInputRegion"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_name.py` & `perian-0.2.0/test/test_instance_type_query_output_cpu.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,44 +10,47 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_name import InstanceTypeQueryName
+from perian.models.instance_type_query_output_cpu import InstanceTypeQueryOutputCpu
 
-class TestInstanceTypeQueryName(unittest.TestCase):
-    """InstanceTypeQueryName unit test stubs"""
+class TestInstanceTypeQueryOutputCpu(unittest.TestCase):
+    """InstanceTypeQueryOutputCpu unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryName:
-        """Test InstanceTypeQueryName
+    def make_instance(self, include_optional) -> InstanceTypeQueryOutputCpu:
+        """Test InstanceTypeQueryOutputCpu
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryName`
+        # uncomment below to create an instance of `InstanceTypeQueryOutputCpu`
         """
-        model = InstanceTypeQueryName()
+        model = InstanceTypeQueryOutputCpu()
         if include_optional:
-            return InstanceTypeQueryName(
+            return InstanceTypeQueryOutputCpu(
                 operator = None,
                 options = None,
-                name = None
+                no = None,
+                cores = None,
+                threads = None,
+                speed = None
             )
         else:
-            return InstanceTypeQueryName(
+            return InstanceTypeQueryOutputCpu(
         )
         """
 
-    def testInstanceTypeQueryName(self):
-        """Test InstanceTypeQueryName"""
+    def testInstanceTypeQueryOutputCpu(self):
+        """Test InstanceTypeQueryOutputCpu"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_network.py` & `perian-0.2.0/test/test_instance_type_query_input_price.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,45 +10,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_network import InstanceTypeQueryNetwork
+from perian.models.instance_type_query_input_price import InstanceTypeQueryInputPrice
 
-class TestInstanceTypeQueryNetwork(unittest.TestCase):
-    """InstanceTypeQueryNetwork unit test stubs"""
+class TestInstanceTypeQueryInputPrice(unittest.TestCase):
+    """InstanceTypeQueryInputPrice unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryNetwork:
-        """Test InstanceTypeQueryNetwork
+    def make_instance(self, include_optional) -> InstanceTypeQueryInputPrice:
+        """Test InstanceTypeQueryInputPrice
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryNetwork`
+        # uncomment below to create an instance of `InstanceTypeQueryInputPrice`
         """
-        model = InstanceTypeQueryNetwork()
+        model = InstanceTypeQueryInputPrice()
         if include_optional:
-            return InstanceTypeQueryNetwork(
+            return InstanceTypeQueryInputPrice(
                 operator = None,
                 options = None,
-                inbound_speed = None,
-                outbound_speed = None
+                unit_price = None
             )
         else:
-            return InstanceTypeQueryNetwork(
+            return InstanceTypeQueryInputPrice(
         )
         """
 
-    def testInstanceTypeQueryNetwork(self):
-        """Test InstanceTypeQueryNetwork"""
+    def testInstanceTypeQueryInputPrice(self):
+        """Test InstanceTypeQueryInputPrice"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_price.py` & `perian-0.2.0/test/test_instance_type_query_output_region.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,46 +10,48 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_price import InstanceTypeQueryPrice
+from perian.models.instance_type_query_output_region import InstanceTypeQueryOutputRegion
 
-class TestInstanceTypeQueryPrice(unittest.TestCase):
-    """InstanceTypeQueryPrice unit test stubs"""
+class TestInstanceTypeQueryOutputRegion(unittest.TestCase):
+    """InstanceTypeQueryOutputRegion unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryPrice:
-        """Test InstanceTypeQueryPrice
+    def make_instance(self, include_optional) -> InstanceTypeQueryOutputRegion:
+        """Test InstanceTypeQueryOutputRegion
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryPrice`
+        # uncomment below to create an instance of `InstanceTypeQueryOutputRegion`
         """
-        model = InstanceTypeQueryPrice()
+        model = InstanceTypeQueryOutputRegion()
         if include_optional:
-            return InstanceTypeQueryPrice(
+            return InstanceTypeQueryOutputRegion(
                 operator = None,
                 options = None,
-                euro_price = None,
-                unit = None,
-                per_hour = None
+                id = None,
+                name = None,
+                location = None,
+                sustainable = None,
+                status = None
             )
         else:
-            return InstanceTypeQueryPrice(
+            return InstanceTypeQueryOutputRegion(
         )
         """
 
-    def testInstanceTypeQueryPrice(self):
-        """Test InstanceTypeQueryPrice"""
+    def testInstanceTypeQueryOutputRegion(self):
+        """Test InstanceTypeQueryOutputRegion"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_provider.py` & `perian-0.2.0/test/test_instance_type_query_input_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,48 +10,48 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_provider import InstanceTypeQueryProvider
+from perian.models.instance_type_query_input_provider import InstanceTypeQueryInputProvider
 
-class TestInstanceTypeQueryProvider(unittest.TestCase):
-    """InstanceTypeQueryProvider unit test stubs"""
+class TestInstanceTypeQueryInputProvider(unittest.TestCase):
+    """InstanceTypeQueryInputProvider unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryProvider:
-        """Test InstanceTypeQueryProvider
+    def make_instance(self, include_optional) -> InstanceTypeQueryInputProvider:
+        """Test InstanceTypeQueryInputProvider
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryProvider`
+        # uncomment below to create an instance of `InstanceTypeQueryInputProvider`
         """
-        model = InstanceTypeQueryProvider()
+        model = InstanceTypeQueryInputProvider()
         if include_optional:
-            return InstanceTypeQueryProvider(
+            return InstanceTypeQueryInputProvider(
                 operator = None,
                 options = None,
                 id = None,
                 name = None,
                 name_short = None,
                 location = None,
                 status = None
             )
         else:
-            return InstanceTypeQueryProvider(
+            return InstanceTypeQueryInputProvider(
         )
         """
 
-    def testInstanceTypeQueryProvider(self):
-        """Test InstanceTypeQueryProvider"""
+    def testInstanceTypeQueryInputProvider(self):
+        """Test InstanceTypeQueryInputProvider"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_reference_id.py` & `perian-0.2.0/test/test_instance_type_query_input_storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,44 +10,48 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_reference_id import InstanceTypeQueryReferenceId
+from perian.models.instance_type_query_input_storage import InstanceTypeQueryInputStorage
 
-class TestInstanceTypeQueryReferenceId(unittest.TestCase):
-    """InstanceTypeQueryReferenceId unit test stubs"""
+class TestInstanceTypeQueryInputStorage(unittest.TestCase):
+    """InstanceTypeQueryInputStorage unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryReferenceId:
-        """Test InstanceTypeQueryReferenceId
+    def make_instance(self, include_optional) -> InstanceTypeQueryInputStorage:
+        """Test InstanceTypeQueryInputStorage
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryReferenceId`
+        # uncomment below to create an instance of `InstanceTypeQueryInputStorage`
         """
-        model = InstanceTypeQueryReferenceId()
+        model = InstanceTypeQueryInputStorage()
         if include_optional:
-            return InstanceTypeQueryReferenceId(
+            return InstanceTypeQueryInputStorage(
                 operator = None,
                 options = None,
-                id = None
+                no = None,
+                size = None,
+                type = None,
+                speed = None,
+                included = None
             )
         else:
-            return InstanceTypeQueryReferenceId(
+            return InstanceTypeQueryInputStorage(
         )
         """
 
-    def testInstanceTypeQueryReferenceId(self):
-        """Test InstanceTypeQueryReferenceId"""
+    def testInstanceTypeQueryInputStorage(self):
+        """Test InstanceTypeQueryInputStorage"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_region.py` & `perian-0.2.0/test/test_instance_type_query_input_zone.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,48 +10,46 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_region import InstanceTypeQueryRegion
+from perian.models.instance_type_query_input_zone import InstanceTypeQueryInputZone
 
-class TestInstanceTypeQueryRegion(unittest.TestCase):
-    """InstanceTypeQueryRegion unit test stubs"""
+class TestInstanceTypeQueryInputZone(unittest.TestCase):
+    """InstanceTypeQueryInputZone unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryRegion:
-        """Test InstanceTypeQueryRegion
+    def make_instance(self, include_optional) -> InstanceTypeQueryInputZone:
+        """Test InstanceTypeQueryInputZone
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryRegion`
+        # uncomment below to create an instance of `InstanceTypeQueryInputZone`
         """
-        model = InstanceTypeQueryRegion()
+        model = InstanceTypeQueryInputZone()
         if include_optional:
-            return InstanceTypeQueryRegion(
+            return InstanceTypeQueryInputZone(
                 operator = None,
                 options = None,
                 id = None,
                 name = None,
-                location = None,
-                sustainable = None,
                 status = None
             )
         else:
-            return InstanceTypeQueryRegion(
+            return InstanceTypeQueryInputZone(
         )
         """
 
-    def testInstanceTypeQueryRegion(self):
-        """Test InstanceTypeQueryRegion"""
+    def testInstanceTypeQueryInputZone(self):
+        """Test InstanceTypeQueryInputZone"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_storage.py` & `perian-0.2.0/test/test_instance_type_query_output_provider.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,48 +10,48 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_storage import InstanceTypeQueryStorage
+from perian.models.instance_type_query_output_provider import InstanceTypeQueryOutputProvider
 
-class TestInstanceTypeQueryStorage(unittest.TestCase):
-    """InstanceTypeQueryStorage unit test stubs"""
+class TestInstanceTypeQueryOutputProvider(unittest.TestCase):
+    """InstanceTypeQueryOutputProvider unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryStorage:
-        """Test InstanceTypeQueryStorage
+    def make_instance(self, include_optional) -> InstanceTypeQueryOutputProvider:
+        """Test InstanceTypeQueryOutputProvider
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryStorage`
+        # uncomment below to create an instance of `InstanceTypeQueryOutputProvider`
         """
-        model = InstanceTypeQueryStorage()
+        model = InstanceTypeQueryOutputProvider()
         if include_optional:
-            return InstanceTypeQueryStorage(
+            return InstanceTypeQueryOutputProvider(
                 operator = None,
                 options = None,
-                no = None,
-                size = None,
-                type = None,
-                speed = None,
-                included = None
+                id = None,
+                name = None,
+                name_short = None,
+                location = None,
+                status = None
             )
         else:
-            return InstanceTypeQueryStorage(
+            return InstanceTypeQueryOutputProvider(
         )
         """
 
-    def testInstanceTypeQueryStorage(self):
-        """Test InstanceTypeQueryStorage"""
+    def testInstanceTypeQueryOutputProvider(self):
+        """Test InstanceTypeQueryOutputProvider"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_type.py` & `perian-0.2.0/test/test_instance_type_query_input_network.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,44 +10,45 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_type import InstanceTypeQueryType
+from perian.models.instance_type_query_input_network import InstanceTypeQueryInputNetwork
 
-class TestInstanceTypeQueryType(unittest.TestCase):
-    """InstanceTypeQueryType unit test stubs"""
+class TestInstanceTypeQueryInputNetwork(unittest.TestCase):
+    """InstanceTypeQueryInputNetwork unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryType:
-        """Test InstanceTypeQueryType
+    def make_instance(self, include_optional) -> InstanceTypeQueryInputNetwork:
+        """Test InstanceTypeQueryInputNetwork
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryType`
+        # uncomment below to create an instance of `InstanceTypeQueryInputNetwork`
         """
-        model = InstanceTypeQueryType()
+        model = InstanceTypeQueryInputNetwork()
         if include_optional:
-            return InstanceTypeQueryType(
+            return InstanceTypeQueryInputNetwork(
                 operator = None,
                 options = None,
-                type = None
+                inbound_speed = None,
+                outbound_speed = None
             )
         else:
-            return InstanceTypeQueryType(
+            return InstanceTypeQueryInputNetwork(
         )
         """
 
-    def testInstanceTypeQueryType(self):
-        """Test InstanceTypeQueryType"""
+    def testInstanceTypeQueryInputNetwork(self):
+        """Test InstanceTypeQueryInputNetwork"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_query_zone.py` & `perian-0.2.0/test/test_instance_type_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,46 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.instance_type_query_zone import InstanceTypeQueryZone
+from perian.models.instance_type_id import InstanceTypeId
 
-class TestInstanceTypeQueryZone(unittest.TestCase):
-    """InstanceTypeQueryZone unit test stubs"""
+class TestInstanceTypeId(unittest.TestCase):
+    """InstanceTypeId unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> InstanceTypeQueryZone:
-        """Test InstanceTypeQueryZone
+    def make_instance(self, include_optional) -> InstanceTypeId:
+        """Test InstanceTypeId
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `InstanceTypeQueryZone`
+        # uncomment below to create an instance of `InstanceTypeId`
         """
-        model = InstanceTypeQueryZone()
+        model = InstanceTypeId()
         if include_optional:
-            return InstanceTypeQueryZone(
-                operator = None,
-                options = None,
-                id = None,
-                name = None,
-                status = None
+            return InstanceTypeId(
             )
         else:
-            return InstanceTypeQueryZone(
+            return InstanceTypeId(
         )
         """
 
-    def testInstanceTypeQueryZone(self):
-        """Test InstanceTypeQueryZone"""
+    def testInstanceTypeId(self):
+        """Test InstanceTypeId"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_instance_type_view.py` & `perian-0.2.0/test/test_instance_type_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,16 +91,16 @@
                             speed = null, )
                         ], ),
                 accelerator = perian.models.accelerator_data_view.AcceleratorDataView(
                     no = 56, 
                     memory = null, 
                     accelerator_types = [
                         perian.models.accelerator_type_view.AcceleratorTypeView(
+                            display_name = '', 
                             id = '', 
-                            name = null, 
                             vendor = null, 
                             memory = null, )
                         ], ),
                 ram = perian.models.memory.Memory(
                     size = '0.0', 
                     unit = null, 
                     bandwidth = null, 
@@ -115,20 +115,18 @@
                             size = null, 
                             speed = null, )
                         ], ),
                 network = perian.models.network.Network(
                     inbound = null, 
                     outbound = null, ),
                 price = perian.models.price_data.PriceData(
-                    euro_price = '0.0', 
-                    prices = [
-                        perian.models.price.Price(
-                            per_hour = '0.0', 
-                            unit = null, )
-                        ], ),
+                    unit_price = '0.0', 
+                    currency = null, 
+                    granularity = null, 
+                    provider_billing_granularity = null, ),
                 availability = perian.models.availability.Availability(
                     available = True, 
                     source = null, )
             )
         else:
             return InstanceTypeView(
         )
```

### Comparing `perian-0.1.25/test/test_job_api.py` & `perian-0.2.0/test/test_job_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,24 +22,38 @@
 
     def setUp(self) -> None:
         self.api = JobApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_create_job_job_post(self) -> None:
-        """Test case for create_job_job_post
+    def test_cancel_job(self) -> None:
+        """Test case for cancel_job
+
+        Cancel Job
+        """
+        pass
+
+    def test_create_job(self) -> None:
+        """Test case for create_job
 
         Create Job
         """
         pass
 
-    def test_get_job_job_get(self) -> None:
-        """Test case for get_job_job_get
+    def test_get_all_jobs(self) -> None:
+        """Test case for get_all_jobs
+
+        Get All Jobs
+        """
+        pass
+
+    def test_get_job_by_id(self) -> None:
+        """Test case for get_job_by_id
 
-        Get Job
+        Get Job By Id
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_job_status.py` & `perian-0.2.0/test/test_job_status.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_job_view.py` & `perian-0.2.0/test/test_size.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,45 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.job_view import JobView
+from perian.models.size import Size
 
-class TestJobView(unittest.TestCase):
-    """JobView unit test stubs"""
+class TestSize(unittest.TestCase):
+    """Size unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> JobView:
-        """Test JobView
+    def make_instance(self, include_optional) -> Size:
+        """Test Size
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `JobView`
+        # uncomment below to create an instance of `Size`
         """
-        model = JobView()
+        model = Size()
         if include_optional:
-            return JobView(
-                id = '',
-                status = 'Queued',
-                done_at = None,
-                logs = None
+            return Size(
             )
         else:
-            return JobView(
+            return Size(
         )
         """
 
-    def testJobView(self):
-        """Test JobView"""
+    def testSize(self):
+        """Test Size"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_location.py` & `perian-0.2.0/test/test_provider_name.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.location import Location
+from perian.models.provider_name import ProviderName
 
-class TestLocation(unittest.TestCase):
-    """Location unit test stubs"""
+class TestProviderName(unittest.TestCase):
+    """ProviderName unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testLocation(self):
-        """Test Location"""
-        # inst = Location()
+    def testProviderName(self):
+        """Test ProviderName"""
+        # inst = ProviderName()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_logs.py` & `perian-0.2.0/test/test_logs.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_memory.py` & `perian-0.2.0/test/test_memory.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_memory_interface.py` & `perian-0.2.0/test/test_memory_interface.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_memory_query.py` & `perian-0.2.0/test/test_cores.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,44 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.memory_query import MemoryQuery
+from perian.models.cores import Cores
 
-class TestMemoryQuery(unittest.TestCase):
-    """MemoryQuery unit test stubs"""
+class TestCores(unittest.TestCase):
+    """Cores unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> MemoryQuery:
-        """Test MemoryQuery
+    def make_instance(self, include_optional) -> Cores:
+        """Test Cores
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `MemoryQuery`
+        # uncomment below to create an instance of `Cores`
         """
-        model = MemoryQuery()
+        model = Cores()
         if include_optional:
-            return MemoryQuery(
-                operator = None,
-                options = None,
-                size = 1.337
+            return Cores(
             )
         else:
-            return MemoryQuery(
+            return Cores(
         )
         """
 
-    def testMemoryQuery(self):
-        """Test MemoryQuery"""
+    def testCores(self):
+        """Test Cores"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_memory_unit.py` & `perian-0.2.0/test/test_status.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.memory_unit import MemoryUnit
+from perian.models.status import Status
 
-class TestMemoryUnit(unittest.TestCase):
-    """MemoryUnit unit test stubs"""
+class TestStatus(unittest.TestCase):
+    """Status unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMemoryUnit(self):
-        """Test MemoryUnit"""
-        # inst = MemoryUnit()
+    def testStatus(self):
+        """Test Status"""
+        # inst = Status()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_name.py` & `perian-0.2.0/test/test_name.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_name_query.py` & `perian-0.2.0/test/test_name1.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,44 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.name_query import NameQuery
+from perian.models.name1 import Name1
 
-class TestNameQuery(unittest.TestCase):
-    """NameQuery unit test stubs"""
+class TestName1(unittest.TestCase):
+    """Name1 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> NameQuery:
-        """Test NameQuery
+    def make_instance(self, include_optional) -> Name1:
+        """Test Name1
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `NameQuery`
+        # uncomment below to create an instance of `Name1`
         """
-        model = NameQuery()
+        model = Name1()
         if include_optional:
-            return NameQuery(
-                operator = None,
-                options = None,
-                name = ''
+            return Name1(
             )
         else:
-            return NameQuery(
+            return Name1(
         )
         """
 
-    def testNameQuery(self):
-        """Test NameQuery"""
+    def testName1(self):
+        """Test Name1"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_network.py` & `perian-0.2.0/test/test_network.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_network_query.py` & `perian-0.2.0/test/test_network_query_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,45 +10,45 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.network_query import NetworkQuery
+from perian.models.network_query_output import NetworkQueryOutput
 
-class TestNetworkQuery(unittest.TestCase):
-    """NetworkQuery unit test stubs"""
+class TestNetworkQueryOutput(unittest.TestCase):
+    """NetworkQueryOutput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> NetworkQuery:
-        """Test NetworkQuery
+    def make_instance(self, include_optional) -> NetworkQueryOutput:
+        """Test NetworkQueryOutput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `NetworkQuery`
+        # uncomment below to create an instance of `NetworkQueryOutput`
         """
-        model = NetworkQuery()
+        model = NetworkQueryOutput()
         if include_optional:
-            return NetworkQuery(
+            return NetworkQueryOutput(
                 operator = None,
                 options = None,
-                inbound_speed = 1.337,
-                outbound_speed = 1.337
+                inbound_speed = '',
+                outbound_speed = ''
             )
         else:
-            return NetworkQuery(
+            return NetworkQueryOutput(
         )
         """
 
-    def testNetworkQuery(self):
-        """Test NetworkQuery"""
+    def testNetworkQueryOutput(self):
+        """Test NetworkQueryOutput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_no_job_found_error.py` & `perian-0.2.0/test/test_no_job_found_error.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_operator.py` & `perian-0.2.0/test/test_billing_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,24 +10,29 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.operator import Operator
+from perian.api.billing_api import BillingApi
 
-class TestOperator(unittest.TestCase):
-    """Operator unit test stubs"""
 
-    def setUp(self):
+class TestBillingApi(unittest.TestCase):
+    """BillingApi unit test stubs"""
+
+    def setUp(self) -> None:
+        self.api = BillingApi()
+
+    def tearDown(self) -> None:
         pass
 
-    def tearDown(self):
+    def test_generate_bill(self) -> None:
+        """Test case for generate_bill
+
+        Generate Bill
+        """
         pass
 
-    def testOperator(self):
-        """Test Operator"""
-        # inst = Operator()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_organization.py` & `perian-0.2.0/test/test_started_at.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,42 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.organization import Organization
+from perian.models.started_at import StartedAt
 
-class TestOrganization(unittest.TestCase):
-    """Organization unit test stubs"""
+class TestStartedAt(unittest.TestCase):
+    """StartedAt unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Organization:
-        """Test Organization
+    def make_instance(self, include_optional) -> StartedAt:
+        """Test StartedAt
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Organization`
+        # uncomment below to create an instance of `StartedAt`
         """
-        model = Organization()
+        model = StartedAt()
         if include_optional:
-            return Organization(
-                name = ''
+            return StartedAt(
             )
         else:
-            return Organization(
+            return StartedAt(
         )
         """
 
-    def testOrganization(self):
-        """Test Organization"""
+    def testStartedAt(self):
+        """Test StartedAt"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_organization_api.py` & `perian-0.2.0/test/test_order_criterion.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,29 +10,24 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.api.organization_api import OrganizationApi
+from perian.models.order_criterion import OrderCriterion
 
+class TestOrderCriterion(unittest.TestCase):
+    """OrderCriterion unit test stubs"""
 
-class TestOrganizationApi(unittest.TestCase):
-    """OrganizationApi unit test stubs"""
-
-    def setUp(self) -> None:
-        self.api = OrganizationApi()
-
-    def tearDown(self) -> None:
+    def setUp(self):
         pass
 
-    def test_create_organization_organization_post(self) -> None:
-        """Test case for create_organization_organization_post
-
-        Create Organization
-        """
+    def tearDown(self):
         pass
 
+    def testOrderCriterion(self):
+        """Test OrderCriterion"""
+        # inst = OrderCriterion()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_organization_name_error.py` & `perian-0.2.0/test/test_job_already_done_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,45 +10,45 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.organization_name_error import OrganizationNameError
+from perian.models.job_already_done_error import JobAlreadyDoneError
 
-class TestOrganizationNameError(unittest.TestCase):
-    """OrganizationNameError unit test stubs"""
+class TestJobAlreadyDoneError(unittest.TestCase):
+    """JobAlreadyDoneError unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> OrganizationNameError:
-        """Test OrganizationNameError
+    def make_instance(self, include_optional) -> JobAlreadyDoneError:
+        """Test JobAlreadyDoneError
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `OrganizationNameError`
+        # uncomment below to create an instance of `JobAlreadyDoneError`
         """
-        model = OrganizationNameError()
+        model = JobAlreadyDoneError()
         if include_optional:
-            return OrganizationNameError(
+            return JobAlreadyDoneError(
                 status = 'Error',
                 message = 'Operation failed due to a client error',
-                detail = 'The provided organization name is not valid',
+                detail = 'The job you are trying to cancel is already complete.',
                 status_code = 56
             )
         else:
-            return OrganizationNameError(
+            return JobAlreadyDoneError(
         )
         """
 
-    def testOrganizationNameError(self):
-        """Test OrganizationNameError"""
+    def testJobAlreadyDoneError(self):
+        """Test JobAlreadyDoneError"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_organization_name_exists_error.py` & `perian-0.2.0/test/test_validation_error.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,45 +10,51 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.organization_name_exists_error import OrganizationNameExistsError
+from perian.models.validation_error import ValidationError
 
-class TestOrganizationNameExistsError(unittest.TestCase):
-    """OrganizationNameExistsError unit test stubs"""
+class TestValidationError(unittest.TestCase):
+    """ValidationError unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> OrganizationNameExistsError:
-        """Test OrganizationNameExistsError
+    def make_instance(self, include_optional) -> ValidationError:
+        """Test ValidationError
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `OrganizationNameExistsError`
+        # uncomment below to create an instance of `ValidationError`
         """
-        model = OrganizationNameExistsError()
+        model = ValidationError()
         if include_optional:
-            return OrganizationNameExistsError(
-                status = 'Error',
-                message = 'Operation failed due to a client error',
-                detail = 'The provided organization name already exists. Please choose another one',
-                status_code = 56
+            return ValidationError(
+                loc = [
+                    null
+                    ],
+                msg = '',
+                type = ''
             )
         else:
-            return OrganizationNameExistsError(
+            return ValidationError(
+                loc = [
+                    null
+                    ],
+                msg = '',
+                type = '',
         )
         """
 
-    def testOrganizationNameExistsError(self):
-        """Test OrganizationNameExistsError"""
+    def testValidationError(self):
+        """Test ValidationError"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_os_storage_config.py` & `perian-0.2.0/test/test_os_storage_config.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_price.py` & `perian-0.2.0/test/test_errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,43 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.price import Price
+from perian.models.errors import Errors
 
-class TestPrice(unittest.TestCase):
-    """Price unit test stubs"""
+class TestErrors(unittest.TestCase):
+    """Errors unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Price:
-        """Test Price
+    def make_instance(self, include_optional) -> Errors:
+        """Test Errors
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Price`
+        # uncomment below to create an instance of `Errors`
         """
-        model = Price()
+        model = Errors()
         if include_optional:
-            return Price(
-                per_hour = '0.0',
-                unit = 'EUR'
+            return Errors(
             )
         else:
-            return Price(
+            return Errors(
         )
         """
 
-    def testPrice(self):
-        """Test Price"""
+    def testErrors(self):
+        """Test Errors"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_price_data.py` & `perian-0.2.0/test/test_id1.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,47 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.price_data import PriceData
+from perian.models.id1 import Id1
 
-class TestPriceData(unittest.TestCase):
-    """PriceData unit test stubs"""
+class TestId1(unittest.TestCase):
+    """Id1 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> PriceData:
-        """Test PriceData
+    def make_instance(self, include_optional) -> Id1:
+        """Test Id1
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PriceData`
+        # uncomment below to create an instance of `Id1`
         """
-        model = PriceData()
+        model = Id1()
         if include_optional:
-            return PriceData(
-                euro_price = '0.0',
-                prices = [
-                    perian.models.price.Price(
-                        per_hour = '0.0', 
-                        unit = null, )
-                    ]
+            return Id1(
             )
         else:
-            return PriceData(
+            return Id1(
         )
         """
 
-    def testPriceData(self):
-        """Test PriceData"""
+    def testId1(self):
+        """Test Id1"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_price_query.py` & `perian-0.2.0/test/test_price_query_output.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,46 +10,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.price_query import PriceQuery
+from perian.models.price_query_output import PriceQueryOutput
 
-class TestPriceQuery(unittest.TestCase):
-    """PriceQuery unit test stubs"""
+class TestPriceQueryOutput(unittest.TestCase):
+    """PriceQueryOutput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> PriceQuery:
-        """Test PriceQuery
+    def make_instance(self, include_optional) -> PriceQueryOutput:
+        """Test PriceQueryOutput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PriceQuery`
+        # uncomment below to create an instance of `PriceQueryOutput`
         """
-        model = PriceQuery()
+        model = PriceQueryOutput()
         if include_optional:
-            return PriceQuery(
+            return PriceQueryOutput(
                 operator = None,
                 options = None,
-                euro_price = 1.337,
-                unit = '',
-                per_hour = 1.337
+                unit_price = ''
             )
         else:
-            return PriceQuery(
+            return PriceQueryOutput(
         )
         """
 
-    def testPriceQuery(self):
-        """Test PriceQuery"""
+    def testPriceQueryOutput(self):
+        """Test PriceQueryOutput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_provider.py` & `perian-0.2.0/test/test_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                     ],
                 location = 'DE',
                 status = 'Active',
                 capabilities = [
                     'PricingAPI'
                     ],
                 properties = perian.models.provider_properties.ProviderProperties(
-                    compute_billing_period = null, )
+                    compute_billing_granularity = null, )
             )
         else:
             return Provider(
         )
         """
 
     def testProvider(self):
```

### Comparing `perian-0.1.25/test/test_provider_capabilities.py` & `perian-0.2.0/test/test_provider_capabilities.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_provider_name.py` & `perian-0.2.0/test/test_storage_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.provider_name import ProviderName
+from perian.models.storage_type import StorageType
 
-class TestProviderName(unittest.TestCase):
-    """ProviderName unit test stubs"""
+class TestStorageType(unittest.TestCase):
+    """StorageType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testProviderName(self):
-        """Test ProviderName"""
-        # inst = ProviderName()
+    def testStorageType(self):
+        """Test StorageType"""
+        # inst = StorageType()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_provider_query.py` & `perian-0.2.0/test/test_provider_query_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,48 +10,48 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.provider_query import ProviderQuery
+from perian.models.provider_query_input import ProviderQueryInput
 
-class TestProviderQuery(unittest.TestCase):
-    """ProviderQuery unit test stubs"""
+class TestProviderQueryInput(unittest.TestCase):
+    """ProviderQueryInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ProviderQuery:
-        """Test ProviderQuery
+    def make_instance(self, include_optional) -> ProviderQueryInput:
+        """Test ProviderQueryInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ProviderQuery`
+        # uncomment below to create an instance of `ProviderQueryInput`
         """
-        model = ProviderQuery()
+        model = ProviderQueryInput()
         if include_optional:
-            return ProviderQuery(
+            return ProviderQueryInput(
                 operator = None,
                 options = None,
                 id = None,
-                name = '',
-                name_short = '',
-                location = '',
-                status = ''
+                name = None,
+                name_short = None,
+                location = None,
+                status = None
             )
         else:
-            return ProviderQuery(
+            return ProviderQueryInput(
         )
         """
 
-    def testProviderQuery(self):
-        """Test ProviderQuery"""
+    def testProviderQueryInput(self):
+        """Test ProviderQueryInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_provider_specific_name.py` & `perian-0.2.0/test/test_provider_specific_name.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_query_options.py` & `perian-0.2.0/test/test_limit.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,44 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.query_options import QueryOptions
+from perian.models.limit import Limit
 
-class TestQueryOptions(unittest.TestCase):
-    """QueryOptions unit test stubs"""
+class TestLimit(unittest.TestCase):
+    """Limit unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> QueryOptions:
-        """Test QueryOptions
+    def make_instance(self, include_optional) -> Limit:
+        """Test Limit
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `QueryOptions`
+        # uncomment below to create an instance of `Limit`
         """
-        model = QueryOptions()
+        model = Limit()
         if include_optional:
-            return QueryOptions(
-                limit = 56,
-                order = '',
-                lazy_loading = True
+            return Limit(
             )
         else:
-            return QueryOptions(
+            return Limit(
         )
         """
 
-    def testQueryOptions(self):
-        """Test QueryOptions"""
+    def testLimit(self):
+        """Test Limit"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_reference.py` & `perian-0.2.0/test/test_reference_id_query_input.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,41 +10,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.reference import Reference
+from perian.models.reference_id_query_input import ReferenceIdQueryInput
 
-class TestReference(unittest.TestCase):
-    """Reference unit test stubs"""
+class TestReferenceIdQueryInput(unittest.TestCase):
+    """ReferenceIdQueryInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Reference:
-        """Test Reference
+    def make_instance(self, include_optional) -> ReferenceIdQueryInput:
+        """Test ReferenceIdQueryInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Reference`
+        # uncomment below to create an instance of `ReferenceIdQueryInput`
         """
-        model = Reference()
+        model = ReferenceIdQueryInput()
         if include_optional:
-            return Reference(
+            return ReferenceIdQueryInput(
+                operator = None,
+                options = None,
+                id = None
             )
         else:
-            return Reference(
+            return ReferenceIdQueryInput(
         )
         """
 
-    def testReference(self):
-        """Test Reference"""
+    def testReferenceIdQueryInput(self):
+        """Test ReferenceIdQueryInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_reference_id_query.py` & `perian-0.2.0/test/test_reference_id_query_output.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,44 +10,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.reference_id_query import ReferenceIdQuery
+from perian.models.reference_id_query_output import ReferenceIdQueryOutput
 
-class TestReferenceIdQuery(unittest.TestCase):
-    """ReferenceIdQuery unit test stubs"""
+class TestReferenceIdQueryOutput(unittest.TestCase):
+    """ReferenceIdQueryOutput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ReferenceIdQuery:
-        """Test ReferenceIdQuery
+    def make_instance(self, include_optional) -> ReferenceIdQueryOutput:
+        """Test ReferenceIdQueryOutput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ReferenceIdQuery`
+        # uncomment below to create an instance of `ReferenceIdQueryOutput`
         """
-        model = ReferenceIdQuery()
+        model = ReferenceIdQueryOutput()
         if include_optional:
-            return ReferenceIdQuery(
+            return ReferenceIdQueryOutput(
                 operator = None,
                 options = None,
-                id = ''
+                id = None
             )
         else:
-            return ReferenceIdQuery(
+            return ReferenceIdQueryOutput(
         )
         """
 
-    def testReferenceIdQuery(self):
-        """Test ReferenceIdQuery"""
+    def testReferenceIdQueryOutput(self):
+        """Test ReferenceIdQueryOutput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_region.py` & `perian-0.2.0/test/test_region.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_region_query.py` & `perian-0.2.0/test/test_region_query_input.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,48 +10,48 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.region_query import RegionQuery
+from perian.models.region_query_input import RegionQueryInput
 
-class TestRegionQuery(unittest.TestCase):
-    """RegionQuery unit test stubs"""
+class TestRegionQueryInput(unittest.TestCase):
+    """RegionQueryInput unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> RegionQuery:
-        """Test RegionQuery
+    def make_instance(self, include_optional) -> RegionQueryInput:
+        """Test RegionQueryInput
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `RegionQuery`
+        # uncomment below to create an instance of `RegionQueryInput`
         """
-        model = RegionQuery()
+        model = RegionQueryInput()
         if include_optional:
-            return RegionQuery(
+            return RegionQueryInput(
                 operator = None,
                 options = None,
                 id = None,
-                name = '',
-                location = '',
-                sustainable = True,
-                status = ''
+                name = None,
+                location = None,
+                sustainable = None,
+                status = None
             )
         else:
-            return RegionQuery(
+            return RegionQueryInput(
         )
         """
 
-    def testRegionQuery(self):
-        """Test RegionQuery"""
+    def testRegionQueryInput(self):
+        """Test RegionQueryInput"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_response400_create_global_admin_admin_post.py` & `perian-0.2.0/test/test_response400_get_accelerator_type_by_id.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,45 +10,45 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.response400_create_global_admin_admin_post import Response400CreateGlobalAdminAdminPost
+from perian.models.response400_get_accelerator_type_by_id import Response400GetAcceleratorTypeById
 
-class TestResponse400CreateGlobalAdminAdminPost(unittest.TestCase):
-    """Response400CreateGlobalAdminAdminPost unit test stubs"""
+class TestResponse400GetAcceleratorTypeById(unittest.TestCase):
+    """Response400GetAcceleratorTypeById unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Response400CreateGlobalAdminAdminPost:
-        """Test Response400CreateGlobalAdminAdminPost
+    def make_instance(self, include_optional) -> Response400GetAcceleratorTypeById:
+        """Test Response400GetAcceleratorTypeById
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Response400CreateGlobalAdminAdminPost`
+        # uncomment below to create an instance of `Response400GetAcceleratorTypeById`
         """
-        model = Response400CreateGlobalAdminAdminPost()
+        model = Response400GetAcceleratorTypeById()
         if include_optional:
-            return Response400CreateGlobalAdminAdminPost(
+            return Response400GetAcceleratorTypeById(
                 status = None,
                 message = None,
                 detail = None,
                 status_code = None
             )
         else:
-            return Response400CreateGlobalAdminAdminPost(
+            return Response400GetAcceleratorTypeById(
         )
         """
 
-    def testResponse400CreateGlobalAdminAdminPost(self):
-        """Test Response400CreateGlobalAdminAdminPost"""
+    def testResponse400GetAcceleratorTypeById(self):
+        """Test Response400GetAcceleratorTypeById"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_response400_create_user_user_post.py` & `perian-0.2.0/test/test_response400_create_job.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,45 +10,45 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.response400_create_user_user_post import Response400CreateUserUserPost
+from perian.models.response400_create_job import Response400CreateJob
 
-class TestResponse400CreateUserUserPost(unittest.TestCase):
-    """Response400CreateUserUserPost unit test stubs"""
+class TestResponse400CreateJob(unittest.TestCase):
+    """Response400CreateJob unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Response400CreateUserUserPost:
-        """Test Response400CreateUserUserPost
+    def make_instance(self, include_optional) -> Response400CreateJob:
+        """Test Response400CreateJob
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Response400CreateUserUserPost`
+        # uncomment below to create an instance of `Response400CreateJob`
         """
-        model = Response400CreateUserUserPost()
+        model = Response400CreateJob()
         if include_optional:
-            return Response400CreateUserUserPost(
+            return Response400CreateJob(
                 status = None,
                 message = None,
                 detail = None,
                 status_code = None
             )
         else:
-            return Response400CreateUserUserPost(
+            return Response400CreateJob(
         )
         """
 
-    def testResponse400CreateUserUserPost(self):
-        """Test Response400CreateUserUserPost"""
+    def testResponse400CreateJob(self):
+        """Test Response400CreateJob"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_response_get_job_job_get.py` & `perian-0.2.0/test/test_response400_get_job_by_id.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,47 +10,45 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.response_get_job_job_get import ResponseGetJobJobGet
+from perian.models.response400_get_job_by_id import Response400GetJobById
 
-class TestResponseGetJobJobGet(unittest.TestCase):
-    """ResponseGetJobJobGet unit test stubs"""
+class TestResponse400GetJobById(unittest.TestCase):
+    """Response400GetJobById unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ResponseGetJobJobGet:
-        """Test ResponseGetJobJobGet
+    def make_instance(self, include_optional) -> Response400GetJobById:
+        """Test Response400GetJobById
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ResponseGetJobJobGet`
+        # uncomment below to create an instance of `Response400GetJobById`
         """
-        model = ResponseGetJobJobGet()
+        model = Response400GetJobById()
         if include_optional:
-            return ResponseGetJobJobGet(
+            return Response400GetJobById(
                 status = None,
                 message = None,
                 detail = None,
-                status_code = None,
-                jobs = None
+                status_code = None
             )
         else:
-            return ResponseGetJobJobGet(
-                jobs = None,
+            return Response400GetJobById(
         )
         """
 
-    def testResponseGetJobJobGet(self):
-        """Test ResponseGetJobJobGet"""
+    def testResponse400GetJobById(self):
+        """Test Response400GetJobById"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_role_not_valid_error.py` & `perian-0.2.0/test/test_no_parameter_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,45 +10,45 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.role_not_valid_error import RoleNotValidError
+from perian.models.no_parameter_error import NoParameterError
 
-class TestRoleNotValidError(unittest.TestCase):
-    """RoleNotValidError unit test stubs"""
+class TestNoParameterError(unittest.TestCase):
+    """NoParameterError unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> RoleNotValidError:
-        """Test RoleNotValidError
+    def make_instance(self, include_optional) -> NoParameterError:
+        """Test NoParameterError
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `RoleNotValidError`
+        # uncomment below to create an instance of `NoParameterError`
         """
-        model = RoleNotValidError()
+        model = NoParameterError()
         if include_optional:
-            return RoleNotValidError(
+            return NoParameterError(
                 status = 'Error',
                 message = 'Operation failed due to a client error',
-                detail = 'The provided role is not valid',
+                detail = 'Please provide a specific job ID',
                 status_code = 56
             )
         else:
-            return RoleNotValidError(
+            return NoParameterError(
         )
         """
 
-    def testRoleNotValidError(self):
-        """Test RoleNotValidError"""
+    def testNoParameterError(self):
+        """Test NoParameterError"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_setup_token_error.py` & `perian-0.2.0/test/test_offset.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,45 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.setup_token_error import SetupTokenError
+from perian.models.offset import Offset
 
-class TestSetupTokenError(unittest.TestCase):
-    """SetupTokenError unit test stubs"""
+class TestOffset(unittest.TestCase):
+    """Offset unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SetupTokenError:
-        """Test SetupTokenError
+    def make_instance(self, include_optional) -> Offset:
+        """Test Offset
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SetupTokenError`
+        # uncomment below to create an instance of `Offset`
         """
-        model = SetupTokenError()
+        model = Offset()
         if include_optional:
-            return SetupTokenError(
-                status = 'Error',
-                message = 'Operation failed due to a client error',
-                detail = 'The provided setup token is invalid',
-                status_code = 56
+            return Offset(
             )
         else:
-            return SetupTokenError(
+            return Offset(
         )
         """
 
-    def testSetupTokenError(self):
-        """Test SetupTokenError"""
+    def testOffset(self):
+        """Test Offset"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_status.py` & `perian-0.2.0/test/test_storage_included.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.status import Status
+from perian.models.storage_included import StorageIncluded
 
-class TestStatus(unittest.TestCase):
-    """Status unit test stubs"""
+class TestStorageIncluded(unittest.TestCase):
+    """StorageIncluded unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStatus(self):
-        """Test Status"""
-        # inst = Status()
+    def testStorageIncluded(self):
+        """Test StorageIncluded"""
+        # inst = StorageIncluded()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_storage.py` & `perian-0.2.0/test/test_storage.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_storage_data.py` & `perian-0.2.0/test/test_storage_data.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_storage_included.py` & `perian-0.2.0/test/test_outbound_speed.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,24 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.storage_included import StorageIncluded
+from perian.models.outbound_speed import OutboundSpeed
 
-class TestStorageIncluded(unittest.TestCase):
-    """StorageIncluded unit test stubs"""
+class TestOutboundSpeed(unittest.TestCase):
+    """OutboundSpeed unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testStorageIncluded(self):
-        """Test StorageIncluded"""
-        # inst = StorageIncluded()
+    def make_instance(self, include_optional) -> OutboundSpeed:
+        """Test OutboundSpeed
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `OutboundSpeed`
+        """
+        model = OutboundSpeed()
+        if include_optional:
+            return OutboundSpeed(
+            )
+        else:
+            return OutboundSpeed(
+        )
+        """
+
+    def testOutboundSpeed(self):
+        """Test OutboundSpeed"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_storage_query.py` & `perian-0.2.0/test/test_end_time.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,48 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.storage_query import StorageQuery
+from perian.models.end_time import EndTime
 
-class TestStorageQuery(unittest.TestCase):
-    """StorageQuery unit test stubs"""
+class TestEndTime(unittest.TestCase):
+    """EndTime unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> StorageQuery:
-        """Test StorageQuery
+    def make_instance(self, include_optional) -> EndTime:
+        """Test EndTime
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `StorageQuery`
+        # uncomment below to create an instance of `EndTime`
         """
-        model = StorageQuery()
+        model = EndTime()
         if include_optional:
-            return StorageQuery(
-                operator = None,
-                options = None,
-                no = 56,
-                size = 1.337,
-                type = '',
-                speed = 1.337,
-                included = ''
+            return EndTime(
             )
         else:
-            return StorageQuery(
+            return EndTime(
         )
         """
 
-    def testStorageQuery(self):
-        """Test StorageQuery"""
+    def testEndTime(self):
+        """Test EndTime"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_type_query.py` & `perian-0.2.0/test/test_name_short.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,44 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.type_query import TypeQuery
+from perian.models.name_short import NameShort
 
-class TestTypeQuery(unittest.TestCase):
-    """TypeQuery unit test stubs"""
+class TestNameShort(unittest.TestCase):
+    """NameShort unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> TypeQuery:
-        """Test TypeQuery
+    def make_instance(self, include_optional) -> NameShort:
+        """Test NameShort
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `TypeQuery`
+        # uncomment below to create an instance of `NameShort`
         """
-        model = TypeQuery()
+        model = NameShort()
         if include_optional:
-            return TypeQuery(
-                operator = None,
-                options = None,
-                type = ''
+            return NameShort(
             )
         else:
-            return TypeQuery(
+            return NameShort(
         )
         """
 
-    def testTypeQuery(self):
-        """Test TypeQuery"""
+    def testNameShort(self):
+        """Test NameShort"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_user_api.py` & `perian-0.2.0/test/test_billing_granularity.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,29 +10,24 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.api.user_api import UserApi
+from perian.models.billing_granularity import BillingGranularity
 
+class TestBillingGranularity(unittest.TestCase):
+    """BillingGranularity unit test stubs"""
 
-class TestUserApi(unittest.TestCase):
-    """UserApi unit test stubs"""
-
-    def setUp(self) -> None:
-        self.api = UserApi()
-
-    def tearDown(self) -> None:
+    def setUp(self):
         pass
 
-    def test_create_user_user_post(self) -> None:
-        """Test case for create_user_user_post
-
-        Create User
-        """
+    def tearDown(self):
         pass
 
+    def testBillingGranularity(self):
+        """Test BillingGranularity"""
+        # inst = BillingGranularity()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_validation_error.py` & `perian-0.2.0/test/test_price_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,51 +10,45 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.validation_error import ValidationError
+from perian.models.price_data import PriceData
 
-class TestValidationError(unittest.TestCase):
-    """ValidationError unit test stubs"""
+class TestPriceData(unittest.TestCase):
+    """PriceData unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ValidationError:
-        """Test ValidationError
+    def make_instance(self, include_optional) -> PriceData:
+        """Test PriceData
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ValidationError`
+        # uncomment below to create an instance of `PriceData`
         """
-        model = ValidationError()
+        model = PriceData()
         if include_optional:
-            return ValidationError(
-                loc = [
-                    null
-                    ],
-                msg = '',
-                type = ''
+            return PriceData(
+                unit_price = '0.0',
+                currency = 'EUR',
+                granularity = 'PER_SECOND',
+                provider_billing_granularity = 'PER_SECOND'
             )
         else:
-            return ValidationError(
-                loc = [
-                    null
-                    ],
-                msg = '',
-                type = '',
+            return PriceData(
         )
         """
 
-    def testValidationError(self):
-        """Test ValidationError"""
+    def testPriceData(self):
+        """Test PriceData"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_validation_error_loc_inner.py` & `perian-0.2.0/test/test_validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `perian-0.1.25/test/test_vendor.py` & `perian-0.2.0/test/test_available.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,41 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.vendor import Vendor
+from perian.models.available import Available
 
-class TestVendor(unittest.TestCase):
-    """Vendor unit test stubs"""
+class TestAvailable(unittest.TestCase):
+    """Available unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Vendor:
-        """Test Vendor
+    def make_instance(self, include_optional) -> Available:
+        """Test Available
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Vendor`
+        # uncomment below to create an instance of `Available`
         """
-        model = Vendor()
+        model = Available()
         if include_optional:
-            return Vendor(
+            return Available(
             )
         else:
-            return Vendor(
+            return Available(
         )
         """
 
-    def testVendor(self):
-        """Test Vendor"""
+    def testAvailable(self):
+        """Test Available"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_zone.py` & `perian-0.2.0/test/test_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,44 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.zone import Zone
+from perian.models.type import Type
 
-class TestZone(unittest.TestCase):
-    """Zone unit test stubs"""
+class TestType(unittest.TestCase):
+    """Type unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Zone:
-        """Test Zone
+    def make_instance(self, include_optional) -> Type:
+        """Test Type
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Zone`
+        # uncomment below to create an instance of `Type`
         """
-        model = Zone()
+        model = Type()
         if include_optional:
-            return Zone(
-                id = '',
-                name = '',
-                status = 'Active'
+            return Type(
             )
         else:
-            return Zone(
+            return Type(
         )
         """
 
-    def testZone(self):
-        """Test Zone"""
+    def testType(self):
+        """Test Type"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `perian-0.1.25/test/test_zone_query.py` & `perian-0.2.0/test/test_start_time.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,46 +10,41 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from perian.models.zone_query import ZoneQuery
+from perian.models.start_time import StartTime
 
-class TestZoneQuery(unittest.TestCase):
-    """ZoneQuery unit test stubs"""
+class TestStartTime(unittest.TestCase):
+    """StartTime unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ZoneQuery:
-        """Test ZoneQuery
+    def make_instance(self, include_optional) -> StartTime:
+        """Test StartTime
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ZoneQuery`
+        # uncomment below to create an instance of `StartTime`
         """
-        model = ZoneQuery()
+        model = StartTime()
         if include_optional:
-            return ZoneQuery(
-                operator = None,
-                options = None,
-                id = None,
-                name = '',
-                status = ''
+            return StartTime(
             )
         else:
-            return ZoneQuery(
+            return StartTime(
         )
         """
 
-    def testZoneQuery(self):
-        """Test ZoneQuery"""
+    def testStartTime(self):
+        """Test StartTime"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

