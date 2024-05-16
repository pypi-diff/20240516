# Comparing `tmp/spider-admin-pro-2.0.8.tar.gz` & `tmp/spider-admin-pro-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider-admin-pro-2.0.8.tar", last modified: Tue Sep 12 13:30:20 2023, max compression
+gzip compressed data, was "spider-admin-pro-2.0.9.tar", last modified: Wed Sep 13 09:40:45 2023, max compression
```

## Comparing `spider-admin-pro-2.0.8.tar` & `spider-admin-pro-2.0.9.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.445741 spider-admin-pro-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)      296 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2023-09-12 13:30:20.441741 spider-admin-pro-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      179 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-12 13:30:20.445741 spider-admin-pro-2.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3372 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.421741 spider-admin-pro-2.0.8/spider_admin_pro/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.425741 spider-admin-pro-2.0.8/spider_admin_pro/api/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/api/action_history_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/api/schedule_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/api/scrapyd_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/api/stats_collection_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/api/system_info_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/api_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.425741 spider-admin-pro-2.0.8/spider_admin_pro/config/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/config/detault_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/config/yaml_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.425741 spider-admin-pro-2.0.8/spider_admin_pro/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/exceptions/api_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/exceptions/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.425741 spider-admin-pro-2.0.8/spider_admin_pro/model/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/model/login_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/model/schedule_history_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/model/stats_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.425741 spider-admin-pro-2.0.8/spider_admin_pro/service/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/service/action_history_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/service/schedule_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/service/scrapyd_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/service/stats_collection_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/service/system_data_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.425741 spider-admin-pro-2.0.8/spider_admin_pro/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.429741 spider-admin-pro-2.0.8/spider_admin_pro/utils/flask_ext/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/flask_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/flask_ext/flask_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.429741 spider-admin-pro-2.0.8/spider_admin_pro/utils/flask_ext/json/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/flask_ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/flask_ext/json/default.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/flask_ext/json/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/flask_ext/json/json_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/flask_ext/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/jwt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/scheduler_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/secret_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/system_info_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/utils/time_util.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.429741 spider-admin-pro-2.0.8/spider_admin_pro/web/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.429741 spider-admin-pro-2.0.8/spider_admin_pro/web/public/
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.429741 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.433741 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/app.542ee7ed.css
--rw-r--r--   0 runner    (1001) docker     (127)    11239 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/app.d8e03581.css
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-30e10370.5063e9f2.css
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-3a584aad.0f317175.css
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-509e3c38.5063e9f2.css
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-5ba798b1.a37cd815.css
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-5fb2979b.71e917d9.css
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-7a44da90.7e3f4dc7.css
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-86cca1a8.5063e9f2.css
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-ad4dfa94.d4179a5f.css
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-b6dae904.5063e9f2.css
--rw-r--r--   0 runner    (1001) docker     (127)   239725 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-elementUI.79db45c7.css
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-libs.3dfb7769.css
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.433741 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/fonts/element-icons.535877f5.woff
--rw-r--r--   0 runner    (1001) docker     (127)    55956 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/fonts/element-icons.732389de.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.433741 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)    98071 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/img/404.a57b6f31.png
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/img/404_cloud.0f4bc32b.png
--rw-r--r--   0 runner    (1001) docker     (127)    17392 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/img/default.343756e6.png
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/img/user-avatar.ecba1844.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.441741 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    84762 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/app.002b3c3b.js
--rw-r--r--   0 runner    (1001) docker     (127)    84737 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/app.3697bf85.js
--rw-r--r--   0 runner    (1001) docker     (127)     9316 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-2810674a.4d765724.js
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-2810674a.5a60b2b4.js
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-2826794e.08f12b98.js
--rw-r--r--   0 runner    (1001) docker     (127)    10779 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-30e10370.056bfd2b.js
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-30e10370.b4dda3cb.js
--rw-r--r--   0 runner    (1001) docker     (127)    10723 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-30e10370.cd8480ae.js
--rw-r--r--   0 runner    (1001) docker     (127)    21406 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-3a584aad.7c8d6dfa.js
--rw-r--r--   0 runner    (1001) docker     (127)    12535 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-509e3c38.6b42b0d4.js
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-509e3c38.c08761a1.js
--rw-r--r--   0 runner    (1001) docker     (127)    12564 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-509e3c38.fe807fb3.js
--rw-r--r--   0 runner    (1001) docker     (127)    13090 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5a91c14f.0ca0207b.js
--rw-r--r--   0 runner    (1001) docker     (127)    13625 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5a91c14f.9c3575ca.js
--rw-r--r--   0 runner    (1001) docker     (127)    13321 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5a91c14f.bb1a87ae.js
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5ba798b1.19a0b874.js
--rw-r--r--   0 runner    (1001) docker     (127)    20964 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5fb2979b.4b7291ae.js
--rw-r--r--   0 runner    (1001) docker     (127)    21289 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5fb2979b.558e48c7.js
--rw-r--r--   0 runner    (1001) docker     (127)    20985 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5fb2979b.d0496d18.js
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-66e64759.7977bf7d.js
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-7a44da90.16d799f3.js
--rw-r--r--   0 runner    (1001) docker     (127)    10751 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-86cca1a8.5960b5a6.js
--rw-r--r--   0 runner    (1001) docker     (127)    10512 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-86cca1a8.8a86f587.js
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-ad4dfa94.7c964a2d.js
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-b6dae904.1d7fa655.js
--rw-r--r--   0 runner    (1001) docker     (127)    13331 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-b6dae904.80ca5c0c.js
--rw-r--r--   0 runner    (1001) docker     (127)    13360 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-b6dae904.d9e523b5.js
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-bafd84ba.81e76f2b.js
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-d40f7e02.48a1f02d.js
--rw-r--r--   0 runner    (1001) docker     (127)   686796 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-elementUI.fee2f969.js
--rw-r--r--   0 runner    (1001) docker     (127)  1082917 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-f43a4744.7d67c8c3.js
--rw-r--r--   0 runner    (1001) docker     (127)   387803 2023-09-12 13:30:06.000000 spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-libs.e99b284d.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-12 13:30:20.421741 spider-admin-pro-2.0.8/spider_admin_pro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2023-09-12 13:30:20.000000 spider-admin-pro-2.0.8/spider_admin_pro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2023-09-12 13:30:20.000000 spider-admin-pro-2.0.8/spider_admin_pro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 13:30:20.000000 spider-admin-pro-2.0.8/spider_admin_pro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-09-12 13:30:20.000000 spider-admin-pro-2.0.8/spider_admin_pro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-12 13:30:20.000000 spider-admin-pro-2.0.8/spider_admin_pro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-12 13:30:20.000000 spider-admin-pro-2.0.8/spider_admin_pro.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.135874 spider-admin-pro-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)      296 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2023-09-13 09:40:45.135874 spider-admin-pro-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      179 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-13 09:40:45.135874 spider-admin-pro-2.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3372 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.119874 spider-admin-pro-2.0.9/spider_admin_pro/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.119874 spider-admin-pro-2.0.9/spider_admin_pro/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/api/action_history_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/api/schedule_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/api/scrapyd_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/api/stats_collection_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/api/system_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/api_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.119874 spider-admin-pro-2.0.9/spider_admin_pro/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/config/detault_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/config/yaml_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.119874 spider-admin-pro-2.0.9/spider_admin_pro/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/exceptions/api_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/exceptions/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.119874 spider-admin-pro-2.0.9/spider_admin_pro/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/model/login_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/model/schedule_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/model/stats_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.119874 spider-admin-pro-2.0.9/spider_admin_pro/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/service/action_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/service/schedule_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/service/scrapyd_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/service/stats_collection_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/service/system_data_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.123874 spider-admin-pro-2.0.9/spider_admin_pro/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.123874 spider-admin-pro-2.0.9/spider_admin_pro/utils/flask_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/flask_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/flask_ext/flask_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.123874 spider-admin-pro-2.0.9/spider_admin_pro/utils/flask_ext/json/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/flask_ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/flask_ext/json/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/flask_ext/json/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/flask_ext/json/json_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/flask_ext/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/jwt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/scheduler_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/secret_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/system_info_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/utils/time_util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.123874 spider-admin-pro-2.0.9/spider_admin_pro/web/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.123874 spider-admin-pro-2.0.9/spider_admin_pro/web/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.123874 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.123874 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/app.542ee7ed.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/app.d8e03581.css
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-30e10370.5063e9f2.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-3a584aad.0f317175.css
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-509e3c38.5063e9f2.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-5ba798b1.a37cd815.css
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-5fb2979b.71e917d9.css
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-7a44da90.7e3f4dc7.css
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-86cca1a8.5063e9f2.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-ad4dfa94.d4179a5f.css
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-b6dae904.5063e9f2.css
+-rw-r--r--   0 runner    (1001) docker     (127)   239725 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-elementUI.79db45c7.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-libs.3dfb7769.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16958 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.123874 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/fonts/element-icons.535877f5.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    55956 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/fonts/element-icons.732389de.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.123874 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    98071 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/img/404.a57b6f31.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/img/404_cloud.0f4bc32b.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17392 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/img/default.343756e6.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/img/user-avatar.ecba1844.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.135874 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    84762 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/app.002b3c3b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84737 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/app.3697bf85.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9316 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-2810674a.4d765724.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-2810674a.5a60b2b4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-2826794e.08f12b98.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-30e10370.056bfd2b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10750 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-30e10370.b4dda3cb.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10723 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-30e10370.cd8480ae.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21406 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-3a584aad.7c8d6dfa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12535 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-509e3c38.6b42b0d4.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-509e3c38.c08761a1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12564 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-509e3c38.fe807fb3.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13090 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5a91c14f.0ca0207b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13625 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5a91c14f.9c3575ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13321 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5a91c14f.bb1a87ae.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5ba798b1.19a0b874.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20964 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5fb2979b.4b7291ae.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21289 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5fb2979b.558e48c7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20985 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5fb2979b.d0496d18.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-66e64759.7977bf7d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-7a44da90.16d799f3.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10751 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-86cca1a8.5960b5a6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10512 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-86cca1a8.8a86f587.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-ad4dfa94.7c964a2d.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-b6dae904.1d7fa655.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13331 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-b6dae904.80ca5c0c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13360 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-b6dae904.d9e523b5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-bafd84ba.81e76f2b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-d40f7e02.48a1f02d.js
+-rw-r--r--   0 runner    (1001) docker     (127)   686796 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-elementUI.fee2f969.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1082917 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-f43a4744.7d67c8c3.js
+-rw-r--r--   0 runner    (1001) docker     (127)   387803 2023-09-13 09:40:36.000000 spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-libs.e99b284d.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-13 09:40:45.119874 spider-admin-pro-2.0.9/spider_admin_pro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2023-09-13 09:40:45.000000 spider-admin-pro-2.0.9/spider_admin_pro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5594 2023-09-13 09:40:45.000000 spider-admin-pro-2.0.9/spider_admin_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 09:40:45.000000 spider-admin-pro-2.0.9/spider_admin_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2023-09-13 09:40:45.000000 spider-admin-pro-2.0.9/spider_admin_pro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-13 09:40:45.000000 spider-admin-pro-2.0.9/spider_admin_pro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-13 09:40:45.000000 spider-admin-pro-2.0.9/spider_admin_pro.egg-info/zip-safe
```

### Comparing `spider-admin-pro-2.0.8/LICENSE` & `spider-admin-pro-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/PKG-INFO` & `spider-admin-pro-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-admin-pro
-Version: 2.0.8
+Version: 2.0.9
 Summary: a spider admin based vue, scrapyd api and APScheduler
 Home-page: https://github.com/mouday/spider-admin-pro
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: spider admin scrapy scrapyd scheduler
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spider-admin-pro-2.0.8/README.md` & `spider-admin-pro-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/setup.py` & `spider-admin-pro-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/api/action_history_api.py` & `spider-admin-pro-2.0.9/spider_admin_pro/api/action_history_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/api/auth_api.py` & `spider-admin-pro-2.0.9/spider_admin_pro/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/api/schedule_api.py` & `spider-admin-pro-2.0.9/spider_admin_pro/api/schedule_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/api/scrapyd_api.py` & `spider-admin-pro-2.0.9/spider_admin_pro/api/scrapyd_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/api/stats_collection_api.py` & `spider-admin-pro-2.0.9/spider_admin_pro/api/stats_collection_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/api/system_info_api.py` & `spider-admin-pro-2.0.9/spider_admin_pro/api/system_info_api.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/api_result.py` & `spider-admin-pro-2.0.9/spider_admin_pro/api_result.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/compat.py` & `spider-admin-pro-2.0.9/spider_admin_pro/compat.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/config/detault_config.py` & `spider-admin-pro-2.0.9/spider_admin_pro/config/detault_config.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/config/yaml_config.py` & `spider-admin-pro-2.0.9/spider_admin_pro/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/main.py` & `spider-admin-pro-2.0.9/spider_admin_pro/main.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/model/base.py` & `spider-admin-pro-2.0.9/spider_admin_pro/model/base.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/model/login_history_model.py` & `spider-admin-pro-2.0.9/spider_admin_pro/model/login_history_model.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/model/schedule_history_model.py` & `spider-admin-pro-2.0.9/spider_admin_pro/model/schedule_history_model.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/model/stats_collection_model.py` & `spider-admin-pro-2.0.9/spider_admin_pro/model/stats_collection_model.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/router.py` & `spider-admin-pro-2.0.9/spider_admin_pro/router.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/service/action_history_service.py` & `spider-admin-pro-2.0.9/spider_admin_pro/service/action_history_service.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/service/auth_service.py` & `spider-admin-pro-2.0.9/spider_admin_pro/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/service/schedule_service.py` & `spider-admin-pro-2.0.9/spider_admin_pro/service/schedule_service.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/service/scrapyd_service.py` & `spider-admin-pro-2.0.9/spider_admin_pro/service/scrapyd_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
     :return:
     """
     params = {
         'base_url': SCRAPYD_SERVER
     }
 
     if SCRAPYD_USERNAME and SCRAPYD_PASSWORD:
-        params = {
+        params.update({
             'auth': HTTPBasicAuth(SCRAPYD_USERNAME, SCRAPYD_PASSWORD)
-        }
+        })
 
     return ScrapydClient(**params)
 
 
 client = get_client()
```

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/service/stats_collection_service.py` & `spider-admin-pro-2.0.9/spider_admin_pro/service/stats_collection_service.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/service/system_data_service.py` & `spider-admin-pro-2.0.9/spider_admin_pro/service/system_data_service.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/utils/flask_ext/flask_app.py` & `spider-admin-pro-2.0.9/spider_admin_pro/utils/flask_ext/flask_app.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/utils/json_util.py` & `spider-admin-pro-2.0.9/spider_admin_pro/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/utils/jwt_util.py` & `spider-admin-pro-2.0.9/spider_admin_pro/utils/jwt_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/utils/scheduler_util.py` & `spider-admin-pro-2.0.9/spider_admin_pro/utils/scheduler_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/utils/secret_util.py` & `spider-admin-pro-2.0.9/spider_admin_pro/utils/secret_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/utils/sqlite_util.py` & `spider-admin-pro-2.0.9/spider_admin_pro/utils/sqlite_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/utils/system_info_util.py` & `spider-admin-pro-2.0.9/spider_admin_pro/utils/system_info_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/utils/time_util.py` & `spider-admin-pro-2.0.9/spider_admin_pro/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/index.html` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/index.html`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/app.542ee7ed.css` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/app.542ee7ed.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/app.d8e03581.css` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/app.d8e03581.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-3a584aad.0f317175.css` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-3a584aad.0f317175.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-5ba798b1.a37cd815.css` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-5ba798b1.a37cd815.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-ad4dfa94.d4179a5f.css` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-ad4dfa94.d4179a5f.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-elementUI.79db45c7.css` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-elementUI.79db45c7.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/css/chunk-libs.3dfb7769.css` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/css/chunk-libs.3dfb7769.css`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/favicon.ico` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/fonts/element-icons.535877f5.woff` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/fonts/element-icons.732389de.ttf` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/img/404.a57b6f31.png` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/img/404.a57b6f31.png`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/img/404_cloud.0f4bc32b.png` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/img/404_cloud.0f4bc32b.png`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/img/default.343756e6.png` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/img/default.343756e6.png`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/img/user-avatar.ecba1844.gif` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/img/user-avatar.ecba1844.gif`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/app.002b3c3b.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/app.002b3c3b.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/app.3697bf85.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/app.3697bf85.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-2810674a.4d765724.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-2810674a.4d765724.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-2810674a.5a60b2b4.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-2810674a.5a60b2b4.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-2826794e.08f12b98.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-2826794e.08f12b98.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-30e10370.056bfd2b.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-30e10370.056bfd2b.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-30e10370.b4dda3cb.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-30e10370.b4dda3cb.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-30e10370.cd8480ae.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-30e10370.cd8480ae.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-3a584aad.7c8d6dfa.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-3a584aad.7c8d6dfa.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-509e3c38.6b42b0d4.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-509e3c38.6b42b0d4.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-509e3c38.c08761a1.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-509e3c38.c08761a1.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-509e3c38.fe807fb3.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-509e3c38.fe807fb3.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5a91c14f.0ca0207b.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5a91c14f.0ca0207b.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5a91c14f.9c3575ca.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5a91c14f.9c3575ca.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5a91c14f.bb1a87ae.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5a91c14f.bb1a87ae.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5ba798b1.19a0b874.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5ba798b1.19a0b874.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5fb2979b.4b7291ae.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5fb2979b.4b7291ae.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5fb2979b.558e48c7.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5fb2979b.558e48c7.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-5fb2979b.d0496d18.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-5fb2979b.d0496d18.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-66e64759.7977bf7d.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-66e64759.7977bf7d.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-7a44da90.16d799f3.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-7a44da90.16d799f3.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-86cca1a8.5960b5a6.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-86cca1a8.5960b5a6.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-86cca1a8.8a86f587.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-86cca1a8.8a86f587.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-ad4dfa94.7c964a2d.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-ad4dfa94.7c964a2d.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-b6dae904.1d7fa655.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-b6dae904.1d7fa655.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-b6dae904.80ca5c0c.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-b6dae904.80ca5c0c.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-b6dae904.d9e523b5.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-b6dae904.d9e523b5.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-bafd84ba.81e76f2b.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-bafd84ba.81e76f2b.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-d40f7e02.48a1f02d.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-d40f7e02.48a1f02d.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-elementUI.fee2f969.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-elementUI.fee2f969.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-f43a4744.7d67c8c3.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-f43a4744.7d67c8c3.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro/web/public/static/js/chunk-libs.e99b284d.js` & `spider-admin-pro-2.0.9/spider_admin_pro/web/public/static/js/chunk-libs.e99b284d.js`

 * *Files identical despite different names*

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro.egg-info/PKG-INFO` & `spider-admin-pro-2.0.9/spider_admin_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-admin-pro
-Version: 2.0.8
+Version: 2.0.9
 Summary: a spider admin based vue, scrapyd api and APScheduler
 Home-page: https://github.com/mouday/spider-admin-pro
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: spider admin scrapy scrapyd scheduler
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spider-admin-pro-2.0.8/spider_admin_pro.egg-info/SOURCES.txt` & `spider-admin-pro-2.0.9/spider_admin_pro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

