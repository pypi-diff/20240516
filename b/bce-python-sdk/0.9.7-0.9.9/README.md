# Comparing `tmp/bce_python_sdk-0.9.7.tar.gz` & `tmp/bce_python_sdk-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bce_python_sdk-0.9.7.tar", last modified: Tue Apr 23 12:37:08 2024, max compression
+gzip compressed data, was "bce_python_sdk-0.9.9.tar", last modified: Mon May 13 04:01:37 2024, max compression
```

## Comparing `bce_python_sdk-0.9.7.tar` & `bce_python_sdk-0.9.9.tar`

### file list

```diff
@@ -1,228 +1,238 @@
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.709573 bce_python_sdk-0.9.7/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      314 2024-04-23 12:37:08.709384 bce_python_sdk-0.9.7/PKG-INFO
--rw-r--r--   0 liuzhongshan   (501) staff       (20)       40 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/README.txt
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.684641 bce_python_sdk-0.9.7/baidubce/
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)      813 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/__init__.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.685120 bce_python_sdk-0.9.7/baidubce/auth/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/auth/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1157 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/auth/bce_credentials.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3211 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/auth/bce_v1_signer.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3428 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/bce_base_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3055 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/bce_client_configuration.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1655 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/bce_response.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3467 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/compat.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1691 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/exception.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.685909 bce_python_sdk-0.9.7/baidubce/http/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     9877 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/bce_http_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     2930 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/handler.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      722 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/http_content_types.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     2659 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/http_headers.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      782 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/http/http_methods.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1151 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/protocol.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      835 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/region.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.686144 bce_python_sdk-0.9.7/baidubce/retry/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/retry/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     4926 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/retry/retry_policy.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.686308 bce_python_sdk-0.9.7/baidubce/services/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/__init__.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.686800 bce_python_sdk-0.9.7/baidubce/services/autoscaling/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/autoscaling/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    22179 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3332 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_handler.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     8501 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.687231 bce_python_sdk-0.9.7/baidubce/services/bbc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bbc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    37306 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bbc/bbc_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1790 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bbc/bbc_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.688029 bce_python_sdk-0.9.7/baidubce/services/bcc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)   237248 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcc/bcc_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5919 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcc/bcc_model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      948 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcc/fpga_card_type.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1054 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcc/gpu_card_type.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.690736 bce_python_sdk-0.9.7/baidubce/services/bcm/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcm/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)   209237 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3315 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_handler.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    22095 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.692081 bce_python_sdk-0.9.7/baidubce/services/bes/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bes/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    22810 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bes/bes_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1784 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bes/bes_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.692730 bce_python_sdk-0.9.7/baidubce/services/blb/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/blb/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)   128513 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/blb/app_blb_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    98620 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/blb/blb_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    17046 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/blb/user_service_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.692938 bce_python_sdk-0.9.7/baidubce/services/bmr/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bmr/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    20565 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bmr/bmr_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.693522 bce_python_sdk-0.9.7/baidubce/services/bos/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      813 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bos/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)   100010 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bos/bos_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1832 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bos/bos_handler.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      723 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bos/canned_acl.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      729 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bos/storage_class.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.693989 bce_python_sdk-0.9.7/baidubce/services/bts/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      749 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bts/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    21916 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bts/bts_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    11520 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bts/model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1521 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/bts/util.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.694315 bce_python_sdk-0.9.7/baidubce/services/cdn/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cdn/__init__.py
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)    59017 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cdn/cdn_client.py
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     1252 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cdn/cdn_stats_param.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.694658 bce_python_sdk-0.9.7/baidubce/services/cert/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cert/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     4659 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cert/cert_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1622 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cert/cert_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.695088 bce_python_sdk-0.9.7/baidubce/services/cfc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cfc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    42843 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cfc/cfc_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3037 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cfc/cfc_handler.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5722 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/cfc/models.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.695564 bce_python_sdk-0.9.7/baidubce/services/csn/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/csn/__init__.py
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     7609 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/csn/csn_api.py
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)    35434 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/csn/csn_client.py
--rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     1308 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/csn/csn_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.695754 bce_python_sdk-0.9.7/baidubce/services/ddc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/ddc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     6834 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/ddc/ddc_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.695980 bce_python_sdk-0.9.7/baidubce/services/dns/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dns/__init__.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.696241 bce_python_sdk-0.9.7/baidubce/services/dns/api/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dns/api/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     4350 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dns/api/dns_api.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    15953 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dns/dns_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.696469 bce_python_sdk-0.9.7/baidubce/services/dumap/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dumap/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3955 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/dumap/dumap_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.697394 bce_python_sdk-0.9.7/baidubce/services/eip/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    13055 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/eip_bp_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    23965 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/eip_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    18955 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/eip_group_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1914 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/eip_group_model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     8798 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/eip_tp_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1769 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eip/model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.697794 bce_python_sdk-0.9.7/baidubce/services/endpoint/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/endpoint/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    12789 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/endpoint/endpoint_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1650 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/endpoint/model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.698148 bce_python_sdk-0.9.7/baidubce/services/eni/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eni/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    27213 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eni/eni_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1165 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/eni/eni_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.698472 bce_python_sdk-0.9.7/baidubce/services/et/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/et/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    31622 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/et/et_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      975 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/et/model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.698589 bce_python_sdk-0.9.7/baidubce/services/havip/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    13846 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/havip/havip_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.698874 bce_python_sdk-0.9.7/baidubce/services/iam/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      668 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/iam/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    24555 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/iam/iam_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.699097 bce_python_sdk-0.9.7/baidubce/services/infinite/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      655 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/infinite/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     8898 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/infinite/infinite_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.699435 bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    19194 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/ipv6gateway_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1698 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/ipv6gateway_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.700065 bce_python_sdk-0.9.7/baidubce/services/kms/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      794 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/keyspec_class.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    17789 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/kms_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      640 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/origin_class.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      633 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/protectedby_class.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      655 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/kms/publickeyencoding_class.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.700399 bce_python_sdk-0.9.7/baidubce/services/lbdc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/lbdc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    10679 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/lbdc/lbdc_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1625 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/lbdc/model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.700624 bce_python_sdk-0.9.7/baidubce/services/localdns/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/localdns/__init__.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.700893 bce_python_sdk-0.9.7/baidubce/services/localdns/api/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/localdns/api/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3294 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/localdns/api/ld_api.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    10461 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/localdns/ld_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.701255 bce_python_sdk-0.9.7/baidubce/services/media/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/media/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    25881 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/media/media_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     2460 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/media/media_handler.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.701494 bce_python_sdk-0.9.7/baidubce/services/mms/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      610 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/mms/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    19332 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/mms/mms_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.701757 bce_python_sdk-0.9.7/baidubce/services/mvs/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      610 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/mvs/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5802 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/mvs/mvs_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.702182 bce_python_sdk-0.9.7/baidubce/services/oos/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/oos/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    10214 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/oos/oos_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     2869 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/oos/oos_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.704175 bce_python_sdk-0.9.7/baidubce/services/rds/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      707 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    13869 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_backup_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5695 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_database_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    17005 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_hot_active_instance_group_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     8479 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_http.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    33785 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_instance_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     9197 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_log_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    17318 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_parameter_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    17078 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_readonly_group_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     4115 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_recycler_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5190 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_security_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3455 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_task_manager.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    10387 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/rds/rds_users_manager.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.704624 bce_python_sdk-0.9.7/baidubce/services/route/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/route/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    13869 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/route/route_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      280 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/route/route_model.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.705040 bce_python_sdk-0.9.7/baidubce/services/scs/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      707 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/scs/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     8355 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/scs/model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    27357 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/scs/scs_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.705445 bce_python_sdk-0.9.7/baidubce/services/sms/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      676 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/sms/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     6592 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/sms/model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    31118 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/sms/sms_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.705721 bce_python_sdk-0.9.7/baidubce/services/sts/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      669 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/sts/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3687 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/sts/sts_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.705957 bce_python_sdk-0.9.7/baidubce/services/subnet/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/subnet/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    14627 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/subnet/subnet_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.706538 bce_python_sdk-0.9.7/baidubce/services/tsdb/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/tsdb/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     4845 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_admin_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     9337 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1744 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_handler.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.706742 bce_python_sdk-0.9.7/baidubce/services/vca/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vca/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     5273 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vca/vca_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.707021 bce_python_sdk-0.9.7/baidubce/services/vcr/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vcr/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    13004 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vcr/vcr_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.707935 bce_python_sdk-0.9.7/baidubce/services/vpc/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    11902 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/acl_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    36440 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/nat_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1688 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/nat_model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    20077 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/peerconn_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     1686 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/peerconn_model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     9875 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpc/vpc_client.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.708407 bce_python_sdk-0.9.7/baidubce/services/vpn/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpn/__init__.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    28554 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpn/vpn_client.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3364 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/services/vpn/vpn_model.py
--rw-r--r--   0 liuzhongshan   (501) staff       (20)    20194 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/baidubce/utils.py
-drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-04-23 12:37:08.709154 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/
--rw-r--r--   0 liuzhongshan   (501) staff       (20)      314 2024-04-23 12:37:08.000000 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     6313 2024-04-23 12:37:08.000000 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        1 2024-04-23 12:37:08.000000 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 liuzhongshan   (501) staff       (20)       45 2024-04-23 12:37:08.000000 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/requires.txt
--rw-r--r--   0 liuzhongshan   (501) staff       (20)        9 2024-04-23 12:37:08.000000 bce_python_sdk-0.9.7/bce_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 liuzhongshan   (501) staff       (20)       38 2024-04-23 12:37:08.709612 bce_python_sdk-0.9.7/setup.cfg
--rw-r--r--   0 liuzhongshan   (501) staff       (20)     3255 2024-04-23 08:43:06.000000 bce_python_sdk-0.9.7/setup.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.777666 bce_python_sdk-0.9.9/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      314 2024-05-13 04:01:37.777453 bce_python_sdk-0.9.9/PKG-INFO
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)       40 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/README.txt
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.755370 bce_python_sdk-0.9.9/baidubce/
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)      813 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/__init__.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.755928 bce_python_sdk-0.9.9/baidubce/auth/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/auth/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1157 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/auth/bce_credentials.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3211 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/auth/bce_v1_signer.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3428 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/bce_base_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3055 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/bce_client_configuration.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1655 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/bce_response.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3467 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/compat.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1691 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/exception.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.756705 bce_python_sdk-0.9.9/baidubce/http/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/http/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     9877 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/http/bce_http_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     2930 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/http/handler.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      722 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/http/http_content_types.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     2659 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/http/http_headers.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      782 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/http/http_methods.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1151 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/protocol.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      835 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/region.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.756959 bce_python_sdk-0.9.9/baidubce/retry/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/retry/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     4926 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/retry/retry_policy.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.757129 bce_python_sdk-0.9.9/baidubce/services/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/__init__.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.757630 bce_python_sdk-0.9.9/baidubce/services/autoscaling/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/autoscaling/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    22179 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/autoscaling/as_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3332 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/autoscaling/as_handler.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     8501 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/autoscaling/as_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.758093 bce_python_sdk-0.9.9/baidubce/services/bbc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bbc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    37306 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bbc/bbc_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1790 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bbc/bbc_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.759019 bce_python_sdk-0.9.9/baidubce/services/bcc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bcc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)   239053 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bcc/bcc_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5919 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bcc/bcc_model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      948 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bcc/fpga_card_type.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1054 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bcc/gpu_card_type.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.759523 bce_python_sdk-0.9.9/baidubce/services/bcm/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bcm/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)   211439 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bcm/bcm_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3315 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bcm/bcm_handler.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    22095 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bcm/bcm_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.759826 bce_python_sdk-0.9.9/baidubce/services/bes/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bes/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    22810 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bes/bes_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1784 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bes/bes_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.760320 bce_python_sdk-0.9.9/baidubce/services/blb/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/blb/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)   128513 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/blb/app_blb_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    98620 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/blb/blb_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    17046 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/blb/user_service_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.760520 bce_python_sdk-0.9.9/baidubce/services/bmr/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bmr/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    20565 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bmr/bmr_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.761092 bce_python_sdk-0.9.9/baidubce/services/bos/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      813 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bos/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)   100010 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bos/bos_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1832 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bos/bos_handler.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      723 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bos/canned_acl.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      729 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bos/storage_class.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.761772 bce_python_sdk-0.9.9/baidubce/services/bts/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      749 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bts/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    21916 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bts/bts_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    11520 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bts/model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1521 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/bts/util.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.762147 bce_python_sdk-0.9.9/baidubce/services/cdn/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/cdn/__init__.py
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)    59017 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/cdn/cdn_client.py
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     1252 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/cdn/cdn_stats_param.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.762486 bce_python_sdk-0.9.9/baidubce/services/cert/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/cert/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     4659 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/cert/cert_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1622 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/cert/cert_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.762924 bce_python_sdk-0.9.9/baidubce/services/cfc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/cfc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    42843 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/cfc/cfc_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3037 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/cfc/cfc_handler.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5722 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/cfc/models.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.763424 bce_python_sdk-0.9.9/baidubce/services/csn/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/csn/__init__.py
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     7609 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/csn/csn_api.py
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)    35434 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/csn/csn_client.py
+-rwxr-xr-x   0 liuzhongshan   (501) staff       (20)     1308 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/csn/csn_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.763628 bce_python_sdk-0.9.9/baidubce/services/ddc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/ddc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     6834 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/ddc/ddc_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.763871 bce_python_sdk-0.9.9/baidubce/services/dns/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/dns/__init__.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.764113 bce_python_sdk-0.9.9/baidubce/services/dns/api/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/dns/api/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     4350 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/dns/api/dns_api.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    15953 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/dns/dns_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.764323 bce_python_sdk-0.9.9/baidubce/services/dumap/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/dumap/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3955 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/dumap/dumap_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.765152 bce_python_sdk-0.9.9/baidubce/services/eip/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/eip/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13055 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/eip/eip_bp_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    23965 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/eip/eip_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    18955 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/eip/eip_group_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1914 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/eip/eip_group_model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     8798 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/eip/eip_tp_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1769 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/eip/model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.765506 bce_python_sdk-0.9.9/baidubce/services/endpoint/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/endpoint/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    12789 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/endpoint/endpoint_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1650 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/endpoint/model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.765822 bce_python_sdk-0.9.9/baidubce/services/eni/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/eni/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    27213 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/eni/eni_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1165 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/eni/eni_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.766167 bce_python_sdk-0.9.9/baidubce/services/esg/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/esg/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13202 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/esg/esg_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3646 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/esg/esg_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.766479 bce_python_sdk-0.9.9/baidubce/services/et/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/et/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    31622 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/et/et_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      975 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/et/model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.766712 bce_python_sdk-0.9.9/baidubce/services/etGateway/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/etGateway/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    14970 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/etGateway/et_gateway_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.766857 bce_python_sdk-0.9.9/baidubce/services/havip/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13846 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/havip/havip_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.767117 bce_python_sdk-0.9.9/baidubce/services/iam/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      668 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/iam/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    24555 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/iam/iam_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.767373 bce_python_sdk-0.9.9/baidubce/services/infinite/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      655 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/infinite/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     8898 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/infinite/infinite_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.767730 bce_python_sdk-0.9.9/baidubce/services/ipv6gateway/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/ipv6gateway/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    19194 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/ipv6gateway/ipv6gateway_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1698 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/ipv6gateway/ipv6gateway_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.768397 bce_python_sdk-0.9.9/baidubce/services/kms/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/kms/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      794 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/kms/keyspec_class.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    17789 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/kms/kms_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      640 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/kms/origin_class.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      633 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/kms/protectedby_class.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      655 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/kms/publickeyencoding_class.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.768752 bce_python_sdk-0.9.9/baidubce/services/lbdc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/lbdc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    10679 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/lbdc/lbdc_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1625 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/lbdc/model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.768981 bce_python_sdk-0.9.9/baidubce/services/localdns/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/localdns/__init__.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.769214 bce_python_sdk-0.9.9/baidubce/services/localdns/api/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/localdns/api/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3294 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/localdns/api/ld_api.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    10461 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/localdns/ld_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.769545 bce_python_sdk-0.9.9/baidubce/services/media/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/media/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    25881 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/media/media_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     2460 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/media/media_handler.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.769778 bce_python_sdk-0.9.9/baidubce/services/mms/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      610 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/mms/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    19332 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/mms/mms_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.770017 bce_python_sdk-0.9.9/baidubce/services/mvs/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      610 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/mvs/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5802 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/mvs/mvs_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.770410 bce_python_sdk-0.9.9/baidubce/services/oos/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/oos/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    10214 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/oos/oos_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     2869 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/oos/oos_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.770619 bce_python_sdk-0.9.9/baidubce/services/probe/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/probe/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    10999 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/probe/probe_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.772477 bce_python_sdk-0.9.9/baidubce/services/rds/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      707 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13869 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_backup_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5695 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_database_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    17005 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_hot_active_instance_group_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     8479 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_http.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    33785 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_instance_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     9197 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_log_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    17318 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_parameter_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    17078 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_readonly_group_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     4115 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_recycler_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5190 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_security_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3455 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_task_manager.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    10387 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/rds/rds_users_manager.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.772889 bce_python_sdk-0.9.9/baidubce/services/route/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/route/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13869 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/route/route_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      280 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/route/route_model.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.773263 bce_python_sdk-0.9.9/baidubce/services/scs/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      707 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/scs/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     8355 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/scs/model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    27357 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/scs/scs_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.773621 bce_python_sdk-0.9.9/baidubce/services/sms/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      676 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/sms/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     6592 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/sms/model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    31118 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/sms/sms_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.773878 bce_python_sdk-0.9.9/baidubce/services/sts/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      669 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/sts/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3687 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/sts/sts_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.774089 bce_python_sdk-0.9.9/baidubce/services/subnet/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/subnet/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    14627 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/subnet/subnet_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.774625 bce_python_sdk-0.9.9/baidubce/services/tsdb/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/tsdb/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     4845 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/tsdb/tsdb_admin_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     9337 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/tsdb/tsdb_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1744 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/tsdb/tsdb_handler.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.774806 bce_python_sdk-0.9.9/baidubce/services/vca/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vca/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     5273 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vca/vca_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.775062 bce_python_sdk-0.9.9/baidubce/services/vcr/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vcr/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    13004 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vcr/vcr_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.775983 bce_python_sdk-0.9.9/baidubce/services/vpc/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vpc/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    11902 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vpc/acl_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    36440 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vpc/nat_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1688 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vpc/nat_model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    20077 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vpc/peerconn_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     1686 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vpc/peerconn_model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     9875 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vpc/vpc_client.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.776381 bce_python_sdk-0.9.9/baidubce/services/vpn/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        0 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vpn/__init__.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    28554 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vpn/vpn_client.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3364 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/services/vpn/vpn_model.py
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)    20194 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/baidubce/utils.py
+drwxr-xr-x   0 liuzhongshan   (501) staff       (20)        0 2024-05-13 04:01:37.777157 bce_python_sdk-0.9.9/bce_python_sdk.egg-info/
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)      314 2024-05-13 04:01:37.000000 bce_python_sdk-0.9.9/bce_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     6583 2024-05-13 04:01:37.000000 bce_python_sdk-0.9.9/bce_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        1 2024-05-13 04:01:37.000000 bce_python_sdk-0.9.9/bce_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)       45 2024-05-13 04:01:37.000000 bce_python_sdk-0.9.9/bce_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)        9 2024-05-13 04:01:37.000000 bce_python_sdk-0.9.9/bce_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)       38 2024-05-13 04:01:37.777705 bce_python_sdk-0.9.9/setup.cfg
+-rw-r--r--   0 liuzhongshan   (501) staff       (20)     3380 2024-05-11 13:28:06.000000 bce_python_sdk-0.9.9/setup.py
```

### Comparing `bce_python_sdk-0.9.7/baidubce/__init__.py` & `bce_python_sdk-0.9.9/baidubce/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 This module defines some common string constants.
 """
 from builtins import str
 from builtins import bytes
 from . import protocol
 
 
-SDK_VERSION = b'0.9.07'
+SDK_VERSION = b'0.9.09'
 DEFAULT_SERVICE_DOMAIN = b'bcebos.com'
 URL_PREFIX = b'/v1'
 DEFAULT_ENCODING = 'UTF-8'
```

### Comparing `bce_python_sdk-0.9.7/baidubce/auth/bce_credentials.py` & `bce_python_sdk-0.9.9/baidubce/auth/bce_credentials.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/auth/bce_v1_signer.py` & `bce_python_sdk-0.9.9/baidubce/auth/bce_v1_signer.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/bce_base_client.py` & `bce_python_sdk-0.9.9/baidubce/bce_base_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/bce_client_configuration.py` & `bce_python_sdk-0.9.9/baidubce/bce_client_configuration.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/bce_response.py` & `bce_python_sdk-0.9.9/baidubce/bce_response.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/compat.py` & `bce_python_sdk-0.9.9/baidubce/compat.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/exception.py` & `bce_python_sdk-0.9.9/baidubce/exception.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/http/bce_http_client.py` & `bce_python_sdk-0.9.9/baidubce/http/bce_http_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/http/handler.py` & `bce_python_sdk-0.9.9/baidubce/http/handler.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/http/http_content_types.py` & `bce_python_sdk-0.9.9/baidubce/http/http_content_types.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/http/http_headers.py` & `bce_python_sdk-0.9.9/baidubce/http/http_headers.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/http/http_methods.py` & `bce_python_sdk-0.9.9/baidubce/http/http_methods.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/protocol.py` & `bce_python_sdk-0.9.9/baidubce/protocol.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/region.py` & `bce_python_sdk-0.9.9/baidubce/region.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/retry/retry_policy.py` & `bce_python_sdk-0.9.9/baidubce/retry/retry_policy.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_client.py` & `bce_python_sdk-0.9.9/baidubce/services/autoscaling/as_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_handler.py` & `bce_python_sdk-0.9.9/baidubce/services/autoscaling/as_handler.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/autoscaling/as_model.py` & `bce_python_sdk-0.9.9/baidubce/services/autoscaling/as_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bbc/bbc_client.py` & `bce_python_sdk-0.9.9/baidubce/services/bbc/bbc_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bbc/bbc_model.py` & `bce_python_sdk-0.9.9/baidubce/services/bbc/bbc_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bcc/bcc_client.py` & `bce_python_sdk-0.9.9/baidubce/services/bcc/bcc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4384,14 +4384,60 @@
         for instance_id in instance_id_list:
             list_of_item.append({'instanceId': instance_id})
         body = {
             "instanceIds": list_of_item
         }
         return self._send_request(http_methods.POST, path, body=json.dumps(body), params=params, config=config)
 
+    @required(instance_ids=(list))
+    def batch_refund_resources(self, instance_ids, related_release_flag=None,
+                               delete_cds_snapshot_flag=None, delete_related_enis_flag=None,
+                               client_token=None, config=None):
+        """
+        Releasing the instance owned by the user.
+        Only the Prepaid instance and the instance has not expired can be released.
+        After releasing the instance, all of the data will be deleted.
+
+        :param instance_ids:
+             The id list of instances.
+        :type instance_ids: list of string
+
+
+        :param related_release_flag:
+            Release or not related resources.
+        :type related_release_flag: bool
+
+        :param delete_cds_snapshot_flag:
+            Delete or not cds snapshot.
+        :type delete_cds_snapshot_flag: bool
+
+        :param delete_related_enis_flag:
+            Delete or not related enis.
+        :type delete_related_enis_flag: bool
+
+        :return:
+        :rtype baidubce.bce_response.BceResponse
+        """
+        params = {}
+        if client_token is None:
+            params['clientToken'] = generate_client_token()
+        else:
+            params['clientToken'] = client_token
+        path = b'/instance/batchRefundResource'
+        body = {
+            "instanceIds": instance_ids
+        }
+        if related_release_flag is not None:
+            body['relatedReleaseFlag'] = related_release_flag
+        if delete_cds_snapshot_flag is not None:
+            body['deleteCdsSnapshotFlag'] = delete_cds_snapshot_flag
+        if delete_related_enis_flag is not None:
+            body['deleteRelatedEnisFlag'] = delete_related_enis_flag
+        return self._send_request(http_methods.POST, path, body=json.dumps(body), params=params, config=config)
+
     @required(instance_type=str, cpu_count=int, memory_cap_in_gb=int)  # ***Unicode***
     def get_bid_instance_price(self, instance_type, cpu_count, memory_cap_in_gb,
                                root_disk_size_in_gb=None, root_disk_storage_type=None, create_cds_list=None,
                                purchase_count=1, name=None, admin_pass=None, key_pair_id=None, asp_id=None,
                                image_id=None, bid_model=None, bid_price=None, network_cap_in_mbps=None,
                                relation_tag=None, tags=None, security_group_id=None, subnet_id=None,
                                zone_name=None, internet_charge_type=None, client_token=None, config=None):
```

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bcc/bcc_model.py` & `bce_python_sdk-0.9.9/baidubce/services/bcc/bcc_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bcc/fpga_card_type.py` & `bce_python_sdk-0.9.9/baidubce/services/bcc/fpga_card_type.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bcc/gpu_card_type.py` & `bce_python_sdk-0.9.9/baidubce/services/bcc/gpu_card_type.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_client.py` & `bce_python_sdk-0.9.9/baidubce/services/bcm/bcm_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5868,7 +5868,83 @@
         if type is not None:
             body["type"] = type
 
         path = b'/data/metricAllData/batch'
         return self._send_csm_request(http_methods.POST, path, version=b'/v2', body=json.dumps(body))
 
 
+    def get_metric_dimension_top(self, user_id, scope, region, dimensions, metric_name, statistics, labels,
+                                 start_time, end_time, order="top", topNum=10):
+
+        """
+        :param user_id: user_id
+        :type string
+
+        :param scope: scope
+        :type string
+
+        :param region: region
+        :type string
+
+        :param dimensions: dimensions
+        :type map
+
+        :param metric_name: metric_name
+        :type string
+
+        :param statistics: statistics
+        :type string
+
+        :param labels: labels
+        :type set
+
+        :param start_time: start_time
+        :type string
+
+        :param end_time: end_time
+        :type string
+
+        :param order: order default top
+        :type string
+
+        :param topNum: topNum default 10
+        :type int
+
+        :return:
+        """
+        if len(user_id) <= 0:
+            raise ValueError("user_id should not be null")
+        if len(scope) <= 0:
+            raise ValueError("scope should not be null")
+        if len(region) <= 0:
+            raise ValueError("region should not be null")
+        if len(metric_name) <= 0:
+            raise ValueError("metric_name should not be null")
+        if len(dimensions) <= 0:
+            raise ValueError("dimensions should not be null")
+        if len(labels) <= 0:
+            raise ValueError("lables should not be null")
+        if len(statistics) <= 0:
+            raise ValueError("statistics should not be null")
+        if len(start_time) <= 0:
+            raise ValueError("start_time should not be null")
+        if len(end_time) <= 0:
+            raise ValueError("end_time should not be null")
+
+        body = {
+            "userId": user_id,
+            "scope": scope,
+            "region": region,
+            "startTime": start_time,
+            "endTime": end_time,
+            "metricName": metric_name,
+            "dimensions": dimensions,
+            "statistics": statistics,
+            "labels": labels,
+            "order": order,
+            "topNum": topNum,
+        }
+
+        path = b'/dimensions/top'
+        return self._send_csm_request(http_methods.POST, path, version=b'/v2', body=json.dumps(body))
+
+
```

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_handler.py` & `bce_python_sdk-0.9.9/baidubce/services/bcm/bcm_handler.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bcm/bcm_model.py` & `bce_python_sdk-0.9.9/baidubce/services/bcm/bcm_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bes/bes_client.py` & `bce_python_sdk-0.9.9/baidubce/services/bes/bes_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bes/bes_model.py` & `bce_python_sdk-0.9.9/baidubce/services/bes/bes_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/blb/app_blb_client.py` & `bce_python_sdk-0.9.9/baidubce/services/blb/app_blb_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/blb/blb_client.py` & `bce_python_sdk-0.9.9/baidubce/services/blb/blb_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/blb/user_service_client.py` & `bce_python_sdk-0.9.9/baidubce/services/blb/user_service_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bmr/bmr_client.py` & `bce_python_sdk-0.9.9/baidubce/services/bmr/bmr_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bos/__init__.py` & `bce_python_sdk-0.9.9/baidubce/services/bos/__init__.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bos/bos_client.py` & `bce_python_sdk-0.9.9/baidubce/services/bos/bos_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bos/bos_handler.py` & `bce_python_sdk-0.9.9/baidubce/services/bos/bos_handler.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bos/canned_acl.py` & `bce_python_sdk-0.9.9/baidubce/services/bos/canned_acl.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bos/storage_class.py` & `bce_python_sdk-0.9.9/baidubce/services/bos/storage_class.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bts/__init__.py` & `bce_python_sdk-0.9.9/baidubce/services/bts/__init__.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bts/bts_client.py` & `bce_python_sdk-0.9.9/baidubce/services/bts/bts_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bts/model.py` & `bce_python_sdk-0.9.9/baidubce/services/bts/model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/bts/util.py` & `bce_python_sdk-0.9.9/baidubce/services/bts/util.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/cdn/cdn_client.py` & `bce_python_sdk-0.9.9/baidubce/services/cdn/cdn_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/cdn/cdn_stats_param.py` & `bce_python_sdk-0.9.9/baidubce/services/cdn/cdn_stats_param.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/cert/cert_client.py` & `bce_python_sdk-0.9.9/baidubce/services/cert/cert_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/cert/cert_model.py` & `bce_python_sdk-0.9.9/baidubce/services/cert/cert_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/cfc/cfc_client.py` & `bce_python_sdk-0.9.9/baidubce/services/cfc/cfc_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/cfc/cfc_handler.py` & `bce_python_sdk-0.9.9/baidubce/services/cfc/cfc_handler.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/cfc/models.py` & `bce_python_sdk-0.9.9/baidubce/services/cfc/models.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/csn/csn_api.py` & `bce_python_sdk-0.9.9/baidubce/services/csn/csn_api.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/csn/csn_client.py` & `bce_python_sdk-0.9.9/baidubce/services/csn/csn_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/csn/csn_model.py` & `bce_python_sdk-0.9.9/baidubce/services/csn/csn_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/ddc/ddc_client.py` & `bce_python_sdk-0.9.9/baidubce/services/ddc/ddc_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/dns/api/dns_api.py` & `bce_python_sdk-0.9.9/baidubce/services/dns/api/dns_api.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/dns/dns_client.py` & `bce_python_sdk-0.9.9/baidubce/services/dns/dns_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/dumap/dumap_client.py` & `bce_python_sdk-0.9.9/baidubce/services/dumap/dumap_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/eip/eip_bp_client.py` & `bce_python_sdk-0.9.9/baidubce/services/eip/eip_bp_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/eip/eip_client.py` & `bce_python_sdk-0.9.9/baidubce/services/eip/eip_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/eip/eip_group_client.py` & `bce_python_sdk-0.9.9/baidubce/services/eip/eip_group_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/eip/eip_group_model.py` & `bce_python_sdk-0.9.9/baidubce/services/eip/eip_group_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/eip/eip_tp_client.py` & `bce_python_sdk-0.9.9/baidubce/services/eip/eip_tp_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/eip/model.py` & `bce_python_sdk-0.9.9/baidubce/services/eip/model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/endpoint/endpoint_client.py` & `bce_python_sdk-0.9.9/baidubce/services/endpoint/endpoint_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/endpoint/model.py` & `bce_python_sdk-0.9.9/baidubce/services/endpoint/model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/eni/eni_client.py` & `bce_python_sdk-0.9.9/baidubce/services/eni/eni_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/eni/eni_model.py` & `bce_python_sdk-0.9.9/baidubce/services/eni/eni_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/et/et_client.py` & `bce_python_sdk-0.9.9/baidubce/services/et/et_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/et/model.py` & `bce_python_sdk-0.9.9/baidubce/services/et/model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/havip/havip_client.py` & `bce_python_sdk-0.9.9/baidubce/services/havip/havip_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/iam/__init__.py` & `bce_python_sdk-0.9.9/baidubce/services/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/iam/iam_client.py` & `bce_python_sdk-0.9.9/baidubce/services/iam/iam_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/infinite/__init__.py` & `bce_python_sdk-0.9.9/baidubce/services/infinite/__init__.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/infinite/infinite_client.py` & `bce_python_sdk-0.9.9/baidubce/services/infinite/infinite_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/ipv6gateway_client.py` & `bce_python_sdk-0.9.9/baidubce/services/ipv6gateway/ipv6gateway_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/ipv6gateway/ipv6gateway_model.py` & `bce_python_sdk-0.9.9/baidubce/services/ipv6gateway/ipv6gateway_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/kms/keyspec_class.py` & `bce_python_sdk-0.9.9/baidubce/services/kms/keyspec_class.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/kms/kms_client.py` & `bce_python_sdk-0.9.9/baidubce/services/kms/kms_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/kms/origin_class.py` & `bce_python_sdk-0.9.9/baidubce/services/kms/origin_class.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/kms/protectedby_class.py` & `bce_python_sdk-0.9.9/baidubce/services/kms/protectedby_class.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/kms/publickeyencoding_class.py` & `bce_python_sdk-0.9.9/baidubce/services/kms/publickeyencoding_class.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/lbdc/lbdc_client.py` & `bce_python_sdk-0.9.9/baidubce/services/lbdc/lbdc_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/lbdc/model.py` & `bce_python_sdk-0.9.9/baidubce/services/lbdc/model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/localdns/api/ld_api.py` & `bce_python_sdk-0.9.9/baidubce/services/localdns/api/ld_api.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/localdns/ld_client.py` & `bce_python_sdk-0.9.9/baidubce/services/localdns/ld_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/media/media_client.py` & `bce_python_sdk-0.9.9/baidubce/services/media/media_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/media/media_handler.py` & `bce_python_sdk-0.9.9/baidubce/services/media/media_handler.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/mms/__init__.py` & `bce_python_sdk-0.9.9/baidubce/services/mms/__init__.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/mms/mms_client.py` & `bce_python_sdk-0.9.9/baidubce/services/mms/mms_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/mvs/__init__.py` & `bce_python_sdk-0.9.9/baidubce/services/mvs/__init__.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/mvs/mvs_client.py` & `bce_python_sdk-0.9.9/baidubce/services/mvs/mvs_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/oos/oos_client.py` & `bce_python_sdk-0.9.9/baidubce/services/oos/oos_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/oos/oos_model.py` & `bce_python_sdk-0.9.9/baidubce/services/oos/oos_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/__init__.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_backup_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_backup_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_database_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_database_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_hot_active_instance_group_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_hot_active_instance_group_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_http.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_http.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_instance_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_instance_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_log_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_log_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_parameter_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_parameter_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_readonly_group_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_readonly_group_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_recycler_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_recycler_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_security_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_security_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_task_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_task_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/rds/rds_users_manager.py` & `bce_python_sdk-0.9.9/baidubce/services/rds/rds_users_manager.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/route/route_client.py` & `bce_python_sdk-0.9.9/baidubce/services/route/route_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/scs/__init__.py` & `bce_python_sdk-0.9.9/baidubce/services/scs/__init__.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/scs/model.py` & `bce_python_sdk-0.9.9/baidubce/services/scs/model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/scs/scs_client.py` & `bce_python_sdk-0.9.9/baidubce/services/scs/scs_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/sms/__init__.py` & `bce_python_sdk-0.9.9/baidubce/services/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/sms/model.py` & `bce_python_sdk-0.9.9/baidubce/services/sms/model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/sms/sms_client.py` & `bce_python_sdk-0.9.9/baidubce/services/sms/sms_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/sts/__init__.py` & `bce_python_sdk-0.9.9/baidubce/services/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/sts/sts_client.py` & `bce_python_sdk-0.9.9/baidubce/services/sts/sts_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/subnet/subnet_client.py` & `bce_python_sdk-0.9.9/baidubce/services/subnet/subnet_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_admin_client.py` & `bce_python_sdk-0.9.9/baidubce/services/tsdb/tsdb_admin_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_client.py` & `bce_python_sdk-0.9.9/baidubce/services/tsdb/tsdb_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/tsdb/tsdb_handler.py` & `bce_python_sdk-0.9.9/baidubce/services/tsdb/tsdb_handler.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/vca/vca_client.py` & `bce_python_sdk-0.9.9/baidubce/services/vca/vca_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/vcr/vcr_client.py` & `bce_python_sdk-0.9.9/baidubce/services/vcr/vcr_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/vpc/acl_client.py` & `bce_python_sdk-0.9.9/baidubce/services/vpc/acl_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/vpc/nat_client.py` & `bce_python_sdk-0.9.9/baidubce/services/vpc/nat_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/vpc/nat_model.py` & `bce_python_sdk-0.9.9/baidubce/services/vpc/nat_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/vpc/peerconn_client.py` & `bce_python_sdk-0.9.9/baidubce/services/vpc/peerconn_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/vpc/peerconn_model.py` & `bce_python_sdk-0.9.9/baidubce/services/vpc/peerconn_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/vpc/vpc_client.py` & `bce_python_sdk-0.9.9/baidubce/services/vpc/vpc_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/vpn/vpn_client.py` & `bce_python_sdk-0.9.9/baidubce/services/vpn/vpn_client.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/services/vpn/vpn_model.py` & `bce_python_sdk-0.9.9/baidubce/services/vpn/vpn_model.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/baidubce/utils.py` & `bce_python_sdk-0.9.9/baidubce/utils.py`

 * *Files identical despite different names*

### Comparing `bce_python_sdk-0.9.7/bce_python_sdk.egg-info/SOURCES.txt` & `bce_python_sdk-0.9.9/bce_python_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,22 @@
 baidubce/services/eip/model.py
 baidubce/services/endpoint/__init__.py
 baidubce/services/endpoint/endpoint_client.py
 baidubce/services/endpoint/model.py
 baidubce/services/eni/__init__.py
 baidubce/services/eni/eni_client.py
 baidubce/services/eni/eni_model.py
+baidubce/services/esg/__init__.py
+baidubce/services/esg/esg_client.py
+baidubce/services/esg/esg_model.py
 baidubce/services/et/__init__.py
 baidubce/services/et/et_client.py
 baidubce/services/et/model.py
+baidubce/services/etGateway/__init__.py
+baidubce/services/etGateway/et_gateway_client.py
 baidubce/services/havip/havip_client.py
 baidubce/services/iam/__init__.py
 baidubce/services/iam/iam_client.py
 baidubce/services/infinite/__init__.py
 baidubce/services/infinite/infinite_client.py
 baidubce/services/ipv6gateway/__init__.py
 baidubce/services/ipv6gateway/ipv6gateway_client.py
@@ -120,14 +125,16 @@
 baidubce/services/mms/__init__.py
 baidubce/services/mms/mms_client.py
 baidubce/services/mvs/__init__.py
 baidubce/services/mvs/mvs_client.py
 baidubce/services/oos/__init__.py
 baidubce/services/oos/oos_client.py
 baidubce/services/oos/oos_model.py
+baidubce/services/probe/__init__.py
+baidubce/services/probe/probe_client.py
 baidubce/services/rds/__init__.py
 baidubce/services/rds/rds_backup_manager.py
 baidubce/services/rds/rds_database_manager.py
 baidubce/services/rds/rds_hot_active_instance_group_manager.py
 baidubce/services/rds/rds_http.py
 baidubce/services/rds/rds_instance_manager.py
 baidubce/services/rds/rds_log_manager.py
```

### Comparing `bce_python_sdk-0.9.7/setup.py` & `bce_python_sdk-0.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,18 @@
               'baidubce.services.rds',
               'baidubce.services.localdns',
               'baidubce.services.localdns.api',
               'baidubce.services.oos',
               'baidubce.services.ipv6gateway',
               'baidubce.services.et',
               'baidubce.services.csn',
-              'baidubce.services.havip'
+              'baidubce.services.havip',
+              'baidubce.services.esg',
+              'baidubce.services.probe',
+              'baidubce.services.etGateway'
               ],
     url='http://bce.baidu.com',
     license='Apache License 2.0',
     author='',
     author_email='',
     description='BCE SDK for python'
 )
```

