# Comparing `tmp/lungo_cli-0.3.0.tar.gz` & `tmp/lungo_cli-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lungo_cli-0.3.0.tar", max compression
+gzip compressed data, was "lungo_cli-0.4.0.tar", max compression
```

## Comparing `lungo_cli-0.3.0.tar` & `lungo_cli-0.4.0.tar`

### file list

```diff
@@ -1,276 +1,296 @@
--rw-r--r--   0        0        0     1075 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0     2410 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/README.md
--rw-r--r--   0        0        0     1116 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/src/lungo_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/src/lungo_cli/app/__init__.py
--rw-r--r--   0        0        0     1264 2024-04-14 19:09:33.552501 lungo_cli-0.3.0/src/lungo_cli/app/main.py
--rw-r--r--   0        0        0     1551 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/app/state.py
--rw-r--r--   0        0        0        0 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/__init__.py
--rw-r--r--   0        0        0      743 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/base.py
--rw-r--r--   0        0        0      478 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/check.py
--rw-r--r--   0        0        0      922 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/down.py
--rw-r--r--   0        0        0     1244 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/install.py
--rw-r--r--   0        0        0     3370 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/list.py
--rw-r--r--   0        0        0     1241 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/uninstall.py
--rw-r--r--   0        0        0     2705 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/commands/up.py
--rw-r--r--   0        0        0        0 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/__init__.py
--rw-r--r--   0        0        0    12436 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/app.py
--rw-r--r--   0        0        0     5973 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/console.py
--rw-r--r--   0        0        0      569 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/constants.py
--rw-r--r--   0        0        0     7390 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/container.py
--rw-r--r--   0        0        0     3174 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/context.py
--rw-r--r--   0        0        0    10206 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/database.py
--rw-r--r--   0        0        0     5978 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/file.py
--rw-r--r--   0        0        0     2599 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/network.py
--rw-r--r--   0        0        0    11815 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/plugin.py
--rw-r--r--   0        0        0     2452 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/renderer.py
--rw-r--r--   0        0        0     5901 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/core/storage.py
--rw-r--r--   0        0        0        0 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/helpers/__init__.py
--rw-r--r--   0        0        0     1275 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/helpers/common.py
--rw-r--r--   0        0        0     1873 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/helpers/crypto.py
--rw-r--r--   0        0        0     1071 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/helpers/format.py
--rw-r--r--   0        0        0        0 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/__init__.py
--rw-r--r--   0        0        0     1002 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/base.py
--rw-r--r--   0        0        0     2876 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/config.py
--rw-r--r--   0        0        0      482 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/context.py
--rw-r--r--   0        0        0      588 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/plugin.py
--rw-r--r--   0        0        0     1865 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/models/users.py
--rw-r--r--   0        0        0        0 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/__init__.py
--rw-r--r--   0        0        0      686 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/Dockerfile.jinja
--rw-r--r--   0        0        0      280 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/README.md
--rw-r--r--   0        0        0     1958 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/compose/compose.yaml.jinja
--rw-r--r--   0        0        0     1197 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/config/config_export.yaml
--rw-r--r--   0        0        0      156 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/config/settings.yaml
--rw-r--r--   0        0        0     1354 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/config/users_export.yaml.jinja
--rw-r--r--   0        0        0     1254 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/nginx/site.conf.jinja
--rw-r--r--   0        0        0      125 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/nginx/upstream.conf.jinja
--rw-r--r--   0        0        0      864 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/oathkeeper/access_rules.yaml.jinja
--rw-r--r--   0        0        0      485 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/plugin.py
--rw-r--r--   0        0        0      792 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderOutline.svelte
--rw-r--r--   0        0        0      734 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderSolid.svelte
--rw-r--r--   0        0        0      100 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/web/routes/[...url]/+page.svelte
--rw-r--r--   0        0        0     1121 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/Dockerfile.jinja
--rw-r--r--   0        0        0      427 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/README.md
--rw-r--r--   0        0        0     1457 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/compose/compose.yaml.jinja
--rw-r--r--   0        0        0     2734 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/config/config.py.jinja
--rw-r--r--   0        0        0     1148 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/nginx/site.conf.jinja
--rw-r--r--   0        0        0      124 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/nginx/upstream.conf.jinja
--rw-r--r--   0        0        0     1624 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/plugin.py
--rw-r--r--   0        0        0       20 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/dependencies.txt
--rw-r--r--   0        0        0     2025 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/lib/icons/Jupyter.svelte
--rw-r--r--   0        0        0       76 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/lib/server/constants.server.ts
--rw-r--r--   0        0        0      144 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/lib/server/constants.server.ts.jinja
--rw-r--r--   0        0        0     1204 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/routes/+layout.server.ts
--rw-r--r--   0        0        0      100 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/routes/[...url]/+page.svelte
--rw-r--r--   0        0        0      384 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/Dockerfile.jinja
--rw-r--r--   0        0        0      275 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/README.md
--rw-r--r--   0        0        0      494 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/compose/compose.yaml.jinja
--rw-r--r--   0        0        0     7466 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/config/conf.php.jinja
--rw-r--r--   0        0        0      765 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/config/site.conf
--rw-r--r--   0        0        0     1115 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/nginx/site.conf.jinja
--rw-r--r--   0        0        0      124 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/nginx/upstream.conf.jinja
--rw-r--r--   0        0        0      865 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/oathkeeper/access_rules.yaml.jinja
--rw-r--r--   0        0        0      691 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/plugin.py
--rw-r--r--   0        0        0      700 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteOutline.svelte
--rw-r--r--   0        0        0      672 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteSolid.svelte
--rw-r--r--   0        0        0      100 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/web/routes/[...url]/+page.svelte
--rw-r--r--   0        0        0      925 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/Dockerfile.jinja
--rw-r--r--   0        0        0      418 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/README.md
--rw-r--r--   0        0        0     1305 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/compose/compose.yaml.jinja
--rw-r--r--   0        0        0      103 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/config/rserver.conf
--rw-r--r--   0        0        0       30 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/config/rsession.conf
--rw-r--r--   0        0        0     1351 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/nginx/site.conf.jinja
--rw-r--r--   0        0        0      121 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/nginx/upstream.conf.jinja
--rw-r--r--   0        0        0     1309 2024-04-14 19:09:33.556501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/plugin.py
--rw-r--r--   0        0        0       20 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/dependencies.txt
--rw-r--r--   0        0        0     1820 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioOutline.svelte
--rw-r--r--   0        0        0     1563 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioSolid.svelte
--rw-r--r--   0        0        0       70 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/server/constants.server.ts
--rw-r--r--   0        0        0      132 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/server/constants.server.ts.jinja
--rw-r--r--   0        0        0     2118 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/routes/+layout.server.ts
--rw-r--r--   0        0        0      100 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/routes/[...url]/+page.svelte
--rw-r--r--   0        0        0      991 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/README.md
--rw-r--r--   0        0        0      502 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/compose/compose.yaml.jinja
--rw-r--r--   0        0        0     1174 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/config/config.json.jinja
--rw-r--r--   0        0        0      362 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/nginx/site.conf.jinja
--rw-r--r--   0        0        0      118 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/nginx/upstream.conf.jinja
--rw-r--r--   0        0        0     1588 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/plugin.py
--rw-r--r--   0        0        0       33 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/dependencies.txt
--rw-r--r--   0        0        0     1594 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/components/CodeBlock.svelte
--rw-r--r--   0        0        0     2133 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/NetworkLock.svelte
--rw-r--r--   0        0        0     1897 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxyOutline.svelte
--rw-r--r--   0        0        0     1808 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxySolid.svelte
--rw-r--r--   0        0        0      205 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/server/constants.server.ts
--rw-r--r--   0        0        0      437 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/server/constants.server.ts.jinja
--rw-r--r--   0        0        0      775 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/routes/+page.server.ts
--rw-r--r--   0        0        0     6649 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/routes/+page.svelte
--rw-r--r--   0        0        0        0 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/__init__.py
--rw-r--r--   0        0        0     5623 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/assets/config_references/config.yaml
--rw-r--r--   0        0        0     1995 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/assets/config_references/users.yaml
--rw-r--r--   0        0        0     6798 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/compose.yaml.jinja
--rw-r--r--   0        0        0      363 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/keto/config.yaml.jinja
--rw-r--r--   0        0        0     2116 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/config.yaml.jinja
--rw-r--r--   0        0        0    14236 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.gotmpl.jinja
--rw-r--r--   0        0        0      408 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.plaintext.gotmpl.jinja
--rw-r--r--   0        0        0       51 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.subject.gotmpl.jinja
--rw-r--r--   0        0        0    14238 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja
--rw-r--r--   0        0        0      410 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.plaintext.gotmpl.jinja
--rw-r--r--   0        0        0       50 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.subject.gotmpl.jinja
--rw-r--r--   0        0        0     2801 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/user.schema.json
--rw-r--r--   0        0        0     1281 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja
--rw-r--r--   0        0        0       92 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/custom.d/jit.conf
--rw-r--r--   0        0        0      203 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/sites/apps.conf.jinja
--rw-r--r--   0        0        0      911 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf
--rw-r--r--   0        0        0      712 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/snippets/auth.conf
--rw-r--r--   0        0        0      592 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/snippets/proxy.conf
--rw-r--r--   0        0        0      375 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/snippets/upstreams.conf.jinja
--rw-r--r--   0        0        0     2257 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja
--rw-r--r--   0        0        0       92 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/custom.d/jit.conf
--rw-r--r--   0        0        0       90 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/snippets/certificate.conf
--rw-r--r--   0        0        0     1586 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja
--rw-r--r--   0        0        0     1609 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja
--rw-r--r--   0        0        0     1303 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja
--rw-r--r--   0        0        0     1634 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja
--rw-r--r--   0        0        0      474 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/dockerfiles/keto_admin/compose.yaml.jinja
--rw-r--r--   0        0        0      820 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja
--rw-r--r--   0        0        0      859 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja
--rw-r--r--   0        0        0       82 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/excluded/kratos/secrets.yaml.jinja
--rw-r--r--   0        0        0      426 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.editorconfig
--rw-r--r--   0        0        0       93 2024-04-14 19:09:33.992508 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.git
--rw-r--r--   0        0        0      519 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes
--rw-r--r--   0        0        0      128 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODEOWNERS
--rw-r--r--   0        0        0      121 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     5476 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      323 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/FUNDING.yml
--rw-r--r--   0        0        0      105 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/dependabot.yml
--rw-r--r--   0        0        0      958 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml
--rw-r--r--   0        0        0      322 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1284 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml
--rw-r--r--   0        0        0       91 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.gitignore
--rw-r--r--   0        0        0    41306 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md
--rw-r--r--   0        0        0     1043 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt
--rw-r--r--   0        0        0     4817 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/README.md
--rw-r--r--   0        0        0      763 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf
--rw-r--r--   0        0        0      932 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf
--rw-r--r--   0        0        0     1434 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf
--rw-r--r--   0        0        0     1133 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf
--rw-r--r--   0        0        0      314 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/basic.conf
--rw-r--r--   0        0        0      739 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf
--rw-r--r--   0        0        0      761 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf
--rw-r--r--   0        0        0      385 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/errors/custom_errors.conf
--rw-r--r--   0        0        0     1706 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf
--rw-r--r--   0        0        0      701 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf
--rw-r--r--   0        0        0      685 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf
--rw-r--r--   0        0        0     1029 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf
--rw-r--r--   0        0        0      650 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf
--rw-r--r--   0        0        0     1198 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf
--rw-r--r--   0        0        0     2102 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf
--rw-r--r--   0        0        0     1121 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf
--rw-r--r--   0        0        0     1135 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf
--rw-r--r--   0        0        0      396 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/server_software_information.conf
--rw-r--r--   0        0        0     2008 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf
--rw-r--r--   0        0        0      871 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf
--rw-r--r--   0        0        0     1800 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf
--rw-r--r--   0        0        0     1136 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf
--rw-r--r--   0        0        0     1235 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf
--rw-r--r--   0        0        0      797 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf
--rw-r--r--   0        0        0     1818 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf
--rw-r--r--   0        0        0     1880 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf
--rw-r--r--   0        0        0     2202 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf
--rw-r--r--   0        0        0     1484 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf
--rw-r--r--   0        0        0     2220 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf
--rw-r--r--   0        0        0     2049 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf
--rw-r--r--   0        0        0     1435 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf
--rw-r--r--   0        0        0      732 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf
--rw-r--r--   0        0        0      572 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf
--rw-r--r--   0        0        0     5775 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types
--rw-r--r--   0        0        0     7293 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf
--rw-r--r--   0        0        0      399 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/default.conf
--rw-r--r--   0        0        0      678 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf
--rw-r--r--   0        0        0      782 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf
--rw-r--r--   0        0        0      126 2024-04-14 19:09:34.644518 lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/www-server.localhost.conf
--rw-r--r--   0        0        0      161 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.dockerignore
--rw-r--r--   0        0        0      160 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.eslintignore
--rw-r--r--   0        0        0      702 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.eslintrc.cjs
--rw-r--r--   0        0        0       19 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.npmrc
--rw-r--r--   0        0        0      160 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.prettierignore
--rw-r--r--   0        0        0      351 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/.prettierrc
--rw-r--r--   0        0        0      773 2024-04-14 19:09:33.560501 lungo_cli-0.3.0/src/lungo_cli/resources/web/Dockerfile.jinja
--rw-r--r--   0        0        0    40573 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json
--rw-r--r--   0        0        0   300951 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json
--rw-r--r--   0        0        0     1728 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/package.json
--rw-r--r--   0        0        0   115548 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/pnpm-lock.yaml
--rw-r--r--   0        0        0      264 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/postcss.config.cjs
--rw-r--r--   0        0        0      304 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/app.d.ts
--rw-r--r--   0        0        0      352 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/app.html
--rw-r--r--   0        0        0     1736 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/app.pcss
--rw-r--r--   0        0        0      248 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/hooks.server.ts
--rw-r--r--   0        0        0     3137 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/actions.ts
--rw-r--r--   0        0        0   146031 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/assets/cover.jpg
--rw-r--r--   0        0        0     1713 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/AccountDropdown.svelte
--rw-r--r--   0        0        0     5068 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/AppShell.svelte
--rw-r--r--   0        0        0     7325 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte
--rw-r--r--   0        0        0      556 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/HeroFrame.svelte
--rw-r--r--   0        0        0      618 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte
--rw-r--r--   0        0        0     1525 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte
--rw-r--r--   0        0        0      887 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte
--rw-r--r--   0        0        0     6343 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/PatchedIFrame.svelte
--rw-r--r--   0        0        0      608 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/SwappableIcon.svelte
--rw-r--r--   0        0        0     1691 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/ThemeSelector.svelte
--rw-r--r--   0        0        0     1719 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/ThemeSelectorDropdown.svelte
--rw-r--r--   0        0        0      566 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/index.ts
--rw-r--r--   0        0        0      237 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/constants.ts
--rw-r--r--   0        0        0     2166 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Account.svelte
--rw-r--r--   0        0        0      414 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/BaseIcon.svelte
--rw-r--r--   0        0        0      432 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Check.svelte
--rw-r--r--   0        0        0     1031 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Close.svelte
--rw-r--r--   0        0        0     1337 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte
--rw-r--r--   0        0        0      427 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Expand.svelte
--rw-r--r--   0        0        0      522 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte
--rw-r--r--   0        0        0     3326 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte
--rw-r--r--   0        0        0      617 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte
--rw-r--r--   0        0        0     1182 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte
--rw-r--r--   0        0        0     1259 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/QuestionMark.svelte
--rw-r--r--   0        0        0     1707 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte
--rw-r--r--   0        0        0     2164 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte
--rw-r--r--   0        0        0     1861 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte
--rw-r--r--   0        0        0     1476 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte
--rw-r--r--   0        0        0      836 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/index.ts
--rw-r--r--   0        0        0      158 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/constants.ts
--rw-r--r--   0        0        0      906 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/utils/api.ts
--rw-r--r--   0        0        0       98 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/utils/index.ts
--rw-r--r--   0        0        0      109 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts
--rw-r--r--   0        0        0      480 2024-04-14 19:09:33.564502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts.jinja
--rw-r--r--   0        0        0     2312 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/stores.ts
--rw-r--r--   0        0        0      307 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/common.ts
--rw-r--r--   0        0        0      247 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/index.ts
--rw-r--r--   0        0        0    31445 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/keto.d.ts
--rw-r--r--   0        0        0   298809 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts
--rw-r--r--   0        0        0      511 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/user.d.ts
--rw-r--r--   0        0        0     2463 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/api.ts
--rw-r--r--   0        0        0      483 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/app.ts
--rw-r--r--   0        0        0     2348 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/common.ts
--rw-r--r--   0        0        0      316 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/index.ts
--rw-r--r--   0        0        0      225 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/stubs.ts
--rw-r--r--   0        0        0     1130 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/stubs.ts.jinja
--rw-r--r--   0        0        0      289 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/+layout.svelte
--rw-r--r--   0        0        0     4621 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts
--rw-r--r--   0        0        0      335 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/account/+page.svelte
--rw-r--r--   0        0        0     6932 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts
--rw-r--r--   0        0        0      590 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte
--rw-r--r--   0        0        0      367 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/logout/+server.ts
--rw-r--r--   0        0        0     5081 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts
--rw-r--r--   0        0        0      369 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.svelte
--rw-r--r--   0        0        0      463 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(apps)/+layout.svelte
--rw-r--r--   0        0        0     1277 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte
--rw-r--r--   0        0        0      448 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(apps)/app/+layout.server.ts
--rw-r--r--   0        0        0      130 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(apps)/app/+page.server.ts
--rw-r--r--   0        0        0     1008 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+error.svelte
--rw-r--r--   0        0        0     2327 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+layout.server.ts
--rw-r--r--   0        0        0      963 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+layout.svelte
--rw-r--r--   0        0        0    25573 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/static/favicon.png
--rw-r--r--   0        0        0      276 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/svelte.config.js
--rw-r--r--   0        0        0     1835 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/tailwind.config.cjs
--rw-r--r--   0        0        0      601 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/tsconfig.json
--rw-r--r--   0        0        0      219 2024-04-14 19:09:33.568502 lungo_cli-0.3.0/src/lungo_cli/resources/web/vite.config.ts
--rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 lungo_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-15 09:34:34.020102 lungo_cli-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2410 2024-05-15 09:34:34.020102 lungo_cli-0.4.0/README.md
+-rw-r--r--   0        0        0     1116 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/app/__init__.py
+-rw-r--r--   0        0        0     1264 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/app/main.py
+-rw-r--r--   0        0        0     1562 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/app/state.py
+-rw-r--r--   0        0        0        0 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/commands/__init__.py
+-rw-r--r--   0        0        0      743 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/commands/base.py
+-rw-r--r--   0        0        0      478 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/commands/check.py
+-rw-r--r--   0        0        0      922 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/commands/down.py
+-rw-r--r--   0        0        0     1246 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/commands/install.py
+-rw-r--r--   0        0        0     3388 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/commands/list.py
+-rw-r--r--   0        0        0     1243 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/commands/uninstall.py
+-rw-r--r--   0        0        0     2188 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/commands/up.py
+-rw-r--r--   0        0        0        0 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/__init__.py
+-rw-r--r--   0        0        0    12557 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/app.py
+-rw-r--r--   0        0        0     5973 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/console.py
+-rw-r--r--   0        0        0     1042 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/constants.py
+-rw-r--r--   0        0        0     7390 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/container.py
+-rw-r--r--   0        0        0     4559 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/context.py
+-rw-r--r--   0        0        0    10356 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/database.py
+-rw-r--r--   0        0        0     5978 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/file.py
+-rw-r--r--   0        0        0     2599 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/network.py
+-rw-r--r--   0        0        0    17104 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/plugin.py
+-rw-r--r--   0        0        0     2315 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/renderer.py
+-rw-r--r--   0        0        0     6583 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/core/storage.py
+-rw-r--r--   0        0        0        0 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1275 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/helpers/common.py
+-rw-r--r--   0        0        0     2494 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/helpers/crypto.py
+-rw-r--r--   0        0        0     1077 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/helpers/format.py
+-rw-r--r--   0        0        0        0 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/models/__init__.py
+-rw-r--r--   0        0        0     1108 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/models/base.py
+-rw-r--r--   0        0        0     2876 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/models/config.py
+-rw-r--r--   0        0        0      676 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/models/context.py
+-rw-r--r--   0        0        0     2964 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/models/plugin.py
+-rw-r--r--   0        0        0     1865 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/models/users.py
+-rw-r--r--   0        0        0        0 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/__init__.py
+-rw-r--r--   0        0        0      660 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/Dockerfile.jinja
+-rw-r--r--   0        0        0      280 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/README.md
+-rw-r--r--   0        0        0     2037 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     1236 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/config/config_export.yaml.jinja
+-rw-r--r--   0        0        0      195 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/config/settings.yaml.jinja
+-rw-r--r--   0        0        0     1258 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/config/users_export.yaml.jinja
+-rw-r--r--   0        0        0     1300 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      928 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/oathkeeper/access_rules.yaml.jinja
+-rw-r--r--   0        0        0      813 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/plugin.py
+-rw-r--r--   0        0        0      792 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderOutline.svelte
+-rw-r--r--   0        0        0      734 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderSolid.svelte
+-rw-r--r--   0        0        0      136 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      100 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0     1100 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/Dockerfile.jinja
+-rw-r--r--   0        0        0      427 2024-05-15 09:34:34.024102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/README.md
+-rw-r--r--   0        0        0     1544 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     2774 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/config/config.py.jinja
+-rw-r--r--   0        0        0     1218 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/nginx/site.conf.jinja
+-rw-r--r--   0        0        0     1799 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/plugin.py
+-rw-r--r--   0        0        0       20 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/web/dependencies.txt
+-rw-r--r--   0        0        0     2025 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/web/lib/icons/Jupyter.svelte
+-rw-r--r--   0        0        0       58 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      116 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      207 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0     1336 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/web/routes/+layout.server.ts
+-rw-r--r--   0        0        0      100 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      366 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/Dockerfile.jinja
+-rw-r--r--   0        0        0      275 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/README.md
+-rw-r--r--   0        0        0      573 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     7494 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/config/conf.php.jinja
+-rw-r--r--   0        0        0      829 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/config/site.conf.jinja
+-rw-r--r--   0        0        0     1159 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      933 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/oathkeeper/access_rules.yaml.jinja
+-rw-r--r--   0        0        0     1030 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/plugin.py
+-rw-r--r--   0        0        0      700 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteOutline.svelte
+-rw-r--r--   0        0        0      672 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteSolid.svelte
+-rw-r--r--   0        0        0      128 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      100 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      919 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/Dockerfile.jinja
+-rw-r--r--   0        0        0      418 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/README.md
+-rw-r--r--   0        0        0     1416 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0      135 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/config/rserver.conf.jinja
+-rw-r--r--   0        0        0       30 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/config/rsession.conf
+-rw-r--r--   0        0        0     1432 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/nginx/site.conf.jinja
+-rw-r--r--   0        0        0     1435 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/plugin.py
+-rw-r--r--   0        0        0       20 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/dependencies.txt
+-rw-r--r--   0        0        0     1820 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioOutline.svelte
+-rw-r--r--   0        0        0     1563 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioSolid.svelte
+-rw-r--r--   0        0        0      140 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      107 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      195 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0     2216 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/routes/+layout.server.ts
+-rw-r--r--   0        0        0      100 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      269 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rustdesk/README.md
+-rw-r--r--   0        0        0      875 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rustdesk/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     1817 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rustdesk/plugin.py
+-rw-r--r--   0        0        0     1246 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rustdesk/web/lib/icons/Rustdesk.svelte
+-rw-r--r--   0        0        0     1257 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rustdesk/web/lib/icons/ScreenCast.svelte
+-rw-r--r--   0        0        0      124 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rustdesk/web/lib/icons/index.ts
+-rw-r--r--   0        0        0       74 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rustdesk/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      127 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rustdesk/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0      248 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rustdesk/web/routes/+page.server.ts
+-rw-r--r--   0        0        0     1586 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/rustdesk/web/routes/+page.svelte
+-rw-r--r--   0        0        0      118 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/stirlingpdf/Dockerfile.jinja
+-rw-r--r--   0        0        0      280 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/stirlingpdf/README.md
+-rw-r--r--   0        0        0      651 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/stirlingpdf/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0      295 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/stirlingpdf/config/settings.yaml
+-rw-r--r--   0        0        0     1013 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/stirlingpdf/nginx/site.conf.jinja
+-rw-r--r--   0        0        0      888 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/stirlingpdf/plugin.py
+-rw-r--r--   0        0        0     1444 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/stirlingpdf/web/lib/icons/StirlingPdf.svelte
+-rw-r--r--   0        0        0       66 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/stirlingpdf/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      100 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/stirlingpdf/web/routes/[...url]/+page.svelte
+-rw-r--r--   0        0        0      991 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/README.md
+-rw-r--r--   0        0        0      599 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/compose/compose.yaml.jinja
+-rw-r--r--   0        0        0     1234 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/config/config.json.jinja
+-rw-r--r--   0        0        0      423 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/nginx/site.conf.jinja
+-rw-r--r--   0        0        0     1692 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/plugin.py
+-rw-r--r--   0        0        0       33 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/dependencies.txt
+-rw-r--r--   0        0        0     1594 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/components/CodeBlock.svelte
+-rw-r--r--   0        0        0       58 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/components/index.ts
+-rw-r--r--   0        0        0     2133 2024-05-15 09:34:34.028102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/icons/NetworkLock.svelte
+-rw-r--r--   0        0        0     1897 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxyOutline.svelte
+-rw-r--r--   0        0        0     1808 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxySolid.svelte
+-rw-r--r--   0        0        0      198 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/icons/index.ts
+-rw-r--r--   0        0        0      239 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/server/constants.server.ts
+-rw-r--r--   0        0        0      508 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/server/constants.server.ts.jinja
+-rw-r--r--   0        0        0      836 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/routes/+page.server.ts
+-rw-r--r--   0        0        0     6645 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/routes/+page.svelte
+-rw-r--r--   0        0        0        0 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/__init__.py
+-rw-r--r--   0        0        0     5623 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/assets/config_references/config.yaml
+-rw-r--r--   0        0        0     1995 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/assets/config_references/users.yaml
+-rw-r--r--   0        0        0     6754 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/compose.yaml.jinja
+-rw-r--r--   0        0        0      363 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/keto/config.yaml.jinja
+-rw-r--r--   0        0        0     2116 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/config.yaml.jinja
+-rw-r--r--   0        0        0    14236 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.gotmpl.jinja
+-rw-r--r--   0        0        0      408 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.plaintext.gotmpl.jinja
+-rw-r--r--   0        0        0       51 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.subject.gotmpl.jinja
+-rw-r--r--   0        0        0    14238 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja
+-rw-r--r--   0        0        0      410 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.plaintext.gotmpl.jinja
+-rw-r--r--   0        0        0       50 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.subject.gotmpl.jinja
+-rw-r--r--   0        0        0     2801 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/user.schema.json
+-rw-r--r--   0        0        0     1281 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja
+-rw-r--r--   0        0        0       92 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx/custom.d/jit.conf
+-rw-r--r--   0        0        0      207 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx/sites/apps.conf.jinja
+-rw-r--r--   0        0        0      834 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf
+-rw-r--r--   0        0        0      712 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx/snippets/auth.conf
+-rw-r--r--   0        0        0      527 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx/snippets/proxy.conf
+-rw-r--r--   0        0        0      558 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx/snippets/upstreams.conf.jinja
+-rw-r--r--   0        0        0     2257 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja
+-rw-r--r--   0        0        0       92 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx_gateway/custom.d/jit.conf
+-rw-r--r--   0        0        0       90 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx_gateway/snippets/certificate.conf
+-rw-r--r--   0        0        0     1547 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja
+-rw-r--r--   0        0        0     1609 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja
+-rw-r--r--   0        0        0     1423 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja
+-rw-r--r--   0        0        0     1634 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja
+-rw-r--r--   0        0        0      456 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/dockerfiles/keto_admin/compose.yaml.jinja
+-rw-r--r--   0        0        0      802 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja
+-rw-r--r--   0        0        0      832 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja
+-rw-r--r--   0        0        0       82 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/excluded/kratos/secrets.yaml.jinja
+-rw-r--r--   0        0        0      426 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.editorconfig
+-rw-r--r--   0        0        0       93 2024-05-15 09:34:34.384100 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.git
+-rw-r--r--   0        0        0      519 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes
+-rw-r--r--   0        0        0      128 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODEOWNERS
+-rw-r--r--   0        0        0      121 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     5476 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      323 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/FUNDING.yml
+-rw-r--r--   0        0        0      105 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/dependabot.yml
+-rw-r--r--   0        0        0      958 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml
+-rw-r--r--   0        0        0      322 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1284 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml
+-rw-r--r--   0        0        0       91 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.gitignore
+-rw-r--r--   0        0        0    41306 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md
+-rw-r--r--   0        0        0     1043 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt
+-rw-r--r--   0        0        0     4817 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/README.md
+-rw-r--r--   0        0        0      763 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf
+-rw-r--r--   0        0        0      932 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf
+-rw-r--r--   0        0        0     1434 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf
+-rw-r--r--   0        0        0     1133 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf
+-rw-r--r--   0        0        0      314 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/basic.conf
+-rw-r--r--   0        0        0      739 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf
+-rw-r--r--   0        0        0      761 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf
+-rw-r--r--   0        0        0      385 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/errors/custom_errors.conf
+-rw-r--r--   0        0        0     1706 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf
+-rw-r--r--   0        0        0      701 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf
+-rw-r--r--   0        0        0      685 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf
+-rw-r--r--   0        0        0     1029 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf
+-rw-r--r--   0        0        0      650 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf
+-rw-r--r--   0        0        0     1198 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf
+-rw-r--r--   0        0        0     2102 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf
+-rw-r--r--   0        0        0     1121 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf
+-rw-r--r--   0        0        0     1135 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf
+-rw-r--r--   0        0        0      396 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/server_software_information.conf
+-rw-r--r--   0        0        0     2008 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf
+-rw-r--r--   0        0        0      871 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf
+-rw-r--r--   0        0        0     1800 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf
+-rw-r--r--   0        0        0     1136 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf
+-rw-r--r--   0        0        0     1235 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf
+-rw-r--r--   0        0        0      797 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf
+-rw-r--r--   0        0        0     1818 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf
+-rw-r--r--   0        0        0     1880 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf
+-rw-r--r--   0        0        0     2202 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf
+-rw-r--r--   0        0        0     1484 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf
+-rw-r--r--   0        0        0     2220 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf
+-rw-r--r--   0        0        0     2049 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf
+-rw-r--r--   0        0        0     1435 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf
+-rw-r--r--   0        0        0      732 2024-05-15 09:34:34.972098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf
+-rw-r--r--   0        0        0      572 2024-05-15 09:34:34.976098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf
+-rw-r--r--   0        0        0     5775 2024-05-15 09:34:34.976098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types
+-rw-r--r--   0        0        0     7293 2024-05-15 09:34:34.976098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf
+-rw-r--r--   0        0        0      399 2024-05-15 09:34:34.976098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/default.conf
+-rw-r--r--   0        0        0      678 2024-05-15 09:34:34.976098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf
+-rw-r--r--   0        0        0      782 2024-05-15 09:34:34.976098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf
+-rw-r--r--   0        0        0      126 2024-05-15 09:34:34.976098 lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/www-server.localhost.conf
+-rw-r--r--   0        0        0      161 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/web/.dockerignore
+-rw-r--r--   0        0        0      160 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/web/.eslintignore
+-rw-r--r--   0        0        0      702 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/web/.eslintrc.cjs
+-rw-r--r--   0        0        0       19 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/web/.npmrc
+-rw-r--r--   0        0        0      160 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/web/.prettierignore
+-rw-r--r--   0        0        0      351 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/web/.prettierrc
+-rw-r--r--   0        0        0      763 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/web/Dockerfile.jinja
+-rw-r--r--   0        0        0    40573 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json
+-rw-r--r--   0        0        0   300951 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json
+-rw-r--r--   0        0        0     1729 2024-05-15 09:34:34.032102 lungo_cli-0.4.0/src/lungo_cli/resources/web/package.json
+-rw-r--r--   0        0        0   120480 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/pnpm-lock.yaml
+-rw-r--r--   0        0        0      264 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/postcss.config.cjs
+-rw-r--r--   0        0        0      304 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/app.d.ts
+-rw-r--r--   0        0        0      352 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/app.html
+-rw-r--r--   0        0        0     1736 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/app.pcss
+-rw-r--r--   0        0        0      248 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/hooks.server.ts
+-rw-r--r--   0        0        0     3137 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/actions.ts
+-rw-r--r--   0        0        0   146031 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/assets/cover.jpg
+-rw-r--r--   0        0        0     1713 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/AccountDropdown.svelte
+-rw-r--r--   0        0        0     5068 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/AppShell.svelte
+-rw-r--r--   0        0        0     7325 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte
+-rw-r--r--   0        0        0      556 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/HeroFrame.svelte
+-rw-r--r--   0        0        0      618 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte
+-rw-r--r--   0        0        0     1525 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte
+-rw-r--r--   0        0        0      887 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte
+-rw-r--r--   0        0        0     6343 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/PatchedIFrame.svelte
+-rw-r--r--   0        0        0      608 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/SwappableIcon.svelte
+-rw-r--r--   0        0        0     1691 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/ThemeSelector.svelte
+-rw-r--r--   0        0        0     1719 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/ThemeSelectorDropdown.svelte
+-rw-r--r--   0        0        0      566 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/index.ts
+-rw-r--r--   0        0        0      237 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/constants.ts
+-rw-r--r--   0        0        0     2166 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Account.svelte
+-rw-r--r--   0        0        0      414 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/BaseIcon.svelte
+-rw-r--r--   0        0        0      432 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Check.svelte
+-rw-r--r--   0        0        0     1031 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Close.svelte
+-rw-r--r--   0        0        0     1337 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte
+-rw-r--r--   0        0        0      427 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Expand.svelte
+-rw-r--r--   0        0        0      522 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte
+-rw-r--r--   0        0        0     3326 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte
+-rw-r--r--   0        0        0      617 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte
+-rw-r--r--   0        0        0     1182 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte
+-rw-r--r--   0        0        0     1259 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/QuestionMark.svelte
+-rw-r--r--   0        0        0     1707 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte
+-rw-r--r--   0        0        0     2164 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte
+-rw-r--r--   0        0        0     1861 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte
+-rw-r--r--   0        0        0     1476 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte
+-rw-r--r--   0        0        0      836 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/index.ts
+-rw-r--r--   0        0        0      158 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/server/constants.ts
+-rw-r--r--   0        0        0      953 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/server/utils/api.ts
+-rw-r--r--   0        0        0       46 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/server/utils/index.ts
+-rw-r--r--   0        0        0      109 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts
+-rw-r--r--   0        0        0      678 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/server/utils/stubs.ts.jinja
+-rw-r--r--   0        0        0     2312 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/stores.ts
+-rw-r--r--   0        0        0      324 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/types/common.ts
+-rw-r--r--   0        0        0      224 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/types/index.ts
+-rw-r--r--   0        0        0    31445 2024-05-15 09:34:34.036102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/types/keto.d.ts
+-rw-r--r--   0        0        0   298809 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts
+-rw-r--r--   0        0        0      511 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/types/user.d.ts
+-rw-r--r--   0        0        0     2524 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/utils/api.ts
+-rw-r--r--   0        0        0      483 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/utils/app.ts
+-rw-r--r--   0        0        0     2348 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/utils/common.ts
+-rw-r--r--   0        0        0       93 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/utils/index.ts
+-rw-r--r--   0        0        0      225 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/utils/stubs.ts
+-rw-r--r--   0        0        0     1283 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/utils/stubs.ts.jinja
+-rw-r--r--   0        0        0      289 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/+layout.svelte
+-rw-r--r--   0        0        0     4699 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts
+-rw-r--r--   0        0        0      335 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/account/+page.svelte
+-rw-r--r--   0        0        0     7010 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts
+-rw-r--r--   0        0        0      590 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte
+-rw-r--r--   0        0        0      438 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/logout/+server.ts
+-rw-r--r--   0        0        0     5159 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts
+-rw-r--r--   0        0        0      369 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.svelte
+-rw-r--r--   0        0        0      463 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(apps)/+layout.svelte
+-rw-r--r--   0        0        0     1277 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte
+-rw-r--r--   0        0        0      448 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(apps)/app/+layout.server.ts
+-rw-r--r--   0        0        0      130 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(apps)/app/+page.server.ts
+-rw-r--r--   0        0        0     1008 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/+error.svelte
+-rw-r--r--   0        0        0     2407 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/+layout.server.ts
+-rw-r--r--   0        0        0      938 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/+layout.svelte
+-rw-r--r--   0        0        0    25573 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/static/favicon.png
+-rw-r--r--   0        0        0      276 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/svelte.config.js
+-rw-r--r--   0        0        0     1835 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/tailwind.config.cjs
+-rw-r--r--   0        0        0      601 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/tsconfig.json
+-rw-r--r--   0        0        0      219 2024-05-15 09:34:34.040102 lungo_cli-0.4.0/src/lungo_cli/resources/web/vite.config.ts
+-rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 lungo_cli-0.4.0/PKG-INFO
```

### Comparing `lungo_cli-0.3.0/LICENSE` & `lungo_cli-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/README.md` & `lungo_cli-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/pyproject.toml` & `lungo_cli-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [tool.black]
 line-length = 120
 
 [tool.poetry]
 name = "lungo-cli"
