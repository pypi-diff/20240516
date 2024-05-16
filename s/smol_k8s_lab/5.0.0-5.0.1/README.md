# Comparing `tmp/smol_k8s_lab-5.0.0.tar.gz` & `tmp/smol_k8s_lab-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smol_k8s_lab-5.0.0.tar", max compression
+gzip compressed data, was "smol_k8s_lab-5.0.1.tar", max compression
```

## Comparing `smol_k8s_lab-5.0.0.tar` & `smol_k8s_lab-5.0.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0    34260 2024-05-15 10:15:14.083655 smol_k8s_lab-5.0.0/LICENSE
--rw-r--r--   0        0        0    27183 2024-05-15 10:15:14.083655 smol_k8s_lab-5.0.0/README.md
--rw-r--r--   0        0        0     3300 2024-05-15 10:15:14.343655 smol_k8s_lab-5.0.0/pyproject.toml
--rwxr-xr-x   0        0        0    16188 2024-05-15 10:15:14.343655 smol_k8s_lab-5.0.0/smol_k8s_lab/__init__.py
--rw-r--r--   0        0        0  5853144 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/audio/audio-en.tar.gz
--rwxr-xr-x   0        0        0    12759 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/bw_cli.py
--rw-r--r--   0        0        0     1679 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden.css
--rw-r--r--   0        0        0     2093 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
--rw-r--r--   0        0        0     4524 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
--rw-r--r--   0        0        0     2395 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
--rw-r--r--   0        0        0     6916 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
--rw-r--r--   0        0        0    17031 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/audio/en.yml
--rw-r--r--   0        0        0     2364 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/audio/nl.yml
--rw-r--r--   0        0        0    76932 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/default_config.yaml
--rw-r--r--   0        0        0     5666 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/keycloak_config.json
--rw-r--r--   0        0        0      237 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/kind/kind-config-cilium.yaml
--rw-r--r--   0        0        0      385 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/kind/kind_cluster_config.yaml
--rw-r--r--   0        0        0      831 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml
--rwxr-xr-x   0        0        0     3008 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/constants.py
--rwxr-xr-x   0        0        0    12945 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/env_config.py
--rw-r--r--   0        0        0     9821 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/__init__.py
--rw-r--r--   0        0        0     7789 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/argocd.py
--rw-r--r--   0        0        0        0 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
--rw-r--r--   0        0        0     6581 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
--rw-r--r--   0        0        0     9763 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
--rw-r--r--   0        0        0    19076 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
--rw-r--r--   0        0        0    20511 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
--rw-r--r--   0        0        0     3372 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
--rw-r--r--   0        0        0     1285 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
--rw-r--r--   0        0        0     9134 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/initial_special.py
--rw-r--r--   0        0        0        0 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/__init__.py
--rw-r--r--   0        0        0     1766 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/cilium.py
--rw-r--r--   0        0        0     2318 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/metallb.py
--rw-r--r--   0        0        0    10977 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/netmaker.py
--rw-r--r--   0        0        0     2383 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/__init__.py
--rw-r--r--   0        0        0     8381 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/minio.py
--rw-r--r--   0        0        0     3617 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
--rw-r--r--   0        0        0     4286 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
--rw-r--r--   0        0        0        0 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
--rw-r--r--   0        0        0     2675 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
--rw-r--r--   0        0        0     3759 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
--rw-r--r--   0        0        0     4805 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py
--rw-r--r--   0        0        0    11623 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/home_assistant.py
--rw-r--r--   0        0        0    21465 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/mastodon.py
--rwxr-xr-x   0        0        0     1706 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
--rw-r--r--   0        0        0    18842 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/matrix.py
--rw-r--r--   0        0        0    20726 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/nextcloud.py
--rwxr-xr-x   0        0        0     6182 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
--rw-r--r--   0        0        0     8034 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/__init__.py
--rw-r--r--   0        0        0     3755 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/k3d.py
--rw-r--r--   0        0        0     8481 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/k3s.py
--rw-r--r--   0        0        0     4821 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/kind.py
--rw-r--r--   0        0        0        1 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/__init__.py
--rw-r--r--   0        0        0     8642 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/argocd_util.py
--rw-r--r--   0        0        0     8689 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/backup.py
--rwxr-xr-x   0        0        0     8607 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/helm.py
--rw-r--r--   0        0        0    14252 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/k8s_lib.py
--rw-r--r--   0        0        0    22222 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/restores.py
--rw-r--r--   0        0        0     1358 2024-05-15 10:15:14.355655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/__init__.py
--rw-r--r--   0        0        0    14333 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
--rw-r--r--   0        0        0     9712 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
--rw-r--r--   0        0        0    18578 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py
--rw-r--r--   0        0        0    14373 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/input_widgets.py
--rwxr-xr-x   0        0        0     4002 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py
--rw-r--r--   0        0        0     6970 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/modify_globals.py
--rw-r--r--   0        0        0     3697 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py
--rwxr-xr-x   0        0        0    17623 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/apps_screen.py
--rw-r--r--   0        0        0    12695 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base.py
--rw-r--r--   0        0        0    32748 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base_widgets/audio_widget.py
--rw-r--r--   0        0        0     7189 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py
--rw-r--r--   0        0        0     3384 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py
--rwxr-xr-x   0        0        0     8873 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/confirm_screen.py
--rw-r--r--   0        0        0     1546 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss
--rw-r--r--   0        0        0     7174 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/apps_config.tcss
--rw-r--r--   0        0        0     1184 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/apps_init_config.tcss
--rw-r--r--   0        0        0     6681 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/base.tcss
--rw-r--r--   0        0        0      988 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/base_modal.tcss
--rw-r--r--   0        0        0     1371 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/cluster_modal.tcss
--rw-r--r--   0        0        0     1278 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/confirm.tcss
--rw-r--r--   0        0        0     1564 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/distro_config.tcss
--rw-r--r--   0        0        0      867 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/help.tcss
--rw-r--r--   0        0        0      984 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/invalid_apps.tcss
--rw-r--r--   0        0        0     2198 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/k3s.tcss
--rw-r--r--   0        0        0     1901 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/kind.tcss
--rw-r--r--   0        0        0     1259 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss
--rw-r--r--   0        0        0      770 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/new_app_modal.tcss
--rw-r--r--   0        0        0      112 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/new_option_modal.tcss
--rw-r--r--   0        0        0     1168 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss
--rw-r--r--   0        0        0     1101 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/node_modal.tcss
--rw-r--r--   0        0        0     3433 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
--rw-r--r--   0        0        0     2554 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/tui_config.tcss
--rwxr-xr-x   0        0        0    10434 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_screen.py
--rw-r--r--   0        0        0        0 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/__init__.py
--rw-r--r--   0        0        0    17221 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py
--rw-r--r--   0        0        0    14337 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py
--rw-r--r--   0        0        0     6754 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/kind_config.py
--rw-r--r--   0        0        0     6060 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
--rw-r--r--   0        0        0     4359 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
--rw-r--r--   0        0        0     4669 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
--rw-r--r--   0        0        0     4138 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/help_screen.py
--rwxr-xr-x   0        0        0     4020 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/make_screenshots.py
--rwxr-xr-x   0        0        0    11190 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/smol_k8s_config_screen.py
--rwxr-xr-x   0        0        0     8826 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/tui_config_screen.py
--rw-r--r--   0        0        0     9872 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/util.py
--rw-r--r--   0        0        0        0 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/validators/__init__.py
--rw-r--r--   0        0        0      579 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/tui/validators/already_exists.py
--rw-r--r--   0        0        0        0 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/__init__.py
--rw-r--r--   0        0        0    16300 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/minio_lib.py
--rw-r--r--   0        0        0     1184 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/passwords.py
--rwxr-xr-x   0        0        0     2423 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/rich_cli/console_logging.py
--rwxr-xr-x   0        0        0     4720 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/rich_cli/help_text.py
--rw-r--r--   0        0        0     2610 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/run/final_cmd.py
--rwxr-xr-x   0        0        0     7483 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/run/subproc.py
--rw-r--r--   0        0        0     2837 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/value_from.py
--rw-r--r--   0        0        0      315 2024-05-15 10:15:14.359655 smol_k8s_lab-5.0.0/smol_k8s_lab/utils/yaml_with_comments.py
--rw-r--r--   0        0        0    28869 1970-01-01 00:00:00.000000 smol_k8s_lab-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-05-15 19:58:52.205433 smol_k8s_lab-5.0.1/LICENSE
+-rw-r--r--   0        0        0    29410 2024-05-15 19:58:52.205433 smol_k8s_lab-5.0.1/README.md
+-rw-r--r--   0        0        0     3300 2024-05-15 19:58:52.469433 smol_k8s_lab-5.0.1/pyproject.toml
+-rwxr-xr-x   0        0        0    16188 2024-05-15 19:58:52.473433 smol_k8s_lab-5.0.1/smol_k8s_lab/__init__.py
+-rw-r--r--   0        0        0  5853144 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/audio/audio-en.tar.gz
+-rwxr-xr-x   0        0        0    12759 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/bw_cli.py
+-rw-r--r--   0        0        0     1679 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/tui/bitwarden.css
+-rw-r--r--   0        0        0     2093 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
+-rw-r--r--   0        0        0     4524 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
+-rw-r--r--   0        0        0     2395 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
+-rw-r--r--   0        0        0     6916 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
+-rw-r--r--   0        0        0    17031 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/config/audio/en.yml
+-rw-r--r--   0        0        0     2364 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/config/audio/nl.yml
+-rw-r--r--   0        0        0    76932 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/config/default_config.yaml
+-rw-r--r--   0        0        0     5666 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/config/keycloak_config.json
+-rw-r--r--   0        0        0      237 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/config/kind/kind-config-cilium.yaml
+-rw-r--r--   0        0        0      385 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/config/kind/kind_cluster_config.yaml
+-rw-r--r--   0        0        0      831 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/config/smol-k8s-lab.appdata.xml
+-rwxr-xr-x   0        0        0     3008 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/constants.py
+-rwxr-xr-x   0        0        0    12945 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/env_config.py
+-rw-r--r--   0        0        0     9821 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/__init__.py
+-rw-r--r--   0        0        0     7789 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/argocd.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
+-rw-r--r--   0        0        0     6581 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
+-rw-r--r--   0        0        0     9763 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
+-rw-r--r--   0        0        0    19076 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
+-rw-r--r--   0        0        0    20511 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
+-rw-r--r--   0        0        0     3372 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
+-rw-r--r--   0        0        0     1285 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
+-rw-r--r--   0        0        0     9134 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/initial_special.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/networking/__init__.py
+-rw-r--r--   0        0        0     1766 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/networking/cilium.py
+-rw-r--r--   0        0        0     2318 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/networking/metallb.py
+-rw-r--r--   0        0        0    10977 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/networking/netmaker.py
+-rw-r--r--   0        0        0     2383 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/operators/__init__.py
+-rw-r--r--   0        0        0     8381 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/operators/minio.py
+-rw-r--r--   0        0        0     3617 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
+-rw-r--r--   0        0        0     4286 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
+-rw-r--r--   0        0        0     2675 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
+-rw-r--r--   0        0        0     3759 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
+-rw-r--r--   0        0        0     4805 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/secrets_management/vault.py
+-rw-r--r--   0        0        0    11623 2024-05-15 19:58:52.481433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/home_assistant.py
+-rw-r--r--   0        0        0    21465 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/mastodon.py
+-rwxr-xr-x   0        0        0     1706 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
+-rw-r--r--   0        0        0    18842 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/matrix.py
+-rw-r--r--   0        0        0    20726 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/nextcloud.py
+-rwxr-xr-x   0        0        0     6182 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
+-rw-r--r--   0        0        0     8034 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_distros/__init__.py
+-rw-r--r--   0        0        0     3755 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_distros/k3d.py
+-rw-r--r--   0        0        0     8481 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_distros/k3s.py
+-rw-r--r--   0        0        0     4821 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_distros/kind.py
+-rw-r--r--   0        0        0        1 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/__init__.py
+-rw-r--r--   0        0        0     8642 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/argocd_util.py
+-rw-r--r--   0        0        0     8689 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/backup.py
+-rwxr-xr-x   0        0        0     8607 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/helm.py
+-rw-r--r--   0        0        0    14252 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/k8s_lib.py
+-rw-r--r--   0        0        0    22222 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/restores.py
+-rw-r--r--   0        0        0     1358 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/__init__.py
+-rw-r--r--   0        0        0    14333 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
+-rw-r--r--   0        0        0     9712 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
+-rw-r--r--   0        0        0    18578 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/backup_and_restore.py
+-rw-r--r--   0        0        0    14373 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/input_widgets.py
+-rwxr-xr-x   0        0        0     4002 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/invalid_apps.py
+-rw-r--r--   0        0        0     6970 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/modify_globals.py
+-rw-r--r--   0        0        0     3697 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/new_app_modal.py
+-rwxr-xr-x   0        0        0    17593 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/apps_screen.py
+-rw-r--r--   0        0        0    12766 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/base.py
+-rw-r--r--   0        0        0    32748 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/base_widgets/audio_widget.py
+-rw-r--r--   0        0        0     7189 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/base_widgets/cluster_modal.py
+-rw-r--r--   0        0        0     3384 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/base_widgets/new_cluster_input.py
+-rwxr-xr-x   0        0        0     8926 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/confirm_screen.py
+-rw-r--r--   0        0        0     1546 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/add_nodes_widget.tcss
+-rw-r--r--   0        0        0     7174 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/apps_config.tcss
+-rw-r--r--   0        0        0     1184 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/apps_init_config.tcss
+-rw-r--r--   0        0        0     6681 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/base.tcss
+-rw-r--r--   0        0        0      988 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/base_modal.tcss
+-rw-r--r--   0        0        0     1371 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/cluster_modal.tcss
+-rw-r--r--   0        0        0     1278 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/confirm.tcss
+-rw-r--r--   0        0        0     1564 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/distro_config.tcss
+-rw-r--r--   0        0        0      927 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/help.tcss
+-rw-r--r--   0        0        0      984 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/invalid_apps.tcss
+-rw-r--r--   0        0        0     2198 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/k3s.tcss
+-rw-r--r--   0        0        0     1901 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/kind.tcss
+-rw-r--r--   0        0        0     1259 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/modify_globals_modal.tcss
+-rw-r--r--   0        0        0      770 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/new_app_modal.tcss
+-rw-r--r--   0        0        0      112 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/new_option_modal.tcss
+-rw-r--r--   0        0        0     1168 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/node_inputs_widget.tcss
+-rw-r--r--   0        0        0     1101 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/node_modal.tcss
+-rw-r--r--   0        0        0     3433 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
+-rw-r--r--   0        0        0     2554 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/tui_config.tcss
+-rwxr-xr-x   0        0        0    10391 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_screen.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/__init__.py
+-rw-r--r--   0        0        0    17214 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/add_nodes.py
+-rw-r--r--   0        0        0    14337 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/k3s_config.py
+-rw-r--r--   0        0        0     6754 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/kind_config.py
+-rw-r--r--   0        0        0     6060 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
+-rw-r--r--   0        0        0     4359 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
+-rw-r--r--   0        0        0     4669 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
+-rw-r--r--   0        0        0     4193 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/help_screen.py
+-rwxr-xr-x   0        0        0     4020 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/make_screenshots.py
+-rwxr-xr-x   0        0        0    11139 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/smol_k8s_config_screen.py
+-rwxr-xr-x   0        0        0     8811 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/tui_config_screen.py
+-rw-r--r--   0        0        0     9872 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/util.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/validators/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-15 19:58:52.485433 smol_k8s_lab-5.0.1/smol_k8s_lab/tui/validators/already_exists.py
+-rw-r--r--   0        0        0        0 2024-05-15 19:58:52.489433 smol_k8s_lab-5.0.1/smol_k8s_lab/utils/__init__.py
+-rw-r--r--   0        0        0    16300 2024-05-15 19:58:52.489433 smol_k8s_lab-5.0.1/smol_k8s_lab/utils/minio_lib.py
+-rw-r--r--   0        0        0     1184 2024-05-15 19:58:52.489433 smol_k8s_lab-5.0.1/smol_k8s_lab/utils/passwords.py
+-rwxr-xr-x   0        0        0     2423 2024-05-15 19:58:52.489433 smol_k8s_lab-5.0.1/smol_k8s_lab/utils/rich_cli/console_logging.py
+-rwxr-xr-x   0        0        0     4720 2024-05-15 19:58:52.489433 smol_k8s_lab-5.0.1/smol_k8s_lab/utils/rich_cli/help_text.py
+-rw-r--r--   0        0        0     2610 2024-05-15 19:58:52.489433 smol_k8s_lab-5.0.1/smol_k8s_lab/utils/run/final_cmd.py
+-rwxr-xr-x   0        0        0     7483 2024-05-15 19:58:52.489433 smol_k8s_lab-5.0.1/smol_k8s_lab/utils/run/subproc.py
+-rw-r--r--   0        0        0     2837 2024-05-15 19:58:52.489433 smol_k8s_lab-5.0.1/smol_k8s_lab/utils/value_from.py
+-rw-r--r--   0        0        0      315 2024-05-15 19:58:52.489433 smol_k8s_lab-5.0.1/smol_k8s_lab/utils/yaml_with_comments.py
+-rw-r--r--   0        0        0    31096 1970-01-01 00:00:00.000000 smol_k8s_lab-5.0.1/PKG-INFO
```

### Comparing `smol_k8s_lab-5.0.0/LICENSE` & `smol_k8s_lab-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/README.md` & `smol_k8s_lab-5.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,30 @@
 ### Features
 - Deploys [Argo CD](https://github.com/argoproj/argo-cd) by default, so you can manage your entire lab using files in [open source git repos](https://github.com/small-hack/argocd-apps)
   - Argo CD ships with a dashboard with a custom theme 💙
 - Supports multiple [k8s distros](#supported-k8s-distributions)
 - Specializes in using Bitwarden (though not required) to store sensitive values both locally and on your cluster
 - Manages all your authentication needs centrally using Zitadel and Vouch 💪
 - Supports initialization on a [range of common self-hosted apps](https://small-hack.github.io/smol-k8s-lab/k8s_apps/argocd/) 📱
+  - featured initialized apps such as [Nextcloud](https://small-hack.github.io/smol-k8s-lab/k8s_apps/nextcloud/), [Matrix](https://small-hack.github.io/smol-k8s-lab/k8s_apps/matrix/), and [Home Assistant](https://small-hack.github.io/smol-k8s-lab/k8s_apps/home_assistant/) include backups
 - Lots o' [docs](https://small-hack.github.io/smol-k8s-lab)
 
+-----------------------------
+
+* [Installation](#installation)
+    * [pipx](#pipx)
+    * [brew (still unstable)](#brew-still-unstable)
+    * [Usage](#usage)
+        * [Initialization](#initialization)
+* [Under the hood](#under-the-hood)
+    * [Supported k8s distributions](#supported-k8s-distributions)
+    * [Default Installed Applications](#default-installed-applications)
+* [Status](#status)
+
+
 # Installation
 B sure to check out our full [installation guide](https://small-hack.github.io/smol-k8s-lab/installation/), but the gist of it is `smol-k8s-lab` can be installed via `pipx` (or `brew` coming soon).
 
 ## pipx
 `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://github.com/pypa/pipx)). If you've already got both and [other pre-reqs](https://small-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be able to:
 
 ```bash
@@ -73,14 +87,51 @@
 After you've followed the installation instructions, if you're *new* to `smol-k8s-lab`,  initialize a new config file:
 
 ```bash
 # we'll walk you through any configuration needed before
 # saving the config and deploying it for you
 smol-k8s-lab
 ```
+
+<details>
+  <summary><b>Upgrading config from v4.x to v5.x</b></summary>
+
+If you've installed smol-k8s-lab prior to `v5.0.0`, please backup your old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the following with either pip or pipx:
+
+*if using pip*:
+```yaml
+# this uninstalls the old smol-k8s-lab for python 3.11
+pip3.11 uninstall smol-k8s-lab
+
+# this installs smol-k8s-lab for python 3.12
+pip3.12 install --upgrade smol-k8s-lab
+
+# this initializes a new configuration
+smol-k8s-lab
+```
+
+*or if using pipx*:
+```yaml
+# this upgrades smol-k8s-lab
+pipx upgrade smol-k8s-lab
+
+# this initializes a new configuration
+smol-k8s-lab
+```
+
+We have done a *masive* upgrade of the config file. You'll need to update your configs based on the details in https://github.com/small-hack/smol-k8s-lab/pull/210 . The main changes are to the following (check each doc link for details):
+
+- [accessibility features](https://small-hack.github.io/smol-k8s-lab/config_file/#tui-and-accessibility-configuration)
+- [k3s nodes section](https://small-hack.github.io/smol-k8s-lab/config_file/#k3s)
+- [backups and restores](https://small-hack.github.io/smol-k8s-lab/config_file/#backups-and-restores)
+- [sensitive values](https://small-hack.github.io/smol-k8s-lab/config_file/#sensitive-values)
+- [k9s has been removed in favor of run command](https://small-hack.github.io/smol-k8s-lab/config_file/#run-command) (hint: you can still use k9s via run command)
+
+</details>
+
 <details>
   <summary><b>Upgrading config from v3.7.1 to v4.x</b></summary>
 
 If you've installed smol-k8s-lab prior to `v4.0.0`, please backup your old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the following with either pip or pipx:
 
 *if using pip*:
 ```yaml
```

#### html2text {}

```diff
@@ -14,76 +14,105 @@
 default, so you can manage your entire lab using files in [open source git
 repos](https://github.com/small-hack/argocd-apps) - Argo CD ships with a
 dashboard with a custom theme ð - Supports multiple [k8s distros]
 (#supported-k8s-distributions) - Specializes in using Bitwarden (though not
 required) to store sensitive values both locally and on your cluster - Manages
 all your authentication needs centrally using Zitadel and Vouch ðª - Supports
 initialization on a [range of common self-hosted apps](https://small-
-hack.github.io/smol-k8s-lab/k8s_apps/argocd/) ð± - Lots o' [docs](https://
-small-hack.github.io/smol-k8s-lab) # Installation B sure to check out our full
-[installation guide](https://small-hack.github.io/smol-k8s-lab/installation/),
-but the gist of it is `smol-k8s-lab` can be installed via `pipx` (or `brew`
-coming soon). ## pipx `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://
-github.com/pypa/pipx)). If you've already got both and [other pre-reqs](https:/
-/small-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be
-able to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help
-menu before proceeding smol-k8s-lab --help ``` ## brew (still unstable)
-[`brew`] is the future preferred installation method for macOS/Debian/Ubuntu,
-as this will also install any non-python prerequisites you need, so you don't
-need to worry about them. This method is new, so please [let us know if
-anything isn't working for you](https://github.com/small-hack/homebrew-tap/
-issues). ```bash # tap the special homebrew repo for our formula and install it
-brew install small-hack/tap/smol-k8s-lab ``` Then you should be able to check
-the version and cli options with: ```bash smol-k8s-lab --help ```
+hack.github.io/smol-k8s-lab/k8s_apps/argocd/) ð± - featured initialized apps
+such as [Nextcloud](https://small-hack.github.io/smol-k8s-lab/k8s_apps/
+nextcloud/), [Matrix](https://small-hack.github.io/smol-k8s-lab/k8s_apps/
+matrix/), and [Home Assistant](https://small-hack.github.io/smol-k8s-lab/
+k8s_apps/home_assistant/) include backups - Lots o' [docs](https://small-
+hack.github.io/smol-k8s-lab) ----------------------------- * [Installation]
+(#installation) * [pipx](#pipx) * [brew (still unstable)](#brew-still-unstable)
+* [Usage](#usage) * [Initialization](#initialization) * [Under the hood]
+(#under-the-hood) * [Supported k8s distributions](#supported-k8s-distributions)
+* [Default Installed Applications](#default-installed-applications) * [Status]
+(#status) # Installation B sure to check out our full [installation guide]
+(https://small-hack.github.io/smol-k8s-lab/installation/), but the gist of it
+is `smol-k8s-lab` can be installed via `pipx` (or `brew` coming soon). ## pipx
+`smol-k8s-lab` requires Python 3.11+ (and [pipx](https://github.com/pypa/
+pipx)). If you've already got both and [other pre-reqs](https://small-
+hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be able
+to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help menu
+before proceeding smol-k8s-lab --help ``` ## brew (still unstable) [`brew`] is
+the future preferred installation method for macOS/Debian/Ubuntu, as this will
+also install any non-python prerequisites you need, so you don't need to worry
+about them. This method is new, so please [let us know if anything isn't
+working for you](https://github.com/small-hack/homebrew-tap/issues). ```bash #
+tap the special homebrew repo for our formula and install it brew install
+small-hack/tap/smol-k8s-lab ``` Then you should be able to check the version
+and cli options with: ```bash smol-k8s-lab --help ```
  _[_O_u_t_p_u_t_ _o_f_ _s_m_o_l_-_k_8_s_-_l_a_b_ _-_-_h_e_l_p_ _a_f_t_e_r_ _c_l_o_n_i_n_g_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g_ _t_h_e
                                 _p_r_e_r_e_q_u_i_s_i_t_e_s_._]
 Checkout our [TUI docs](https://small-hack.github.io/smol-k8s-lab/tui/
 create_modify_screens/) for more info on how to get started playing with `smol-
 k8s-lab` :-) ## Usage ### Initialization After you've followed the installation
 instructions, if you're *new* to `smol-k8s-lab`, initialize a new config file:
 ```bash # we'll walk you through any configuration needed before # saving the
-config and deploying it for you smol-k8s-lab ``` UUppggrraaddiinngg ccoonnffiigg ffrroomm vv33..77..11
-ttoo vv44..xx If you've installed smol-k8s-lab prior to `v4.0.0`, please backup your
-old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or
+config and deploying it for you smol-k8s-lab ``` UUppggrraaddiinngg ccoonnffiigg ffrroomm vv44..xx ttoo
+vv55..xx If you've installed smol-k8s-lab prior to `v5.0.0`, please backup your old
+configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or
 `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the
-following with either pip or pipx: *if using pip*: ```yaml # this upgrades
-smol-k8s-lab pip3.11 install --upgrade smol-k8s-lab # this initializes a new
-configuration smol-k8s-lab ``` *or if using pipx*: ```yaml # this upgrades
-smol-k8s-lab pipx upgrade smol-k8s-lab # this initializes a new configuration
-smol-k8s-lab ``` The main breaking changes between `v3.7.1` and `v4.0.0` are
-that we now default enable metrics on most apps. Because of this, you need to
-have the Prometheus ServiceMonitor CRD installed ahead of time. Luckily, we now
-provide that as an app as well :) If you deleted your config and created a new
-one, it will already be there, but if you want to reuse your old config, you
-can add the app like this: ```yaml apps: prometheus_crds: description: |
-[link=https://prometheus.io/docs/introduction/overview/]Prometheus[/link] CRDs
-to start with. You can optionally disable this if you don't want to deploy apps
-with metrics. enabled: true argo: # secrets keys to make available to Argo CD
-ApplicationSets secret_keys: {} # git repo to install the Argo CD app from
-repo: https://github.com/small-hack/argocd-apps # path in the argo repo to
-point to. Trailing slash very important! path: prometheus/crds/ # either the
-branch or tag to point at in the argo repo above revision: main # namespace to
-install the k8s app in namespace: prometheus # recurse directories in the
-provided git repo directory_recursion: false # source repos for Argo CD App
-Project (in addition to argo.repo) project: name: prometheus source_repos: -
-https://github.com/prometheus-community/helm-charts.git destination: #
-automatically includes the app's namespace and argocd's namespace namespaces: -
-kube-system - prometheus ``` If using the default repos, please also disable
-directory directory_recursion for: - your prometheus stack app - zitadel For
-all changes, please check out [PR #206](https://github.com/small-hack/smol-k8s-
-lab/pull/206). UUppggrraaddiinngg ccoonnffiigg ffrroomm vv22..22..44 ttoo vv33..xx If you've installed smol-
-k8s-lab prior to `v3.0.0`, please backup your old configuration, and then
-remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-
-lab/config.yaml`) file entirely, then run the following with either pip or
-pipx: *if using pip*: ```yaml # this upgrades smol-k8s-lab pip3.11 install --
-upgrade smol-k8s-lab # this initializes a new configuration smol-k8s-lab ```
-*or if using pipx*: ```yaml # this upgrades smol-k8s-lab pipx upgrade smol-k8s-
-lab # this initializes a new configuration smol-k8s-lab ``` The main breaking
-changes between `v2.2.4` and `v3.0` are as follows: - *home assistant has
-graduated from demo app to live app* You'll need to change
+following with either pip or pipx: *if using pip*: ```yaml # this uninstalls
+the old smol-k8s-lab for python 3.11 pip3.11 uninstall smol-k8s-lab # this
+installs smol-k8s-lab for python 3.12 pip3.12 install --upgrade smol-k8s-lab #
+this initializes a new configuration smol-k8s-lab ``` *or if using pipx*:
+```yaml # this upgrades smol-k8s-lab pipx upgrade smol-k8s-lab # this
+initializes a new configuration smol-k8s-lab ``` We have done a *masive*
+upgrade of the config file. You'll need to update your configs based on the
+details in https://github.com/small-hack/smol-k8s-lab/pull/210 . The main
+changes are to the following (check each doc link for details): -
+[accessibility features](https://small-hack.github.io/smol-k8s-lab/config_file/
+#tui-and-accessibility-configuration) - [k3s nodes section](https://small-
+hack.github.io/smol-k8s-lab/config_file/#k3s) - [backups and restores](https://
+small-hack.github.io/smol-k8s-lab/config_file/#backups-and-restores) -
+[sensitive values](https://small-hack.github.io/smol-k8s-lab/config_file/
+#sensitive-values) - [k9s has been removed in favor of run command](https://
+small-hack.github.io/smol-k8s-lab/config_file/#run-command) (hint: you can
+still use k9s via run command) UUppggrraaddiinngg ccoonnffiigg ffrroomm vv33..77..11 ttoo vv44..xx If you've
+installed smol-k8s-lab prior to `v4.0.0`, please backup your old configuration,
+and then remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/
+smol-k8s-lab/config.yaml`) file entirely, then run the following with either
+pip or pipx: *if using pip*: ```yaml # this upgrades smol-k8s-lab pip3.11
+install --upgrade smol-k8s-lab # this initializes a new configuration smol-k8s-
+lab ``` *or if using pipx*: ```yaml # this upgrades smol-k8s-lab pipx upgrade
+smol-k8s-lab # this initializes a new configuration smol-k8s-lab ``` The main
+breaking changes between `v3.7.1` and `v4.0.0` are that we now default enable
+metrics on most apps. Because of this, you need to have the Prometheus
+ServiceMonitor CRD installed ahead of time. Luckily, we now provide that as an
+app as well :) If you deleted your config and created a new one, it will
+already be there, but if you want to reuse your old config, you can add the app
+like this: ```yaml apps: prometheus_crds: description: | [link=https://
+prometheus.io/docs/introduction/overview/]Prometheus[/link] CRDs to start with.
+You can optionally disable this if you don't want to deploy apps with metrics.
+enabled: true argo: # secrets keys to make available to Argo CD ApplicationSets
+secret_keys: {} # git repo to install the Argo CD app from repo: https://
+github.com/small-hack/argocd-apps # path in the argo repo to point to. Trailing
+slash very important! path: prometheus/crds/ # either the branch or tag to
+point at in the argo repo above revision: main # namespace to install the k8s
+app in namespace: prometheus # recurse directories in the provided git repo
+directory_recursion: false # source repos for Argo CD App Project (in addition
+to argo.repo) project: name: prometheus source_repos: - https://github.com/
+prometheus-community/helm-charts.git destination: # automatically includes the
+app's namespace and argocd's namespace namespaces: - kube-system - prometheus
+``` If using the default repos, please also disable directory
+directory_recursion for: - your prometheus stack app - zitadel For all changes,
+please check out [PR #206](https://github.com/small-hack/smol-k8s-lab/pull/
+206). UUppggrraaddiinngg ccoonnffiigg ffrroomm vv22..22..44 ttoo vv33..xx If you've installed smol-k8s-lab
+prior to `v3.0.0`, please backup your old configuration, and then remove the
+`~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-lab/
+config.yaml`) file entirely, then run the following with either pip or pipx:
+*if using pip*: ```yaml # this upgrades smol-k8s-lab pip3.11 install --upgrade
+smol-k8s-lab # this initializes a new configuration smol-k8s-lab ``` *or if
+using pipx*: ```yaml # this upgrades smol-k8s-lab pipx upgrade smol-k8s-lab #
+this initializes a new configuration smol-k8s-lab ``` The main breaking changes
+between `v2.2.4` and `v3.0` are as follows: - *home assistant has graduated
+from demo app to live app* You'll need to change
 `apps.home_assistant.argo.path` to either `home-assistant/
 toleration_and_affinity/` if you're using node labels and taints, or `home-
 assistant/` if you're deploying to a single node cluster. Here's an example
 with no tolerations or node affinity: ```yaml apps: home_assistant: enabled:
 false description: | [link=https://home-assistant.io]Home Assistant[/link] is a
 home IOT management solution. By default, we assume you want to use node
 affinity and tolerations to keep home assistant pods on certain nodes and keep
```

### Comparing `smol_k8s_lab-5.0.0/pyproject.toml` & `smol_k8s_lab-5.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "smol_k8s_lab"
-version       = "5.0.0"
+version       = "5.0.1"
 description   = "CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD"
 authors       = ["Jesse Hitch <jessebot@linux.com>",
                  "Max Roby <emax@cloudydev.net>"]
 readme        = "README.md"
 packages      = [{include = "smol_k8s_lab"}]
 license       = "AGPL-3.0-or-later"
 homepage      = "https://small-hack.github.io/smol-k8s-lab"
```

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/__init__.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/audio/audio-en.tar.gz` & `smol_k8s_lab-5.0.1/smol_k8s_lab/audio/audio-en.tar.gz`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/bw_cli.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/bw_cli.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden.css` & `smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/tui/bitwarden.css`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/config/audio/en.yml` & `smol_k8s_lab-5.0.1/smol_k8s_lab/config/audio/en.yml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/config/audio/nl.yml` & `smol_k8s_lab-5.0.1/smol_k8s_lab/config/audio/nl.yml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/config/default_config.yaml` & `smol_k8s_lab-5.0.1/smol_k8s_lab/config/default_config.yaml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/config/keycloak_config.json` & `smol_k8s_lab-5.0.1/smol_k8s_lab/config/keycloak_config.json`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml` & `smol_k8s_lab-5.0.1/smol_k8s_lab/config/smol-k8s-lab.appdata.xml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/constants.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/constants.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/env_config.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/env_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/__init__.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/argocd.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/argocd.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/identity_provider/vouch.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/ingress/cert_manager.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/initial_special.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/initial_special.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/cilium.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/networking/cilium.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/metallb.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/networking/metallb.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/networking/netmaker.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/networking/netmaker.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/__init__.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/minio.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/operators/minio.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/operators/postgres_operators.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/operators/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/secrets_management/infisical.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/secrets_management/vault.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/home_assistant.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/home_assistant.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/mastodon.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/mastodon.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/mastodon_rake.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/matrix.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/matrix.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/nextcloud.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/nextcloud.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/__init__.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_distros/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/k3d.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_distros/k3d.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/k3s.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_distros/k3s.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_distros/kind.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_distros/kind.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/argocd_util.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/argocd_util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/backup.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/backup.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/helm.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/helm.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/k8s_lib.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/k8s_lib.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/k8s_tools/restores.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/k8s_tools/restores.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/__init__.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/argocd_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/input_widgets.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/input_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/invalid_apps.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/modify_globals.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/modify_globals.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/app_widgets/new_app_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/apps_screen.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/apps_screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3.11
 # smol-k8s-lab libraries
-from smol_k8s_lab.utils.run.subproc import subproc
+from smol_k8s_lab.constants import VERSION
 from smol_k8s_lab.k8s_tools.k8s_lib import K8s
 from smol_k8s_lab.k8s_tools.argocd_util import ArgoCD
 from smol_k8s_lab.tui.app_widgets.invalid_apps import InvalidAppsModalScreen
 from smol_k8s_lab.tui.app_widgets.app_inputs_confg import AppInputs
 from smol_k8s_lab.tui.app_widgets.new_app_modal import NewAppModalScreen
 from smol_k8s_lab.tui.app_widgets.modify_globals import ModifyAppGlobals
 from smol_k8s_lab.tui.util import format_description
+from smol_k8s_lab.utils.run.subproc import subproc
 
 # external libraries
 from kubernetes.config import ConfigException
 from os import environ
 from textual import on, work
 from textual.app import ComposeResult
 from textual.binding import Binding
@@ -120,16 +121,15 @@
             with VerticalScroll(id="app-notes-container"):
                 yield Label("", id="app-description")
 
     def on_mount(self) -> None:
         """
         screen and box border styling
         """
-        self.title = "ʕ ᵔᴥᵔʔ smol-k8s-lab "
-        sub_title = f"Apps Configuration for {self.app.current_cluster} (now with more 🦑)"
+        sub_title = f"Apps Configuration for {self.app.current_cluster}"
         self.sub_title = sub_title
 
         self.generate_app_selection_list()
 
         # if text to speech is on, read screen title
         self.call_after_refresh(self.app.play_screen_audio, screen="apps")
```

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # smol-k8s-lab libraries
-from smol_k8s_lab.constants import INITIAL_USR_CONFIG, XDG_CONFIG_FILE
+from smol_k8s_lab.constants import INITIAL_USR_CONFIG, XDG_CONFIG_FILE, VERSION
 from smol_k8s_lab.k8s_distros import check_all_contexts
 from smol_k8s_lab.tui.apps_screen import AppsConfigScreen
 from smol_k8s_lab.tui.base_widgets.audio_widget import SmolAudio
 from smol_k8s_lab.tui.base_widgets.cluster_modal import ClusterModalScreen
 from smol_k8s_lab.tui.base_widgets.new_cluster_input import NewClusterInput
 from smol_k8s_lab.tui.confirm_screen import ConfirmConfig
 from smol_k8s_lab.tui.distro_screen import DistroConfigScreen
@@ -95,14 +95,15 @@
         self.audio = audio
 
     def on_mount(self) -> None:
         """
         screen and box border styling + new cluster input + cluster table if clusters exists
         Also says the screen title outloud if there that feature is enabled
         """
+        self.title = f"ʕ ᵔᴥᵔʔ smol-k8s-lab {VERSION}"
         # main box title
         title = "[#ffaff9]Create[/] a [i]new[/] [#C1FF87]cluster[/] with the name below"
         self.get_widget_by_id("base-new-cluster-input-box-grid").border_title = title
 
         # get all clusters
         clusters = check_all_contexts()
```

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base_widgets/audio_widget.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/base_widgets/audio_widget.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/base_widgets/cluster_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/base_widgets/new_cluster_input.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/confirm_screen.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/confirm_screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3.11
 # smol-k8s-lab libraries
 from smol_k8s_lab.bitwarden.tui.bitwarden_credentials_modal_screen import (
         BitwardenCredentialsScreen)
+from smol_k8s_lab.constants import VERSION
 from smol_k8s_lab.utils.yaml_with_comments import syntax_highlighted_yaml
 
 # external libraries
 from os import environ as env
 from textual import on
 from textual.binding import Binding
 from textual.app import ComposeResult
@@ -92,15 +93,15 @@
             back = Button("✋Go Back", id="back-button")
             yield back
 
     def on_mount(self) -> None:
         """
         screen and box border styling
         """
-        self.title = "ʕ ᵔᴥᵔʔ smol-k8s-lab "
+        self.title = f"ʕ ᵔᴥᵔʔ smol-k8s-lab {VERSION}"
         sub_title = f"Review your configuration for {self.app.current_cluster} (last step!)"
         self.sub_title = sub_title
 
         self.call_after_refresh(self.app.play_screen_audio, screen="confirm")
 
         # confirm box title styling
         confirm_box = self.query_one(TabbedContent)
```

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/add_nodes_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/apps_config.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/apps_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/apps_init_config.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/apps_init_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/base.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/base.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/base_modal.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/base_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/cluster_modal.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/cluster_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/confirm.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/confirm.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/distro_config.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/distro_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/help.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/help.tcss`

 * *Files 17% similar despite different names*

```diff
@@ -18,22 +18,27 @@
 HelpScreen {
    align: center middle;
 }
 
 #help-container {
    align: center middle;
    padding-left: 1;
+   padding-right: 1;
    padding-top: 1;
-   width: 79;
-   height: 90%;
+   width: 84;
+   height: 92%;
    border: round $cornflower 80%;
    border-title-color: $sky_blue;
    border-subtitle-color: $sky_blue;
    background: $navy;
    grid-rows: 0.1fr 1fr;
    grid-gutter: 1;
 }
 
 #help-options {
    align: center middle;
    width: 100%;
 }
+
+#key-mappings-table {
+   width: 76;
+}
```

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/invalid_apps.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/invalid_apps.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/k3s.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/k3s.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/kind.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/kind.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/modify_globals_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/new_app_modal.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/new_app_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/node_inputs_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/node_modal.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/node_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/css/tui_config.tcss` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/css/tui_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_screen.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3.11
 # smol-k8s-lab libraries
-from smol_k8s_lab.constants import DEFAULT_DISTRO_OPTIONS
+from smol_k8s_lab.constants import DEFAULT_DISTRO_OPTIONS, VERSION
 from smol_k8s_lab.env_config import process_k8s_distros
 from smol_k8s_lab.tui.distro_widgets.k3s_config import K3sConfigWidget
 from smol_k8s_lab.tui.distro_widgets.kind_config import (KindNetworkingConfig,
                                                          KindConfigWidget)
 from smol_k8s_lab.tui.util import NewOptionModal
 
 # external libraries
@@ -102,15 +102,14 @@
                                 id="distro-description")
 
 
     def on_mount(self) -> None:
         """
         screen and box border styling
         """
-        self.title = "ʕ ᵔᴥᵔʔ smol-k8s-lab "
         sub_title = f"Kubernetes distro config for {self.app.current_cluster}"
         self.sub_title = sub_title
 
         top_row = self.get_widget_by_id("top-distro-row")
         top_row.border_title = "🌱 Select a [#C1FF87]k8s distro[/]"
         top_row.border_subtitle = "[i]Inputs below are optional"
```

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/add_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-#!/usr/bin/env python3.11
-from smol_k8s_lab.constants import HOME_DIR
+from smol_k8s_lab.constants import HOME_DIR, VERSION
 from smol_k8s_lab.k8s_distros.k3s import join_k3s_nodes
 from smol_k8s_lab.k8s_tools.k8s_lib import K8s
 from smol_k8s_lab.tui.util import input_field, drop_down
 from smol_k8s_lab.tui.distro_widgets.modify_node_modal import NodeModalScreen
 
 from os.path import join
 from rich.text import Text
@@ -417,15 +416,15 @@
                               existing_cluster=self.existing_cluster,
                               id=self.node_box_id)
 
     def on_mount(self) -> None:
         """
         screen and box border styling
         """
-        self.title = "ʕ ᵔᴥᵔʔ smol-k8s-lab "
+        self.title = f"ʕ ᵔᴥᵔʔ smol-k8s-lab {VERSION}"
         sub_title = f"Kubernetes nodes config for {self.app.current_cluster}"
         self.sub_title = sub_title
 
         self.call_after_refresh(self.app.play_screen_audio, screen="nodes")
 
     def action_add_node(self) -> None:
         """
```

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/k3s_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/kind_config.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/kind_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/kubelet_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/distro_widgets/node_adjustment.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/help_screen.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/help_screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3.11
+from smol_k8s_lab.constants import VERSION
 from rich.text import Text
 from textual.app import ComposeResult
 from textual.containers import Grid
 from textual.binding import Binding
 from textual.screen import ModalScreen
 from textual.widgets import Label, DataTable
 
@@ -36,15 +37,15 @@
             yield Label(welcome, classes="help-text")
             yield Grid(id="help-options")
 
     def on_mount(self) -> None:
         # styling for the select-apps tab - select apps container - left
         select_apps_title = ('[i]Welcome[/] to [steel_blue]'
                              '[link=https://github.com/small-hack/smol-k8s-lab]'
-                             'smol-k8s-lab[/][/]')
+                             f'smol-k8s-lab[/][/] v{VERSION}')
         help_container = self.get_widget_by_id("help-container")
         help_container.border_title = select_apps_title
         help_container.border_subtitle = (
                 "made with 💙 + 🐍 + [steel_blue][i][link="
                 "https://github.com/Textualize/textual]textual[/][/][/]"
                 )
```

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/make_screenshots.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/make_screenshots.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/smol_k8s_config_screen.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/smol_k8s_config_screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,14 @@
             # configure command to run after tui phase
             yield RunCommandConfig(self.cfg['run_command'])
 
     def on_mount(self) -> None:
         """
         screen and box border styling
         """
-        self.title = "ʕ ᵔᴥᵔʔ smol k8s lab"
         sub_title = "Configure logging and password manager"
         self.sub_title = sub_title
 
         self.call_after_refresh(self.app.play_screen_audio, screen="config")
 
 
 class LoggingConfig(Widget):
```

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/tui_config_screen.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/tui_config_screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from smol_k8s_lab.constants import VERSION
 from smol_k8s_lab.tui.util import bool_option, input_field
 from textual import on
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Grid
 from textual.screen import Screen
-from textual.widgets import Footer, Header, Input, Label, Switch
+from textual.widgets import Footer, Header, Input, Switch
 from textual.widget import Widget
 
 
 class TuiConfigScreen(Screen):
     """
     Textual app to configure smol-k8s-lab itself
     """
@@ -45,15 +46,14 @@
             # tui config for hide_footer, enabled
             yield TuiConfig(self.cfg, id="tui-config")
 
     def on_mount(self) -> None:
         """
         screen and box border styling and read the screen title aloud
         """
-        self.title = "ʕ ᵔᴥᵔʔ smol k8s lab"
         sub_title = "Configure Terminal UI and Accessibility features"
         self.sub_title = sub_title
 
         # turn on the footer if it's enabled in the root app cfg
         if self.app.cfg['smol_k8s_lab']['tui']['show_footer']:
             self.query_one(Footer).display = True
```

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/util.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/tui/validators/already_exists.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/tui/validators/already_exists.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/minio_lib.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/utils/minio_lib.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/passwords.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/utils/passwords.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/rich_cli/console_logging.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/utils/rich_cli/console_logging.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/rich_cli/help_text.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/utils/rich_cli/help_text.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/run/final_cmd.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/utils/run/final_cmd.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/run/subproc.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/utils/run/subproc.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/smol_k8s_lab/utils/value_from.py` & `smol_k8s_lab-5.0.1/smol_k8s_lab/utils/value_from.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.0/PKG-INFO` & `smol_k8s_lab-5.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smol_k8s_lab
-Version: 5.0.0
+Version: 5.0.1
 Summary: CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD
 Home-page: https://small-hack.github.io/smol-k8s-lab
 License: AGPL-3.0-or-later
 Keywords: kubernetes,homelab,kind,k3s,k8s
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<3.13
@@ -63,16 +63,30 @@
 ### Features
 - Deploys [Argo CD](https://github.com/argoproj/argo-cd) by default, so you can manage your entire lab using files in [open source git repos](https://github.com/small-hack/argocd-apps)
   - Argo CD ships with a dashboard with a custom theme 💙
 - Supports multiple [k8s distros](#supported-k8s-distributions)
 - Specializes in using Bitwarden (though not required) to store sensitive values both locally and on your cluster
 - Manages all your authentication needs centrally using Zitadel and Vouch 💪
 - Supports initialization on a [range of common self-hosted apps](https://small-hack.github.io/smol-k8s-lab/k8s_apps/argocd/) 📱
+  - featured initialized apps such as [Nextcloud](https://small-hack.github.io/smol-k8s-lab/k8s_apps/nextcloud/), [Matrix](https://small-hack.github.io/smol-k8s-lab/k8s_apps/matrix/), and [Home Assistant](https://small-hack.github.io/smol-k8s-lab/k8s_apps/home_assistant/) include backups
 - Lots o' [docs](https://small-hack.github.io/smol-k8s-lab)
 
+-----------------------------
+
+* [Installation](#installation)
+    * [pipx](#pipx)
+    * [brew (still unstable)](#brew-still-unstable)
+    * [Usage](#usage)
+        * [Initialization](#initialization)
+* [Under the hood](#under-the-hood)
+    * [Supported k8s distributions](#supported-k8s-distributions)
+    * [Default Installed Applications](#default-installed-applications)
+* [Status](#status)
+
+
 # Installation
 B sure to check out our full [installation guide](https://small-hack.github.io/smol-k8s-lab/installation/), but the gist of it is `smol-k8s-lab` can be installed via `pipx` (or `brew` coming soon).
 
 ## pipx
 `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://github.com/pypa/pipx)). If you've already got both and [other pre-reqs](https://small-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be able to:
 
 ```bash
@@ -112,14 +126,51 @@
 After you've followed the installation instructions, if you're *new* to `smol-k8s-lab`,  initialize a new config file:
 
 ```bash
 # we'll walk you through any configuration needed before
 # saving the config and deploying it for you
 smol-k8s-lab
 ```
+
+<details>
+  <summary><b>Upgrading config from v4.x to v5.x</b></summary>
+
+If you've installed smol-k8s-lab prior to `v5.0.0`, please backup your old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the following with either pip or pipx:
+
+*if using pip*:
+```yaml
+# this uninstalls the old smol-k8s-lab for python 3.11
+pip3.11 uninstall smol-k8s-lab
+
+# this installs smol-k8s-lab for python 3.12
+pip3.12 install --upgrade smol-k8s-lab
+
+# this initializes a new configuration
+smol-k8s-lab
+```
+
+*or if using pipx*:
+```yaml
+# this upgrades smol-k8s-lab
+pipx upgrade smol-k8s-lab
+
+# this initializes a new configuration
+smol-k8s-lab
+```
+
+We have done a *masive* upgrade of the config file. You'll need to update your configs based on the details in https://github.com/small-hack/smol-k8s-lab/pull/210 . The main changes are to the following (check each doc link for details):
+
+- [accessibility features](https://small-hack.github.io/smol-k8s-lab/config_file/#tui-and-accessibility-configuration)
+- [k3s nodes section](https://small-hack.github.io/smol-k8s-lab/config_file/#k3s)
+- [backups and restores](https://small-hack.github.io/smol-k8s-lab/config_file/#backups-and-restores)
+- [sensitive values](https://small-hack.github.io/smol-k8s-lab/config_file/#sensitive-values)
+- [k9s has been removed in favor of run command](https://small-hack.github.io/smol-k8s-lab/config_file/#run-command) (hint: you can still use k9s via run command)
+
+</details>
+
 <details>
   <summary><b>Upgrading config from v3.7.1 to v4.x</b></summary>
 
 If you've installed smol-k8s-lab prior to `v4.0.0`, please backup your old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the following with either pip or pipx:
 
 *if using pip*:
 ```yaml
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smol_k8s_lab Version: 5.0.0 Summary: CLI and TUI to
+Metadata-Version: 2.1 Name: smol_k8s_lab Version: 5.0.1 Summary: CLI and TUI to
 quickly install slimmer Kubernetes distros and then manage apps declaratively
 using Argo CD Home-page: https://small-hack.github.io/smol-k8s-lab License:
 AGPL-3.0-or-later Keywords: kubernetes,homelab,kind,k3s,k8s Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<3.13 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Operating System :: MacOS :: MacOS X
@@ -37,76 +37,105 @@
 default, so you can manage your entire lab using files in [open source git
 repos](https://github.com/small-hack/argocd-apps) - Argo CD ships with a
 dashboard with a custom theme ð - Supports multiple [k8s distros]
 (#supported-k8s-distributions) - Specializes in using Bitwarden (though not
 required) to store sensitive values both locally and on your cluster - Manages
 all your authentication needs centrally using Zitadel and Vouch ðª - Supports
 initialization on a [range of common self-hosted apps](https://small-
-hack.github.io/smol-k8s-lab/k8s_apps/argocd/) ð± - Lots o' [docs](https://
-small-hack.github.io/smol-k8s-lab) # Installation B sure to check out our full
-[installation guide](https://small-hack.github.io/smol-k8s-lab/installation/),
-but the gist of it is `smol-k8s-lab` can be installed via `pipx` (or `brew`
-coming soon). ## pipx `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://
-github.com/pypa/pipx)). If you've already got both and [other pre-reqs](https:/
-/small-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be
-able to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help
-menu before proceeding smol-k8s-lab --help ``` ## brew (still unstable)
-[`brew`] is the future preferred installation method for macOS/Debian/Ubuntu,
-as this will also install any non-python prerequisites you need, so you don't
-need to worry about them. This method is new, so please [let us know if
-anything isn't working for you](https://github.com/small-hack/homebrew-tap/
-issues). ```bash # tap the special homebrew repo for our formula and install it
-brew install small-hack/tap/smol-k8s-lab ``` Then you should be able to check
-the version and cli options with: ```bash smol-k8s-lab --help ```
+hack.github.io/smol-k8s-lab/k8s_apps/argocd/) ð± - featured initialized apps
+such as [Nextcloud](https://small-hack.github.io/smol-k8s-lab/k8s_apps/
+nextcloud/), [Matrix](https://small-hack.github.io/smol-k8s-lab/k8s_apps/
+matrix/), and [Home Assistant](https://small-hack.github.io/smol-k8s-lab/
+k8s_apps/home_assistant/) include backups - Lots o' [docs](https://small-
+hack.github.io/smol-k8s-lab) ----------------------------- * [Installation]
+(#installation) * [pipx](#pipx) * [brew (still unstable)](#brew-still-unstable)
+* [Usage](#usage) * [Initialization](#initialization) * [Under the hood]
+(#under-the-hood) * [Supported k8s distributions](#supported-k8s-distributions)
+* [Default Installed Applications](#default-installed-applications) * [Status]
+(#status) # Installation B sure to check out our full [installation guide]
+(https://small-hack.github.io/smol-k8s-lab/installation/), but the gist of it
+is `smol-k8s-lab` can be installed via `pipx` (or `brew` coming soon). ## pipx
+`smol-k8s-lab` requires Python 3.11+ (and [pipx](https://github.com/pypa/
+pipx)). If you've already got both and [other pre-reqs](https://small-
+hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be able
+to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help menu
+before proceeding smol-k8s-lab --help ``` ## brew (still unstable) [`brew`] is
+the future preferred installation method for macOS/Debian/Ubuntu, as this will
+also install any non-python prerequisites you need, so you don't need to worry
+about them. This method is new, so please [let us know if anything isn't
+working for you](https://github.com/small-hack/homebrew-tap/issues). ```bash #
+tap the special homebrew repo for our formula and install it brew install
+small-hack/tap/smol-k8s-lab ``` Then you should be able to check the version
+and cli options with: ```bash smol-k8s-lab --help ```
  _[_O_u_t_p_u_t_ _o_f_ _s_m_o_l_-_k_8_s_-_l_a_b_ _-_-_h_e_l_p_ _a_f_t_e_r_ _c_l_o_n_i_n_g_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g_ _t_h_e
                                 _p_r_e_r_e_q_u_i_s_i_t_e_s_._]
 Checkout our [TUI docs](https://small-hack.github.io/smol-k8s-lab/tui/
 create_modify_screens/) for more info on how to get started playing with `smol-
 k8s-lab` :-) ## Usage ### Initialization After you've followed the installation
 instructions, if you're *new* to `smol-k8s-lab`, initialize a new config file:
 ```bash # we'll walk you through any configuration needed before # saving the
-config and deploying it for you smol-k8s-lab ``` UUppggrraaddiinngg ccoonnffiigg ffrroomm vv33..77..11
-ttoo vv44..xx If you've installed smol-k8s-lab prior to `v4.0.0`, please backup your
-old configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or
+config and deploying it for you smol-k8s-lab ``` UUppggrraaddiinngg ccoonnffiigg ffrroomm vv44..xx ttoo
+vv55..xx If you've installed smol-k8s-lab prior to `v5.0.0`, please backup your old
+configuration, and then remove the `~/.config/smol-k8s-lab/config.yaml` (or
 `$XDG_CONFIG_HOME/smol-k8s-lab/config.yaml`) file entirely, then run the
-following with either pip or pipx: *if using pip*: ```yaml # this upgrades
-smol-k8s-lab pip3.11 install --upgrade smol-k8s-lab # this initializes a new
-configuration smol-k8s-lab ``` *or if using pipx*: ```yaml # this upgrades
-smol-k8s-lab pipx upgrade smol-k8s-lab # this initializes a new configuration
-smol-k8s-lab ``` The main breaking changes between `v3.7.1` and `v4.0.0` are
-that we now default enable metrics on most apps. Because of this, you need to
-have the Prometheus ServiceMonitor CRD installed ahead of time. Luckily, we now
-provide that as an app as well :) If you deleted your config and created a new
-one, it will already be there, but if you want to reuse your old config, you
-can add the app like this: ```yaml apps: prometheus_crds: description: |
-[link=https://prometheus.io/docs/introduction/overview/]Prometheus[/link] CRDs
-to start with. You can optionally disable this if you don't want to deploy apps
-with metrics. enabled: true argo: # secrets keys to make available to Argo CD
-ApplicationSets secret_keys: {} # git repo to install the Argo CD app from
-repo: https://github.com/small-hack/argocd-apps # path in the argo repo to
-point to. Trailing slash very important! path: prometheus/crds/ # either the
-branch or tag to point at in the argo repo above revision: main # namespace to
-install the k8s app in namespace: prometheus # recurse directories in the
-provided git repo directory_recursion: false # source repos for Argo CD App
-Project (in addition to argo.repo) project: name: prometheus source_repos: -
-https://github.com/prometheus-community/helm-charts.git destination: #
-automatically includes the app's namespace and argocd's namespace namespaces: -
-kube-system - prometheus ``` If using the default repos, please also disable
-directory directory_recursion for: - your prometheus stack app - zitadel For
-all changes, please check out [PR #206](https://github.com/small-hack/smol-k8s-
-lab/pull/206). UUppggrraaddiinngg ccoonnffiigg ffrroomm vv22..22..44 ttoo vv33..xx If you've installed smol-
-k8s-lab prior to `v3.0.0`, please backup your old configuration, and then
-remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-
-lab/config.yaml`) file entirely, then run the following with either pip or
-pipx: *if using pip*: ```yaml # this upgrades smol-k8s-lab pip3.11 install --
-upgrade smol-k8s-lab # this initializes a new configuration smol-k8s-lab ```
-*or if using pipx*: ```yaml # this upgrades smol-k8s-lab pipx upgrade smol-k8s-
-lab # this initializes a new configuration smol-k8s-lab ``` The main breaking
-changes between `v2.2.4` and `v3.0` are as follows: - *home assistant has
-graduated from demo app to live app* You'll need to change
+following with either pip or pipx: *if using pip*: ```yaml # this uninstalls
+the old smol-k8s-lab for python 3.11 pip3.11 uninstall smol-k8s-lab # this
+installs smol-k8s-lab for python 3.12 pip3.12 install --upgrade smol-k8s-lab #
+this initializes a new configuration smol-k8s-lab ``` *or if using pipx*:
+```yaml # this upgrades smol-k8s-lab pipx upgrade smol-k8s-lab # this
+initializes a new configuration smol-k8s-lab ``` We have done a *masive*
+upgrade of the config file. You'll need to update your configs based on the
+details in https://github.com/small-hack/smol-k8s-lab/pull/210 . The main
+changes are to the following (check each doc link for details): -
+[accessibility features](https://small-hack.github.io/smol-k8s-lab/config_file/
+#tui-and-accessibility-configuration) - [k3s nodes section](https://small-
+hack.github.io/smol-k8s-lab/config_file/#k3s) - [backups and restores](https://
+small-hack.github.io/smol-k8s-lab/config_file/#backups-and-restores) -
+[sensitive values](https://small-hack.github.io/smol-k8s-lab/config_file/
+#sensitive-values) - [k9s has been removed in favor of run command](https://
+small-hack.github.io/smol-k8s-lab/config_file/#run-command) (hint: you can
+still use k9s via run command) UUppggrraaddiinngg ccoonnffiigg ffrroomm vv33..77..11 ttoo vv44..xx If you've
+installed smol-k8s-lab prior to `v4.0.0`, please backup your old configuration,
+and then remove the `~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/
+smol-k8s-lab/config.yaml`) file entirely, then run the following with either
+pip or pipx: *if using pip*: ```yaml # this upgrades smol-k8s-lab pip3.11
+install --upgrade smol-k8s-lab # this initializes a new configuration smol-k8s-
+lab ``` *or if using pipx*: ```yaml # this upgrades smol-k8s-lab pipx upgrade
+smol-k8s-lab # this initializes a new configuration smol-k8s-lab ``` The main
+breaking changes between `v3.7.1` and `v4.0.0` are that we now default enable
+metrics on most apps. Because of this, you need to have the Prometheus
+ServiceMonitor CRD installed ahead of time. Luckily, we now provide that as an
+app as well :) If you deleted your config and created a new one, it will
+already be there, but if you want to reuse your old config, you can add the app
+like this: ```yaml apps: prometheus_crds: description: | [link=https://
+prometheus.io/docs/introduction/overview/]Prometheus[/link] CRDs to start with.
+You can optionally disable this if you don't want to deploy apps with metrics.
+enabled: true argo: # secrets keys to make available to Argo CD ApplicationSets
+secret_keys: {} # git repo to install the Argo CD app from repo: https://
+github.com/small-hack/argocd-apps # path in the argo repo to point to. Trailing
+slash very important! path: prometheus/crds/ # either the branch or tag to
+point at in the argo repo above revision: main # namespace to install the k8s
+app in namespace: prometheus # recurse directories in the provided git repo
+directory_recursion: false # source repos for Argo CD App Project (in addition
+to argo.repo) project: name: prometheus source_repos: - https://github.com/
+prometheus-community/helm-charts.git destination: # automatically includes the
+app's namespace and argocd's namespace namespaces: - kube-system - prometheus
+``` If using the default repos, please also disable directory
+directory_recursion for: - your prometheus stack app - zitadel For all changes,
+please check out [PR #206](https://github.com/small-hack/smol-k8s-lab/pull/
+206). UUppggrraaddiinngg ccoonnffiigg ffrroomm vv22..22..44 ttoo vv33..xx If you've installed smol-k8s-lab
+prior to `v3.0.0`, please backup your old configuration, and then remove the
+`~/.config/smol-k8s-lab/config.yaml` (or `$XDG_CONFIG_HOME/smol-k8s-lab/
+config.yaml`) file entirely, then run the following with either pip or pipx:
+*if using pip*: ```yaml # this upgrades smol-k8s-lab pip3.11 install --upgrade
+smol-k8s-lab # this initializes a new configuration smol-k8s-lab ``` *or if
+using pipx*: ```yaml # this upgrades smol-k8s-lab pipx upgrade smol-k8s-lab #
+this initializes a new configuration smol-k8s-lab ``` The main breaking changes
+between `v2.2.4` and `v3.0` are as follows: - *home assistant has graduated
+from demo app to live app* You'll need to change
 `apps.home_assistant.argo.path` to either `home-assistant/
 toleration_and_affinity/` if you're using node labels and taints, or `home-
 assistant/` if you're deploying to a single node cluster. Here's an example
 with no tolerations or node affinity: ```yaml apps: home_assistant: enabled:
 false description: | [link=https://home-assistant.io]Home Assistant[/link] is a
 home IOT management solution. By default, we assume you want to use node
 affinity and tolerations to keep home assistant pods on certain nodes and keep
```