-version = "0.3.0"
+version = "0.4.0"
 description = "A user-friendly home lab setup designed for small-to-mid-scale on-premises hosting."
 authors = ["raymond-u <36328498+raymond-u@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/raymond-u/lungo"
 documentation = "https://raymond-u.github.io/lungo/"
 keywords = ["homelab", "self-host"]
 packages = [{ include = "lungo_cli", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 aenum = "^3.1.15"
-cryptography = "^42.0.5"
-jinja2 = "^3.1.3"
+cryptography = "^42.0.7"
+jinja2 = "^3.1.4"
 packaging = "^24.0"
-platformdirs = "^4.2.0"
-pydantic = { extras = ["email"], version = "^2.6.4" }
+platformdirs = "^4.2.2"
+pydantic = { extras = ["email"], version = "^2.7.1" }
 pydantic-yaml = "^1.3.0"
 requests = "^2.31.0"
 typer = "^0.12.3"
 
 [tool.poetry.group.dev.dependencies]
-black = "^24.4.0"
+black = "^24.4.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mike = "^2.0.0"
-mkdocs-glightbox = "^0.3.7"
-mkdocs-material = "^9.5.17"
+mike = "^2.1.1"
+mkdocs-glightbox = "^0.4.0"
+mkdocs-material = "^9.5.22"
 mkdocs-typer = "^0.0.3"
 
 [tool.poetry.scripts]
 lungo = "lungo_cli.app.main:app_wrapper"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/app/main.py` & `lungo_cli-0.4.0/src/lungo_cli/app/main.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/app/state.py` & `lungo_cli-0.4.0/src/lungo_cli/app/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 _console = Console()
 _client = HttpApiClient(_console)
 _file_utils = FileUtils(_console)
 _storage = Storage(_console, _file_utils)
 _context_manager = ContextManager(_console, _file_utils, _storage)
 _container = Container(_console, _context_manager, _file_utils, _storage)
-_plugin_manager = PluginManager(_console, _context_manager, _file_utils, _storage)
 _renderer = Renderer(_console, _context_manager, _file_utils, _storage)
+_plugin_manager = PluginManager(_console, _context_manager, _file_utils, _renderer, _storage)
 _account_manager = AccountManager(_client, _console, _container, _file_utils, _storage)
 _app_manager = AppManager(
     _account_manager, _console, _context_manager, _file_utils, _plugin_manager, _renderer, _storage
 )
 
 
 def console() -> Console:
@@ -39,21 +39,21 @@
     return _context_manager
 
 
 def container() -> Container:
     return _container
 
 
-def plugin_manager() -> PluginManager:
-    return _plugin_manager
-
-
 def renderer() -> Renderer:
     return _renderer
 
 
+def plugin_manager() -> PluginManager:
+    return _plugin_manager
+
+
 def account_manager() -> AccountManager:
     return _account_manager
 
 
 def app_manager() -> AppManager:
     return _app_manager
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/commands/base.py` & `lungo_cli-0.4.0/src/lungo_cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/commands/down.py` & `lungo_cli-0.4.0/src/lungo_cli/commands/down.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/commands/install.py` & `lungo_cli-0.4.0/src/lungo_cli/commands/uninstall.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 from ..helpers.format import format_input
 
 
 def main(
     args: Annotated[
         list[str],
         Argument(
-            help="Names of the plugins to add.",
+            help="Names of the plugins to remove.",
             show_default=False,
         ),
     ],
     config_dir: ConfigDirType = None,
     dev: DevType = False,
     quiet: QuietType = False,
     verbosity: VerbosityType = 0,
 ) -> None:
     """
-    Install or upgrade plugins.
+    Uninstall plugins.
     """
     app_manager().process_cli_options(config_dir, dev, quiet, verbosity)
     app_manager().load_core_config()
 
     count = 0
 
     for arg in args:
-        plugin_cls = next((x for x in plugin_manager().installable_plugin_classes if x.config.name == arg), None)
+        plugin_cls = next((x for x in plugin_manager().installed_plugin_classes if x.manifest.name == arg), None)
 
         if plugin_cls is None:
-            console().print_warning(f"Plugin {format_input(arg)} not found or not installable. Skipping it.")
+            console().print_warning(f"Plugin {format_input(arg)} not found or not installed. Skipping it.")
             continue
 
-        if plugin_manager().add_plugin(plugin_cls):
+        if plugin_manager().remove_plugin(plugin_cls):
             count += 1
 
     if count == 1:
-        console().print("1 plugin added successfully.")
+        console().print("1 plugin removed successfully.")
     elif count > 1:
-        console().print(f"{count} plugins added successfully.")
+        console().print(f"{count} plugins removed successfully.")
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/commands/list.py` & `lungo_cli-0.4.0/src/lungo_cli/commands/list.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,62 +26,63 @@
     """
     app_manager().process_cli_options(config_dir, dev, quiet, verbosity)
     app_manager().load_core_config()
 
     plugin_classes = plugin_manager().compatible_plugin_classes
 
     for installable_plugin_cls in plugin_manager().installable_plugin_classes:
-        if plugin_cls := next((x for x in plugin_classes if x.config.name == installable_plugin_cls.config.name), None):
-            plugin_cls.installable = True
-            plugin_cls.alt_version = installable_plugin_cls.config.version
+        if plugin_cls := next(
+            (x for x in plugin_classes if x.manifest.name == installable_plugin_cls.manifest.name), None
+        ):
+            plugin_cls.is_installable = True
+            plugin_cls.alt_version = installable_plugin_cls.manifest.version
         else:
-            installable_plugin_cls.alt_version = installable_plugin_cls.config.version
+            installable_plugin_cls.alt_version = installable_plugin_cls.manifest.version
             plugin_classes.append(installable_plugin_cls)
 
     if args:
         for arg in args:
-            if plugin_cls := next((x for x in plugin_classes if x.config.name == arg), None):
+            if plugin_cls := next((x for x in plugin_classes if x.manifest.name == arg), None):
                 console().print(
-                    f"Name: {plugin_cls.config.name}"
-                    f"{f' ({plugin_cls.config.descriptive_name})' if plugin_cls.config.descriptive_name else ''}"
+                    f"Name: {plugin_cls.manifest.name}"
+                    f"{f' ({plugin_cls.manifest.descriptive_name})' if plugin_cls.manifest.descriptive_name else ''}"
                 )
                 console().print(
-                    f"Version: {(plugin_cls.installed and plugin_cls.config.version) or '-'}"
-                    f" -> {(plugin_cls.installable and plugin_cls.alt_version) or '-'}"
-                    if plugin_cls.installable
+                    f"Version: {plugin_cls.manifest.version if plugin_cls.is_installed else '-'} -> {plugin_cls.alt_version}"
+                    if plugin_cls.is_installable
                     else ""
                 )
                 console().print(
-                    f"Status: {'installable' if plugin_cls.installable else 'not installable'}, "
-                    f"{'installed' if plugin_cls.installed else 'not installed'} "
-                    f"({'custom' if plugin_cls.custom else 'built-in'} plugin)."
+                    f"Status: {'installable' if plugin_cls.is_installable else 'not installable'}, "
+                    f"{'installed' if plugin_cls.is_installed else 'not installed'} "
+                    f"({'custom' if plugin_cls.is_custom else 'built-in'} plugin)."
                 )
-                console().print(f"Description: {plugin_cls.config.description or 'No description.'}")
+                console().print(f"Description: {plugin_cls.manifest.description or 'No description.'}")
             else:
                 console().print(f"Plugin {format_input(arg)} not found. Skipping it.")
 
             console().request_newline()
     else:
         if len(plugin_classes) == 0:
             console().print("No plugins found.")
             return
 
-        plugin_classes.sort(key=lambda x: x.config.name)
-        plugin_classes.sort(key=lambda x: not x.installed)
+        plugin_classes.sort(key=lambda x: x.manifest.name)
+        plugin_classes.sort(key=lambda x: not x.is_installed)
 
         table = Table()
         table.add_column("Name")
         table.add_column("Current")
         table.add_column("Available")
         table.add_column("Installable")
         table.add_column("Installed")
 
         for plugin_cls in plugin_classes:
             table.add_row(
-                plugin_cls.config.name,
-                (plugin_cls.installed and plugin_cls.config.version) or "-",
-                (plugin_cls.installable and plugin_cls.alt_version) or "-",
-                "Yes" if plugin_cls.installable else "No",
-                "Yes" if plugin_cls.installed else "No",
+                plugin_cls.manifest.name,
+                plugin_cls.manifest.version if plugin_cls.is_installed else "-",
+                plugin_cls.alt_version if plugin_cls.is_installable else "-",
+                "Yes" if plugin_cls.is_installable else "No",
+                "Yes" if plugin_cls.is_installed else "No",
             )
 
         console().print(table)
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/commands/uninstall.py` & `lungo_cli-0.4.0/src/lungo_cli/commands/install.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 from ..helpers.format import format_input
 
 
 def main(
     args: Annotated[
         list[str],
         Argument(
-            help="Names of the plugins to remove.",
+            help="Names of the plugins to add.",
             show_default=False,
         ),
     ],
     config_dir: ConfigDirType = None,
     dev: DevType = False,
     quiet: QuietType = False,
     verbosity: VerbosityType = 0,
 ) -> None:
     """
-    Uninstall plugins.
+    Install or upgrade plugins.
     """
     app_manager().process_cli_options(config_dir, dev, quiet, verbosity)
     app_manager().load_core_config()
 
     count = 0
 
     for arg in args:
-        plugin_cls = next((x for x in plugin_manager().installed_plugin_classes if x.config.name == arg), None)
+        plugin_cls = next((x for x in plugin_manager().installable_plugin_classes if x.manifest.name == arg), None)
 
         if plugin_cls is None:
-            console().print_warning(f"Plugin {format_input(arg)} not found or not installed. Skipping it.")
+            console().print_warning(f"Plugin {format_input(arg)} not found or not installable. Skipping it.")
             continue
 
-        if plugin_manager().remove_plugin(plugin_cls):
+        if plugin_manager().add_plugin(plugin_cls):
             count += 1
 
     if count == 1:
-        console().print("1 plugin removed successfully.")
+        console().print("1 plugin added successfully.")
     elif count > 1:
-        console().print(f"{count} plugins removed successfully.")
+        console().print(f"{count} plugins added successfully.")
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/commands/up.py` & `lungo_cli-0.4.0/src/lungo_cli/commands/up.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Annotated, Optional
 
-from typer import Exit, Option
+from typer import Option
 
 from .base import ConfigDirType, DevType, ForceInitType, QuietType, VerbosityType
 from ..app.state import app_manager, console, container, context_manager, file_utils, storage
 from ..core.constants import APP_NAME, APP_NAME_CAPITALIZED
-from ..helpers.common import port_is_available
-from ..helpers.format import format_command, format_input, format_link
+from ..helpers.format import format_command, format_link
 from ..models.base import EContainer
 
 
 def main(
     build_only: Annotated[bool, Option("--build-only", help="Only build the containers.", show_default=False)] = False,
     container_tool: Annotated[
         Optional[EContainer], Option("--container-tool", help="Container management tool to use.", show_default=False)
@@ -30,39 +29,30 @@
     """
     app_manager().process_cli_options(config_dir, dev, quiet, verbosity, force_init)
     app_manager().load_full_config()
 
     if remove_lock:
         file_utils().remove(storage().lock_file)
 
-    app_manager().update_app_data()
+    app_manager().initialize()
 
     if render_only:
         return
 
     container().set_preferred_tool(container_tool)
 
     if build_only:
         with console().status(
             "Building containers (could take a few minutes, depending on the internet connection)..."
         ):
             container().build()
 
         console().print("Build completed.")
     else:
-        http_port = context_manager().config.network.http.port
-        https_port = context_manager().config.network.https.port
-
-        if context_manager().config.network.http.enabled and not port_is_available(http_port):
-            console().print_error(f"Port {format_input(http_port)} is in use.")
-            raise Exit(code=1)
-
-        if not port_is_available(https_port):
-            console().print_error(f"Port {format_input(https_port)} is in use.")
-            raise Exit(code=1)
+        app_manager().ensure_port_availability()
 
         with console().status(
             "Starting the service (could take a few minutes, depending on the internet connection)..."
         ):
             container().up()
 
         console().print(
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/core/app.py` & `lungo_cli-0.4.0/src/lungo_cli/core/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from .constants import PACKAGE_NAME
 from .context import ContextManager
 from .database import AccountManager
 from .file import FileUtils
 from .plugin import PluginManager
 from .renderer import Renderer
 from .storage import Storage
-from ..helpers.common import get_app_version, get_file_permissions
+from ..helpers.common import get_app_version, get_file_permissions, port_is_available
 from ..helpers.crypto import generate_random_hex, generate_self_signed_cert, hash_text
-from ..helpers.format import format_input, format_path
+from ..helpers.format import format_input, format_path, format_program
 from ..models.base import EApp
 from ..models.config import Config, CoreConfig
 from ..models.users import Users
 
 
 class AppManager:
     """Manager for the application."""
@@ -113,14 +113,16 @@
         core_config = self.file_utils.parse_yaml(self.storage.config_file, CoreConfig)
 
         if core_config.directories.cache_dir:
             self.storage.cache_dir = core_config.directories.cache_dir.resolve()
         if core_config.directories.data_dir:
             self.storage.data_dir = core_config.directories.data_dir.resolve()
 
+        self.storage.migrate_if_needed()
+
     def load_full_config(self) -> None:
         """Load the full configuration files into the context manager."""
         self.load_core_config()
         self.plugin_manager.extend_models()
 
         config = self.file_utils.parse_yaml(self.storage.config_file, Config)
         users = self.file_utils.parse_yaml(self.storage.users_file, Users)
@@ -134,15 +136,15 @@
         """Verify the configuration files."""
         shared_dirs = list(map(lambda x: x.name, config.directories.shared_dirs))
         anonymous_account_exists = False
 
         for account in users.accounts:
             if account.username == "anonymous":
                 self.console.print_info(
-                    f"Found username {format_input('anonymous')}. "
+                    f"Found username {format_input("anonymous")}. "
                     "This user will serve as a shared account for anonymous access."
                 )
                 anonymous_account_exists = True
 
             if not (path := (account.extra.user_dir or config.directories.users_dir / account.username)).is_dir():
                 if os.access(path.parent, os.W_OK):
                     self.console.print_info(f"Creating user directory at {format_path(path)}...")
@@ -170,117 +172,139 @@
             for allowed_app in config.rules.privileges.unregistered.allowed_apps:
                 # Pydantic does not distinguish between a string and an enum value
                 if type(allowed_app) is EApp:
                     allowed_app = allowed_app.value
 
                 if next(
                     (
-                        plugin_cls.config.require_account
+                        plugin_cls.manifest.require_account
                         for plugin_cls in self.plugin_manager.compatible_plugin_classes
-                        if plugin_cls.config.name == allowed_app
+                        if plugin_cls.manifest.name == allowed_app
                     ),
                     False,
                 ):
                     self.console.print_error(
                         "An anonymous account is required when the unregistered role "
                         "has access to applications that require an account."
                     )
                     raise Exit(code=1)
 
     def generate_config_hash(self) -> str:
         """Generate a hash of the configuration files."""
-        ordered_plugins = sorted(self.plugin_manager.compatible_plugin_classes, key=lambda x: x.config.name)
+        ordered_plugins = sorted(self.plugin_manager.compatible_plugin_classes, key=lambda x: x.manifest.name)
 
         return hash_text(
             "+".join(
                 [
                     f"v{get_app_version()}",
                     *(
                         map(
-                            lambda x: f"{x.config.name}{f'v{x.config.version}' if x.config.version else ''}",
+                            lambda x: f"{x.manifest.name}v{x.manifest.version}",
                             ordered_plugins,
                         )
                     ),
                     self.file_utils.hash_sha256(self.storage.config_file),
                     self.file_utils.hash_sha256(self.storage.users_file),
                 ]
             )
         )
 
-    def update_app_data(self) -> None:
-        """Ensure that all the application data exists and is up-to-date."""
-        config_hash = self.generate_config_hash()
+    def initialize_core(self) -> None:
+        """Initialize the core part of the application."""
+        if not self.storage.nginx_gateway_cert_file.is_file() or not self.storage.nginx_gateway_key_file.is_file():
+            self.console.print_info("Generating self-signed certificate...")
+            cert, key = generate_self_signed_cert()
+            self.file_utils.write_bytes(self.storage.nginx_gateway_cert_file, cert)
+            self.file_utils.write_bytes(self.storage.nginx_gateway_key_file, key, True)
+
+        # Remove the socket file every time to avoid binding issues
+        self.file_utils.remove(self.storage.nginx_gateway_socket_file)
+
+        if not self.storage.kratos_secrets_file.is_file():
+            self.console.print_info("Generating Kratos secrets...")
+            self.renderer.render(
+                self.storage.template_kratos_secrets_rel,
+                self.storage.kratos_secrets_file,
+                secret_cookie=generate_random_hex(),
+            )
+            self.file_utils.change_mode(self.storage.kratos_secrets_file, 0o600)
+
+    def render_core(self) -> None:
+        """Render core templates."""
+        app_web_path_map = {plugin.manifest.name: plugin.manifest.web_path for plugin in self.plugin_manager.plugins}
+        self.account_manager.update(self.context_manager.config, self.context_manager.users, app_web_path_map)
+
+        self.storage.update_bundled_files()
+        self.renderer.render_core()
+
+    def initialize(self) -> None:
+        """Initialize the application."""
+        with self.console.status("Initializing..."):
+            config_hash = self.generate_config_hash()
 
-        with self.console.status("Updating app data..."):
-            self.storage.validate()
+            # Always ensure that the required directories exist
+            self.storage.create_dirs()
+
+            self.plugin_manager.initialize_plugins()
+            self.initialize_core()
 
             if (
                 self.force_init
                 or not self.storage.bundled_dir.is_dir()
                 or not self.storage.init_file.is_file()
                 or self.file_utils.read_text(self.storage.init_file) != config_hash
             ):
-                self.console.print_info("Updating bundled resources...")
+                self.plugin_manager.render_plugins()
+                self.render_core()
 
-                # Backup the installed plugins directory if it exists
-                if self.storage.installed_plugins_dir.is_dir():
-                    self.file_utils.move(self.storage.installed_plugins_dir, self.storage.cache_plugins_dir)
-
-                self.file_utils.copy_package_resources(f"{PACKAGE_NAME}.resources", ".", self.storage.bundled_dir)
-
-                if self.storage.cache_plugins_dir.is_dir():
-                    self.file_utils.move(self.storage.cache_plugins_dir, self.storage.installed_plugins_dir)
-
-                self.file_utils.change_mode(self.storage.bundled_dir, 0o700)
-                self.file_utils.remove(self.storage.init_file)
-
-            if not self.storage.nginx_gateway_cert_file.is_file() or not self.storage.nginx_gateway_key_file.is_file():
-                self.console.print_info("Generating self-signed certificate...")
-                cert, key = generate_self_signed_cert()
-                self.file_utils.write_bytes(self.storage.nginx_gateway_cert_file, cert)
-                self.file_utils.write_bytes(self.storage.nginx_gateway_key_file, key, True)
-
-            # Remove the socket file every time to avoid binding issues
-            self.file_utils.remove(self.storage.nginx_gateway_socket_file)
-
-            if not self.storage.kratos_secrets_file.is_file():
-                self.console.print_info("Generating Kratos secrets...")
-                self.renderer.render(
-                    self.storage.template_kratos_secrets_rel,
-                    self.storage.kratos_secrets_file,
-                    secret_cookie=generate_random_hex(),
-                )
-                self.file_utils.change_mode(self.storage.kratos_secrets_file, 0o600)
+                # Delay copying the web files until the templates have all been rendered
+                self.plugin_manager.update_rendered_plugin_files()
+                self.file_utils.write_text(self.storage.init_file, config_hash)
 
-            self.plugin_manager.initialize_plugins()
+    def ensure_port_availability(self) -> None:
+        """Ensure that the required ports are available."""
+        ports: list[tuple[int, str]] = []
+
+        if self.context_manager.config.network.http.enabled:
+            ports.append((self.context_manager.config.network.http.port, "HTTP service"))
+
+        ports.append((self.context_manager.config.network.https.port, "HTTPS service"))
+
+        ports.extend(
+            (
+                (port, plugin_cls.manifest.name)
+                for plugin_cls in self.plugin_manager.compatible_plugin_classes
+                for port in (plugin_cls.manifest.backend_host_ports or [])
+            )
+        )
 
-            if not self.storage.init_file.is_file():
-                for plugin in self.plugin_manager.plugins:
-                    self.renderer.render_plugin(plugin)
-                    self.context_manager.plugin_outputs.append(plugin.output)
+        unique_ports: list[tuple[int, str]] = []
+        duplicate_ports: list[tuple[int, list[str]]] = []
 
-                self.renderer.render_main()
-                self.account_manager.update(self.context_manager.config, self.context_manager.users)
+        for port, name in ports:
+            for p, n in unique_ports:
+                if port == p:
+                    for pp, nn in duplicate_ports:
+                        if port == pp:
+                            nn.append(name)
+                            break
+                    else:
+                        duplicate_ports.append((port, [n, name]))
+                    break
+            else:
+                unique_ports.append((port, name))
 
-                # Delay copying the web files until the templates have all been rendered
-                for plugin in self.plugin_manager.plugins:
-                    for web_dir in (self.storage.installed_plugins_dir / plugin.config.name / "web").iterdir():
-                        if web_dir.name == "lib":
-                            dst_prefix = self.storage.bundled_dir / "web" / "src" / "lib" / "plugins"
-                            self.file_utils.copy(web_dir, dst_prefix / plugin.config.name)
-                        elif web_dir.name == "routes":
-                            dst_prefix = self.storage.bundled_dir / "web" / "src" / "routes" / "(apps)" / "app"
-                            self.file_utils.copy(web_dir, dst_prefix / plugin.config.name)
-
-                if self.context_manager.config.branding.cover:
-                    self.file_utils.copy(
-                        self.context_manager.config.branding.cover,
-                        self.storage.bundled_dir / "web" / "src" / "lib" / "assets" / "cover.jpg",
-                    )
+        if duplicate_ports:
+            for port, names in duplicate_ports:
+                self.console.print_error(
+                    f"Port {format_input(port)} is required by multiple services "
+                    f"({', '.join(map(format_program, names))})."
+                )
+            raise Exit(code=1)
 
-                if self.context_manager.config.branding.logo:
-                    self.file_utils.copy(
-                        self.context_manager.config.branding.logo,
-                        self.storage.bundled_dir / "web" / "static" / "favicon.png",
-                    )
+        for port, name in ports:
 
-                self.file_utils.write_text(self.storage.init_file, config_hash)
+            if not port_is_available(port):
+                self.console.print_error(
+                    f"Port {format_input(port)} is in use but is required by {format_program(name)}."
+                )
+                raise Exit(code=1)
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/core/console.py` & `lungo_cli-0.4.0/src/lungo_cli/core/console.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/core/container.py` & `lungo_cli-0.4.0/src/lungo_cli/core/container.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/core/context.py` & `lungo_cli-0.4.0/src/lungo_cli/core/context.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,30 @@
+import socket
 from ipaddress import IPv4Address
 
 from typer import Exit
 
 from .console import Console
+from .constants import (
+    APP_NAME,
+    APP_NAME_CAPITALIZED,
+    ARCHITECTURE,
+    KETO_VERSION,
+    KRATOS_VERSION,
+    NODE_VERSION,
+    OATHKEEPER_VERSION,
+    OPENRESTY_VERSION,
+    PACKAGE_NAME,
+)
 from .file import FileUtils
 from .storage import Storage
 from ..helpers.format import format_input
-from ..models.base import EApp, ECoreService
+from ..models.base import AppDirs, EApp, ECoreService
 from ..models.config import Config
-from ..models.context import AppDirs, Context
+from ..models.context import Constants, Context
 from ..models.plugin import PluginOutput
 from ..models.users import Users
 
 
 class ContextManager:
     """Manage the context of the application, can be passed to the renderer to render templates."""
 
@@ -21,14 +33,29 @@
         self.file_utils = file_utils
         self.storage = storage
 
         self._config = None
         self._users = None
         self._plugin_outputs = []
         self._dev = False
+        self._local_ip = None
+
+    @property
+    def constants(self) -> Constants:
+        return Constants(
+            app_name=APP_NAME,
+            app_name_capitalized=APP_NAME_CAPITALIZED,
+            architecture=ARCHITECTURE,
+            package_name=PACKAGE_NAME,
+            openresty_version=OPENRESTY_VERSION,
+            keto_version=KETO_VERSION,
+            kratos_version=KRATOS_VERSION,
+            oathkeeper_version=OATHKEEPER_VERSION,
+            node_version=NODE_VERSION,
+        )
 
     @property
     def config(self) -> Config:
         if self._config is None:
             self.console.print_error("Config is not set.")
             raise Exit(code=1)
 
@@ -60,15 +87,15 @@
 
     @property
     def app_dirs(self) -> AppDirs:
         return AppDirs(
             cache_dir=str(self.storage.cache_latest_dir),
             generated_dir=str(self.storage.generated_dir),
             managed_dir=str(self.storage.managed_dir),
-            plugin_dir="./plugins",
+            plugin_dir=str(self.storage.plugins_rel),
         )
 
     @property
     def base_url(self) -> str:
         port = f":{self.config.network.https.port}" if self.config.network.https.port != 443 else ""
         return f"https://{self.config.network.hostname}{port}/"
 
@@ -88,20 +115,37 @@
                 "Please change it to a subnet with at least 256 addresses."
             )
             raise Exit(code=1)
 
         hosts = list(self.config.network.subnet.hosts())
 
         # Reserve the first 16 addresses for gateway and other services
+        # Assign an IP address to each service, regardless of whether it is needed or not
         return {app.value: hosts[i + 16] for i, app in enumerate((*ECoreService, *EApp))}
 
     @property
+    def local_ip(self) -> IPv4Address:
+        if self._local_ip is None:
+            with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
+                try:
+                    s.settimeout(0)
+                    s.connect(("10.254.254.254", 1))
+
+                    self._local_ip = IPv4Address(s.getsockname()[0])
+                except Exception:
+                    self._local_ip = IPv4Address("127.0.0.1")
+
+        return self._local_ip
+
+    @property
     def context(self) -> Context:
         return Context(
+            constants=self.constants,
             config=self.config,
             users=self.users,
             plugin_outputs=self.plugin_outputs,
             app_dirs=self.app_dirs,
             base_url=self.base_url,
             dev=self.dev,
             ip_addresses=self.ip_addresses,
+            local_ip=self.local_ip,
         )
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/core/database.py` & `lungo_cli-0.4.0/src/lungo_cli/core/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     ):
         self.client = client
         self.console = console
         self.container = container
         self.file_utils = file_utils
         self.storage = storage
 
-    def update(self, config: Config, users: Users) -> None:
+    def update(self, config: Config, users: Users, app_web_path_map: dict[str, str]) -> None:
         # Ensure that the container can always be started even if it failed last time
+        self.console.print_info("Updating user accounts...")
+
         self.container.down(self.storage.service_keto_admin_dir)
         self.container.down(self.storage.service_kratos_admin_dir)
 
         self.container.up(self.storage.service_keto_admin_dir)
         self.container.up(self.storage.service_kratos_admin_dir)
 
         self.console.print_debug("Connecting to Keto Admin API...")
@@ -85,15 +87,15 @@
             if getattr(config.plugins, app.value).enabled:
                 enabled_apps.append(app)
                 data.append(
                     {
                         "action": "insert",
                         "relation_tuple": {
                             "namespace": "app",
-                            "object": app.value,
+                            "object": app_web_path_map[app.value],
                             "relation": "access",
                             "subject_set": {"namespace": "app", "object": "all", "relation": "access"},
                         },
                     }
                 )
 
         # Add role privileges
@@ -120,15 +122,15 @@
 
                     if allowed_app in enabled_apps:
                         data.append(
                             {
                                 "action": "insert",
                                 "relation_tuple": {
                                     "namespace": "app",
-                                    "object": allowed_app.value,
+                                    "object": app_web_path_map[allowed_app.value],
                                     "relation": "access",
                                     "subject_set": {"namespace": "role", "object": role, "relation": "member"},
                                 },
                             },
                         )
 
         # Add account privileges
@@ -167,15 +169,15 @@
 
                     if allowed_app in enabled_apps:
                         data.append(
                             {
                                 "action": "insert",
                                 "relation_tuple": {
                                     "namespace": "app",
-                                    "object": allowed_app.value,
+                                    "object": app_web_path_map[allowed_app.value],
                                     "relation": "access",
                                     "subject_id": account.username,
                                 },
                             },
                         )
 
         self.console.print_debug("Creating new relation tuples...")
@@ -206,19 +208,19 @@
                 if old_account["traits"]["name"]["first"] != new_account.name.first:
                     data.append({"op": "replace", "path": "/traits/name/first", "value": new_account.name.first})
                 if old_account["traits"]["name"]["last"] != new_account.name.last:
                     data.append({"op": "replace", "path": "/traits/name/last", "value": new_account.name.last})
 
                 if data:
                     self.console.print_debug(f"Updating account {format_input(new_account.username)}...")
-                    self.client.patch(f"{KRATOS_ADMIN_API_BASE_URL}/admin/identities/{old_account['id']}", data)
+                    self.client.patch(f"{KRATOS_ADMIN_API_BASE_URL}/admin/identities/{old_account["id"]}", data)
             else:
                 # Remove the account
-                self.console.print_debug(f"Removing account {format_input(old_account['traits']['username'])}...")
-                self.client.delete(f"{KRATOS_ADMIN_API_BASE_URL}/admin/identities/{old_account['id']}")
+                self.console.print_debug(f"Removing account {format_input(old_account["traits"]["username"])}...")
+                self.client.delete(f"{KRATOS_ADMIN_API_BASE_URL}/admin/identities/{old_account["id"]}")
 
         for new_account in accounts:
             # Create the account
             data = {
                 "schema_id": "user",
                 "state": "active" if new_account.enabled else "inactive",
                 "traits": {
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/core/file.py` & `lungo_cli-0.4.0/src/lungo_cli/core/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,14 @@
                         if type(loc) is int:
                             error_msg += f"[{loc}]"
                         else:
                             error_msg += f".{loc}"
                 else:
                     error_msg += "root"
 
-                error_msg += f": {error['msg']}"
+                error_msg += f": {error["msg"]}"
 
             self.console.print_error(error_msg)
             raise Exit(code=1)
         except Exception as e:
             self.console.print_error(f"Failed to parse {format_path(path)} ({e}).")
             raise Exit(code=1)
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/core/network.py` & `lungo_cli-0.4.0/src/lungo_cli/core/network.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/core/plugin.py` & `lungo_cli-0.4.0/src/lungo_cli/core/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,49 @@
+import os
 import sys
 from abc import ABC
 from importlib import import_module
 from importlib.resources import as_file, files
 from os import PathLike
 from pathlib import Path
 from typing import Any, ClassVar, final
 
 from aenum import extend_enum
 from packaging.specifiers import InvalidSpecifier, SpecifierSet
 from pydantic.fields import FieldInfo
 from typer import Exit
 
 from .console import Console
-from .constants import PACKAGE_NAME
+from .constants import PACKAGE_NAME, PLUGIN_WEB_ENTRYPOINT
 from .context import ContextManager
 from .file import FileUtils
+from .renderer import Renderer
 from .storage import Storage
 from ..helpers.common import extract_multiline_value_from_yaml, get_app_version
 from ..helpers.format import format_path, format_program
-from ..models.base import EApp
+from ..models.base import AppDirs, EApp
 from ..models.config import Config, Plugins, Privilege, Privileges, Rules
 from ..models.context import Context
-from ..models.plugin import BaseSettings, PluginConfig, PluginOutput
+from ..models.plugin import BaseSettings, PluginContext, PluginManifest, PluginOutput
 from ..models.users import Account, Extra, Users
 
 
 class BasePlugin[T: BaseSettings](ABC):
     """Base class for all plugins."""
 
-    config: ClassVar[PluginConfig]
+    manifest: ClassVar[PluginManifest]
 
-    custom: ClassVar[bool] = False
-    installable: ClassVar[bool] = False
-    installed: ClassVar[bool] = False
-    compatible: ClassVar[bool] = True
+    is_custom: ClassVar[bool] = False
+    is_installable: ClassVar[bool] = False
+    is_installed: ClassVar[bool] = False
+    is_compatible: ClassVar[bool] = True
     alt_version: ClassVar[str | None] = None
+    source: ClassVar[Path | None] = None
 
-    rendered: ClassVar[bool] = False
+    is_rendered: ClassVar[bool] = False
 
     def __init__(
         self,
         settings: T,
         console: Console,
         context_manager: ContextManager,
         file_utils: FileUtils,
@@ -54,53 +57,118 @@
 
         self._output = None
 
     # Chaining `classmethod` descriptor with `property` descriptor is no longer supported
     # `ClassVar` parameter cannot include type variables
     @classmethod
     def get_plugin_settings_cls(cls) -> type[T]:
+        """
+        Retrieve the settings class for the plugin.
+
+        This method returns the class that defines the settings for the plugin. An instance of this class will be
+        passed to the plugin during its initialization, which is set by the user.
+
+        This method can be overridden in subclasses to provide custom settings classes. If not overridden, the default
+        implementation returns the `BaseSettings` class.
+        """
         return BaseSettings
 
-    def get_render_context(self) -> dict[str, Any]:
+    def get_custom_rendering_context(self) -> dict[str, Any]:
+        """
+        Retrieve the custom template rendering context.
+
+        This method returns a dictionary that can be used to provide custom context data for template rendering.
+        The returned dictionary can be accessed in the templates under the `plugin.custom` key.
+
+        This method can be overridden in subclasses to provide custom context data. If not overridden, the default
+        implementation returns an empty dictionary.
+        """
         return {}
 
-    def update_data(self) -> None: ...
+    def on_plugin_initialization(self) -> None:
+        """
+        Execute during the plugin initialization event.
+
+        This method is invoked when the plugin is initialized. It can be used to perform actions like creating
+        directories, generating secrets, etc.
+
+        This method can be overridden in subclasses to provide custom initialization behavior. If not overridden, the
+        default implementation does nothing.
+        """
+        ...
+
+    def on_plugin_rendering(self) -> None:
+        """
+        Execute before the plugin rendering process.
+
+        The rendering process is triggered when there are changes in the settings, the plugin itself, or the
+        application. This method is intended to handle actions that cannot be performed with templates, such as
+        updating database records.
+
+        This method can be overridden in subclasses to provide custom behavior during the rendering process. If not
+        overridden, the default implementation of this method does nothing.
+        """
+        ...
 
     @classmethod
     @final
     def mark_as_rendered(cls) -> None:
-        cls.rendered = True
+        cls.is_rendered = True
+
+    @property
+    @final
+    def context(self) -> PluginContext:
+        base_url = self.context_manager.base_url
+        ip_addresses = self.context_manager.ip_addresses
+
+        return PluginContext(
+            manifest=self.manifest,
+            backend_base_url=(
+                f"http://{ip_addresses[self.manifest.name]}:{self.manifest.backend_port}/"
+                if self.manifest.backend_port
+                else None
+            ),
+            dirs=AppDirs(
+                cache_dir=str(self.storage.cache_latest_dir / self.manifest.name),
+                generated_dir=str(self.storage.generated_dir / self.manifest.name),
+                managed_dir=str(self.storage.managed_dir / self.manifest.name),
+                plugin_dir=os.path.join(".", self.storage.plugins_rel / self.manifest.name),
+            ),
+            ip_address=ip_addresses[self.manifest.name],
+            oathkeeper_url_regex=f"{base_url}{PLUGIN_WEB_ENTRYPOINT}/<{self.manifest.web_path}>",
+            web_base_url=f"{base_url}{PLUGIN_WEB_ENTRYPOINT}/{self.manifest.web_path}/",
+            web_prefix=f"/{PLUGIN_WEB_ENTRYPOINT}/{self.manifest.web_path}",
+            custom=self.get_custom_rendering_context(),
+        )
 
     @property
     @final
     def output(self) -> PluginOutput:
         if self._output is None:
-            if not self.rendered:
-                self.console.print_error(f"Plugin {format_program(self.config.name)} has not been rendered.")
+            if not self.is_rendered:
+                self.console.print_error(f"Plugin {format_program(self.manifest.name)} has not been rendered.")
                 raise Exit(code=1)
 
-            plugin_dir = self.storage.installed_plugins_dir / self.config.name
+            plugin_dir = self.storage.installed_plugins_dir / self.manifest.name
 
             compose_content = self.file_utils.read_text(plugin_dir / "compose" / "compose.yaml", not_exist_ok=True)
             compose_services = extract_multiline_value_from_yaml(compose_content, "services")
             compose_secrets = extract_multiline_value_from_yaml(compose_content, "secrets")
-            nginx_upstream = self.file_utils.read_text(plugin_dir / "nginx" / "upstream.conf", not_exist_ok=True)
             nginx_site = self.file_utils.read_text(plugin_dir / "nginx" / "site.conf", not_exist_ok=True)
             oathkeeper_rules = self.file_utils.read_text(
                 plugin_dir / "oathkeeper" / "access_rules.yaml", not_exist_ok=True
             )
             web_dependencies = self.file_utils.read_text(
                 plugin_dir / "web" / "dependencies.txt", not_exist_ok=True
             ).splitlines()
 
             self._output = PluginOutput(
-                config=self.config,
+                manifest=self.manifest,
                 compose_services=compose_services,
                 compose_secrets=compose_secrets,
-                nginx_upstream=nginx_upstream,
                 nginx_site=nginx_site,
                 oathkeeper_rules=oathkeeper_rules,
                 web_dependencies=web_dependencies,
             )
 
         return self._output
 
@@ -109,19 +177,21 @@
     """Manager for plugins."""
 
     def __init__(
         self,
         console: Console,
         context_manager: ContextManager,
         file_utils: FileUtils,
+        renderer: Renderer,
         storage: Storage,
     ):
         self.console = console
         self.context_manager = context_manager
         self.file_utils = file_utils
+        self.renderer = renderer
         self.storage = storage
 
         self._builtin_plugin_classes = None
         self._custom_plugin_classes = None
         self._installable_plugin_classes = None
         self._installed_plugin_classes = None
         self._compatible_plugin_classes = None
@@ -130,28 +200,28 @@
     @property
     def builtin_plugin_classes(self) -> list[type[BasePlugin]]:
         if self._builtin_plugin_classes is None:
             with as_file(files(f"{PACKAGE_NAME}.plugins")) as package_dir:
                 plugin_classes = self.import_plugins(package_dir)
 
                 for plugin_cls in plugin_classes:
-                    plugin_cls.installable = True
+                    plugin_cls.is_installable = True
 
                 self._builtin_plugin_classes = plugin_classes
 
         return self._builtin_plugin_classes
 
     @property
     def custom_plugin_classes(self) -> list[type[BasePlugin]]:
         if self._custom_plugin_classes is None:
             plugin_classes = self.import_plugins(self.storage.custom_plugins_dir)
 
             for plugin_cls in plugin_classes:
-                plugin_cls.custom = True
-                plugin_cls.installable = True
+                plugin_cls.is_custom = True
+                plugin_cls.is_installable = True
 
             self._custom_plugin_classes = plugin_classes
 
         return self._custom_plugin_classes
 
     @property
     def installable_plugin_classes(self) -> list[type[BasePlugin]]:
@@ -162,62 +232,62 @@
 
     @property
     def installed_plugin_classes(self) -> list[type[BasePlugin]]:
         if self._installed_plugin_classes is None:
             plugin_classes = self.import_plugins(self.storage.installed_plugins_dir)
 
             for plugin_cls in plugin_classes:
-                plugin_cls.installed = True
+                plugin_cls.is_installed = True
 
             self._installed_plugin_classes = plugin_classes
 
         return self._installed_plugin_classes
 
     @property
     def compatible_plugin_classes(self) -> list[type[BasePlugin]]:
         if self._compatible_plugin_classes is None:
             self._compatible_plugin_classes = [
-                plugin_cls for plugin_cls in self.installed_plugin_classes if plugin_cls.compatible
+                plugin_cls for plugin_cls in self.installed_plugin_classes if plugin_cls.is_compatible
             ]
 
         return self._compatible_plugin_classes
 
     @property
     def plugins(self) -> list[BasePlugin]:
         return self._plugins
 
     def add_plugin(self, plugin_cls: type[BasePlugin]) -> bool:
         """Add a plugin to the application."""
-        if not plugin_cls.installable:
+        if not plugin_cls.is_installable:
             self.console.print_warning(
-                f"Plugin {format_program(plugin_cls.config.name)} is not installable. Skipping it."
+                f"Plugin {format_program(plugin_cls.manifest.name)} is not installable. Skipping it."
             )
             return False
 
-        dst = self.storage.installed_plugins_dir / plugin_cls.config.name
+        dst = self.storage.installed_plugins_dir / plugin_cls.manifest.name
 
-        if plugin_cls.custom:
-            self.file_utils.copy(self.storage.custom_plugins_dir / plugin_cls.config.name, dst)
+        if plugin_cls.is_custom:
+            self.file_utils.copy(plugin_cls.source, dst)
         else:
-            self.file_utils.copy_package_resources(f"{PACKAGE_NAME}.plugins", plugin_cls.config.name, dst)
+            self.file_utils.copy_package_resources(f"{PACKAGE_NAME}.plugins", plugin_cls.manifest.name, dst)
 
-        plugin_cls.installed = True
+        plugin_cls.is_installed = True
         return True
 
     def remove_plugin(self, plugin_cls: type[BasePlugin]) -> bool:
         """Remove a plugin from the application."""
-        if not plugin_cls.installed:
+        if not plugin_cls.is_installed:
             self.console.print_warning(
-                f"Plugin {format_program(plugin_cls.config.name)} is not installed. Skipping it."
+                f"Plugin {format_program(plugin_cls.manifest.name)} is not installed. Skipping it."
             )
             return False
 
-        self.file_utils.remove(self.storage.installed_plugins_dir / plugin_cls.config.name)
+        self.file_utils.remove(self.storage.installed_plugins_dir / plugin_cls.manifest.name)
 
-        plugin_cls.installed = False
+        plugin_cls.is_installed = False
         return True
 
     def import_plugins(self, src: str | PathLike[str]) -> list[type[BasePlugin]]:
         """Import plugins from the specified directory."""
         src = Path(src)
 
         if not src.is_dir():
@@ -236,36 +306,35 @@
                 continue
 
             # Import modules with the same name from different directories
             try:
                 sys.path.insert(0, str(plugin_dir))
 
                 plugin_cls = import_module("plugin").Plugin
+                plugin_version = plugin_cls.manifest.version
 
-                if plugin_cls.config.compatible_with:
-                    plugin_version = plugin_cls.config.version
-
-                    try:
-                        if get_app_version() not in SpecifierSet(plugin_cls.config.compatible_with):
-                            self.console.print_warning(
-                                f"Plugin {format_program(plugin_cls.config.name)} "
-                                f"{f'version {plugin_version}' if plugin_version else 'with an unknown version'} "
-                                "is not compatible with the current version of the application. Skipping it."
-                            )
-
-                            plugin_cls.compatible = False
-                    except InvalidSpecifier:
+                try:
+                    if get_app_version() not in SpecifierSet(plugin_cls.manifest.compatible_with):
                         self.console.print_warning(
-                            f"Plugin {format_program(plugin_cls.config.name)} "
-                            f"{f'version {plugin_version}' if plugin_version else 'with an unknown version'} "
-                            "has an invalid version specifier. Skipping it."
+                            f"Plugin {format_program(plugin_cls.manifest.name)} "
+                            f"{f"version {plugin_version}" if plugin_version else "with an unknown version"} "
+                            "is not compatible with the current version of the application. Skipping it."
                         )
 
-                        plugin_cls.compatible = False
+                        plugin_cls.is_compatible = False
+                except InvalidSpecifier:
+                    self.console.print_warning(
+                        f"Plugin {format_program(plugin_cls.manifest.name)} "
+                        f"{f"version {plugin_version}" if plugin_version else "with an unknown version"} "
+                        "has an invalid version specifier. Skipping it."
+                    )
+
+                    plugin_cls.is_compatible = False
 
+                plugin_cls.source = plugin_dir
                 plugin_classes.append(plugin_cls)
             except Exception as e:
                 self.console.print_warning(
                     f"Failed to import plugin from {format_path(plugin_dir)} ({e}). Skipping it."
                 )
             finally:
                 sys.modules.pop("plugin", None)
@@ -273,22 +342,22 @@
 
         return plugin_classes
 
     def extend_models(self) -> None:
         """Extend the models with fields for installed plugins."""
         for plugin_cls in self.compatible_plugin_classes:
             try:
-                extend_enum(EApp, plugin_cls.config.name.upper(), plugin_cls.config.name)
+                extend_enum(EApp, plugin_cls.manifest.name.upper(), plugin_cls.manifest.name)
 
                 settings_cls = plugin_cls.get_plugin_settings_cls()
                 field_info = FieldInfo(annotation=settings_cls, default=settings_cls())
-                Plugins.model_fields[plugin_cls.config.name] = field_info
+                Plugins.model_fields[plugin_cls.manifest.name] = field_info
             except Exception as e:
                 self.console.print_warning(
-                    f"Failed to load plugin {format_program(plugin_cls.config.name)} ({e}). Skipping it."
+                    f"Failed to load plugin {format_program(plugin_cls.manifest.name)} ({e}). Skipping it."
                 )
                 continue
 
         Plugins.model_rebuild(force=True)
         Privilege.model_rebuild(force=True)
         Privileges.model_rebuild(force=True)
         Rules.model_rebuild(force=True)
@@ -297,17 +366,64 @@
         Account.model_rebuild(force=True)
         Users.model_rebuild(force=True)
         Context.model_rebuild(force=True)
 
     def initialize_plugins(self) -> None:
         """Initialize all plugins."""
         for plugin_cls in self.compatible_plugin_classes:
-            plugin_settings = getattr(self.context_manager.config.plugins, plugin_cls.config.name, None)
+            plugin_settings = getattr(self.context_manager.config.plugins, plugin_cls.manifest.name, None)
 
             if plugin_settings is None:
-                self.console.print_error(f"Settings for plugin {format_program(plugin_cls.config.name)} are missing.")
+                self.console.print_error(f"Settings for plugin {format_program(plugin_cls.manifest.name)} are missing.")
                 raise Exit(code=1)
 
             plugin = plugin_cls(plugin_settings, self.console, self.context_manager, self.file_utils, self.storage)
-            plugin.update_data()
+
+            try:
+                plugin.on_plugin_initialization()
+            except Exit:
+                raise
+            except Exception as e:
+                self.console.print_error(f"Failed to initialize plugin {format_program(plugin.manifest.name)} ({e}).")
+                raise Exit(code=1)
+
             self.plugins.append(plugin)
-            self.console.print_debug(f"Loaded plugin {format_program(plugin.config.name)}.")
+            self.console.print_debug(f"Initialized plugin {format_program(plugin.manifest.name)}.")
+
+    def render_plugins(self) -> None:
+        """Render all plugins."""
+        for plugin in self.plugins:
+            try:
+                plugin.on_plugin_rendering()
+            except Exit:
+                raise
+            except Exception as e:
+                self.console.print_error(f"Failed to render plugin {format_program(plugin.manifest.name)} ({e}).")
+                raise Exit(code=1)
+
+            self.renderer.render_plugin(plugin.manifest.name, plugin.context.model_dump())
+            plugin.mark_as_rendered()
+
+            self.context_manager.plugin_outputs.append(plugin.output)
+            self.console.print_debug(f"Rendered plugin {format_program(plugin.manifest.name)}.")
+
+    def update_rendered_plugin_files(self) -> None:
+        for plugin in self.plugins:
+            for web_dir in (self.storage.installed_plugins_dir / plugin.manifest.name / "web").iterdir():
+                if web_dir.name == "lib":
+                    dst_prefix = self.storage.bundled_dir / "web" / "src" / "lib" / "plugins"
+                    self.file_utils.copy(web_dir, dst_prefix / plugin.manifest.name)
+                elif web_dir.name == "routes":
+                    dst_prefix = self.storage.bundled_dir / "web" / "src" / "routes" / "(apps)" / "app"
+                    self.file_utils.copy(web_dir, dst_prefix / plugin.manifest.web_path)
+
+        if self.context_manager.config.branding.cover:
+            self.file_utils.copy(
+                self.context_manager.config.branding.cover,
+                self.storage.bundled_dir / "web" / "src" / "lib" / "assets" / "cover.jpg",
+            )
+
+        if self.context_manager.config.branding.logo:
+            self.file_utils.copy(
+                self.context_manager.config.branding.logo,
+                self.storage.bundled_dir / "web" / "static" / "favicon.png",
+            )
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/core/storage.py` & `lungo_cli-0.4.0/src/lungo_cli/core/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os import PathLike
 from pathlib import Path
 
 from platformdirs import user_cache_path, user_config_path, user_data_path
 from typer import Exit
 
 from .console import Console
-from .constants import APP_AUTHOR, APP_NAME, STORAGE_PREFIX, STORAGE_VERSION
+from .constants import APP_AUTHOR, APP_NAME, PACKAGE_NAME, STORAGE_PREFIX, STORAGE_VERSION
 from .file import FileUtils
 from ..helpers.format import format_path
 from ..models.base import EApp, ECoreService
 
 
 class Storage:
     """Contain all the paths used by the application."""
@@ -156,32 +156,15 @@
     def nginx_gateway_socket_file(self) -> Path:
         return self.managed_dir / "nginx_gateway" / "sockets" / "nginx.sock"
 
     @property
     def kratos_secrets_file(self) -> Path:
         return self.generated_dir / "kratos" / "secrets.yaml"
 
-    def validate(self) -> None:
-        if self.data_latest_dir.is_dir():
-            return
-
-        largest_version = -1
-
-        # List all directories in the data directory
-        for dir_ in self.data_dir.glob(f"{STORAGE_PREFIX}*{os.sep}"):
-            if (version := dir_.name.split(STORAGE_PREFIX, 1)[1]).isdigit():
-                version_number = int(version)
-
-                if version_number > largest_version:
-                    largest_version = version_number
-
-        if largest_version >= 0:
-            self.migrate(self.data_dir / f"{STORAGE_PREFIX}{largest_version}")
-
-        # Always make sure the directories exist
+    def create_dirs(self) -> None:
         app: EApp | ECoreService
         for app in *EApp, *ECoreService:
             self.file_utils.create_dir(self.cache_latest_dir / app.value)
             self.file_utils.change_mode(self.cache_latest_dir / app.value, 0o700)
             self.file_utils.create_dir(self.managed_dir / app.value)
             self.file_utils.change_mode(self.managed_dir / app.value, 0o700)
 
@@ -190,7 +173,37 @@
 
         # FIXME: use `unshare` to copy the files generated by the container to avoid permission issues
         try:
             self.file_utils.copy(from_ / self.generated_rel, self.generated_dir)
             self.file_utils.copy(from_ / self.managed_rel, self.managed_dir)
         except Exit:
             ...
+
+    def migrate_if_needed(self) -> None:
+        if not self.data_latest_dir.is_dir():
+            largest_version = -1
+
+            # List all directories in the data directory
+            for dir_ in self.data_dir.glob(f"{STORAGE_PREFIX}*{os.sep}"):
+                if (version := dir_.name.split(STORAGE_PREFIX, 1)[1]).isdigit():
+                    version_number = int(version)
+
+                    if version_number > largest_version:
+                        largest_version = version_number
+
+            if largest_version >= 0:
+                self.migrate(self.data_dir / f"{STORAGE_PREFIX}{largest_version}")
+
+    def update_bundled_files(self) -> None:
+        self.console.print_info("Updating bundled files...")
+
+        # Backup installed plugins before overwriting the whole directory
+        if self.installed_plugins_dir.is_dir():
+            self.file_utils.move(self.installed_plugins_dir, self.cache_plugins_dir)
+
+        self.file_utils.copy_package_resources(f"{PACKAGE_NAME}.resources", ".", self.bundled_dir)
+
+        if self.cache_plugins_dir.is_dir():
+            self.file_utils.move(self.cache_plugins_dir, self.installed_plugins_dir)
+
+        self.file_utils.change_mode(self.bundled_dir, 0o700)
+        self.file_utils.remove(self.init_file)
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/helpers/common.py` & `lungo_cli-0.4.0/src/lungo_cli/helpers/common.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/helpers/crypto.py` & `lungo_cli-0.4.0/src/lungo_cli/helpers/crypto.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,37 @@
 from datetime import datetime, timedelta, UTC
 from secrets import token_hex
 from typing import BinaryIO
 
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import rsa
+from cryptography.hazmat.primitives.asymmetric import ed25519, rsa
 
 from ..core.constants import APP_NAME_CAPITALIZED
 
 
+def generate_raw_ed25519_keypair() -> tuple[bytes, bytes]:
+    """Generate a raw Ed25519 keypair."""
+    private_key = ed25519.Ed25519PrivateKey.generate()
+    public_key = private_key.public_key()
+
+    public_key_bytes = public_key.public_bytes(
+        encoding=serialization.Encoding.Raw,
+        format=serialization.PublicFormat.Raw,
+    )
+    private_key_bytes = private_key.private_bytes(
+        encoding=serialization.Encoding.Raw,
+        format=serialization.PrivateFormat.Raw,
+        encryption_algorithm=serialization.NoEncryption(),
+    )
+
+    return public_key_bytes, private_key_bytes
+
+
 def generate_self_signed_cert() -> tuple[bytes, bytes]:
     """Generate a self-signed certificate."""
     key = rsa.generate_private_key(public_exponent=65537, key_size=2048, backend=default_backend())
     name = x509.Name([x509.NameAttribute(x509.oid.NameOID.ORGANIZATION_NAME, APP_NAME_CAPITALIZED)])
     serial_number = x509.random_serial_number()
     now = datetime.now(UTC)
     basic_constraints = x509.BasicConstraints(ca=True, path_length=0)
@@ -27,22 +45,22 @@
         .serial_number(serial_number)
         .not_valid_before(now)
         .not_valid_after(now + timedelta(days=36500))
         .add_extension(basic_constraints, False)
         .sign(key, hashes.SHA256(), default_backend())
     )
 
-    cert_pem = cert.public_bytes(encoding=serialization.Encoding.PEM)
-    key_pem = key.private_bytes(
+    cert_bytes = cert.public_bytes(encoding=serialization.Encoding.PEM)
+    key_bytes = key.private_bytes(
         encoding=serialization.Encoding.PEM,
         format=serialization.PrivateFormat.TraditionalOpenSSL,
         encryption_algorithm=serialization.NoEncryption(),
     )
 
-    return cert_pem, key_pem
+    return cert_bytes, key_bytes
 
 
 def generate_random_hex() -> str:
     """Generate a random hex string."""
     return token_hex(32)
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/helpers/format.py` & `lungo_cli-0.4.0/src/lungo_cli/helpers/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,13 +26,13 @@
     """Format a link for console output."""
     if title:
         return f"[link={value}]{title}[/link]"
     else:
         return f"[link={value}]{format_path(value)}[/link]"
 
 
-def format_input(value: str | Enum) -> str:
+def format_input(value: int | str | Enum) -> str:
     """Format user input for console output."""
     if isinstance(value, Enum):
         return f"[cyan]{value.value}[/cyan]"
     else:
         return f"[cyan]{value}[/cyan]"
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/models/base.py` & `lungo_cli-0.4.0/src/lungo_cli/models/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from typing import Annotated, Final, Literal
 
 from aenum import auto, StrEnum
 from pydantic import BaseModel, ConfigDict, Field
 
 
-class Base(BaseModel):
-    model_config = ConfigDict(extra="forbid", frozen=True, str_strip_whitespace=True, use_enum_values=True)
-
-
 class EApp(StrEnum):
     pass
 
 
 class EContainer(StrEnum):
     DOCKER = auto()
     DOCKER_COMPOSE = "docker-compose"
@@ -29,12 +25,23 @@
 
 class ERole(StrEnum):
     GUEST = auto()
     USER = auto()
     ADMIN = auto()
 
 
+class Base(BaseModel):
+    model_config = ConfigDict(extra="forbid", frozen=True, str_strip_whitespace=True, use_enum_values=True)
+
+
+class AppDirs(Base):
+    cache_dir: str
+    generated_dir: str
+    managed_dir: str
+    plugin_dir: str
+
+
 AllowedAppsType: Final = Literal["all"] | list[EApp]
 FileNameType: Final = Annotated[str, Field(pattern=r"^[a-zA-Z0-9._-]+$")]
 NameStrType: Final = Annotated[str, Field(max_length=32)]
 PortType: Final = Annotated[int, Field(ge=1, le=65535)]
 UsernameType: Final = Annotated[str, Field(pattern=r"^[a-z_](?:[a-z0-9_-]{0,31}|[a-z0-9_-]{0,30}\$)$")]
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/models/config.py` & `lungo_cli-0.4.0/src/lungo_cli/models/config.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/models/users.py` & `lungo_cli-0.4.0/src/lungo_cli/models/users.py`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/Dockerfile.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/Dockerfile.jinja`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-{% set FILEBROWSER_VER = 'v2.27.0' %}
-
-FROM docker.io/filebrowser/filebrowser:{{ FILEBROWSER_VER }}
-RUN : && \
+FROM docker.io/rocker/verse:{{ plugin.custom.rstudio_version }}
+RUN \
     {% for account in users.accounts %}
-    mkdir -p '/root/home/{{ account.username }}' && \
-    ln -s '/mnt/home/{{ account.username }}' '/root/home/{{ account.username }}/home' && \
+        {% if account.role == 'admin' %}
+    useradd --no-log-init -g root -G sudo -m -s /usr/bin/bash '{{ account.username }}' && \
+        {% else %}
+    useradd --no-log-init -g root -m -s /usr/bin/bash '{{ account.username }}' && \
+        {% endif %}
+    echo '{{ account.username }}:{{ plugin.custom.rstudio_password }}' | chpasswd && \
+    ln -s '/mnt/home/{{ account.username }}' '/home/{{ account.username }}/home' && \
         {% for shared_dir in account.extra.shared_dirs %}
-    ln -s '/mnt/{{ shared_dir.name }}' '/root/home/{{ account.username }}/{{ shared_dir.name }}' && \
+    ln -s '/mnt/{{ shared_dir.name }}' '/home/{{ account.username }}/{{ shared_dir.name }}' && \
         {% endfor %}
         {% for shared_dir in config.directories.shared_dirs %}
-    ln -s '/mnt/{{ shared_dir.name }}' '/root/home/{{ account.username }}/{{ shared_dir.name }}' && \
+    ln -s '/mnt/{{ shared_dir.name }}' '/home/{{ account.username }}/{{ shared_dir.name }}' && \
         {% endfor %}
     {% endfor %}
     :
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/compose/compose.yaml.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/compose/compose.yaml.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+{% set directories = config.directories %}
+{% set plugin_name = plugin.manifest.name %}
+
 services:
-  filebrowser:
-    container_name: filebrowser
-    hostname: filebrowser
+  {{ plugin_name }}:
+    container_name: {{ plugin_name }}
+    hostname: {{ plugin_name }}
 
     build:
-      context: {{ app_dirs.plugin_dir }}/filebrowser
+      context: {{ plugin.dirs.plugin_dir }}
 
     user: root
     entrypoint: [ ]
     command: >-
       sh -c 'if ! cmp -s /etc/filebrowser/users_export.yaml /var/lib/filebrowser/users_export.old.yaml; then
                rm -f /var/lib/filebrowser/filebrowser.db;
                /filebrowser -c /etc/filebrowser/settings.yaml config init --auth.method=noauth;
@@ -17,30 +20,30 @@
                cp /etc/filebrowser/users_export.yaml /var/lib/filebrowser/users_export.old.yaml;
              fi;
              umask 002;
              /filebrowser -c /etc/filebrowser/settings.yaml'
 
     networks:
       static:
-        ipv4_address: {{ ip_addresses['filebrowser'] }}
+        ipv4_address: {{ plugin.ip_address }}
     expose:
-      - 80
+      - {{ plugin.manifest.backend_port }}
 
     volumes:
-      - '{{ app_dirs.plugin_dir }}/filebrowser/config:/etc/filebrowser:ro'
-      - '{{ app_dirs.cache_dir }}/filebrowser:/var/log/filebrowser:rw'
-      - '{{ app_dirs.managed_dir }}/filebrowser:/var/lib/filebrowser:rw'
+      - '{{ plugin.dirs.plugin_dir }}/config:/etc/filebrowser:ro'
+      - '{{ plugin.dirs.cache_dir }}:/var/log/filebrowser:rw'
+      - '{{ plugin.dirs.managed_dir }}:/var/lib/filebrowser:rw'
       {% for account in users.accounts %}
         {% if account.extra.user_dir %}
       - '{{ account.extra.user_dir }}:/mnt/home/{{ account.username }}:rw'
         {% else %}
-      - '{{ config.directories.users_dir }}/{{ account.username }}:/mnt/home/{{ account.username }}:rw'
+      - '{{ directories.users_dir }}/{{ account.username }}:/mnt/home/{{ account.username }}:rw'
         {% endif %}
         {% for shared_dir in account.extra.shared_dirs %}
       - '{{ shared_dir.source }}:/mnt/{{ shared_dir.name }}:{{ 'ro' if shared_dir.read_only else 'rw' }}'
         {% endfor %}
       {% endfor %}
-      {% for shared_dir in config.directories.shared_dirs %}
+      {% for shared_dir in directories.shared_dirs %}
       - '{{ shared_dir.source }}:/mnt/{{ shared_dir.name }}:{{ 'ro' if shared_dir.read_only else 'rw' }}'
       {% endfor %}
 
     restart: 'unless-stopped'
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/config/config_export.yaml` & `lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/config/config_export.yaml.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -51,19 +51,19 @@
 
   shell: [ ]
 
   rules: [ ]
 
 server:
   root: /
-  baseurl: /app/filebrowser
+  baseurl: {{ plugin.web_prefix }}
   socket: ""
   tlskey: ""
   tlscert: ""
-  port: "80"
+  port: "{{ plugin.manifest.backend_port }}"
   address: 0.0.0.0
   log: /var/log/filebrowser/filebrowser.log
   enablethumbnails: false
   resizepreview: false
   enableexec: false
   typedetectionbyheader: false
   authhook: ""
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/config/users_export.yaml.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/config/users_export.yaml.jinja`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-{% set FILEBROWSER_DEFAULT_PASSWORD_HASH = '$2a$10$aulj1r/ROe0VnA1iE2/ojOItBBFeHK0KLMv5mnl3ECXfiNLKfcKHi' %}
-
 {% for account in users.accounts %}
 - id: 0
   username: {{ account.username }}
-  password: {{ FILEBROWSER_DEFAULT_PASSWORD_HASH }}
+  password: {{ plugin.custom.filebrowser_default_password_hash }}
   scope: /root/home/{{ account.username }}
   locale: en
   lockpassword: true
   viewmode: list
   singleclick: false
   perm:
     admin:
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/oathkeeper/access_rules.yaml.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/oathkeeper/access_rules.yaml.jinja`

 * *Files 24% similar despite different names*

```diff
@@ -27,20 +27,22 @@
     handler: allow
   mutators:
     - handler: noop
   errors:
     - handler: json
 {% endset %}
 
-- id: filebrowser-private
+{% set plugin_name = plugin.manifest.name %}
+
+- id: {{ plugin_name }}-private
   match:
-    url: '{{ base_url }}app/<filebrowser><(?:$|/)(?!(?:api/public|share|static)/).*>'
+    url: '{{ plugin.oathkeeper_url_regex }}<(?:$|/)(?!(?:api/public|share|static)/).*>'
     methods:
       {{ ALL }}
   {{ AUTH }}
 
-- id: filebrowser-public
+- id: {{ plugin_name }}-public
   match:
-    url: '{{ base_url }}app/filebrowser<(?=/(?:api/public|share|static)/).*>'
+    url: '{{ plugin.oathkeeper_url_regex }}<(?=/(?:api/public|share|static)/).*>'
     methods:
       {{ ALL }}
   {{ PASS }}
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderOutline.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderOutline.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderSolid.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/filebrowser/web/lib/icons/FolderSolid.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/Dockerfile.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/Dockerfile.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-{% set JUPYTERHUB_VER = '4.1.5' %}
-{% set JUPYTERLAB_VER = '4.1.6' %}
-
-FROM docker.io/jupyterhub/jupyterhub:{{ JUPYTERHUB_VER }}
+FROM docker.io/jupyterhub/jupyterhub:{{ plugin.custom.jupyterhub_version }}
 RUN python3 -m pip install --no-cache-dir --upgrade setuptools pip && \
-    python3 -m pip install --no-cache-dir 'jupyterlab=={{ JUPYTERLAB_VER }}' && \
+    python3 -m pip install --no-cache-dir 'jupyterlab=={{ plugin.custom.jupyterlab_version }}' && \
     {% for account in users.accounts %}
         {% if account.role == 'admin' %}
     useradd --no-log-init -g root -G sudo -m -s /usr/bin/bash '{{ account.username }}' && \
         {% else %}
     useradd --no-log-init -g root -m -s /usr/bin/bash '{{ account.username }}' && \
         {% endif %}
-    echo '{{ account.username }}:{{ jupyterhub_password }}' | chpasswd && \
+    echo '{{ account.username }}:{{ plugin.custom.jupyterhub_password }}' | chpasswd && \
     ln -s '/mnt/home/{{ account.username }}' '/home/{{ account.username }}/home' && \
         {% for shared_dir in account.extra.shared_dirs %}
     ln -s '/mnt/{{ shared_dir.name }}' '/home/{{ account.username }}/{{ shared_dir.name }}' && \
         {% endfor %}
         {% for shared_dir in config.directories.shared_dirs %}
     ln -s '/mnt/{{ shared_dir.name }}' '/home/{{ account.username }}/{{ shared_dir.name }}' && \
         {% endfor %}
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/compose/compose.yaml.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/compose/compose.yaml.jinja`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,40 @@
+{% set directories = config.directories %}
+{% set plugin_name = plugin.manifest.name %}
+
 services:
-  jupyterhub:
-    container_name: jupyterhub
-    hostname: jupyterhub
+  {{ plugin_name }}:
+    container_name: {{ plugin_name }}
+    hostname: {{ plugin_name }}
 
     build:
-      context: {{ app_dirs.plugin_dir }}/jupyterhub
+      context: {{ plugin.dirs.plugin_dir }}
 
     user: root
     entrypoint: [ ]
-    command: sh -c 'umask 002; jupyterhub -f /etc/jupyterhub/config.py'
+    command: sh -c 'umask 002; /init'
 
     networks:
       static:
-        ipv4_address: {{ ip_addresses['jupyterhub'] }}
+        ipv4_address: {{ plugin.ip_address }}
     expose:
-      - 80
+      - {{ plugin.manifest.backend_port }}
 
     volumes:
-      - '{{ app_dirs.plugin_dir }}/jupyterhub/config:/etc/jupyterhub:ro'
-      - '{{ app_dirs.managed_dir }}/jupyterhub:/srv/jupyterhub:rw'
-        {% for account in users.accounts %}
-          {% if account.extra.user_dir %}
+      - '{{ plugin.dirs.plugin_dir }}/config/rserver.conf:/etc/rstudio/rserver.conf:ro'
+      - '{{ plugin.dirs.plugin_dir }}/config/rsession.conf:/etc/rstudio/rsession.conf:ro'
+      - '{{ plugin.dirs.managed_dir }}:/var/lib/rstudio-server:rw'
+      {% for account in users.accounts %}
+        {% if account.extra.user_dir %}
       - '{{ account.extra.user_dir }}:/mnt/home/{{ account.username }}:rw'
-          {% else %}
-      - '{{ config.directories.users_dir }}/{{ account.username }}:/mnt/home/{{ account.username }}:rw'
-          {% endif %}
-          {% for shared_dir in account.extra.shared_dirs %}
+        {% else %}
+      - '{{ directories.users_dir }}/{{ account.username }}:/mnt/home/{{ account.username }}:rw'
+        {% endif %}
+        {% for shared_dir in account.extra.shared_dirs %}
       - '{{ shared_dir.source }}:/mnt/{{ shared_dir.name }}:{{ 'ro' if shared_dir.read_only else 'rw' }}'
-          {% endfor %}
         {% endfor %}
-        {% for shared_dir in config.directories.shared_dirs %}
+      {% endfor %}
+      {% for shared_dir in directories.shared_dirs %}
       - '{{ shared_dir.source }}:/mnt/{{ shared_dir.name }}:{{ 'ro' if shared_dir.read_only else 'rw' }}'
-        {% endfor %}
-
-    secrets:
-      - source: JUPYTERHUB_COOKIE_SECRET
-        target: /etc/jupyterhub/cookie_secret
+      {% endfor %}
 
     restart: 'unless-stopped'
-
-secrets:
-  JUPYTERHUB_COOKIE_SECRET:
-    file: '{{ app_dirs.generated_dir }}/jupyterhub/cookie_secret'
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/config/config.py.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/config/config.py.jinja`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ## Allow named single-user servers per user
 c.JupyterHub.allow_named_servers = True
 
 ## Class for authenticating users
 c.JupyterHub.authenticator_class = 'jupyterhub.auth.PAMAuthenticator'
 
 ## The public facing URL of the whole JupyterHub application
-c.JupyterHub.bind_url = 'http://0.0.0.0:80/app/jupyterhub/'
+c.JupyterHub.bind_url = 'http://0.0.0.0:{{ plugin.manifest.backend_port }}{{ plugin.web_prefix }}/'
 
 ## The config file to load
 c.JupyterHub.config_file = '/etc/jupyterhub/config.py'
 
 ## File in which to store the cookie secret
 c.JupyterHub.cookie_secret_file = '/etc/jupyterhub/cookie_secret'
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/nginx/site.conf.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/nginx/site.conf.jinja`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-{% set APP_NAME = 'jupyterhub' %}
+{% set plugin_name = plugin.manifest.name %}
 
-location = /app/{{ APP_NAME }} {
+location = {{ plugin.web_prefix }} {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     if ($arg_iframe) {
-        return 307 $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}/?$args;
+        return 307 $http_x_forwarded_proto://$http_x_forwarded_host{{ plugin.web_prefix }}/?$args;
     }
 
     proxy_pass http://node;
 }
 
-location /app/{{ APP_NAME }}/ {
+location {{ plugin.web_prefix }}/ {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     if ($arg_iframe) {
         return 480;
     }
 
@@ -24,18 +24,24 @@
         return 480;
     }
 
     if ($http_referer ~* \?.*iframe=1.*$) {
         return 307 $http_x_forwarded_proto://$http_x_forwarded_host$escaped_uri?iframe=1&$args;
     }
 
-    error_page 480 = @{{ APP_NAME }};
+    error_page 480 = @{{ plugin_name }};
     proxy_pass http://node;
 }
 
-location @{{ APP_NAME }} {
+location @{{ plugin_name }} {
     include snippets/proxy.conf;
     include snippets/auth.conf;
+    proxy_send_timeout 3600s;
 
-    proxy_pass http://{{ APP_NAME }}$escaped_uri?$filtered_args;
-    proxy_redirect ~*^(?:https?://[^/]+)?/app/{{ APP_NAME }}([^?]*)\??(.*)$ $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}$1?iframe=1&$2;
+    # Break into two lines to avoid regex capturing group being overwritten
+    rewrite ^ $escaped_uri?$filtered_args?;
+    rewrite ^{{ plugin.web_prefix }}/(.*)$ /$1 break;
+
+    proxy_set_header X-RStudio-Root-Path {{ plugin.web_prefix }};
+    proxy_pass http://{{ plugin_name }};
+    proxy_redirect ~*^(?:https?://[^/]+)?{{ plugin.web_prefix }}([^?]*)\??(.*)$ $http_x_forwarded_proto://$http_x_forwarded_host{{ plugin.web_prefix }}$1?iframe=1&$2;
 }
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/plugin.py` & `lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 from pathlib import Path
 from typing import Any, override
 
-from lungo_cli.core.plugin import BasePlugin, BaseSettings, PluginConfig
+from lungo_cli.core.plugin import BasePlugin, BaseSettings, PluginManifest
 from lungo_cli.helpers.crypto import generate_random_hex
 
 
 class Settings(BaseSettings):
     password: str | None = None
 
 
 class Plugin(BasePlugin[Settings]):
-    config = PluginConfig(
+    manifest = PluginManifest(
         name="jupyterhub",
+        version="0.2.0",
         descriptive_name="JupyterHub",
-        version="0.1.0",
         description="JupyterHub as a Lungo plugin.",
-        compatible_with="~=0.3.0",
+        compatible_with="~=0.4.0",
         have_backend=True,
+        backend_port=80,
         require_account=True,
         web_icon="icons/Jupyter.svelte",
     )
 
     @property
     def cookie_secret_file(self) -> Path:
-        return self.storage.generated_dir / "jupyterhub" / "cookie_secret"
+        return self.storage.generated_dir / self.manifest.name / "cookie_secret"
 
     @property
     def password_file(self) -> Path:
-        return self.storage.generated_dir / "jupyterhub" / "password"
+        return self.storage.generated_dir / self.manifest.name / "password"
 
     @classmethod
     @override
     def get_plugin_settings_cls(cls) -> type[Settings]:
         return Settings
 
     @override
-    def get_render_context(self) -> dict[str, Any]:
-        return {"jupyterhub_password": self.settings.password or self.file_utils.read_text(self.password_file)}
+    def get_custom_rendering_context(self) -> dict[str, Any]:
+        return {
+            "jupyterhub_password": self.settings.password or self.file_utils.read_text(self.password_file),
+            "jupyterhub_version": "4.1.5",
+            "jupyterlab_version": "4.2.0",
+        }
 
     @override
-    def update_data(self) -> None:
+    def on_plugin_initialization(self) -> None:
         if not self.cookie_secret_file.is_file():
             self.console.print_info("Generating JupyterHub cookie secret...")
             self.file_utils.write_text(self.cookie_secret_file, generate_random_hex(), True)
 
         if not self.password_file.is_file():
             self.console.print_info("Generating JupyterHub password...")
             self.file_utils.write_text(self.password_file, generate_random_hex(), True)
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/lib/icons/Jupyter.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/web/lib/icons/Jupyter.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/jupyterhub/web/routes/+layout.server.ts` & `lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/web/routes/+layout.server.ts`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import { load as loadHtmlString } from "cheerio"
-import { JUPYTERHUB_BASE_URL, JUPYTERHUB_PASSWORD } from "$lib/plugins/jupyterhub/server/constants.server"
-import { wrapFetch } from "$lib/utils"
+import {
+    JUPYTERHUB_BASE_URL,
+    JUPYTERHUB_PASSWORD,
+    JUPYTERHUB_WEB_PREFIX,
+} from "$lib/plugins/jupyterhub/server/constants.server"
+import { getCookieHeader, wrapFetch } from "$lib/utils"
 
-export async function load({ cookies, fetch, parent }) {
+export async function load({ cookies, fetch, parent, request }) {
     const wrappedFetch = wrapFetch({
         fetch,
         baseUrl: JUPYTERHUB_BASE_URL,
+        cookieHeader: getCookieHeader(request),
+        cookiePath: JUPYTERHUB_WEB_PREFIX,
         cookies,
-        cookiePath: "/app/jupyterhub",
         credentials: "include",
         ensureOk: true,
     })
 
-    const response = await wrappedFetch("/app/jupyterhub/hub/login", { redirect: "manual" })
+    const response = await wrappedFetch(`${JUPYTERHUB_WEB_PREFIX}/hub/login`, { redirect: "manual" })
 
     // If the user is already logged in, return
     if (response.status == 302) {
         return
     }
 
     const $ = loadHtmlString(await response.text())
     const csrf = $("#login-main input[name=_xsrf]").attr("value")!
 
     const { userInfo } = await parent()
     const username = userInfo?.username ?? "anonymous"
 
-    await wrappedFetch("/app/jupyterhub/hub/login", {
+    await wrappedFetch(`${JUPYTERHUB_WEB_PREFIX}/hub/login`, {
         method: "POST",
         redirect: "manual",
         headers: { "Content-Type": "application/x-www-form-urlencoded" },
         body: new URLSearchParams({
             _xsrf: csrf,
             username,
             password: JUPYTERHUB_PASSWORD,
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/config/conf.php.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/config/conf.php.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ;<?php http_response_code(403); /*
 ; config file for PrivateBin
 ;
 ; An explanation of each setting can be find online at https://github.com/PrivateBin/PrivateBin/wiki/Configuration.
 
 [main]
 ; (optional) set a project name to be displayed on the website
-name = "Pastebin"
+name = "{{ plugin.manifest.descriptive_name }}"
 
 ; The full URL, with the domain name and directories that point to the
 ; PrivateBin files, including an ending slash (/). This URL is essential to
 ; allow Opengraph images to be displayed on social networks.
-basepath = "{{ base_url }}app/pastebin/"
+basepath = "{{ plugin.web_base_url }}"
 
 ; enable or disable the discussion feature, defaults to true
 discussion = true
 
 ; preselect the discussion feature, defaults to false
 opendiscussion = false
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/config/site.conf` & `lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/config/site.conf.jinja`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 server {
-    listen 80 default_server;
-    listen [::]:80 default_server;
+    listen {{ plugin.manifest.backend_port }} default_server;
+    listen [::]:{{ plugin.manifest.backend_port }} default_server;
 
     root /var/www;
     index index.php index.html index.htm;
 
     location / {
         # no-transform tells Cloudflare and others to not change the content of the file and thus breaking SRI
         # https://developers.cloudflare.com/cache/about/cache-control#other
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/nginx/site.conf.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/nginx/site.conf.jinja`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-{% set APP_NAME = 'privatebin' %}
+{% set plugin_name = plugin.manifest.name %}
 
-location = /app/{{ APP_NAME }} {
+location = {{ plugin.web_prefix }} {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     if ($arg_iframe) {
-        return 307 $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}/?$args;
+        return 307 $http_x_forwarded_proto://$http_x_forwarded_host{{ plugin.web_prefix }}/?$args;
     }
 
     proxy_pass http://node;
 }
 
-location /app/{{ APP_NAME }}/ {
+location {{ plugin.web_prefix }}/ {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     if ($arg_iframe) {
         return 480;
     }
 
     if ($http_referer ~* \?.*iframe=1.*$) {
         return 307 $http_x_forwarded_proto://$http_x_forwarded_host$escaped_uri?iframe=1&$args;
     }
 
-    error_page 480 = @{{ APP_NAME }};
+    error_page 480 = @{{ plugin_name }};
     proxy_pass http://node;
 }
 
-location @{{ APP_NAME }} {
+location @{{ plugin_name }} {
     include snippets/proxy.conf;
     include snippets/auth.conf;
 
     # Break into two lines to avoid regex capturing group being overwritten
     rewrite ^ $escaped_uri?$filtered_args?;
-    rewrite ^/app/{{ APP_NAME }}/(.*)$ /$1 break;
+    rewrite ^{{ plugin.web_prefix }}/(.*)$ /$1 break;
 
-    proxy_pass http://{{ APP_NAME }};
-    proxy_redirect ~*^(?:https?://[^/]+)?/app/{{ APP_NAME }}([^?]*)\??(.*)$ $http_x_forwarded_proto://$http_x_forwarded_host/app/{{ APP_NAME }}?iframe=1&$2;
+    proxy_pass http://{{ plugin_name }};
+    proxy_redirect ~*^(?:https?://[^/]+)?{{ plugin.web_prefix }}([^?]*)\??(.*)$ $http_x_forwarded_proto://$http_x_forwarded_host{{ plugin.web_prefix }}?iframe=1&$2;
 }
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteOutline.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteOutline.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteSolid.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/privatebin/web/lib/icons/NoteSolid.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/compose/compose.yaml.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/jupyterhub/compose/compose.yaml.jinja`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,47 @@
+{% set directories = config.directories %}
+{% set plugin_name = plugin.manifest.name %}
+
 services:
-  rstudio:
-    container_name: rstudio
-    hostname: rstudio
+  {{ plugin_name }}:
+    container_name: {{ plugin_name }}
+    hostname: {{ plugin_name }}
 
     build:
-      context: {{ app_dirs.plugin_dir }}/rstudio
+      context: {{ plugin.dirs.plugin_dir }}
 
     user: root
     entrypoint: [ ]
-    command: sh -c 'umask 002; /init'
+    command: sh -c 'umask 002; jupyterhub -f /etc/jupyterhub/config.py'
 
     networks:
       static:
-        ipv4_address: {{ ip_addresses['rstudio'] }}
+        ipv4_address: {{ plugin.ip_address }}
     expose:
-      - 80
+      - {{ plugin.manifest.backend_port }}
 
     volumes:
-      - '{{ app_dirs.plugin_dir }}/rstudio/config/rserver.conf:/etc/rstudio/rserver.conf:ro'
-      - '{{ app_dirs.plugin_dir }}/rstudio/config/rsession.conf:/etc/rstudio/rsession.conf:ro'
-      - '{{ app_dirs.managed_dir }}/rstudio:/var/lib/rstudio-server:rw'
-      {% for account in users.accounts %}
-        {% if account.extra.user_dir %}
+      - '{{ plugin.dirs.plugin_dir }}/config:/etc/jupyterhub:ro'
+      - '{{ plugin.dirs.managed_dir }}:/srv/jupyterhub:rw'
+        {% for account in users.accounts %}
+          {% if account.extra.user_dir %}
       - '{{ account.extra.user_dir }}:/mnt/home/{{ account.username }}:rw'
-        {% else %}
-      - '{{ config.directories.users_dir }}/{{ account.username }}:/mnt/home/{{ account.username }}:rw'
-        {% endif %}
-        {% for shared_dir in account.extra.shared_dirs %}
+          {% else %}
+      - '{{ directories.users_dir }}/{{ account.username }}:/mnt/home/{{ account.username }}:rw'
+          {% endif %}
+          {% for shared_dir in account.extra.shared_dirs %}
       - '{{ shared_dir.source }}:/mnt/{{ shared_dir.name }}:{{ 'ro' if shared_dir.read_only else 'rw' }}'
+          {% endfor %}
         {% endfor %}
-      {% endfor %}
-      {% for shared_dir in config.directories.shared_dirs %}
+        {% for shared_dir in directories.shared_dirs %}
       - '{{ shared_dir.source }}:/mnt/{{ shared_dir.name }}:{{ 'ro' if shared_dir.read_only else 'rw' }}'
-      {% endfor %}
+        {% endfor %}
+
+    secrets:
+      - source: JUPYTERHUB_COOKIE_SECRET
+        target: /etc/jupyterhub/cookie_secret
 
     restart: 'unless-stopped'
+
+secrets:
+  JUPYTERHUB_COOKIE_SECRET:
+    file: '{{ plugin.dirs.generated_dir }}/cookie_secret'
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/plugin.py` & `lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/plugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 from pathlib import Path
 from typing import Any, override
 
-from lungo_cli.core.plugin import BasePlugin, BaseSettings, PluginConfig
+from lungo_cli.core.plugin import BasePlugin, BaseSettings, PluginManifest
 from lungo_cli.helpers.crypto import generate_random_hex
 
 
 class Settings(BaseSettings):
     password: str | None = None
 
 
 class Plugin(BasePlugin[Settings]):
-    config = PluginConfig(
+    manifest = PluginManifest(
         name="rstudio",
+        version="0.2.0",
         descriptive_name="RStudio",
-        version="0.1.0",
         description="RStudio as a Lungo plugin.",
-        compatible_with="~=0.3.0",
+        compatible_with="~=0.4.0",
         have_backend=True,
+        backend_port=80,
         require_account=True,
         web_icon="icons/RStudioOutline.svelte",
         web_alt_icon="icons/RStudioSolid.svelte",
     )
 
     @property
     def password_file(self) -> Path:
-        return self.storage.generated_dir / "rstudio" / "password"
+        return self.storage.generated_dir / self.manifest.name / "password"
 
     @classmethod
     @override
     def get_plugin_settings_cls(cls) -> type[Settings]:
         return Settings
 
     @override
-    def get_render_context(self) -> dict[str, Any]:
-        return {"rstudio_password": self.settings.password or self.file_utils.read_text(self.password_file)}
+    def get_custom_rendering_context(self) -> dict[str, Any]:
+        return {
+            "rstudio_password": self.settings.password or self.file_utils.read_text(self.password_file),
+            "rstudio_version": "4.4.0",
+        }
 
     @override
-    def update_data(self) -> None:
+    def on_plugin_initialization(self) -> None:
         if not self.password_file.is_file():
             self.console.print_info("Generating RStudio password...")
             self.file_utils.write_text(self.password_file, generate_random_hex(), True)
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioOutline.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioOutline.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioSolid.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/lib/icons/RStudioSolid.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/rstudio/web/routes/+layout.server.ts` & `lungo_cli-0.4.0/src/lungo_cli/plugins/rstudio/web/routes/+layout.server.ts`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import { load as loadHtmlString } from "cheerio"
-import { RSTUDIO_BASE_URL, RSTUDIO_PASSWORD } from "$lib/plugins/rstudio/server/constants.server"
-import { wrapFetch } from "$lib/utils"
+import { RSTUDIO_BASE_URL, RSTUDIO_PASSWORD, RSTUDIO_WEB_PREFIX } from "$lib/plugins/rstudio/server/constants.server"
+import { getCookieHeader, wrapFetch } from "$lib/utils"
 
-export async function load({ cookies, fetch, parent }) {
+export async function load({ cookies, fetch, parent, request }) {
     const wrappedFetch = wrapFetch({
         fetch,
         baseUrl: RSTUDIO_BASE_URL,
+        cookieHeader: getCookieHeader(request),
+        cookiePath: RSTUDIO_WEB_PREFIX,
         cookies,
-        cookiePath: "/app/rstudio",
         credentials: "include",
         ensureOk: true,
     })
 
     const response = await wrappedFetch("/auth-sign-in", { redirect: "manual" })
 
     // If the user is already logged in, return
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/README.md` & `lungo_cli-0.4.0/src/lungo_cli/plugins/xray/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 ## Configuration
 
 ```yaml
 # ========
 # plugins:
 # ========
 
-#   # Settings for the Xray module
+#   # Settings for the Xray plugin
 #   xray:
 
-#     # Enable or disable the module
+#     # Enable or disable the plugin
 #     # Type: boolean
 #     # Default: true
 #     # Required: no
 #     enabled: true
 
 #     # Domain whitelist (used only as a template for configuring the proxy client)
 #     # Type: array
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/config/config.json.jinja` & `lungo_cli-0.4.0/src/lungo_cli/plugins/xray/config/config.json.jinja`

 * *Files 20% similar despite different names*

```diff
@@ -5,18 +5,18 @@
         "loglevel": "{{ 'debug' if dev else 'warning' }}",
         "dnsLog": false
     },
     "inbounds": [
         {
             "protocol": "vless",
             "listen": "0.0.0.0",
-            "port": 80,
+            "port": {{ plugin.manifest.backend_port }},
             "settings": {
                 "clients": [
-                    {% for account in xray_accounts %}
+                    {% for account in plugin.custom.xray_accounts %}
                     {
                         "email": "{{ account[0] }}",
                         "id": "{{ account[1]|string }}"
                     }
                     {{- '' if loop.last else ',' }}
                     {% endfor %}
                 ],
@@ -27,15 +27,15 @@
                 "security": "none",
                 "tlsSettings": {
                     "alpn": [
                         "http/1.1"
                     ]
                 },
                 "wsSettings": {
-                    "path": "/app/xray"
+                    "path": "{{ plugin.web_prefix }}"
                 }
             }
         }
     ],
     "outbounds": [
         {
             "protocol": "freedom"
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/plugin.py` & `lungo_cli-0.4.0/src/lungo_cli/plugins/xray/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 from ipaddress import IPv4Network
 from pathlib import Path
 from typing import Any, override
 from uuid import UUID, uuid1, uuid5
 
-from lungo_cli.core.plugin import BasePlugin, BaseSettings, PluginConfig
+from lungo_cli.core.plugin import BasePlugin, BaseSettings, PluginManifest
 
 
 class Settings(BaseSettings):
     domain_whitelist: list[str] = []
     domain_keyword_whitelist: list[str] = []
     domain_suffix_whitelist: list[str] = []
     ip_range_whitelist: list[IPv4Network] = []
 
 
 class Plugin(BasePlugin[Settings]):
-    config = PluginConfig(
+    manifest = PluginManifest(
         name="xray",
+        version="0.2.0",
         descriptive_name="Xray",
-        version="0.1.0",
         description="Xray as a Lungo plugin.",
-        compatible_with="~=0.3.0",
+        compatible_with="~=0.4.0",
         have_backend=True,
+        backend_port=80,
         require_account=True,
         web_icon="icons/ProxyOutline.svelte",
         web_alt_icon="icons/ProxySolid.svelte",
     )
 
     @property
     def salt_file(self) -> Path:
-        return self.storage.generated_dir / "xray" / "salt"
+        return self.storage.generated_dir / self.manifest.name / "salt"
 
     @classmethod
     @override
     def get_plugin_settings_cls(cls) -> type[Settings]:
         return Settings
 
     @override
-    def get_render_context(self) -> dict[str, Any]:
+    def get_custom_rendering_context(self) -> dict[str, Any]:
         salt = UUID(self.file_utils.read_text(self.salt_file))
 
         return {
             "xray_accounts": [
                 (account.email, uuid5(salt, account.username)) for account in self.context_manager.users.accounts
             ],
             "xray_salt": salt,
+            "xray_version": "1.8.11",
         }
 
     @override
-    def update_data(self) -> None:
+    def on_plugin_initialization(self) -> None:
         if not self.salt_file.is_file():
             self.console.print_info("Generating Xray salt...")
             self.file_utils.write_text(self.salt_file, str(uuid1()), True)
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/components/CodeBlock.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/components/CodeBlock.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/NetworkLock.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/icons/NetworkLock.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxyOutline.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxyOutline.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxySolid.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/lib/icons/ProxySolid.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/routes/+page.server.ts` & `lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/routes/+page.server.ts`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import { v5 as uuidv5 } from "uuid"
 import {
     XRAY_DOMAIN_KEYWORD_WHITELIST,
     XRAY_DOMAIN_SUFFIX_WHITELIST,
     XRAY_DOMAIN_WHITELIST,
     XRAY_IP_RANGE_WHITELIST,
     XRAY_SALT,
+    XRAY_WEB_PREFIX,
 } from "$lib/plugins/xray/server/constants.server"
 
 export async function load({ parent }) {
     const { userInfo } = await parent()
     const username = userInfo?.username ?? "anonymous"
 
     return {
         xrayDomainKeywordWhitelist: JSON.parse(XRAY_DOMAIN_KEYWORD_WHITELIST) as string[],
         xrayDomainSuffixWhitelist: JSON.parse(XRAY_DOMAIN_SUFFIX_WHITELIST) as string[],
         xrayDomainWhitelist: JSON.parse(XRAY_DOMAIN_WHITELIST) as string[],
         xrayId: uuidv5(username, XRAY_SALT),
         xrayIpRangeWhitelist: JSON.parse(XRAY_IP_RANGE_WHITELIST) as string[],
+        xrayWebPrefix: XRAY_WEB_PREFIX,
     }
 }
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/plugins/xray/web/routes/+page.svelte` & `lungo_cli-0.4.0/src/lungo_cli/plugins/xray/web/routes/+page.svelte`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <script lang="ts">
     import { HOSTNAME, HTTPS_PORT } from "$lib/constants"
-    import CodeBlock from "$lib/plugins/xray/components/CodeBlock.svelte"
-    import NetworkLockIcon from "$lib/plugins/xray/icons/NetworkLock.svelte"
+    import { CodeBlock } from "$lib/plugins/xray/components"
+    import { NetworkLockIcon } from "$lib/plugins/xray/icons"
 
     export let data
 
     const clashConfig = `
         proxies:
           - name: VPN
             type: vless
@@ -13,15 +13,15 @@
             port: ${HTTPS_PORT}
             uuid: "${data.xrayId}"
             tls: true
             skip-cert-verify: true
             udp: true
             network: ws
             ws-opts:
-              path: /app/xray
+              path: ${data.xrayWebPrefix}
     `
     const xrayConfig = `
         "outbounds": [
           {
             "tag": "VPN",
             "protocol": "vless",
             "settings": {
@@ -41,15 +41,15 @@
             "streamSettings": {
               "network": "ws",
               "security": "tls",
               "tlsSettings": {
                 "allowInsecure": true,
               },
               "wsSettings": {
-                "path": "/app/xray"
+                "path": "${data.xrayWebPrefix}"
               }
             }
           }
         ]
     `
 
     let clashRules = [] as string[]
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/assets/config_references/config.yaml` & `lungo_cli-0.4.0/src/lungo_cli/resources/assets/config_references/config.yaml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/assets/config_references/users.yaml` & `lungo_cli-0.4.0/src/lungo_cli/resources/assets/config_references/users.yaml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/compose.yaml.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/compose.yaml.jinja`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-{% set KETO_VER = 'v0.12.0' %}
-{% set KRATOS_VER = 'v1.1.0' %}
-{% set OATHKEEPER_VER = 'v0.40.7' %}
-
 {% set accounts = users.accounts %}
 {% set branding = config.branding %}
 {% set directories = config.directories %}
 {% set network = config.network %}
 {% set plugins = config.plugins %}
 
 services:
@@ -84,30 +80,30 @@
 
     depends_on:
       - keto
       - kratos
       - oathkeeper
       - node
       {% for plugin_output in plugin_outputs %}
-        {% if plugin_output.config.have_backend and plugins[plugin_output.config.name].enabled %}
-      - {{ plugin_output.config.name }}
+        {% if plugin_output.manifest.have_backend and plugins[plugin_output.manifest.name].enabled %}
+      - {{ plugin_output.manifest.name }}
         {% endif %}
       {% endfor %}
 
     restart: 'unless-stopped'
 
   # ============================== #
   # Identity and access management #
   # ============================== #
 
   keto:
     container_name: keto
     hostname: keto
 
-    image: 'docker.io/oryd/keto:{{ KETO_VER }}'
+    image: 'docker.io/oryd/keto:{{ constants.keto_version }}'
 
     user: root
     entrypoint: [ ]
     command: >-
       sh -c 'keto migrate up -c /etc/keto/config.yaml -y;
       keto serve -c /etc/keto/config.yaml --sqa-opt-out >/var/log/keto/main.log 2>&1'
 
@@ -124,15 +120,15 @@
 
     restart: 'unless-stopped'
 
   kratos:
     container_name: kratos
     hostname: kratos
 
-    image: 'docker.io/oryd/kratos:{{ KRATOS_VER }}'
+    image: 'docker.io/oryd/kratos:{{ constants.kratos_version }}'
 
     user: root
     entrypoint: [ ]
     command: >-
       sh -c 'kratos migrate sql -c /etc/kratos/config.yaml -c /etc/kratos/secrets.yaml -e -y;
       kratos serve -c /etc/kratos/config.yaml -c /etc/kratos/secrets.yaml --sqa-opt-out --watch-courier
       >/var/log/kratos/main.log 2>&1'
@@ -144,27 +140,28 @@
       - 80
 
     volumes:
       - './config/kratos:/etc/kratos:ro'
       - '{{ app_dirs.cache_dir }}/kratos:/var/log/kratos:rw'
       - '{{ app_dirs.managed_dir }}/kratos:/var/lib/kratos:rw'
 
-    environment:
-      - DSN=sqlite:////var/lib/kratos/db.sqlite3?_fk=true&mode=rwc
     secrets:
       - source: KRATOS_SECRETS
         target: /etc/kratos/secrets.yaml
 
+    environment:
+      - DSN=sqlite:////var/lib/kratos/db.sqlite3?_fk=true&mode=rwc
+
     restart: 'unless-stopped'
 
   oathkeeper:
     container_name: oathkeeper
     hostname: oathkeeper
 
-    image: 'docker.io/oryd/oathkeeper:{{ OATHKEEPER_VER }}'
+    image: 'docker.io/oryd/oathkeeper:{{ constants.oathkeeper_version }}'
 
     user: root
     entrypoint: [ ]
     command: oathkeeper serve -c /etc/oathkeeper/config.yaml --sqa-opt-out >/var/log/oathkeeper/main.log 2>&1
 
     networks:
       static:
@@ -220,15 +217,15 @@
     restart: 'unless-stopped'
 
   # =============== #
   # Custom services #
   # =============== #
 
   {% for plugin_output in plugin_outputs %}
-    {% if plugin_output.config.have_backend and plugins[plugin_output.config.name].enabled %}
+    {% if plugin_output.manifest.have_backend and plugins[plugin_output.manifest.name].enabled %}
   {{ plugin_output.compose_services }}
     {% endif %}
   {% endfor %}
 
 networks:
   static:
     ipam:
@@ -242,11 +239,11 @@
       {{ network.https.tls.key }}
       {% else %}
       {{ app_dirs.generated_dir }}/nginx_gateway/lungo.key
       {% endif %}
   KRATOS_SECRETS:
     file: '{{ app_dirs.generated_dir }}/kratos/secrets.yaml'
   {% for plugin_output in plugin_outputs %}
-    {% if plugin_output.config.have_backend and plugins[plugin_output.config.name].enabled %}
+    {% if plugin_output.manifest.have_backend and plugins[plugin_output.manifest.name].enabled %}
   {{ plugin_output.compose_secrets }}
     {% endif %}
   {% endfor %}
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/config.yaml.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/config.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.gotmpl.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/email_templates/login_code/valid/email.body.gotmpl.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/email_templates/recovery_code/valid/email.body.gotmpl.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/kratos/user.schema.json` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/kratos/user.schema.json`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx/conf.d/default.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx/sites/oathkeeper.conf`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,15 @@
     client_body_buffer_size 128k;
     proxy_http_version 1.1;
     proxy_cache_bypass $cookie_lungo_session;
     proxy_no_cache $cookie_lungo_session;
     proxy_buffers 64 256k;
 
     ## Advanced Proxy Configuration
-    send_timeout 5m;
-    proxy_read_timeout 240;
-    proxy_send_timeout 240;
-    proxy_connect_timeout 240;
+    proxy_connect_timeout 10s;
 
     ## Disable request body
     proxy_set_header Content-Length "";
     proxy_pass_request_body off;
 
     proxy_pass http://oathkeeper/decisions$request_uri;
 }
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx/snippets/auth.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx/snippets/auth.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx_gateway/conf.d/default.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx_gateway/snippets/proxy.conf.jinja`

 * *Files 4% similar despite different names*

```diff
@@ -39,11 +39,9 @@
 {% for proxy in network.trusted_proxies %}
 set_real_ip_from {{ proxy }};
 {% endfor %}
 real_ip_header X-Forwarded-For;
 real_ip_recursive on;
 
 ## Advanced Proxy Configuration
-send_timeout 5m;
-proxy_read_timeout 240;
-proxy_send_timeout 240;
-proxy_connect_timeout 240;
+proxy_send_timeout 3600s;
+proxy_connect_timeout 10s;
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/nginx_gateway/snippets/rate_limiting.conf.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/oathkeeper/access_rules.yaml.jinja`

 * *Files 16% similar despite different names*

```diff
@@ -29,31 +29,32 @@
     - handler: noop
   errors:
     - handler: json
 {% endset %}
 
 {% set plugins = config.plugins %}
 {% set app_with_rules %}
-  {% for plugin_output in plugin_outputs if plugins[plugin_output.config.name].enabled and plugin_output.oathkeeper_rules -%}
-    {{ plugin_output.config.name ~ '$' ~ '|' ~ plugin_output.config.name ~ '/' }}{{ '|' if not loop.last }}
+  {% for plugin_output in plugin_outputs if plugins[plugin_output.manifest.name].enabled and plugin_output.oathkeeper_rules %}
+    {% set plugin_web_path = plugin_output.manifest.web_path_name or plugin_output.manifest.name -%}
+    {{ plugin_web_path ~ '$' ~ '|' ~ plugin_web_path ~ '/' }}{{ '|' if not loop.last }}
   {%- endfor %}
 {% endset %}
 
 - id: apps
   match:
-    url: '{{ base_url }}app/<(?!(?:{{ app_with_rules }}))[^/]*><.*>'
+    url: '{{ base_url }}app/<(?!(?:{{ '$|' ~ app_with_rules if app_with_rules else '$' }}))[^/]*><.*>'
     methods:
       {{ ALL }}
   {{ AUTH }}
 
 {% for plugin_output in plugin_outputs %}
-  {% if plugins[plugin_output.config.name].enabled and plugin_output.oathkeeper_rules %}
+  {% if plugins[plugin_output.manifest.name].enabled and plugin_output.oathkeeper_rules %}
 {{ plugin_output.oathkeeper_rules }}
   {% endif %}
 {% endfor %}
 
 - id: catch-all
   match:
-    url: '{{ base_url }}<(?!app/).*>'
+    url: '{{ base_url }}<(?!app/.+).*>'
     methods:
       {{ ALL }}
   {{ PASS }}
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/config/oathkeeper/config.yaml.jinja`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/dockerfiles/kratos_admin/compose.yaml.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-{% set KRATOS_VER = 'v1.1.0' %}
-
 services:
   kratos_admin:
     container_name: kratos_admin
     hostname: kratos_admin
 
-    image: 'docker.io/oryd/kratos:{{ KRATOS_VER }}'
+    image: 'docker.io/oryd/kratos:{{ constants.kratos_version }}'
 
     user: root
     entrypoint: [ ]
     command: >-
       sh -c 'kratos migrate sql -c /etc/kratos/config.yaml -c /etc/kratos/secrets.yaml -e -y;
       kratos serve -c /etc/kratos/config.yaml -c /etc/kratos/secrets.yaml --sqa-opt-out'
 
     ports:
       - '3940:8080'
 
     volumes:
       - '../../config/kratos:/etc/kratos:ro'
       - '{{ app_dirs.managed_dir }}/kratos:/var/lib/kratos:rw'
 
-    environment:
-      - DSN=sqlite:////var/lib/kratos/db.sqlite3?_fk=true&mode=rwc
     secrets:
       - source: KRATOS_SECRETS
         target: /etc/kratos/secrets.yaml
 
+    environment:
+      - DSN=sqlite:////var/lib/kratos/db.sqlite3?_fk=true&mode=rwc
+
 secrets:
   KRATOS_SECRETS:
     file: '{{ app_dirs.generated_dir }}/kratos/secrets.yaml'
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/dockerfiles/nginx.Dockerfile.jinja`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-{% set NGINX_VER = '1.25.3.1-alpine-apk' %}
-
-FROM docker.io/openresty/openresty:{{ NGINX_VER }}
+FROM docker.io/openresty/openresty:{{ constants.openresty_version }}
 RUN adduser -D -H -S www-data && \
     apk add --no-cache logrotate && \
     printf '%s\n' >/etc/logrotate.d/nginx \
         '/var/log/nginx/*.log {' \
         '    daily' \
         '    compress' \
         '    delaycompress' \
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.gitattributes`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/auto-merge.yml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/.github/workflows/server.yml`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/README.md` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/README.md`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/.default.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/no-ssl.default.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/example.com.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/conf.d/templates/no-ssl.example.com.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/requests.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/cross-origin/resource_timing.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/security_file_access.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_filename-based_cache_busting.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/location/web_performance_svgz-compression.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/character_encodings.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/media_types/media_types.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/content-security-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/cross-origin-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/permissions-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/referrer-policy.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/strict-transport-security.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-content-type-options.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/security/x-frame-options.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/certificate_files.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ocsp_stapling.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_balanced.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/policy_strict.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/tls/ssl_engine.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-control.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache-file-descriptors.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/cache_expiration.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/compression.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/content_transformation.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_brotli.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/h5bp/web_performance/pre-compressed_content_gzip.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/mime.types`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/secure.server.localhost.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf` & `lungo_cli-0.4.0/src/lungo_cli/resources/third_party/server_configs_nginx/test/vhosts/server.localhost.conf`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/.eslintrc.cjs` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/.eslintrc.cjs`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/assets/schemas/keto.openapi.json`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/assets/schemas/kratos.openapi.json`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/package.json` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9188034188034189%*

 * *Differences: {"'dependencies'": "{'openapi-fetch': '^0.9.5'}",*

 * * "'devDependencies'": "{'@sveltejs/kit': '^2.5.8', '@tailwindcss/typography': '^0.5.13', "*

 * *                      "'@typescript-eslint/eslint-plugin': '^7.9.0', '@typescript-eslint/parser': "*

 * *                      "'^7.9.0', 'daisyui': '^4.11.1', 'eslint-plugin-svelte': '^2.39.0', "*

 * *                      "'json-schema-to-typescript': '^14.0.4', 'prettier-plugin-tailwindcss': "*

 * *                      "'^0.5.14', 'svelte': '^4.2.17', 'svelte-check': '^3.7.1', 'v […]*

```diff
@@ -1,46 +1,46 @@
 {
     "dependencies": {
-        "openapi-fetch": "^0.8.2",
+        "openapi-fetch": "^0.9.5",
         "set-cookie-parser": "^2.6.0"
     },
     "devDependencies": {
         "@sveltejs/adapter-node": "^5.0.1",
         "@sveltejs/enhanced-img": "^0.2.0",
-        "@sveltejs/kit": "^2.5.6",
+        "@sveltejs/kit": "^2.5.8",
         "@sveltejs/vite-plugin-svelte": "^3.1.0",
-        "@tailwindcss/typography": "^0.5.12",
+        "@tailwindcss/typography": "^0.5.13",
         "@types/set-cookie-parser": "^2.4.7",
-        "@typescript-eslint/eslint-plugin": "^7.6.0",
-        "@typescript-eslint/parser": "^7.6.0",
+        "@typescript-eslint/eslint-plugin": "^7.9.0",
+        "@typescript-eslint/parser": "^7.9.0",
         "autoprefixer": "^10.4.19",
-        "daisyui": "^4.10.1",
+        "daisyui": "^4.11.1",
         "eslint": "^8.57.0",
         "eslint-config-prettier": "^9.1.0",
-        "eslint-plugin-svelte": "^2.37.0",
-        "json-schema-to-typescript": "^13.1.2",
+        "eslint-plugin-svelte": "^2.39.0",
+        "json-schema-to-typescript": "^14.0.4",
         "openapi-typescript": "^6.7.5",
         "postcss": "^8.4.38",
         "postcss-load-config": "^4.0.2",
         "prettier": "^3.2.5",
         "prettier-plugin-svelte": "^3.2.3",
-        "prettier-plugin-tailwindcss": "^0.5.13",
-        "svelte": "^4.2.14",
-        "svelte-check": "^3.6.9",
+        "prettier-plugin-tailwindcss": "^0.5.14",
+        "svelte": "^4.2.17",
+        "svelte-check": "^3.7.1",
         "tailwindcss": "^3.4.3",
         "tslib": "^2.6.2",
         "typescript": "^5.4.5",
-        "vite": "^5.2.8"
+        "vite": "^5.2.11"
     },
     "engines": {
         "node": ">=20.0.0",
         "pnpm": "^8.0.0"
     },
     "name": "lungo",
-    "packageManager": "pnpm@8.15.7",
+    "packageManager": "pnpm@8.15.8",
     "private": true,
     "scripts": {
         "build": "vite build",
         "check": "svelte-kit sync && svelte-check --tsconfig ./tsconfig.json",
         "check:watch": "svelte-kit sync && svelte-check --tsconfig ./tsconfig.json --watch",
         "dev": "vite dev",
         "format": "prettier --write .",
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/pnpm-lock.yaml` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/pnpm-lock.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -2,99 +2,99 @@
 
 settings:
   autoInstallPeers: true
   excludeLinksFromLockfile: false
 
 dependencies:
   openapi-fetch:
-    specifier: ^0.8.2
-    version: 0.8.2
+    specifier: ^0.9.5
+    version: 0.9.5
   set-cookie-parser:
     specifier: ^2.6.0
     version: 2.6.0
 
 devDependencies:
   '@sveltejs/adapter-node':
     specifier: ^5.0.1
-    version: 5.0.1(@sveltejs/kit@2.5.6)
+    version: 5.0.1(@sveltejs/kit@2.5.8)
   '@sveltejs/enhanced-img':
     specifier: ^0.2.0
-    version: 0.2.0(svelte@4.2.14)
+    version: 0.2.0(svelte@4.2.17)
   '@sveltejs/kit':
-    specifier: ^2.5.6
-    version: 2.5.6(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.14)(vite@5.2.8)
+    specifier: ^2.5.8
+    version: 2.5.8(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11)
   '@sveltejs/vite-plugin-svelte':
     specifier: ^3.1.0
-    version: 3.1.0(svelte@4.2.14)(vite@5.2.8)
+    version: 3.1.0(svelte@4.2.17)(vite@5.2.11)
   '@tailwindcss/typography':
-    specifier: ^0.5.12
-    version: 0.5.12(tailwindcss@3.4.3)
+    specifier: ^0.5.13
+    version: 0.5.13(tailwindcss@3.4.3)
   '@types/set-cookie-parser':
     specifier: ^2.4.7
     version: 2.4.7
   '@typescript-eslint/eslint-plugin':
-    specifier: ^7.6.0
-    version: 7.6.0(@typescript-eslint/parser@7.6.0)(eslint@8.57.0)(typescript@5.4.5)
+    specifier: ^7.9.0
+    version: 7.9.0(@typescript-eslint/parser@7.9.0)(eslint@8.57.0)(typescript@5.4.5)
   '@typescript-eslint/parser':
-    specifier: ^7.6.0
-    version: 7.6.0(eslint@8.57.0)(typescript@5.4.5)
+    specifier: ^7.9.0
+    version: 7.9.0(eslint@8.57.0)(typescript@5.4.5)
   autoprefixer:
     specifier: ^10.4.19
     version: 10.4.19(postcss@8.4.38)
   daisyui:
-    specifier: ^4.10.1
-    version: 4.10.1(postcss@8.4.38)
+    specifier: ^4.11.1
+    version: 4.11.1(postcss@8.4.38)
   eslint:
     specifier: ^8.57.0
     version: 8.57.0
   eslint-config-prettier:
     specifier: ^9.1.0
     version: 9.1.0(eslint@8.57.0)
   eslint-plugin-svelte:
-    specifier: ^2.37.0
-    version: 2.37.0(eslint@8.57.0)(svelte@4.2.14)
+    specifier: ^2.39.0
+    version: 2.39.0(eslint@8.57.0)(svelte@4.2.17)
   json-schema-to-typescript:
-    specifier: ^13.1.2
-    version: 13.1.2
+    specifier: ^14.0.4
+    version: 14.0.4
   openapi-typescript:
     specifier: ^6.7.5
     version: 6.7.5
   postcss:
     specifier: ^8.4.38
     version: 8.4.38
   postcss-load-config:
     specifier: ^4.0.2
     version: 4.0.2(postcss@8.4.38)
   prettier:
     specifier: ^3.2.5
     version: 3.2.5
   prettier-plugin-svelte:
     specifier: ^3.2.3
-    version: 3.2.3(prettier@3.2.5)(svelte@4.2.14)
+    version: 3.2.3(prettier@3.2.5)(svelte@4.2.17)
   prettier-plugin-tailwindcss:
-    specifier: ^0.5.13
-    version: 0.5.13(prettier-plugin-svelte@3.2.3)(prettier@3.2.5)
+    specifier: ^0.5.14
+    version: 0.5.14(prettier-plugin-svelte@3.2.3)(prettier@3.2.5)
   svelte:
-    specifier: ^4.2.14
-    version: 4.2.14
+    specifier: ^4.2.17
+    version: 4.2.17
   svelte-check:
-    specifier: ^3.6.9
-    version: 3.6.9(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.14)
+    specifier: ^3.7.1
+    version: 3.7.1(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.17)
   tailwindcss:
     specifier: ^3.4.3
     version: 3.4.3
   tslib:
     specifier: ^2.6.2
     version: 2.6.2
   typescript:
     specifier: ^5.4.5
     version: 5.4.5
   vite:
-    specifier: ^5.2.8
-    version: 5.2.8
+    specifier: ^5.2.11
+    version: 5.2.11
 
 packages:
 
   /@aashutoshrathi/word-wrap@1.2.6:
     resolution: {integrity: sha512-1Yjs2SvM8TflER/OD3cOjhWWOZb58A2t7wpE2S9XfBYTiIl+XFhQG2bjy4Pu1I+EAlCNUzRDYDdFwFYUKvXcIA==}
     engines: {node: '>=0.10.0'}
     dev: true
@@ -108,21 +108,20 @@
     resolution: {integrity: sha512-lFMjJTrFL3j7L9yBxwYfCq2k6qqwHyzuUl/XBnif78PWTJYyL/dfowQHWE3sp6U6ZzqWiiIZnpTMO96zhkjwtg==}
     engines: {node: '>=6.0.0'}
     dependencies:
       '@jridgewell/gen-mapping': 0.3.3
       '@jridgewell/trace-mapping': 0.3.20
     dev: true
 
-  /@bcherny/json-schema-ref-parser@10.0.5-fork:
-    resolution: {integrity: sha512-E/jKbPoca1tfUPj3iSbitDZTGnq6FUFjkH6L8U2oDwSuwK1WhnnVtCG7oFOTg/DDnyoXbQYUiUiGOibHqaGVnw==}
+  /@apidevtools/json-schema-ref-parser@11.6.1:
+    resolution: {integrity: sha512-DxjgKBCoyReu4p5HMvpmgSOfRhhBcuf5V5soDDRgOTZMwsA4KSFzol1abFZgiCTE11L2kKGca5Md9GwDdXVBwQ==}
     engines: {node: '>= 16'}
     dependencies:
       '@jsdevtools/ono': 7.1.3
       '@types/json-schema': 7.0.15
-      call-me-maybe: 1.0.2
       js-yaml: 4.1.0
     dev: true
 
   /@emnapi/runtime@1.1.1:
     resolution: {integrity: sha512-3bfqkzuR1KLx57nZfjr2NLnFOobvyS0aTszaEGCGqmYMVDRaGvgIZbjGSV/MHSSmLgQ/b9JFHQ5xm5WRZYd+XQ==}
     requiresBuild: true
     dependencies:
@@ -583,14 +582,26 @@
     engines: {node: ^18.17.0 || ^20.3.0 || >=21.0.0, npm: '>=9.6.5', pnpm: '>=7.1.0', yarn: '>=3.2.0'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
+  /@isaacs/cliui@8.0.2:
+    resolution: {integrity: sha512-O8jcjabXaleOG9DQ0+ARXWZBTfnP4WNAqzuiJK7ll44AmxGKv/J2M4TPjxjY3znBCfvBXFzucm1twdyFybFqEA==}
+    engines: {node: '>=12'}
+    dependencies:
+      string-width: 5.1.2
+      string-width-cjs: /string-width@4.2.3
+      strip-ansi: 7.1.0
+      strip-ansi-cjs: /strip-ansi@6.0.1
+      wrap-ansi: 8.1.0
+      wrap-ansi-cjs: /wrap-ansi@7.0.0
+    dev: true
+
   /@jridgewell/gen-mapping@0.3.3:
     resolution: {integrity: sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==}
     engines: {node: '>=6.0.0'}
     dependencies:
       '@jridgewell/set-array': 1.1.2
       '@jridgewell/sourcemap-codec': 1.4.15
       '@jridgewell/trace-mapping': 0.3.20
@@ -638,14 +649,21 @@
     resolution: {integrity: sha512-oGB+UxlgWcgQkgwo8GcEGwemoTFt3FIO9ababBmaGwXIoBKZ+GTy0pP185beGg7Llih/NSHSV2XAs1lnznocSg==}
     engines: {node: '>= 8'}
     dependencies:
       '@nodelib/fs.scandir': 2.1.5
       fastq: 1.15.0
     dev: true
 
+  /@pkgjs/parseargs@0.11.0:
+    resolution: {integrity: sha512-+1VkjdD0QBLPodGrJUeqarH8VAIvQODIbwh9XpP5Syisf7YoQgsJKPNFoqqLQlu+VQ/tVSshMR6loPMn8U+dPg==}
+    engines: {node: '>=14'}
+    requiresBuild: true
+    dev: true
+    optional: true
+
   /@polka/url@1.0.0-next.24:
     resolution: {integrity: sha512-2LuNTFBIO0m7kKIQvvPHN6UE63VjpmL9rnEEaOOaiSPbZK+zUOYIzBAWcED+3XYzhYsd/0mD57VdxAEqqV52CQ==}
     dev: true
 
   /@rollup/plugin-commonjs@25.0.7(rollup@4.12.0):
     resolution: {integrity: sha512-nEvcR+LRjEjsaSsc4x3XZfCCvZIaSMenZu/OiwOKGN2UhQpAYI7ru7czFvyWbErlpoGjnSX3D5Ch5FcMA3kRWQ==}
     engines: {node: '>=14.0.0'}
@@ -930,102 +948,102 @@
     resolution: {integrity: sha512-aGg7iToJjdklmxlUlJh/PaPNa4PmqHfyRMLunbL3eaMO0gp656+q1zOKkpJ/CVe9CryJv6tAN1HDoR8cNGzkag==}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@sveltejs/adapter-node@5.0.1(@sveltejs/kit@2.5.6):
+  /@sveltejs/adapter-node@5.0.1(@sveltejs/kit@2.5.8):
     resolution: {integrity: sha512-eYdmxdUWMW+dad1JfMsWBPY2vjXz9eE+52A2AQnXPScPJlIxIVk5mmbaEEzrZivLfO2wEcLTZ5vdC03W69x+iA==}
     peerDependencies:
       '@sveltejs/kit': ^2.4.0
     dependencies:
       '@rollup/plugin-commonjs': 25.0.7(rollup@4.12.0)
       '@rollup/plugin-json': 6.1.0(rollup@4.12.0)
       '@rollup/plugin-node-resolve': 15.2.3(rollup@4.12.0)
-      '@sveltejs/kit': 2.5.6(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.14)(vite@5.2.8)
+      '@sveltejs/kit': 2.5.8(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11)
       rollup: 4.12.0
     dev: true
 
-  /@sveltejs/enhanced-img@0.2.0(svelte@4.2.14):
+  /@sveltejs/enhanced-img@0.2.0(svelte@4.2.17):
     resolution: {integrity: sha512-W6wG0RxQYoL13LmUl8IBHeQatMXSd2ybrjg/WQuE5EoIJq+wUkf1hUDaMp9PHe4ubpnzWK/c0QaE5Ls+zjHimA==}
     dependencies:
       magic-string: 0.30.8
-      svelte-parse-markup: 0.1.2(svelte@4.2.14)
+      svelte-parse-markup: 0.1.2(svelte@4.2.17)
       vite-imagetools: 7.0.1
     transitivePeerDependencies:
       - rollup
       - svelte
     dev: true
 
-  /@sveltejs/kit@2.5.6(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.14)(vite@5.2.8):
-    resolution: {integrity: sha512-AYb02Jm5MfNqJHc8zrj7ScQAFAKmTUCkpkfoi8EVaZZDdnjkvI7L2GtnTDhpiXSAZRVitZX4qm59sMS1FgL+lQ==}
+  /@sveltejs/kit@2.5.8(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11):
+    resolution: {integrity: sha512-ZQXYaVHd1p0kDGwOi4l82i5kAiUQtrhMthDKtJi0zVzmNupKJ0ZlBVAoceuarCuIntPNctyQchW29h5DkFxd1Q==}
     engines: {node: '>=18.13'}
     hasBin: true
     requiresBuild: true
     peerDependencies:
       '@sveltejs/vite-plugin-svelte': ^3.0.0
       svelte: ^4.0.0 || ^5.0.0-next.0
       vite: ^5.0.3
     dependencies:
-      '@sveltejs/vite-plugin-svelte': 3.1.0(svelte@4.2.14)(vite@5.2.8)
+      '@sveltejs/vite-plugin-svelte': 3.1.0(svelte@4.2.17)(vite@5.2.11)
       '@types/cookie': 0.6.0
       cookie: 0.6.0
-      devalue: 4.3.2
+      devalue: 5.0.0
       esm-env: 1.0.0
       import-meta-resolve: 4.0.0
       kleur: 4.1.5
       magic-string: 0.30.5
       mrmime: 2.0.0
       sade: 1.8.1
       set-cookie-parser: 2.6.0
       sirv: 2.0.4
-      svelte: 4.2.14
+      svelte: 4.2.17
       tiny-glob: 0.2.9
-      vite: 5.2.8
+      vite: 5.2.11
     dev: true
 
-  /@sveltejs/vite-plugin-svelte-inspector@2.0.0(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.14)(vite@5.2.8):
+  /@sveltejs/vite-plugin-svelte-inspector@2.0.0(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11):
     resolution: {integrity: sha512-gjr9ZFg1BSlIpfZ4PRewigrvYmHWbDrq2uvvPB1AmTWKuM+dI1JXQSUu2pIrYLb/QncyiIGkFDFKTwJ0XqQZZg==}
     engines: {node: ^18.0.0 || >=20}
     peerDependencies:
       '@sveltejs/vite-plugin-svelte': ^3.0.0
       svelte: ^4.0.0 || ^5.0.0-next.0
       vite: ^5.0.0
     dependencies:
-      '@sveltejs/vite-plugin-svelte': 3.1.0(svelte@4.2.14)(vite@5.2.8)
+      '@sveltejs/vite-plugin-svelte': 3.1.0(svelte@4.2.17)(vite@5.2.11)
       debug: 4.3.4
-      svelte: 4.2.14
-      vite: 5.2.8
+      svelte: 4.2.17
+      vite: 5.2.11
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@sveltejs/vite-plugin-svelte@3.1.0(svelte@4.2.14)(vite@5.2.8):
+  /@sveltejs/vite-plugin-svelte@3.1.0(svelte@4.2.17)(vite@5.2.11):
     resolution: {integrity: sha512-sY6ncCvg+O3njnzbZexcVtUqOBE3iYmQPJ9y+yXSkOwG576QI/xJrBnQSRXFLGwJNBa0T78JEKg5cIR0WOAuUw==}
     engines: {node: ^18.0.0 || >=20}
     peerDependencies:
       svelte: ^4.0.0 || ^5.0.0-next.0
       vite: ^5.0.0
     dependencies:
-      '@sveltejs/vite-plugin-svelte-inspector': 2.0.0(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.14)(vite@5.2.8)
+      '@sveltejs/vite-plugin-svelte-inspector': 2.0.0(@sveltejs/vite-plugin-svelte@3.1.0)(svelte@4.2.17)(vite@5.2.11)
       debug: 4.3.4
       deepmerge: 4.3.1
       kleur: 4.1.5
       magic-string: 0.30.9
-      svelte: 4.2.14
-      svelte-hmr: 0.16.0(svelte@4.2.14)
-      vite: 5.2.8
-      vitefu: 0.2.5(vite@5.2.8)
+      svelte: 4.2.17
+      svelte-hmr: 0.16.0(svelte@4.2.17)
+      vite: 5.2.11
+      vitefu: 0.2.5(vite@5.2.11)
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@tailwindcss/typography@0.5.12(tailwindcss@3.4.3):
-    resolution: {integrity: sha512-CNwpBpconcP7ppxmuq3qvaCxiRWnbhANpY/ruH4L5qs2GCiVDJXde/pjj2HWPV1+Q4G9+V/etrwUYopdcjAlyg==}
+  /@tailwindcss/typography@0.5.13(tailwindcss@3.4.3):
+    resolution: {integrity: sha512-ADGcJ8dX21dVVHIwTRgzrcunY6YY9uSlAHHGVKvkA+vLc5qLwEszvKts40lx7z0qc4clpjclwLeK5rVCV2P/uw==}
     peerDependencies:
       tailwindcss: '>=3.0.0 || insiders'
     dependencies:
       lodash.castarray: 4.4.0
       lodash.isplainobject: 4.0.6
       lodash.merge: 4.6.2
       postcss-selector-parser: 6.0.10
@@ -1036,190 +1054,166 @@
     resolution: {integrity: sha512-4Kh9a6B2bQciAhf7FSuMRRkUWecJgJu9nPnx3yzpsfXX/c50REIqpHY4C82bXP90qrLtXtkDxTZosYO3UpOwlA==}
     dev: true
 
   /@types/estree@1.0.5:
     resolution: {integrity: sha512-/kYRxGDLWzHOB7q+wtSUQlFrtcdUccpfy+X+9iMBpHK8QLLhx2wIPYuS5DYtR9Wa/YlZAbIovy7qVdB1Aq6Lyw==}
     dev: true
 
-  /@types/glob@7.2.0:
-    resolution: {integrity: sha512-ZUxbzKl0IfJILTS6t7ip5fQQM/J3TJYubDm3nMbgubNNYS62eXeUpoLUC8/7fJNiFYHTrGPQn7hspDUzIHX3UA==}
-    dependencies:
-      '@types/minimatch': 5.1.2
-      '@types/node': 20.9.0
-    dev: true
-
   /@types/json-schema@7.0.15:
     resolution: {integrity: sha512-5+fP8P8MFNC+AyZCDxrB2pkZFPGzqQWUzpSeuuVLvm8VMcorNYavBqoFcxK8bQz4Qsbn4oUEEem4wDLfcysGHA==}
     dev: true
 
-  /@types/lodash@4.14.201:
-    resolution: {integrity: sha512-y9euML0cim1JrykNxADLfaG0FgD1g/yTHwUs/Jg9ZIU7WKj2/4IW9Lbb1WZbvck78W/lfGXFfe+u2EGfIJXdLQ==}
-    dev: true
-
-  /@types/minimatch@5.1.2:
-    resolution: {integrity: sha512-K0VQKziLUWkVKiRVrx4a40iPaxTUefQmjtkQofBkYRcoaaL/8rhwDWww9qWbrgicNOgnpIsMxyNIUM4+n6dUIA==}
+  /@types/lodash@4.17.0:
+    resolution: {integrity: sha512-t7dhREVv6dbNj0q17X12j7yDG4bD/DHYX7o5/DbDxobP0HnGPgpRz2Ej77aL7TZT3DSw13fqUTj8J4mMnqa7WA==}
     dev: true
 
   /@types/node@20.9.0:
     resolution: {integrity: sha512-nekiGu2NDb1BcVofVcEKMIwzlx4NjHlcjhoxxKBNLtz15Y1z7MYf549DFvkHSId02Ax6kGwWntIBPC3l/JZcmw==}
     dependencies:
       undici-types: 5.26.5
     dev: true
 
-  /@types/prettier@2.7.3:
-    resolution: {integrity: sha512-+68kP9yzs4LMp7VNh8gdzMSPZFL44MLGqiHWvttYJe+6qnuVr4Ek9wSBQoveqY/r+LwjCcU29kNVkidwim+kYA==}
-    dev: true
-
   /@types/pug@2.0.10:
     resolution: {integrity: sha512-Sk/uYFOBAB7mb74XcpizmH0KOR2Pv3D2Hmrh1Dmy5BmK3MpdSa5kqZcg6EKBdklU0bFXX9gCfzvpnyUehrPIuA==}
     dev: true
 
   /@types/resolve@1.20.2:
     resolution: {integrity: sha512-60BCwRFOZCQhDncwQdxxeOEEkbc5dIMccYLwbxsS4TUNeVECQ/pBJ0j09mrHOl/JJvpRPGwO9SvE4nR2Nb/a4Q==}
     dev: true
 
-  /@types/semver@7.5.8:
-    resolution: {integrity: sha512-I8EUhyrgfLrcTkzV3TSsGyl1tSuPrEDzr0yd5m90UgNxQkyDXULk3b6MlQqTCpZpNtWe1K0hzclnZkTcLBe2UQ==}
-    dev: true
-
   /@types/set-cookie-parser@2.4.7:
     resolution: {integrity: sha512-+ge/loa0oTozxip6zmhRIk8Z/boU51wl9Q6QdLZcokIGMzY5lFXYy/x7Htj2HTC6/KZP1hUbZ1ekx8DYXICvWg==}
     dependencies:
       '@types/node': 20.9.0
     dev: true
 
-  /@typescript-eslint/eslint-plugin@7.6.0(@typescript-eslint/parser@7.6.0)(eslint@8.57.0)(typescript@5.4.5):
-    resolution: {integrity: sha512-gKmTNwZnblUdnTIJu3e9kmeRRzV2j1a/LUO27KNNAnIC5zjy1aSvXSRp4rVNlmAoHlQ7HzX42NbKpcSr4jF80A==}
+  /@typescript-eslint/eslint-plugin@7.9.0(@typescript-eslint/parser@7.9.0)(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-6e+X0X3sFe/G/54aC3jt0txuMTURqLyekmEHViqyA2VnxhLMpvA6nqmcjIy+Cr9tLDHPssA74BP5Mx9HQIxBEA==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       '@typescript-eslint/parser': ^7.0.0
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
       '@eslint-community/regexpp': 4.10.0
-      '@typescript-eslint/parser': 7.6.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/scope-manager': 7.6.0
-      '@typescript-eslint/type-utils': 7.6.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/utils': 7.6.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/visitor-keys': 7.6.0
-      debug: 4.3.4
+      '@typescript-eslint/parser': 7.9.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.9.0
+      '@typescript-eslint/type-utils': 7.9.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.9.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.9.0
       eslint: 8.57.0
       graphemer: 1.4.0
       ignore: 5.3.1
       natural-compare: 1.4.0
-      semver: 7.6.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/parser@7.6.0(eslint@8.57.0)(typescript@5.4.5):
-    resolution: {integrity: sha512-usPMPHcwX3ZoPWnBnhhorc14NJw9J4HpSXQX4urF2TPKG0au0XhJoZyX62fmvdHONUkmyUe74Hzm1//XA+BoYg==}
+  /@typescript-eslint/parser@7.9.0(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-qHMJfkL5qvgQB2aLvhUSXxbK7OLnDkwPzFalg458pxQgfxKDfT1ZDbHQM/I6mDIf/svlMkj21kzKuQ2ixJlatQ==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/scope-manager': 7.6.0
-      '@typescript-eslint/types': 7.6.0
-      '@typescript-eslint/typescript-estree': 7.6.0(typescript@5.4.5)
-      '@typescript-eslint/visitor-keys': 7.6.0
+      '@typescript-eslint/scope-manager': 7.9.0
+      '@typescript-eslint/types': 7.9.0
+      '@typescript-eslint/typescript-estree': 7.9.0(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.9.0
       debug: 4.3.4
       eslint: 8.57.0
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/scope-manager@7.6.0:
-    resolution: {integrity: sha512-ngttyfExA5PsHSx0rdFgnADMYQi+Zkeiv4/ZxGYUWd0nLs63Ha0ksmp8VMxAIC0wtCFxMos7Lt3PszJssG/E6w==}
+  /@typescript-eslint/scope-manager@7.9.0:
+    resolution: {integrity: sha512-ZwPK4DeCDxr3GJltRz5iZejPFAAr4Wk3+2WIBaj1L5PYK5RgxExu/Y68FFVclN0y6GGwH8q+KgKRCvaTmFBbgQ==}
     engines: {node: ^18.18.0 || >=20.0.0}
     dependencies:
-      '@typescript-eslint/types': 7.6.0
-      '@typescript-eslint/visitor-keys': 7.6.0
+      '@typescript-eslint/types': 7.9.0
+      '@typescript-eslint/visitor-keys': 7.9.0
     dev: true
 
-  /@typescript-eslint/type-utils@7.6.0(eslint@8.57.0)(typescript@5.4.5):
-    resolution: {integrity: sha512-NxAfqAPNLG6LTmy7uZgpK8KcuiS2NZD/HlThPXQRGwz6u7MDBWRVliEEl1Gj6U7++kVJTpehkhZzCJLMK66Scw==}
+  /@typescript-eslint/type-utils@7.9.0(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-6Qy8dfut0PFrFRAZsGzuLoM4hre4gjzWJB6sUvdunCYZsYemTkzZNwF1rnGea326PHPT3zn5Lmg32M/xfJfByA==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/typescript-estree': 7.6.0(typescript@5.4.5)
-      '@typescript-eslint/utils': 7.6.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/typescript-estree': 7.9.0(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.9.0(eslint@8.57.0)(typescript@5.4.5)
       debug: 4.3.4
       eslint: 8.57.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/types@7.6.0:
-    resolution: {integrity: sha512-h02rYQn8J+MureCvHVVzhl69/GAfQGPQZmOMjG1KfCl7o3HtMSlPaPUAPu6lLctXI5ySRGIYk94clD/AUMCUgQ==}
+  /@typescript-eslint/types@7.9.0:
+    resolution: {integrity: sha512-oZQD9HEWQanl9UfsbGVcZ2cGaR0YT5476xfWE0oE5kQa2sNK2frxOlkeacLOTh9po4AlUT5rtkGyYM5kew0z5w==}
     engines: {node: ^18.18.0 || >=20.0.0}
     dev: true
 
-  /@typescript-eslint/typescript-estree@7.6.0(typescript@5.4.5):
-    resolution: {integrity: sha512-+7Y/GP9VuYibecrCQWSKgl3GvUM5cILRttpWtnAu8GNL9j11e4tbuGZmZjJ8ejnKYyBRb2ddGQ3rEFCq3QjMJw==}
+  /@typescript-eslint/typescript-estree@7.9.0(typescript@5.4.5):
+    resolution: {integrity: sha512-zBCMCkrb2YjpKV3LA0ZJubtKCDxLttxfdGmwZvTqqWevUPN0FZvSI26FalGFFUZU/9YQK/A4xcQF9o/VVaCKAg==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
     dependencies:
-      '@typescript-eslint/types': 7.6.0
-      '@typescript-eslint/visitor-keys': 7.6.0
+      '@typescript-eslint/types': 7.9.0
+      '@typescript-eslint/visitor-keys': 7.9.0
       debug: 4.3.4
       globby: 11.1.0
       is-glob: 4.0.3
       minimatch: 9.0.4
-      semver: 7.6.0
+      semver: 7.6.2
       ts-api-utils: 1.3.0(typescript@5.4.5)
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
     dev: true
 
-  /@typescript-eslint/utils@7.6.0(eslint@8.57.0)(typescript@5.4.5):
-    resolution: {integrity: sha512-x54gaSsRRI+Nwz59TXpCsr6harB98qjXYzsRxGqvA5Ue3kQH+FxS7FYU81g/omn22ML2pZJkisy6Q+ElK8pBCA==}
+  /@typescript-eslint/utils@7.9.0(eslint@8.57.0)(typescript@5.4.5):
+    resolution: {integrity: sha512-5KVRQCzZajmT4Ep+NEgjXCvjuypVvYHUW7RHlXzNPuak2oWpVoD1jf5xCP0dPAuNIchjC7uQyvbdaSTFaLqSdA==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
     dependencies:
       '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
-      '@types/json-schema': 7.0.15
-      '@types/semver': 7.5.8
-      '@typescript-eslint/scope-manager': 7.6.0
-      '@typescript-eslint/types': 7.6.0
-      '@typescript-eslint/typescript-estree': 7.6.0(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.9.0
+      '@typescript-eslint/types': 7.9.0
+      '@typescript-eslint/typescript-estree': 7.9.0(typescript@5.4.5)
       eslint: 8.57.0
-      semver: 7.6.0
     transitivePeerDependencies:
       - supports-color
       - typescript
     dev: true
 
-  /@typescript-eslint/visitor-keys@7.6.0:
-    resolution: {integrity: sha512-4eLB7t+LlNUmXzfOu1VAIAdkjbu5xNSerURS9X/S5TUKWFRpXRQZbmtPqgKmYx8bj3J0irtQXSiWAOY82v+cgw==}
+  /@typescript-eslint/visitor-keys@7.9.0:
+    resolution: {integrity: sha512-iESPx2TNLDNGQLyjKhUvIKprlP49XNEK+MvIf9nIO7ZZaZdbnfWKHnXAgufpxqfA0YryH8XToi4+CjBgVnFTSQ==}
     engines: {node: ^18.18.0 || >=20.0.0}
     dependencies:
-      '@typescript-eslint/types': 7.6.0
+      '@typescript-eslint/types': 7.9.0
       eslint-visitor-keys: 3.4.3
     dev: true
 
   /@ungap/structured-clone@1.2.0:
     resolution: {integrity: sha512-zuVdFrMJiuCDQUMCzQaD6KL28MjnqqN8XnAqiEq9PNm/hCPTSGfrXCOfwj1ow4LFb/tNymJPwsNbVePc1xFqrQ==}
     dev: true
 
@@ -1252,21 +1246,31 @@
     dev: true
 
   /ansi-regex@5.0.1:
     resolution: {integrity: sha512-quJQXlTSUGL2LH9SUXo8VwsY4soanhgo6LNSm84E1LBcE8s3O0wpdiRzyR9z/ZZJMlMWv37qOOb9pdJlMUEKFQ==}
     engines: {node: '>=8'}
     dev: true
 
+  /ansi-regex@6.0.1:
+    resolution: {integrity: sha512-n5M855fKb2SsfMIiFFoVrABHJC8QtHwVx+mHWP3QcEqBHYienj5dHSgjbxtC0WEZXYt4wcD6zrQElDPhFuZgfA==}
+    engines: {node: '>=12'}
+    dev: true
+
   /ansi-styles@4.3.0:
     resolution: {integrity: sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==}
     engines: {node: '>=8'}
     dependencies:
       color-convert: 2.0.1
     dev: true
 
+  /ansi-styles@6.2.1:
+    resolution: {integrity: sha512-bN798gFfQX+viw3R7yrGWRqnrN2oRkEkUjjl4JNn4E8GxxbjtG3FbrEIIY3l8/hrwUwIeCZvi4QuOTP4MErVug==}
+    engines: {node: '>=12'}
+    dev: true
+
   /any-promise@1.3.0:
     resolution: {integrity: sha512-7UvmKalWRt1wgjL1RrGxoSJW/0QZFIegpeGvZG9kjp8vrRu55XTHbwnqq2GpXm9uLbcuhxm3IqX9OB4MZR1b2A==}
     dev: true
 
   /anymatch@3.1.3:
     resolution: {integrity: sha512-KMReFUr0B4t+D+OBkjR3KYqvocp2XaSzO55UcB6mgQMd3KbcE+mWTyvVV7D/zsdEbNnV6acZUutkiHQXvTr1Rw==}
     engines: {node: '>= 8'}
@@ -1361,18 +1365,14 @@
     dev: true
 
   /builtin-modules@3.3.0:
     resolution: {integrity: sha512-zhaCDicdLuWN5UbN5IMnFqNMhNfo919sH85y2/ea+5Yg9TsTkeZxpL+JLbp6cgYFS4sRLp3YV4S6yDuqVWHYOw==}
     engines: {node: '>=6'}
     dev: true
 
-  /call-me-maybe@1.0.2:
-    resolution: {integrity: sha512-HpX65o1Hnr9HH25ojC1YGs7HCQLq0GCOibSaWER0eNpgJ/Z1MZv2mTc7+xh6WOPxbRVcmgbv4hGU+uSQ/2xFZQ==}
-    dev: true
-
   /callsites@3.1.0:
     resolution: {integrity: sha512-P8BjAsXvZS+VIDUI11hHCQEv74YT67YUi5JJFNWIqL235sBmjX4+qx9Muvls5ivyNENctx46xQLQ3aTuE7ssaQ==}
     engines: {node: '>=6'}
     dev: true
 
   /camelcase-css@2.0.1:
     resolution: {integrity: sha512-QOSvevhslijgYwRx6Rv7zKdMF8lbRmx+uQGx2+vDc+KI/eBnsy9kit5aj23AgGu3pa4t9AgwbnXWqS+iOY+2aA==}
@@ -1402,20 +1402,20 @@
       is-glob: 4.0.3
       normalize-path: 3.0.0
       readdirp: 3.6.0
     optionalDependencies:
       fsevents: 2.3.3
     dev: true
 
-  /cli-color@2.0.3:
-    resolution: {integrity: sha512-OkoZnxyC4ERN3zLzZaY9Emb7f/MhBOIpePv0Ycok0fJYT+Ouo00UBEIwsVsr0yoow++n5YWlSUgST9GKhNHiRQ==}
+  /cli-color@2.0.4:
+    resolution: {integrity: sha512-zlnpg0jNcibNrO7GG9IeHH7maWFeCz+Ja1wx/7tZNU5ASSSSZ+/qZciM0/LHCYxSdqv5h2sdbQ/PXYdOuetXvA==}
     engines: {node: '>=0.10'}
     dependencies:
-      d: 1.0.1
-      es5-ext: 0.10.62
+      d: 1.0.2
+      es5-ext: 0.10.64
       es6-iterator: 2.0.3
       memoizee: 0.4.15
       timers-ext: 0.1.7
     dev: true
 
   /code-red@1.0.4:
     resolution: {integrity: sha512-7qJWqItLA8/VPVlKJlFXU+NBlo/qyfs39aJcuMT/2ere32ZqvF5OSxgdM5xOfJJ7O429gg2HM47y8v9P+9wrNw==}
@@ -1502,33 +1502,39 @@
     dev: true
 
   /culori@3.2.0:
     resolution: {integrity: sha512-HIEbTSP7vs1mPq/2P9In6QyFE0Tkpevh0k9a+FkjhD+cwsYm9WRSbn4uMdW9O0yXlNYC3ppxL3gWWPOcvEl57w==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
     dev: true
 
-  /d@1.0.1:
-    resolution: {integrity: sha512-m62ShEObQ39CfralilEQRjH6oAMtNCV1xJyEx5LpRYUVN+EviphDgUc/F3hnYbADmkiNs67Y+3ylmlG7Lnu+FA==}
+  /d@1.0.2:
+    resolution: {integrity: sha512-MOqHvMWF9/9MX6nza0KgvFH4HpMU0EF5uUDXqX/BtxtU8NfB0QzRtJ8Oe/6SuS4kbhyzVJwjd97EA4PKrzJ8bw==}
+    engines: {node: '>=0.12'}
     dependencies:
-      es5-ext: 0.10.62
-      type: 1.2.0
+      es5-ext: 0.10.64
+      type: 2.7.2
     dev: true
 
-  /daisyui@4.10.1(postcss@8.4.38):
-    resolution: {integrity: sha512-Ds0Z0Fv+Xf6ZEqV4Q5JIOeKfg83xxnww0Lzid0V94vPtlQ0yYmucEa33zSctsX2VEgBALtmk5zVEqd59pnUbuQ==}
+  /daisyui@4.11.1(postcss@8.4.38):
+    resolution: {integrity: sha512-obT9CUbQdW6eoHwSeT5VwaRrWlwrM4OT5qlfdJ0oQlSIEYhwnEl2+L2fwu5PioLbitwuMdYC2X8I1cyy8Pf6LQ==}
     engines: {node: '>=16.9.0'}
     dependencies:
       css-selector-tokenizer: 0.8.0
       culori: 3.2.0
       picocolors: 1.0.0
       postcss-js: 4.0.1(postcss@8.4.38)
     transitivePeerDependencies:
       - postcss
     dev: true
 
+  /data-uri-to-buffer@4.0.1:
+    resolution: {integrity: sha512-0R9ikRb668HB7QDxT1vkpuUBtqc53YyAwMwGeUFKRojY/NWKvdZ+9UYtRfGmhqNbRkTSVpMbmyhXipFFv2cb/A==}
+    engines: {node: '>= 12'}
+    dev: true
+
   /debug@4.3.4:
     resolution: {integrity: sha512-PRWFHuSU3eDtQJPvnNY7Jcket1j0t5OuOsFzPPzsekD52Zl8qUfFIPEiswXqIvHWGVHOgX+7G/vCNNhehwxfkQ==}
     engines: {node: '>=6.0'}
     peerDependencies:
       supports-color: '*'
     peerDependenciesMeta:
       supports-color:
@@ -1557,16 +1563,16 @@
     dev: true
 
   /detect-libc@2.0.3:
     resolution: {integrity: sha512-bwy0MGW55bG41VqxxypOsdSdGqLwXPI/focwgTYCFMbdUiBAxLg9CFzG08sz2aqzknwiX7Hkl0bQENjg8iLByw==}
     engines: {node: '>=8'}
     dev: true
 
-  /devalue@4.3.2:
-    resolution: {integrity: sha512-KqFl6pOgOW+Y6wJgu80rHpo2/3H07vr8ntR9rkkFIRETewbf5GaYYcakYfiKz89K+sLsuPkQIZaXDMjUObZwWg==}
+  /devalue@5.0.0:
+    resolution: {integrity: sha512-gO+/OMXF7488D+u3ue+G7Y4AA3ZmUnB3eHJXmBTgNHvr4ZNzl36A0ZtG+XCRNYCkYx/bFmw4qtkoFLa+wSrwAA==}
     dev: true
 
   /didyoumean@1.2.2:
     resolution: {integrity: sha512-gxtyfqMg7GKyhQmb056K7M3xszy/myH8w+B4RT+QXBQsvAOdc3XymqDDPHx1BgPgsdAA5SIifona89YtRATDzw==}
     dev: true
 
   /dir-glob@3.0.1:
@@ -1583,54 +1589,68 @@
   /doctrine@3.0.0:
     resolution: {integrity: sha512-yS+Q5i3hBf7GBkd4KG8a7eBNNWNGLTaEwwYWUijIYM7zrlYDM0BFXHjjPWlWZ1Rg7UaddZeIDmi9jF3HmqiQ2w==}
     engines: {node: '>=6.0.0'}
     dependencies:
       esutils: 2.0.3
     dev: true
 
+  /eastasianwidth@0.2.0:
+    resolution: {integrity: sha512-I88TYZWc9XiYHRQ4/3c5rjjfgkjhLyW2luGIheGERbNQ6OY7yTybanSpDXZa8y7VUP9YmDcYa+eyq4ca7iLqWA==}
+    dev: true
+
   /electron-to-chromium@1.4.677:
     resolution: {integrity: sha512-erDa3CaDzwJOpyvfKhOiJjBVNnMM0qxHq47RheVVwsSQrgBA9ZSGV9kdaOfZDPXcHzhG7lBxhj6A7KvfLJBd6Q==}
     dev: true
 
-  /es5-ext@0.10.62:
-    resolution: {integrity: sha512-BHLqn0klhEpnOKSrzn/Xsz2UIW8j+cGmo9JLzr8BiUapV8hPL9+FliFqjwr9ngW7jWdnxv6eO+/LqyhJVqgrjA==}
+  /emoji-regex@8.0.0:
+    resolution: {integrity: sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==}
+    dev: true
+
+  /emoji-regex@9.2.2:
+    resolution: {integrity: sha512-L18DaJsXSUk2+42pv8mLs5jJT2hqFkFE4j21wOmgbUqsZ2hL72NsUU785g9RXgo3s0ZNgVl42TiHp3ZtOv/Vyg==}
+    dev: true
+
+  /es5-ext@0.10.64:
+    resolution: {integrity: sha512-p2snDhiLaXe6dahss1LddxqEm+SkuDvV8dnIQG0MWjyHpcMNfXKPE+/Cc0y+PhxJX3A4xGNeFCj5oc0BUh6deg==}
     engines: {node: '>=0.10'}
     requiresBuild: true
     dependencies:
       es6-iterator: 2.0.3
-      es6-symbol: 3.1.3
+      es6-symbol: 3.1.4
+      esniff: 2.0.1
       next-tick: 1.1.0
     dev: true
 
   /es6-iterator@2.0.3:
     resolution: {integrity: sha512-zw4SRzoUkd+cl+ZoE15A9o1oQd920Bb0iOJMQkQhl3jNc03YqVjAhG7scf9C5KWRU/R13Orf588uCC6525o02g==}
     dependencies:
-      d: 1.0.1
-      es5-ext: 0.10.62
-      es6-symbol: 3.1.3
+      d: 1.0.2
+      es5-ext: 0.10.64
+      es6-symbol: 3.1.4
     dev: true
 
   /es6-promise@3.3.1:
     resolution: {integrity: sha512-SOp9Phqvqn7jtEUxPWdWfWoLmyt2VaJ6MpvP9Comy1MceMXqE6bxvaTu4iaxpYYPzhny28Lc+M87/c2cPK6lDg==}
     dev: true
 
-  /es6-symbol@3.1.3:
-    resolution: {integrity: sha512-NJ6Yn3FuDinBaBRWl/q5X/s4koRHBrgKAu+yGI6JCBeiu3qrcbJhwT2GeR/EXVfylRk8dpQVJoLEFhK+Mu31NA==}
+  /es6-symbol@3.1.4:
+    resolution: {integrity: sha512-U9bFFjX8tFiATgtkJ1zg25+KviIXpgRvRHS8sau3GfhVzThRQrOeksPeT0BWW2MNZs1OEWJ1DPXOQMn0KKRkvg==}
+    engines: {node: '>=0.12'}
     dependencies:
-      d: 1.0.1
+      d: 1.0.2
       ext: 1.7.0
     dev: true
 
   /es6-weak-map@2.0.3:
     resolution: {integrity: sha512-p5um32HOTO1kP+w7PRnB+5lQ43Z6muuMuIMffvDN8ZB4GcnjLBV6zGStpbASIMk4DCAvEaamhe2zhyCb/QXXsA==}
     dependencies:
-      d: 1.0.1
-      es5-ext: 0.10.62
+      d: 1.0.2
+      es5-ext: 0.10.64
       es6-iterator: 2.0.3
-      es6-symbol: 3.1.3
+      es6-symbol: 3.1.4
     dev: true
 
   /esbuild@0.20.2:
     resolution: {integrity: sha512-WdOOppmUNU+IbZ0PaDiTst80zjnrOkyJNHoKupIcVyU8Lvla3Ugx94VzkQ32Ijqd7UhHJy75gNWDMUekcrSJ6g==}
     engines: {node: '>=12'}
     hasBin: true
     requiresBuild: true
@@ -1685,38 +1705,38 @@
     hasBin: true
     peerDependencies:
       eslint: '>=7.0.0'
     dependencies:
       eslint: 8.57.0
     dev: true
 
-  /eslint-plugin-svelte@2.37.0(eslint@8.57.0)(svelte@4.2.14):
-    resolution: {integrity: sha512-H/2Gz7agYHEMEEzRuLYuCmAIdjuBnbhFG9hOK0yCdSBvvJGJMkjo+lR6j67OIvLOavgp4L7zA5LnDKi8WqdPhQ==}
+  /eslint-plugin-svelte@2.39.0(eslint@8.57.0)(svelte@4.2.17):
+    resolution: {integrity: sha512-FXktBLXsrxbA+6ZvJK2z/sQOrUKyzSg3fNWK5h0reSCjr2fjAsc9ai/s/JvSl4Hgvz3nYVtTIMwarZH5RcB7BA==}
     engines: {node: ^14.17.0 || >=16.0.0}
     peerDependencies:
       eslint: ^7.0.0 || ^8.0.0-0 || ^9.0.0-0
-      svelte: ^3.37.0 || ^4.0.0 || ^5.0.0-next.95
+      svelte: ^3.37.0 || ^4.0.0 || ^5.0.0-next.112
     peerDependenciesMeta:
       svelte:
         optional: true
     dependencies:
       '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
       '@jridgewell/sourcemap-codec': 1.4.15
       debug: 4.3.4
       eslint: 8.57.0
       eslint-compat-utils: 0.5.0(eslint@8.57.0)
       esutils: 2.0.3
-      known-css-properties: 0.30.0
+      known-css-properties: 0.31.0
       postcss: 8.4.38
       postcss-load-config: 3.1.4(postcss@8.4.38)
       postcss-safe-parser: 6.0.0(postcss@8.4.38)
       postcss-selector-parser: 6.0.16
       semver: 7.6.0
-      svelte: 4.2.14
-      svelte-eslint-parser: 0.34.1(svelte@4.2.14)
+      svelte: 4.2.17
+      svelte-eslint-parser: 0.36.0(svelte@4.2.17)
     transitivePeerDependencies:
       - supports-color
       - ts-node
     dev: true
 
   /eslint-scope@7.2.2:
     resolution: {integrity: sha512-dOt21O7lTMhDM+X9mB4GX+DZrZtCUJPL/wlcTqxyrx5IvO0IYtILdtrQGQp+8n5S0gwSVmOf9NQrjMOgfQZlIg==}
@@ -1778,14 +1798,24 @@
       - supports-color
     dev: true
 
   /esm-env@1.0.0:
     resolution: {integrity: sha512-Cf6VksWPsTuW01vU9Mk/3vRue91Zevka5SjyNf3nEpokFRuqt/KjUQoGAwq9qMmhpLTHmXzSIrFRw8zxWzmFBA==}
     dev: true
 
+  /esniff@2.0.1:
+    resolution: {integrity: sha512-kTUIGKQ/mDPFoJ0oVfcmyJn4iBDRptjNVIzwIFR7tqWXdVI9xfA2RMwY/gbSpJG3lkdWNEjLap/NqVHZiJsdfg==}
+    engines: {node: '>=0.10'}
+    dependencies:
+      d: 1.0.2
+      es5-ext: 0.10.64
+      event-emitter: 0.3.5
+      type: 2.7.2
+    dev: true
+
   /espree@9.6.1:
     resolution: {integrity: sha512-oruZaFkjorTpF32kDSI5/75ViwGeZginGGy2NoOSg3Q9bnwlnmDm4HLnkl0RE3n+njDXR037aY1+x58Z/zFdwQ==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     dependencies:
       acorn: 8.11.2
       acorn-jsx: 5.3.2(acorn@8.11.2)
       eslint-visitor-keys: 3.4.3
@@ -1824,16 +1854,16 @@
     resolution: {integrity: sha512-kVscqXk4OCp68SZ0dkgEKVi6/8ij300KBWTJq32P/dYeWTSwK41WyTxalN1eRmA5Z9UU/LX9D7FWSmV9SAYx6g==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /event-emitter@0.3.5:
     resolution: {integrity: sha512-D9rRn9y7kLPnJ+hMq7S/nhvoKwwvVJahBi2BPmx3bvbsEdK3W9ii8cBSGjP+72/LnM4n6fo3+dkCX5FeTQruXA==}
     dependencies:
-      d: 1.0.1
-      es5-ext: 0.10.62
+      d: 1.0.2
+      es5-ext: 0.10.64
     dev: true
 
   /ext@1.7.0:
     resolution: {integrity: sha512-6hxeJYaL110a9b5TEJSj0gojyHQAmA2ch5Os+ySCiA1QGdS697XWY1pzsrSjqA9LDEEgdB/KypIlR59RcLuHYw==}
     dependencies:
       type: 2.7.2
     dev: true
@@ -1867,14 +1897,22 @@
 
   /fastq@1.15.0:
     resolution: {integrity: sha512-wBrocU2LCXXa+lWBt8RoIRD89Fi8OdABODa/kEnyeyjS5aZO5/GNvI5sEINADqP/h8M29UHTHUb53sUu5Ihqdw==}
     dependencies:
       reusify: 1.0.4
     dev: true
 
+  /fetch-blob@3.2.0:
+    resolution: {integrity: sha512-7yAQpD2UMJzLi1Dqv7qFYnPbaPx7ZfFK6PiIxQ4PfkGPyNyl2Ugx+a/umUonmKqjhM4DnfbMvdX6otXq83soQQ==}
+    engines: {node: ^12.20 || >= 14.13}
+    dependencies:
+      node-domexception: 1.0.0
+      web-streams-polyfill: 3.3.3
+    dev: true
+
   /file-entry-cache@6.0.1:
     resolution: {integrity: sha512-7Gps/XWymbLk2QLYK4NzpMOrYjMhdIxXuIvy2QBsLE6ljuodKvdkWs/cpyJJ3CVIVpH0Oi1Hvg1ovbMzLdFBBg==}
     engines: {node: ^10.12.0 || >=12.0.0}
     dependencies:
       flat-cache: 3.2.0
     dev: true
 
@@ -1902,14 +1940,29 @@
       rimraf: 3.0.2
     dev: true
 
   /flatted@3.2.9:
     resolution: {integrity: sha512-36yxDn5H7OFZQla0/jFJmbIKTdZAQHngCedGxiMmpNfEZM0sdEeT+WczLQrjK6D7o2aiyLYDnkw0R3JK0Qv1RQ==}
     dev: true
 
+  /foreground-child@3.1.1:
+    resolution: {integrity: sha512-TMKDUnIte6bfb5nWv7V/caI169OHgvwjb7V4WkeUvbQQdjr5rWKqHFiKWb/fcOwB+CzBT+qbWjvj+DVwRskpIg==}
+    engines: {node: '>=14'}
+    dependencies:
+      cross-spawn: 7.0.3
+      signal-exit: 4.1.0
+    dev: true
+
+  /formdata-polyfill@4.0.10:
+    resolution: {integrity: sha512-buewHzMvYL29jdeQTVILecSaZKnt/RJWjoZCF5OW60Z67/GmSLBkOFM7qh1PI3zFNtJbaZL5eQu1vLfazOwj4g==}
+    engines: {node: '>=12.20.0'}
+    dependencies:
+      fetch-blob: 3.2.0
+    dev: true
+
   /fraction.js@4.3.7:
     resolution: {integrity: sha512-ZsDfxO51wGAXREY55a7la9LScWpwv9RxIrYABrlvOFBlH/ShPnrtsXeuUIfXKKOVicNxQ+o8JTbJvjS4M89yew==}
     dev: true
 
   /fs.realpath@1.0.0:
     resolution: {integrity: sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==}
     dev: true
@@ -1922,41 +1975,38 @@
     dev: true
     optional: true
 
   /function-bind@1.1.2:
     resolution: {integrity: sha512-7XHNxH7qX9xG5mIwxkhumTox/MIRNcOgDrxWsMt2pAr23WHp6MrRlN7FBSFpCpr+oVO0F744iUgR82nJMfG2SA==}
     dev: true
 
-  /get-stdin@8.0.0:
-    resolution: {integrity: sha512-sY22aA6xchAzprjyqmSEQv4UbAAzRN0L2dQB0NlN5acTTK9Don6nhoc3eAbUnpZiCANAMfd/+40kVdKfFygohg==}
-    engines: {node: '>=10'}
-    dev: true
-
   /glob-parent@5.1.2:
     resolution: {integrity: sha512-AOIgSQCepiJYwP3ARnGx+5VnTu2HBYdzbGP45eLw1vr3zB3vZLeyed1sC9hnbcOc9/SrMyM5RPQrkGz4aS9Zow==}
     engines: {node: '>= 6'}
     dependencies:
       is-glob: 4.0.3
     dev: true
 
   /glob-parent@6.0.2:
     resolution: {integrity: sha512-XxwI8EOhVQgWp6iDL+3b0r86f4d6AX6zSU55HfB4ydCEuXLXc5FcYeOu+nnGftS4TEju/11rt4KJPTMgbfmv4A==}
     engines: {node: '>=10.13.0'}
     dependencies:
       is-glob: 4.0.3
     dev: true
 
-  /glob-promise@4.2.2(glob@7.2.3):
-    resolution: {integrity: sha512-xcUzJ8NWN5bktoTIX7eOclO1Npxd/dyVqUJxlLIDasT4C7KZyqlPIwkdJ0Ypiy3p2ZKahTjK4M9uC3sNSfNMzw==}
-    engines: {node: '>=12'}
-    peerDependencies:
-      glob: ^7.1.6
+  /glob@10.3.12:
+    resolution: {integrity: sha512-TCNv8vJ+xz4QiqTpfOJA7HvYv+tNIRHKfUWw/q+v2jdgN4ebz+KY9tGx5J4rHP0o84mNP+ApH66HRX8us3Khqg==}
+    engines: {node: '>=16 || 14 >=14.17'}
+    hasBin: true
     dependencies:
-      '@types/glob': 7.2.0
-      glob: 7.2.3
+      foreground-child: 3.1.1
+      jackspeak: 2.3.6
+      minimatch: 9.0.4
+      minipass: 7.0.4
+      path-scurry: 1.10.2
     dev: true
 
   /glob@7.1.6:
     resolution: {integrity: sha512-LwaxwyZ72Lk7vZINtNNrywX0ZuLyStrdDtabefZKAY5ZGJhVtgdznluResxNmPitE0SAO+O26sWTHeKSI2wMBA==}
     dependencies:
       fs.realpath: 1.0.0
       inflight: 1.0.6
@@ -2105,14 +2155,19 @@
     dev: true
 
   /is-extglob@2.1.1:
     resolution: {integrity: sha512-SbKbANkN603Vi4jEZv49LeVJMn4yGwsbzZworEoyEiutsN3nJYdbO36zfhGJ6QEDpOZIFkDtnq5JRxmvl3jsoQ==}
     engines: {node: '>=0.10.0'}
     dev: true
 
+  /is-fullwidth-code-point@3.0.0:
+    resolution: {integrity: sha512-zymm5+u+sCsSWyD9qNaejV3DFvhCKclKdizYaJUuHA83RLjb7nSuGnddCHGv0hk+KY7BMAlsWeK4Ueg6EV6XQg==}
+    engines: {node: '>=8'}
+    dev: true
+
   /is-glob@4.0.3:
     resolution: {integrity: sha512-xelSayHH36ZgE7ZWhli7pW34hNbNl8Ojv5KVmkJD4hBdD3th8Tfk9vYasLM+mXWOZhFkgZfxhLSnrwRr4elSSg==}
     engines: {node: '>=0.10.0'}
     dependencies:
       is-extglob: 2.1.1
     dev: true
 
@@ -2146,14 +2201,23 @@
       '@types/estree': 1.0.5
     dev: true
 
   /isexe@2.0.0:
     resolution: {integrity: sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==}
     dev: true
 
+  /jackspeak@2.3.6:
+    resolution: {integrity: sha512-N3yCS/NegsOBokc8GAdM8UcmfsKiSS8cipheD/nivzr700H+nsMOxJjQnvwOcRYVuFkdH0wGUvW2WbXGmrZGbQ==}
+    engines: {node: '>=14'}
+    dependencies:
+      '@isaacs/cliui': 8.0.2
+    optionalDependencies:
+      '@pkgjs/parseargs': 0.11.0
+    dev: true
+
   /jiti@1.21.0:
     resolution: {integrity: sha512-gFqAIbuKyyso/3G2qhiO2OM6shY6EPP/R0+mkDbyspxKazh8BXDC5FiFsUjlczgdNz/vfra0da2y+aHrusLG/Q==}
     hasBin: true
     dev: true
 
   /js-yaml@4.1.0:
     resolution: {integrity: sha512-wpxZs9NoxZaJESJGIZTyDEaYpl0FKSA+FB9aJiyemKhMwkxQg63h4T1KJgUGHpTqPDNRcmmYLugrRjJlBtWvRA==}
@@ -2162,33 +2226,32 @@
       argparse: 2.0.1
     dev: true
 
   /json-buffer@3.0.1:
     resolution: {integrity: sha512-4bV5BfR2mqfQTJm+V5tPPdf+ZpuhiIvTuAB5g8kcrXOZpTT/QwwVRWBywX1ozr6lEuPdbHxwaJlm9G6mI2sfSQ==}
     dev: true
 
-  /json-schema-to-typescript@13.1.2:
-    resolution: {integrity: sha512-17G+mjx4nunvOpkPvcz7fdwUwYCEwyH8vR3Ym3rFiQ8uzAL3go+c1306Kk7iGRk8HuXBXqy+JJJmpYl0cvOllw==}
-    engines: {node: '>=12.0.0'}
+  /json-schema-to-typescript@14.0.4:
+    resolution: {integrity: sha512-covPOp3hrbD+oEcMvDxP5Rh6xNZj7lOTZkXAeQoDyu1PuEl1A6oRZ3Sy05HN11vXXmdJ6gLh5P3Qz0mgMPTzzw==}
+    engines: {node: '>=16.0.0'}
     hasBin: true
     dependencies:
-      '@bcherny/json-schema-ref-parser': 10.0.5-fork
+      '@apidevtools/json-schema-ref-parser': 11.6.1
       '@types/json-schema': 7.0.15
-      '@types/lodash': 4.14.201
-      '@types/prettier': 2.7.3
-      cli-color: 2.0.3
-      get-stdin: 8.0.0
-      glob: 7.2.3
-      glob-promise: 4.2.2(glob@7.2.3)
+      '@types/lodash': 4.17.0
+      cli-color: 2.0.4
+      glob: 10.3.12
       is-glob: 4.0.3
+      js-yaml: 4.1.0
       lodash: 4.17.21
       minimist: 1.2.8
-      mkdirp: 1.0.4
+      mkdirp: 3.0.1
       mz: 2.7.0
-      prettier: 2.8.8
+      node-fetch: 3.3.2
+      prettier: 3.2.5
     dev: true
 
   /json-schema-traverse@0.4.1:
     resolution: {integrity: sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==}
     dev: true
 
   /json-stable-stringify-without-jsonify@1.0.1:
@@ -2202,16 +2265,16 @@
     dev: true
 
   /kleur@4.1.5:
     resolution: {integrity: sha512-o+NO+8WrRiQEE4/7nwRJhN1HWpVmJm511pBHUxPLtp0BUISzlBplORYSmTclCnJvQq2tKu/sgl3xVpkc7ZWuQQ==}
     engines: {node: '>=6'}
     dev: true
 
-  /known-css-properties@0.30.0:
-    resolution: {integrity: sha512-VSWXYUnsPu9+WYKkfmJyLKtIvaRJi1kXUqVmBACORXZQxT5oZDsoZ2vQP+bQFDnWtpI/4eq3MLoRMjI2fnLzTQ==}
+  /known-css-properties@0.31.0:
+    resolution: {integrity: sha512-sBPIUGTNF0czz0mwGGUoKKJC8Q7On1GPbCSFPfyEsfHb2DyBG0Y4QtV+EVWpINSaiGKZblDNuF5AezxSgOhesQ==}
     dev: true
 
   /levn@0.4.1:
     resolution: {integrity: sha512-+bT2uH4E5LGE7h/n3evcS/sQlJXCpIp6ym8OWJ5eV6+67Dsql/LaaT7qJBAt2rzfoa/5QBGBhxDix1dMt2kQKQ==}
     engines: {node: '>= 0.8.0'}
     dependencies:
       prelude-ls: 1.2.1
@@ -2255,25 +2318,30 @@
     resolution: {integrity: sha512-0KpjqXRVvrYyCsX1swR/XTK0va6VQkQM6MNo7PqW77ByjAhoARA8EfrP1N4+KlKj8YS0ZUCtRT/YUuhyYDujIQ==}
     dev: true
 
   /lodash@4.17.21:
     resolution: {integrity: sha512-v2kDEe57lecTulaDIuNTPy3Ry4gLGJ6Z1O3vE1krgXZNrsQ+LFTGHVxVjcXPs17LhbZVGedAJv8XZ1tvj5FvSg==}
     dev: true
 
+  /lru-cache@10.2.0:
+    resolution: {integrity: sha512-2bIM8x+VAf6JT4bKAljS1qUWgMsqZRPGJS6FSahIMPVvctcNhyVp7AJu7quxOW9jwkryBReKZY5tY5JYv2n/7Q==}
+    engines: {node: 14 || >=16.14}
+    dev: true
+
   /lru-cache@6.0.0:
     resolution: {integrity: sha512-Jo6dJ04CmSjuznwJSS3pUeWmd/H0ffTlkXXgwZi+eq1UCmqQwCh+eLsYOYCwY991i2Fah4h1BEMCx4qThGbsiA==}
     engines: {node: '>=10'}
     dependencies:
       yallist: 4.0.0
     dev: true
 
   /lru-queue@0.1.0:
     resolution: {integrity: sha512-BpdYkt9EvGl8OfWHDQPISVpcl5xZthb+XPsbELj5AQXxIC8IriDZIQYjBJPEm5rS420sjZ0TLEzRcq5KdBhYrQ==}
     dependencies:
-      es5-ext: 0.10.62
+      es5-ext: 0.10.64
     dev: true
 
   /magic-string@0.30.5:
     resolution: {integrity: sha512-7xlpfBaQaP/T6Vh8MO/EqXSW5En6INHEvEXQiuff7Gku0PWjU3uf6w/j9o7O+SpB5fOAkrI5HeoNgwjEO0pFsA==}
     engines: {node: '>=12'}
     dependencies:
       '@jridgewell/sourcemap-codec': 1.4.15
@@ -2296,16 +2364,16 @@
   /mdn-data@2.0.30:
     resolution: {integrity: sha512-GaqWWShW4kv/G9IEucWScBx9G1/vsFZZJUO+tD26M8J8z3Kw5RDQjaoZe03YAClgeS/SWPOcb4nkFBTEi5DUEA==}
     dev: true
 
   /memoizee@0.4.15:
     resolution: {integrity: sha512-UBWmJpLZd5STPm7PMUlOw/TSy972M+z8gcyQ5veOnSDRREz/0bmpyTfKt3/51DhEBqCZQn1udM/5flcSPYhkdQ==}
     dependencies:
-      d: 1.0.1
-      es5-ext: 0.10.62
+      d: 1.0.2
+      es5-ext: 0.10.64
       es6-weak-map: 2.0.3
       event-emitter: 0.3.5
       is-promise: 2.2.2
       lru-queue: 0.1.0
       next-tick: 1.1.0
       timers-ext: 0.1.7
     dev: true
@@ -2348,23 +2416,28 @@
       brace-expansion: 2.0.1
     dev: true
 
   /minimist@1.2.8:
     resolution: {integrity: sha512-2yyAR8qBkN3YuheJanUpWC5U3bb5osDywNB8RzDVlDwDHbocAJveqqj1u8+SVD7jkWT4yvsHCpWqqWqAxb0zCA==}
     dev: true
 
+  /minipass@7.0.4:
+    resolution: {integrity: sha512-jYofLM5Dam9279rdkWzqHozUo4ybjdZmCsDHePy5V/PbBcVMiSZR97gmAy45aqi8CK1lG2ECd356FU86avfwUQ==}
+    engines: {node: '>=16 || 14 >=14.17'}
+    dev: true
+
   /mkdirp@0.5.6:
     resolution: {integrity: sha512-FP+p8RB8OWpF3YZBCrP5gtADmtXApB5AMLn+vdyA+PyxCjrCs00mjyUozssO33cwDeT3wNGdLxJ5M//YqtHAJw==}
     hasBin: true
     dependencies:
       minimist: 1.2.8
     dev: true
 
-  /mkdirp@1.0.4:
-    resolution: {integrity: sha512-vVqVZQyf3WLx2Shd0qJ9xuvqgAyKPLAiqITEtqW0oIUjzo3PePDd6fW9iFz30ef7Ysp/oiWqbhszeGWW2T6Gzw==}
+  /mkdirp@3.0.1:
+    resolution: {integrity: sha512-+NsyUUAZDmo6YVHzL/stxSu3t9YS1iljliy3BSDrXJ/dkn1KYdmtZODGGjLcc9XLgVVpH4KshHB8XmZgMhaBXg==}
     engines: {node: '>=10'}
     hasBin: true
     dev: true
 
   /mri@1.2.0:
     resolution: {integrity: sha512-tzzskb3bG8LvYGFF/mDTpq3jpI6Q9wc3LEmBaghu+DdCssd1FakN7Bc0hVNmEyGq1bq3RgfkCb3cmQLpNPOroA==}
     engines: {node: '>=4'}
@@ -2397,14 +2470,28 @@
     resolution: {integrity: sha512-OWND8ei3VtNC9h7V60qff3SVobHr996CTwgxubgyQYEpg290h9J0buyECNNJexkFm5sOajh5G116RYA1c8ZMSw==}
     dev: true
 
   /next-tick@1.1.0:
     resolution: {integrity: sha512-CXdUiJembsNjuToQvxayPZF9Vqht7hewsvy2sOWafLvi2awflj9mOC6bHIg50orX8IJvWKY9wYQ/zB2kogPslQ==}
     dev: true
 
+  /node-domexception@1.0.0:
+    resolution: {integrity: sha512-/jKZoMpw0F8GRwl4/eLROPA3cfcXtLApP0QzLmUT/HuPCZWyB7IY9ZrMeKw2O/nFIqPQB3PVM9aYm0F312AXDQ==}
+    engines: {node: '>=10.5.0'}
+    dev: true
+
+  /node-fetch@3.3.2:
+    resolution: {integrity: sha512-dRB78srN/l6gqWulah9SrxeYnxeddIG30+GOqK/9OlLVyLg3HPnr6SqOWTWOXKRwC2eGYCkZ59NNuSgvSrpgOA==}
+    engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
+    dependencies:
+      data-uri-to-buffer: 4.0.1
+      fetch-blob: 3.2.0
+      formdata-polyfill: 4.0.10
+    dev: true
+
   /node-releases@2.0.14:
     resolution: {integrity: sha512-y10wOWt8yZpqXmOgRo77WaHEmhYQYGNA6y421PKsKYWEK8aW+cqAphborZDhqfyKrbZEN92CN1X2KbafY2s7Yw==}
     dev: true
 
   /normalize-path@3.0.0:
     resolution: {integrity: sha512-6eZs5Ls3WtCisHWp9S2GUy8dqkpGi4BVSz3GaqiE6ezub0512ESztXUwUB6C6IKbQkY2Pnb/mD4WYojCRwcwLA==}
     engines: {node: '>=0.10.0'}
@@ -2427,22 +2514,22 @@
 
   /once@1.4.0:
     resolution: {integrity: sha512-lNaJgI+2Q5URQBkccEKHTQOPaXdUxnZZElQTZY0MFUAuaEqe1E+Nyvgdz/aIyNi6Z9MzO5dv1H8n58/GELp3+w==}
     dependencies:
       wrappy: 1.0.2
     dev: true
 
-  /openapi-fetch@0.8.2:
-    resolution: {integrity: sha512-4g+NLK8FmQ51RW6zLcCBOVy/lwYmFJiiT+ckYZxJWxUxH4XFhsNcX2eeqVMfVOi+mDNFja6qDXIZAz2c5J/RVw==}
+  /openapi-fetch@0.9.5:
+    resolution: {integrity: sha512-ToRnypJB2G5bEUZqJ4mGty/qDVgAZ4BW0znlXQAECxAp4EM8dYtgQ1mrw2Ij6W7knN4VawHvFq8uTqzXyMGNPA==}
     dependencies:
-      openapi-typescript-helpers: 0.0.5
+      openapi-typescript-helpers: 0.0.8
     dev: false
 
-  /openapi-typescript-helpers@0.0.5:
-    resolution: {integrity: sha512-MRffg93t0hgGZbYTxg60hkRIK2sRuEOHEtCUgMuLgbCC33TMQ68AmxskzUlauzZYD47+ENeGV/ElI7qnWqrAxA==}
+  /openapi-typescript-helpers@0.0.8:
+    resolution: {integrity: sha512-1eNjQtbfNi5Z/kFhagDIaIRj6qqDzhjNJKz8cmMW0CVdGwT6e1GLbAfgI0d28VTJa1A8jz82jm/4dG8qNoNS8g==}
     dev: false
 
   /openapi-typescript@6.7.5:
     resolution: {integrity: sha512-ZD6dgSZi0u1QCP55g8/2yS5hNJfIpgqsSGHLxxdOjvY7eIrXzj271FJEQw33VwsZ6RCtO/NOuhxa7GBWmEudyA==}
     hasBin: true
     dependencies:
       ansi-colors: 4.1.3
@@ -2501,14 +2588,22 @@
     engines: {node: '>=8'}
     dev: true
 
   /path-parse@1.0.7:
     resolution: {integrity: sha512-LDJzPVEEEPR+y48z93A0Ed0yXb8pAByGWo/k5YYdYgpY2/2EsOsksJrq7lOHxryrVOn1ejG6oAp8ahvOIQD8sw==}
     dev: true
 
+  /path-scurry@1.10.2:
+    resolution: {integrity: sha512-7xTavNy5RQXnsjANvVvMkEjvloOinkAjv/Z6Ildz9v2RinZ4SBKTWFOVRbaF8p0vpHnyjV/UwNDdKuUv6M5qcA==}
+    engines: {node: '>=16 || 14 >=14.17'}
+    dependencies:
+      lru-cache: 10.2.0
+      minipass: 7.0.4
+    dev: true
+
   /path-type@4.0.0:
     resolution: {integrity: sha512-gDKb8aZMDeD/tZWs9P6+q0J9Mwkdl6xMV8TjnGP3qJVJ06bdMgkbBlLU8IdfOsIsFz2BW1rNVT3XuNEl8zPAvw==}
     engines: {node: '>=8'}
     dev: true
 
   /periscopic@3.1.0:
     resolution: {integrity: sha512-vKiQ8RRtkl9P+r/+oefh25C3fhybptkHKCZSPlcXiJux2tJF55GnEj3BVn4A5gKfq9NWWXXrxkHBwVPUfH0opw==}
@@ -2659,26 +2754,26 @@
     dev: true
 
   /prelude-ls@1.2.1:
     resolution: {integrity: sha512-vkcDPrRZo1QZLbn5RLGPpg/WmIQ65qoWWhcGKf/b5eplkkarX0m9z8ppCat4mlOqUsWpyNuYgO3VRyrYHSzX5g==}
     engines: {node: '>= 0.8.0'}
     dev: true
 
-  /prettier-plugin-svelte@3.2.3(prettier@3.2.5)(svelte@4.2.14):
+  /prettier-plugin-svelte@3.2.3(prettier@3.2.5)(svelte@4.2.17):
     resolution: {integrity: sha512-wJq8RunyFlWco6U0WJV5wNCM7zpBFakS76UBSbmzMGpncpK98NZABaE+s7n8/APDCEVNHXC5Mpq+MLebQtsRlg==}
     peerDependencies:
       prettier: ^3.0.0
       svelte: ^3.2.0 || ^4.0.0-next.0 || ^5.0.0-next.0
     dependencies:
       prettier: 3.2.5
-      svelte: 4.2.14
+      svelte: 4.2.17
     dev: true
 
-  /prettier-plugin-tailwindcss@0.5.13(prettier-plugin-svelte@3.2.3)(prettier@3.2.5):
-    resolution: {integrity: sha512-2tPWHCFNC+WRjAC4SIWQNSOdcL1NNkydXim8w7TDqlZi+/ulZYz2OouAI6qMtkggnPt7lGamboj6LcTMwcCvoQ==}
+  /prettier-plugin-tailwindcss@0.5.14(prettier-plugin-svelte@3.2.3)(prettier@3.2.5):
+    resolution: {integrity: sha512-Puaz+wPUAhFp8Lo9HuciYKM2Y2XExESjeT+9NQoVFXZsPPnc9VYss2SpxdQ6vbatmt8/4+SN0oe0I1cPDABg9Q==}
     engines: {node: '>=14.21.3'}
     peerDependencies:
       '@ianvs/prettier-plugin-sort-imports': '*'
       '@prettier/plugin-pug': '*'
       '@shopify/prettier-plugin-liquid': '*'
       '@trivago/prettier-plugin-sort-imports': '*'
       '@zackad/prettier-plugin-twig-melody': '*'
@@ -2722,21 +2817,15 @@
         optional: true
       prettier-plugin-style-order:
         optional: true
       prettier-plugin-svelte:
         optional: true
     dependencies:
       prettier: 3.2.5
-      prettier-plugin-svelte: 3.2.3(prettier@3.2.5)(svelte@4.2.14)
-    dev: true
-
-  /prettier@2.8.8:
-    resolution: {integrity: sha512-tdN8qQGvNjw4CHbY+XXk0JgCXn9QiF21a55rBe5LJAU+kDyC4WQn4+awm2Xfk2lQMk5fKup9XgzTZtGkjBdP9Q==}
-    engines: {node: '>=10.13.0'}
-    hasBin: true
+      prettier-plugin-svelte: 3.2.3(prettier@3.2.5)(svelte@4.2.17)
     dev: true
 
   /prettier@3.2.5:
     resolution: {integrity: sha512-3/GWa9aOC0YeD7LUfvOG2NiDyhOWRvt1k+rcKhOuYnMY24iiCphgneUfJDyFXd6rZCAnuLBv6UeAULtrhT/F4A==}
     engines: {node: '>=14'}
     hasBin: true
     dev: true
@@ -2870,14 +2959,20 @@
     resolution: {integrity: sha512-EnwXhrlwXMk9gKu5/flx5sv/an57AkRplG3hTK68W7FRDN+k+OWBj65M7719OkA82XLBxrcX0KSHj+X5COhOVg==}
     engines: {node: '>=10'}
     hasBin: true
     dependencies:
       lru-cache: 6.0.0
     dev: true
 
+  /semver@7.6.2:
+    resolution: {integrity: sha512-FNAIBWCx9qcRhoHcgcJ0gvU7SN1lYU2ZXuSfl04bSC5OpvDHFyJCjdNHomPXxjQlCBU67YW64PzY7/VIEH7F2w==}
+    engines: {node: '>=10'}
+    hasBin: true
+    dev: true
+
   /set-cookie-parser@2.6.0:
     resolution: {integrity: sha512-RVnVQxTXuerk653XfuliOxBP81Sf0+qfQE73LIYKcyMYHG94AuH0kgrQpRDuTZnSmjpysHmzxJXKNfa6PjFhyQ==}
 
   /sharp@0.33.3:
     resolution: {integrity: sha512-vHUeXJU1UvlO/BNwTpT0x/r53WkLUVxrmb5JTgW92fdFCFk0ispLMAeu/jPO2vjkXM1fYUi3K7/qcLF47pwM1A==}
     engines: {libvips: '>=8.15.2', node: ^18.17.0 || ^20.3.0 || >=21.0.0}
     requiresBuild: true
@@ -2915,14 +3010,19 @@
     dev: true
 
   /shebang-regex@3.0.0:
     resolution: {integrity: sha512-7++dFhtcx3353uBaq8DDR4NuxBetBzC7ZQOhmTQInHEd6bSrXdiEyzCvG07Z44UYdLShWUyXt5M/yhz8ekcb1A==}
     engines: {node: '>=8'}
     dev: true
 
+  /signal-exit@4.1.0:
+    resolution: {integrity: sha512-bzyZ1e88w9O1iNJbKnOlvYTrWPDl46O1bG0D3XInv+9tkPrxrN8jUUTiFlDkkmKWgn1M6CfIA13SuGqOa9Korw==}
+    engines: {node: '>=14'}
+    dev: true
+
   /simple-swizzle@0.2.2:
     resolution: {integrity: sha512-JA//kQgZtbuY83m+xT+tXJkmJncGMTFT+C+g2h2R9uxkYIrE2yy9sgmcLhCnw57/WSD+Eh3J97FPEDFnbXnDUg==}
     dependencies:
       is-arrayish: 0.3.2
     dev: true
 
   /sirv@2.0.4:
@@ -2955,21 +3055,46 @@
     dev: true
 
   /source-map-js@1.2.0:
     resolution: {integrity: sha512-itJW8lvSA0TXEphiRoawsCksnlf8SyvmFzIhltqAHluXd88pkCd+cXJVHTDwdCr0IzwptSm035IHQktUu1QUMg==}
     engines: {node: '>=0.10.0'}
     dev: true
 
+  /string-width@4.2.3:
+    resolution: {integrity: sha512-wKyQRQpjJ0sIp62ErSZdGsjMJWsap5oRNihHhu6G7JVO/9jIB6UyevL+tXuOqrng8j/cxKTWyWUwvSTriiZz/g==}
+    engines: {node: '>=8'}
+    dependencies:
+      emoji-regex: 8.0.0
+      is-fullwidth-code-point: 3.0.0
+      strip-ansi: 6.0.1
+    dev: true
+
+  /string-width@5.1.2:
+    resolution: {integrity: sha512-HnLOCR3vjcY8beoNLtcjZ5/nxn2afmME6lhrDrebokqMap+XbeW8n9TXpPDOqdGK5qcI3oT0GKTW6wC7EMiVqA==}
+    engines: {node: '>=12'}
+    dependencies:
+      eastasianwidth: 0.2.0
+      emoji-regex: 9.2.2
+      strip-ansi: 7.1.0
+    dev: true
+
   /strip-ansi@6.0.1:
     resolution: {integrity: sha512-Y38VPSHcqkFrCpFnQ9vuSXmquuv5oXOKpGeT6aGrr3o3Gc9AlVa6JBfUSOCnbxGGZF+/0ooI7KrPuUSztUdU5A==}
     engines: {node: '>=8'}
     dependencies:
       ansi-regex: 5.0.1
     dev: true
 
+  /strip-ansi@7.1.0:
+    resolution: {integrity: sha512-iq6eVVI64nQQTRYq2KtEg2d2uU7LElhTJwsH4YzIHZshxlgZms/wIc4VoDQTlG/IvVIrBKG06CrZnp0qv7hkcQ==}
+    engines: {node: '>=12'}
+    dependencies:
+      ansi-regex: 6.0.1
+    dev: true
+
   /strip-indent@3.0.0:
     resolution: {integrity: sha512-laJTa3Jb+VQpaC6DseHhF7dXVqHTfJPCRDaEbid/drOhgitgYku/letMUqOXFoWV0zIIUbjpdH2t+tYj4bQMRQ==}
     engines: {node: '>=8'}
     dependencies:
       min-indent: 1.0.1
     dev: true
 
@@ -3005,76 +3130,76 @@
     dev: true
 
   /supports-preserve-symlinks-flag@1.0.0:
     resolution: {integrity: sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==}
     engines: {node: '>= 0.4'}
     dev: true
 
-  /svelte-check@3.6.9(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.14):
-    resolution: {integrity: sha512-hDQrk3L0osX07djQyMiXocKysTLfusqi8AriNcCiQxhQR49/LonYolcUGMtZ0fbUR8HTR198Prrgf52WWU9wEg==}
+  /svelte-check@3.7.1(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.17):
+    resolution: {integrity: sha512-U4uJoLCzmz2o2U33c7mPDJNhRYX/DNFV11XTUDlFxaKLsO7P+40gvJHMPpoRfa24jqZfST4/G9fGNcUGMO8NAQ==}
     hasBin: true
     peerDependencies:
       svelte: ^3.55.0 || ^4.0.0-next.0 || ^4.0.0 || ^5.0.0-next.0
     dependencies:
       '@jridgewell/trace-mapping': 0.3.20
       chokidar: 3.5.3
       fast-glob: 3.3.2
       import-fresh: 3.3.0
       picocolors: 1.0.0
       sade: 1.8.1
-      svelte: 4.2.14
-      svelte-preprocess: 5.1.3(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.14)(typescript@5.4.5)
+      svelte: 4.2.17
+      svelte-preprocess: 5.1.3(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.17)(typescript@5.4.5)
       typescript: 5.4.5
     transitivePeerDependencies:
       - '@babel/core'
       - coffeescript
       - less
       - postcss
       - postcss-load-config
       - pug
       - sass
       - stylus
       - sugarss
     dev: true
 
-  /svelte-eslint-parser@0.34.1(svelte@4.2.14):
-    resolution: {integrity: sha512-9+uLA1pqI9AZioKVGJzYYmlOZWxfoCXSbAM9iaNm7H01XlYlzRTtJfZgl9o3StQGN41PfGJIbkKkfk3e/pHFfA==}
+  /svelte-eslint-parser@0.36.0(svelte@4.2.17):
+    resolution: {integrity: sha512-/6YmUSr0FAVxW8dXNdIMydBnddPMHzaHirAZ7RrT21XYdgGGZMh0LQG6CZsvAFS4r2Y4ItUuCQc8TQ3urB30mQ==}
     engines: {node: ^12.22.0 || ^14.17.0 || >=16.0.0}
     peerDependencies:
-      svelte: ^3.37.0 || ^4.0.0 || ^5.0.0-next.94
+      svelte: ^3.37.0 || ^4.0.0 || ^5.0.0-next.115
     peerDependenciesMeta:
       svelte:
         optional: true
     dependencies:
       eslint-scope: 7.2.2
       eslint-visitor-keys: 3.4.3
       espree: 9.6.1
       postcss: 8.4.38
       postcss-scss: 4.0.9(postcss@8.4.38)
-      svelte: 4.2.14
+      svelte: 4.2.17
     dev: true
 
-  /svelte-hmr@0.16.0(svelte@4.2.14):
+  /svelte-hmr@0.16.0(svelte@4.2.17):
     resolution: {integrity: sha512-Gyc7cOS3VJzLlfj7wKS0ZnzDVdv3Pn2IuVeJPk9m2skfhcu5bq3wtIZyQGggr7/Iim5rH5cncyQft/kRLupcnA==}
     engines: {node: ^12.20 || ^14.13.1 || >= 16}
     peerDependencies:
       svelte: ^3.19.0 || ^4.0.0
     dependencies:
-      svelte: 4.2.14
+      svelte: 4.2.17
     dev: true
 
-  /svelte-parse-markup@0.1.2(svelte@4.2.14):
+  /svelte-parse-markup@0.1.2(svelte@4.2.17):
     resolution: {integrity: sha512-DycY7DJr7VqofiJ63ut1/NEG92HrWWL56VWITn/cJCu+LlZhMoBkBXT4opUitPEEwbq1nMQbv4vTKUfbOqIW1g==}
     peerDependencies:
       svelte: ^3.0.0 || ^4.0.0
     dependencies:
-      svelte: 4.2.14
+      svelte: 4.2.17
     dev: true
 
-  /svelte-preprocess@5.1.3(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.14)(typescript@5.4.5):
+  /svelte-preprocess@5.1.3(postcss-load-config@4.0.2)(postcss@8.4.38)(svelte@4.2.17)(typescript@5.4.5):
     resolution: {integrity: sha512-xxAkmxGHT+J/GourS5mVJeOXZzne1FR5ljeOUAMXUkfEhkLEllRreXpbl3dIYJlcJRfL1LO1uIAPpBpBfiqGPw==}
     engines: {node: '>= 16.0.0', pnpm: ^8.0.0}
     requiresBuild: true
     peerDependencies:
       '@babel/core': ^7.10.2
       coffeescript: ^2.5.1
       less: ^3.11.3 || ^4.0.0
@@ -3111,20 +3236,20 @@
       '@types/pug': 2.0.10
       detect-indent: 6.1.0
       magic-string: 0.30.8
       postcss: 8.4.38
       postcss-load-config: 4.0.2(postcss@8.4.38)
       sorcery: 0.11.0
       strip-indent: 3.0.0
-      svelte: 4.2.14
+      svelte: 4.2.17
       typescript: 5.4.5
     dev: true
 
-  /svelte@4.2.14:
-    resolution: {integrity: sha512-ry3+YlWqZpHxLy45MW4MZIxNdvB+Wl7p2nnstWKbOAewaJyNJuOtivSbRChcfIej6wFBjWqyKmf/NgK1uW2JAA==}
+  /svelte@4.2.17:
+    resolution: {integrity: sha512-N7m1YnoXtRf5wya5Gyx3TWuTddI4nAyayyIWFojiWV5IayDYNV5i2mRp/7qNGol4DtxEYxljmrbgp1HM6hUbmQ==}
     engines: {node: '>=16'}
     dependencies:
       '@ampproject/remapping': 2.2.1
       '@jridgewell/sourcemap-codec': 1.4.15
       '@jridgewell/trace-mapping': 0.3.20
       '@types/estree': 1.0.5
       acorn: 8.11.2
@@ -3186,15 +3311,15 @@
     dependencies:
       any-promise: 1.3.0
     dev: true
 
   /timers-ext@0.1.7:
     resolution: {integrity: sha512-b85NUNzTSdodShTIbky6ZF02e8STtVVfD+fu4aXXShEELpozH+bCpJLYMPZbsABN2wDH7fJpqIoXxJpzbf0NqQ==}
     dependencies:
-      es5-ext: 0.10.62
+      es5-ext: 0.10.64
       next-tick: 1.1.0
     dev: true
 
   /tiny-glob@0.2.9:
     resolution: {integrity: sha512-g/55ssRPUjShh+xkfx9UPDXqhckHEsHr4Vd9zX55oSdGZc/MD0m3sferOkwWtp98bv+kcVfEHtRJgBVJzelrzg==}
     dependencies:
       globalyzer: 0.1.0
@@ -3238,18 +3363,14 @@
     dev: true
 
   /type-fest@0.20.2:
     resolution: {integrity: sha512-Ne+eE4r0/iWnpAxD852z3A+N0Bt5RN//NjJwRd2VFHEmrywxf5vsZlh4R6lixl6B+wz/8d+maTSAkN1FIkI3LQ==}
     engines: {node: '>=10'}
     dev: true
 
-  /type@1.2.0:
-    resolution: {integrity: sha512-+5nt5AAniqsCnu2cEQQdpzCAh33kVx8n0VoFidKpB1dVVLAN/F+bgVOqOJqOnEnrhp222clB5p3vUlD+1QAnfg==}
-    dev: true
-
   /type@2.7.2:
     resolution: {integrity: sha512-dzlvlNlt6AXU7EBSfpAscydQ7gXB+pPGsPnfJnZpiNJBDj7IaJzQlBZYGdEi4R9HmPdBv2XmWJ6YUtoTa7lmCw==}
     dev: true
 
   /typescript@5.4.5:
     resolution: {integrity: sha512-vcI4UpRgg81oIRUFwR0WSIHKt11nJ7SAVlYNIu+QpqeyXP+gpQJy/Z4+F0aGxSE4MqwjyXvW/TzgkLAx2AGHwQ==}
     engines: {node: '>=14.17'}
@@ -3294,16 +3415,16 @@
     dependencies:
       '@rollup/pluginutils': 5.1.0(rollup@4.12.0)
       imagetools-core: 7.0.0
     transitivePeerDependencies:
       - rollup
     dev: true
 
-  /vite@5.2.8:
-    resolution: {integrity: sha512-OyZR+c1CE8yeHw5V5t59aXsUPPVTHMDjEZz8MgguLL/Q7NblxhZUlTu9xSPqlsUO/y+X7dlU05jdhvyycD55DA==}
+  /vite@5.2.11:
+    resolution: {integrity: sha512-HndV31LWW05i1BLPMUCE1B9E9GFbOu1MbenhS58FuK6owSO5qHm7GiCotrNY1YE5rMeQSFBGmT5ZaLEjFizgiQ==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     peerDependencies:
       '@types/node': ^18.0.0 || >=20.0.0
       less: '*'
       lightningcss: ^1.21.0
       sass: '*'
@@ -3329,33 +3450,56 @@
       esbuild: 0.20.2
       postcss: 8.4.38
       rollup: 4.14.0
     optionalDependencies:
       fsevents: 2.3.3
     dev: true
 
-  /vitefu@0.2.5(vite@5.2.8):
+  /vitefu@0.2.5(vite@5.2.11):
     resolution: {integrity: sha512-SgHtMLoqaeeGnd2evZ849ZbACbnwQCIwRH57t18FxcXoZop0uQu0uzlIhJBlF/eWVzuce0sHeqPcDo+evVcg8Q==}
     peerDependencies:
       vite: ^3.0.0 || ^4.0.0 || ^5.0.0
     peerDependenciesMeta:
       vite:
         optional: true
     dependencies:
-      vite: 5.2.8
+      vite: 5.2.11
+    dev: true
+
+  /web-streams-polyfill@3.3.3:
+    resolution: {integrity: sha512-d2JWLCivmZYTSIoge9MsgFCZrt571BikcWGYkjC1khllbTeDlGqZ2D8vD8E/lJa8WGWbb7Plm8/XJYV7IJHZZw==}
+    engines: {node: '>= 8'}
     dev: true
 
   /which@2.0.2:
     resolution: {integrity: sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==}
     engines: {node: '>= 8'}
     hasBin: true
     dependencies:
       isexe: 2.0.0
     dev: true
 
+  /wrap-ansi@7.0.0:
+    resolution: {integrity: sha512-YVGIj2kamLSTxw6NsZjoBxfSwsn0ycdesmc4p+Q21c5zPuZ1pl+NfxVdxPtdHvmNVOQ6XSYG4AUtyt/Fi7D16Q==}
+    engines: {node: '>=10'}
+    dependencies:
+      ansi-styles: 4.3.0
+      string-width: 4.2.3
+      strip-ansi: 6.0.1
+    dev: true
+
+  /wrap-ansi@8.1.0:
+    resolution: {integrity: sha512-si7QWI6zUMq56bESFvagtmzMdGOtoxfR+Sez11Mobfc7tm+VkUckk9bW2UeffTGVUbOksxmSw0AA2gs8g71NCQ==}
+    engines: {node: '>=12'}
+    dependencies:
+      ansi-styles: 6.2.1
+      string-width: 5.1.2
+      strip-ansi: 7.1.0
+    dev: true
+
   /wrappy@1.0.2:
     resolution: {integrity: sha512-l4Sp/DRseor9wL6EvV2+TuQn63dMkPjZ/sp9XkghTEbV9KlPS1xUsZ3u7/IQO4wxtcFB4bgpQPRcR3QCvezPcQ==}
     dev: true
 
   /yallist@4.0.0:
     resolution: {integrity: sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==}
     dev: true
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/app.pcss` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/app.pcss`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/actions.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/actions.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/assets/cover.jpg` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/assets/cover.jpg`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/AccountDropdown.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/AccountDropdown.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/AppShell.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/AppShell.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/FormBuilder.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/HeroFrame.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/HeroFrame.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/LoadingIndicator.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/NavRail.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/PasswordInput.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/PatchedIFrame.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/PatchedIFrame.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/SwappableIcon.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/SwappableIcon.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/ThemeSelector.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/ThemeSelector.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/ThemeSelectorDropdown.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/ThemeSelectorDropdown.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/components/index.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/components/index.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Account.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Account.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Close.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Close.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/DarkMode.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Fullscreen.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/LightMode.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Logout.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Menu.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/QuestionMark.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/QuestionMark.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Reset.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/Settings.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOff.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/VisibilityOn.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/icons/index.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/icons/index.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/server/utils/api.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/server/utils/api.ts`

 * *Files 22% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 import { type Cookies } from "@sveltejs/kit"
 import { KETO_API_BASE_URL, KRATOS_API_BASE_URL } from "$lib/server/constants"
 import type { KetoPaths, KratosPaths } from "$lib/types"
 import { wrapFetch } from "$lib/utils"
 
 export const createKetoClient = (fetch: typeof global.fetch) => {
     return createClient<KetoPaths>({
+        baseUrl: KETO_API_BASE_URL,
         fetch: wrapFetch({
             fetch,
-            baseUrl: KETO_API_BASE_URL,
             credentials: "include",
             headers: { Accept: "application/json" },
         }),
     })
 }
 
-export const createKratosClient = (cookies: Cookies, fetch: typeof global.fetch) => {
+export const createKratosClient = (cookieHeader: string | null, cookies: Cookies, fetch: typeof global.fetch) => {
     return createClient<KratosPaths>({
+        baseUrl: KRATOS_API_BASE_URL,
         fetch: wrapFetch({
             fetch,
-            baseUrl: KRATOS_API_BASE_URL,
+            cookieHeader,
             cookies,
             credentials: "include",
             headers: { Accept: "application/json" },
         }),
     })
 }
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/stores.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/stores.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/keto.d.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/types/keto.d.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/types/kratos.d.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/api.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/utils/api.ts`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 import { type Cookies, error } from "@sveltejs/kit"
 import parser from "set-cookie-parser"
 import { concatenateUrl } from "$lib/utils"
 
+export function getCookieHeader(request: Request): string | null {
+    return request.headers.get("Cookie")
+}
+
 export function wrapFetch({
     fetch,
     baseUrl,
-    cookies,
+    cookieHeader,
     cookiePath,
+    cookies,
     credentials,
     headers,
     ensureOk,
 }: {
     fetch: typeof global.fetch
     baseUrl?: string | URL
-    cookies?: Cookies
+    cookieHeader?: string | null
     cookiePath?: string
+    cookies?: Cookies
     credentials?: RequestCredentials
     headers?: HeadersInit
     ensureOk?: boolean
 }): typeof global.fetch {
     return async (input, init?) => {
         let response: Response
 
         try {
+            init ??= {}
+
+            if (input instanceof Request) {
+                init.headers = new Headers(init.headers || input.headers)
+            } else {
+                init.headers = new Headers(init.headers)
+            }
+
             if (baseUrl) {
                 if (typeof input === "string" || input instanceof URL) {
                     input = concatenateUrl(input, baseUrl)
                 } else if (input instanceof Request) {
                     input = new Request(concatenateUrl(input.url, baseUrl), input)
                 }
             }
 
-            if (cookies && cookies.getAll().length > 0) {
-                init ??= {}
-                init.headers = new Headers(init.headers)
-                init.headers.set(
-                    "Cookie",
-                    cookies
-                        .getAll()
-                        .map(({ name, value }) => `${name}=${value}`)
-                        .join("; ")
-                )
+            if (cookieHeader) {
+                init.headers.set("Cookie", cookieHeader)
             }
 
             if (credentials) {
-                init ??= {}
                 init.credentials = credentials
             }
 
             if (headers) {
-                init ??= {}
-                init.headers = new Headers(init.headers)
                 for (const [key, value] of Object.entries(headers)) {
                     init.headers.set(key, value)
                 }
             }
 
-            // @ts-expect-error fetch type definition is incomplete
-            response = await fetch(input, init)
+            if (input instanceof Request) {
+                response = await fetch(new Request(input, init))
+            } else {
+                response = await fetch(input, init)
+            }
 
             if (cookies) {
                 for (const cookie of parser.parse(response.headers.getSetCookie(), { decodeValues: false })) {
                     cookies.set(cookie.name, cookie.value, {
                         encode: (value) => value,
                         path: cookiePath || "/",
                         expires: cookie.expires,
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/common.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/utils/common.ts`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/lib/utils/stubs.ts.jinja` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/lib/utils/stubs.ts.jinja`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import type { ComponentType } from "svelte"
 import { QuestionMarkIcon } from "$lib/icons"
-{% for plugin in plugin_outputs %}
-    {% set plugin_prefix = plugin.config.name|capitalize %}
-    {% if plugin.config.web_icon %}
-import {{ plugin_prefix ~ 'Icon' }} from "$lib/plugins/{{ plugin.config.name }}/{{ plugin.config.web_icon }}"
+{% for plugin_output in plugin_outputs %}
+    {% set plugin_name = plugin_output.manifest.name %}
+    {% set plugin_prefix = plugin_name|capitalize %}
+    {% if plugin_output.manifest.web_icon %}
+import {{ plugin_prefix ~ 'Icon' }} from "$lib/plugins/{{ plugin_name }}/{{ plugin_output.manifest.web_icon }}"
     {% endif %}
-    {% if plugin.config.web_alt_icon %}
-import {{ plugin_prefix ~ 'AltIcon' }} from "$lib/plugins/{{ plugin.config.name }}/{{ plugin.config.web_alt_icon }}"
+    {% if plugin_output.manifest.web_alt_icon %}
+import {{ plugin_prefix ~ 'AltIcon' }} from "$lib/plugins/{{ plugin_name }}/{{ plugin_output.manifest.web_alt_icon }}"
     {% endif %}
 {% endfor %}
 
 export function useAppIcon(name: string): { icon: ComponentType; altIcon: ComponentType } {
     const icons = {
-        {% for plugin in plugin_outputs %}
-            {% set plugin_prefix = plugin.config.name|capitalize %}
-            {% set plugin_icon = plugin_prefix ~ 'Icon' if plugin.config.web_icon else 'QuestionMarkIcon' %}
-        "{{ plugin.config.name }}":
+        {% for plugin_output in plugin_outputs %}
+            {% set plugin_name = plugin_output.manifest.name %}
+            {% set plugin_prefix = plugin_name|capitalize %}
+            {% set plugin_icon = plugin_prefix ~ 'Icon' if plugin_output.manifest.web_icon else 'QuestionMarkIcon' %}
+        "{{ plugin_name }}":
             {
                 icon: {{ plugin_icon }},
-                altIcon: {{ plugin_prefix ~ 'AltIcon' if plugin.config.web_alt_icon else plugin_icon }},
+                altIcon: {{ plugin_prefix ~ 'AltIcon' if plugin_output.manifest.web_alt_icon else plugin_icon }},
             },
         {% endfor %}
     }
 
     return icons[name]
 }
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/account/+page.server.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import { fail, redirect } from "@sveltejs/kit"
 import { createKratosClient } from "$lib/server/utils"
 import type { KratosComponents } from "$lib/types"
-import { getFlowId, getRandomId } from "$lib/utils"
+import { getCookieHeader, getFlowId, getRandomId } from "$lib/utils"
 
 export const actions = {
     default: async ({ cookies, fetch, request }) => {
         const data = await request.formData()
 
-        const client = createKratosClient(cookies, fetch)
+        const client = createKratosClient(getCookieHeader(request), cookies, fetch)
         const response = await client.POST("/self-service/settings", {
             params: { query: { flow: data.get("flow") as string } },
             body: {
                 csrf_token: data.get("csrf_token") as string,
                 method: data.get("method") as string,
                 password: data.get("password") as string,
             },
@@ -50,16 +50,16 @@
                         },
                     ],
                 })
         }
     },
 }
 
-export async function load({ cookies, fetch }) {
-    const client = createKratosClient(cookies, fetch)
+export async function load({ cookies, fetch, request }) {
+    const client = createKratosClient(getCookieHeader(request), cookies, fetch)
     const response = await client.GET("/self-service/settings/browser", { params: {} })
 
     switch (response.response.status) {
         case 200:
             return {
                 flow: getFlowId(response.data!.ui.action),
                 messages: response.data!.ui.messages,
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.server.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import { fail, redirect } from "@sveltejs/kit"
 import { createKratosClient } from "$lib/server/utils"
 import type { KratosComponents } from "$lib/types"
-import { getFlowId, getRandomId } from "$lib/utils"
+import { getCookieHeader, getFlowId, getRandomId } from "$lib/utils"
 
 export const actions = {
     default: async ({ cookies, fetch, request }) => {
         const data = await request.formData()
 
-        const client = createKratosClient(cookies, fetch)
+        const client = createKratosClient(getCookieHeader(request), cookies, fetch)
         const response = await client.POST("/self-service/login", {
             params: { query: { flow: data.get("flow") as string } },
             body: {
                 csrf_token: data.get("csrf_token") as string,
                 method: data.get("method") as string,
                 identifier: data.get("identifier") as string,
                 ...(data.get("resend")
@@ -52,16 +52,16 @@
                         },
                     ],
                 })
         }
     },
 }
 
-export async function load({ cookies, fetch }) {
-    const client = createKratosClient(cookies, fetch)
+export async function load({ cookies, fetch, request }) {
+    const client = createKratosClient(getCookieHeader(request), cookies, fetch)
     const response = await client.GET("/self-service/login/browser", { params: {} })
 
     switch (response.response.status) {
         case 200:
             return {
                 flow: getFlowId(response.data!.ui.action),
                 messages: response.data!.ui.messages,
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/login/+page.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(account)/recover/+page.server.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import { fail, redirect } from "@sveltejs/kit"
 import { createKratosClient } from "$lib/server/utils"
 import type { KratosComponents } from "$lib/types"
-import { getFlowId, getRandomId } from "$lib/utils"
+import { getCookieHeader, getFlowId, getRandomId } from "$lib/utils"
 
 export const actions = {
     default: async ({ cookies, fetch, request }) => {
         const data = await request.formData()
 
-        const client = createKratosClient(cookies, fetch)
+        const client = createKratosClient(getCookieHeader(request), cookies, fetch)
         const response = await client.POST("/self-service/recovery", {
             params: { query: { flow: data.get("flow") as string } },
             body: {
                 csrf_token: data.get("csrf_token") as string,
                 method: data.get("method") as "code" | "link",
                 ...(data.get("email") ? { email: data.get("email") as string } : { code: data.get("code") as string }),
             },
@@ -60,16 +60,16 @@
                         },
                     ],
                 })
         }
     },
 }
 
-export async function load({ cookies, fetch }) {
-    const client = createKratosClient(cookies, fetch)
+export async function load({ cookies, fetch, request }) {
+    const client = createKratosClient(getCookieHeader(request), cookies, fetch)
     const response = await client.GET("/self-service/recovery/browser", { params: {} })
 
     switch (response.response.status) {
         case 200:
             return {
                 flow: getFlowId(response.data!.ui.action),
                 messages: response.data!.ui.messages,
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/(apps)/+page.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+error.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/+error.svelte`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+layout.server.ts` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/+layout.server.ts`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import { createKetoClient, createKratosClient, getAllApps } from "$lib/server/utils"
 import type { AppInfo, User } from "$lib/types"
+import { getCookieHeader } from "$lib/utils"
 
 async function getAllowedApps(fetch: typeof global.fetch, username?: string): Promise<AppInfo[]> {
     const client = createKetoClient(fetch)
     const apps = []
 
     for (const app of getAllApps()) {
         const response = await client.GET("/relation-tuples/check", {
             params: {
                 query: {
                     namespace: "app",
-                    object: app.name,
+                    object: app.path,
                     relation: "access",
                     subject_id: username ?? "anonymous",
                 },
             },
         })
 
         switch (response.response.status) {
@@ -23,18 +24,18 @@
                 break
         }
     }
 
     return apps
 }
 
-export async function load({ cookies, fetch, url }) {
+export async function load({ cookies, fetch, request, url }) {
     const title = url.pathname.split("/").pop() || "home"
 
-    const client = createKratosClient(cookies, fetch)
+    const client = createKratosClient(getCookieHeader(request), cookies, fetch)
     const response = await client.GET("/sessions/whoami", { params: {} })
 
     switch (response.response.status) {
         case 200:
             break
         default:
             return {
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/src/routes/+layout.svelte` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/src/routes/+layout.svelte`

 * *Files 19% similar despite different names*

```diff
@@ -7,17 +7,15 @@
     import { createStore, usePageTitle } from "$lib/utils"
 
     const { allowScroll, currentTheme, isSafari } = createStore()
 
     onMount(() => {
         const theme = localStorage.getItem("theme")
         $currentTheme = theme && Object.values(ETheme).includes(theme as ETheme) ? (theme as ETheme) : ETheme.Auto
-
-        // @ts-expect-error exists for Safari on macOS
-        $isSafari = window.safari !== undefined
+        $isSafari = /^((?!chrome|android).)*safari/i.test(navigator.userAgent)
     })
 </script>
 
 <div>
     <LoadingIndicator />
     <AppShell>
         <slot />
```

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/static/favicon.png` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/static/favicon.png`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/tailwind.config.cjs` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/tailwind.config.cjs`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/src/lungo_cli/resources/web/tsconfig.json` & `lungo_cli-0.4.0/src/lungo_cli/resources/web/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lungo_cli-0.3.0/PKG-INFO` & `lungo_cli-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lungo-cli
-Version: 0.3.0
+Version: 0.4.0
 Summary: A user-friendly home lab setup designed for small-to-mid-scale on-premises hosting.
 Home-page: https://github.com/raymond-u/lungo
 Keywords: homelab,self-host
 Author: raymond-u
 Author-email: 36328498+raymond-u@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aenum (>=3.1.15,<4.0.0)
-Requires-Dist: cryptography (>=42.0.5,<43.0.0)
-Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: cryptography (>=42.0.7,<43.0.0)
+Requires-Dist: jinja2 (>=3.1.4,<4.0.0)
 Requires-Dist: packaging (>=24.0,<25.0)
-Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
+Requires-Dist: platformdirs (>=4.2.2,<5.0.0)
 Requires-Dist: pydantic-yaml (>=1.3.0,<2.0.0)
-Requires-Dist: pydantic[email] (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic[email] (>=2.7.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Documentation, https://raymond-u.github.io/lungo/
 Project-URL: Repository, https://github.com/raymond-u/lungo
 Description-Content-Type: text/markdown
 
 <br>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: lungo-cli Version: 0.3.0 Summary: A user-friendly
+Metadata-Version: 2.1 Name: lungo-cli Version: 0.4.0 Summary: A user-friendly
 home lab setup designed for small-to-mid-scale on-premises hosting. Home-page:
 https://github.com/raymond-u/lungo Keywords: homelab,self-host Author: raymond-
 u Author-email: 36328498+raymond-u@users.noreply.github.com Requires-Python:
 >=3.12,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: aenum (>=3.1.15,<4.0.0)
-Requires-Dist: cryptography (>=42.0.5,<43.0.0) Requires-Dist: jinja2
-(>=3.1.3,<4.0.0) Requires-Dist: packaging (>=24.0,<25.0) Requires-Dist:
-platformdirs (>=4.2.0,<5.0.0) Requires-Dist: pydantic-yaml (>=1.3.0,<2.0.0)
-Requires-Dist: pydantic[email] (>=2.6.4,<3.0.0) Requires-Dist: requests
+Requires-Dist: cryptography (>=42.0.7,<43.0.0) Requires-Dist: jinja2
+(>=3.1.4,<4.0.0) Requires-Dist: packaging (>=24.0,<25.0) Requires-Dist:
+platformdirs (>=4.2.2,<5.0.0) Requires-Dist: pydantic-yaml (>=1.3.0,<2.0.0)
+Requires-Dist: pydantic[email] (>=2.7.1,<3.0.0) Requires-Dist: requests
 (>=2.31.0,<3.0.0) Requires-Dist: typer (>=0.12.3,<0.13.0) Project-URL:
 Documentation, https://raymond-u.github.io/lungo/ Project-URL: Repository,
 https://github.com/raymond-u/lungo Description-Content-Type: text/markdown
                                 ************ _[[_LL_uu_nn_gg_oo_]]
                                      LLuunnggoo
                                      ************
   A user-friendly home lab setup designed for small-to-mid-scale on-premises
```

